# Comparing `tmp/omigo_core-0.5.0.tar.gz` & `tmp/omigo_core-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_core-0.5.0.tar", last modified: Sat Mar 25 01:56:34 2023, max compression
+gzip compressed data, was "omigo_core-0.5.1.tar", last modified: Thu May 25 19:09:59 2023, max compression
```

## Comparing `omigo_core-0.5.0.tar` & `omigo_core-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:34.290450 omigo_core-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-25 01:56:34.290450 omigo_core-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:18.000000 omigo_core-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-25 01:56:18.000000 omigo_core-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-25 01:56:34.290450 omigo_core-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:34.286450 omigo_core-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:34.290450 omigo_core-0.5.0/src/omigo_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/file_io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/file_paths_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/file_paths_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/file_paths_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/funclib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/local_fs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/s3_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/s3io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)   204413 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)    28372 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/tsvutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-03-25 01:56:18.000000 omigo_core-0.5.0/src/omigo_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:34.290450 omigo_core-0.5.0/src/omigo_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-25 01:56:34.000000 omigo_core-0.5.0/src/omigo_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-25 01:56:34.000000 omigo_core-0.5.0/src/omigo_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:56:34.000000 omigo_core-0.5.0/src/omigo_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-25 01:56:34.000000 omigo_core-0.5.0/src/omigo_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-25 01:56:34.000000 omigo_core-0.5.0/src/omigo_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:34.290450 omigo_core-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-25 01:56:18.000000 omigo_core-0.5.0/test/test_tsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:09:59.765351 omigo_core-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_core-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:09:39.000000 omigo_core-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 19:09:59.765351 omigo_core-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.761351 omigo_core-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/src/omigo_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_paths_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_paths_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_paths_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/funclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/local_fs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/s3_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/s3io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213923 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/tsvutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/src/omigo_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 19:09:39.000000 omigo_core-0.5.1/test/test_tsv.py
```

### Comparing `omigo_core-0.5.0/PKG-INFO` & `omigo_core-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_core
-Version: 0.5.0
+Version: 0.5.1
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.0/setup.cfg` & `omigo_core-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_core
-version = 0.5.0
+version = 0.5.1
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_core-0.5.0/src/omigo_core/etl.py` & `omigo_core-0.5.1/src/omigo_core/etl.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.0/src/omigo_core/file_io_wrapper.py` & `omigo_core-0.5.1/src/omigo_core/file_io_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def close(self):
         output_zipf = None
         output_file = None
         if (self.output_file_name.startswith("s3://")):
             content = "".join(self.data)
             bucket_name, object_key = utils.split_s3_path(self.output_file_name)
-            s3_wrapper.put_s3_file_with_text_content(bucket_name, object_key, content, self.s3_region, self.aws_profile)
+            s3_wrapper.put_file_with_text_content(bucket_name, object_key, content, self.s3_region, self.aws_profile)
         else:
             # construct output file
             if (self.output_file_name.endswith(".gz")):
                 output_file = gzip.open(self.output_file_name, "wt")
                 # write all the content
                 for line in self.data:
                     output_file.write(line)
@@ -61,15 +61,15 @@
 
     def save(self, xtsv, output_file_name):
         output_zipf = None
         output_file = None
         if (output_file_name.startswith("s3://")):
             content = xtsv.get_header() + "\n" + "\n".join(xtsv.get_data()) if (xtsv.num_rows() > 0) else xtsv.get_header()
             bucket_name, object_key = utils.split_s3_path(output_file_name)
-            s3_wrapper.put_s3_file_with_text_content(bucket_name, object_key, content, self.s3_region, self.aws_profile)
+            s3_wrapper.put_file_with_text_content(bucket_name, object_key, content, self.s3_region, self.aws_profile)
         else:
             # construct output file
             if (output_file_name.endswith(".gz")):
                 output_file = gzip.open(output_file_name, "wt")
                 # write header
                 output_file.write(xtsv.get_header() + "\n")
                 # write all the content
```

### Comparing `omigo_core-0.5.0/src/omigo_core/file_paths_data_reader.py` & `omigo_core-0.5.1/src/omigo_core/file_paths_data_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.0/src/omigo_core/file_paths_reader.py` & `omigo_core-0.5.1/src/omigo_core/file_paths_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.0/src/omigo_core/file_paths_util.py` & `omigo_core-0.5.1/src/omigo_core/file_paths_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
     return header_map
 
 def read_file_content_as_lines(path, s3_region = None, aws_profile = None):
     # check for s3
     if (path.startswith("s3://")):
         bucket_name, object_key = utils.split_s3_path(path)
-        data = s3_wrapper.get_s3_file_content_as_text(bucket_name, object_key, s3_region, aws_profile)
+        data = s3_wrapper.get_file_content_as_text(bucket_name, object_key, s3_region, aws_profile)
         data = data.split("\n")
     else:
         if (path.endswith(".gz")):
             fin = gzip.open(path, mode = "rt")
             data = [x.rstrip("\n") for x in fin.readlines()]
             fin.close()
         elif (path.endswith(".zip")):
```

### Comparing `omigo_core-0.5.0/src/omigo_core/funclib.py` & `omigo_core-0.5.1/src/omigo_core/funclib.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """library of function to be used in general purpose data processing for TSV class"""
 
 import statistics
 import numpy as np
 from dateutil import parser
 import datetime
+from omigo_core import utils
+
+# TODO: mkstr variantgs needs to use *args
 
 def parse_image_file_base_name(x):
     if (len(x) <= 1):
         return x
 
     index = -1
     if ("\\" in x):
@@ -123,14 +126,54 @@
     max_value = str(vs[0])
     for v in vs[1:]:
         if (str(v) > max_value):
             max_value = str(v)
 
     return str(max_value)
 
+def minint_failsafe(vs):
+    if (vs is None or len(vs) == 0):
+        return "" 
+    else:
+        vs = list(filter(lambda t: t != "", vs))
+        if (len(vs) == 0):
+            return "" 
+        else:
+            return minint(vs) 
+
+def maxint_failsafe(vs):
+    if (vs is None or len(vs) == 0):
+        return "" 
+    else:
+        vs = list(filter(lambda t: t != "", vs))
+        if (len(vs) == 0):
+            return "" 
+        else:
+            return maxint(vs) 
+
+def minstr_failsafe(vs):
+    if (vs is None or len(vs) == 0):
+        return "" 
+    else:
+        vs = list(filter(lambda t: t != "", vs))
+        if (len(vs) == 0):
+            return "" 
+        else:
+            return minstr(vs) 
+            
+def maxstr_failsafe(vs):
+    if (vs is None or len(vs) == 0):
+        return "" 
+    else:
+        vs = list(filter(lambda t: t != "", vs))
+        if (len(vs) == 0):
+            return "" 
+        else:
+            return maxstr(vs)
+
 def sumint(vs):
     if (len(vs) == 0):
         return 0
     else:
         return sum([int(float(t)) for t in vs])
 
 def sumfloat(vs):
@@ -223,14 +266,47 @@
     mp2 = {}
     for k in mp.keys():
         if (k not in excluded_keys):
             mp2[k] = str(mp[k])
 
     return mp2
 
+def datetime_to_utctimestamp_millis(x):
+    # convert this to string first for failsafe
+    x = str(x)
+
+    # 1681202675933
+    if (len(str(x)) == 13 and str(x).isnumeric() == True):
+        # this looks like numeric timestamp in millis
+        return int(x)
+
+    # 1681202675.933
+    if (len(str(x)) == 14 and str(x).find(".") == 10 and str(x).isnumeric() == True):
+        # this looks like numeric timestamp in millis
+        return int(x)
+
+    # 2023-04-11T08:44:35.933Z
+    if (len(x) == 24 and x[19] == "." and x.endswith("Z")):
+        return int(float(parser.parse(x).timestamp() * 1000))
+
+    # 2023-04-15T15:05:16.175000Z
+    if (len(x) == 27 and x[19] == "." and x.endswith("Z")):
+        return int(float(parser.parse(x).timestamp() * 1000))
+
+    # 2023-04-11T08:44:35.933+00:00
+    if (len(x) == 29 and x[-6] == "+"):
+        return int(float(parser.parse(x).timestamp() * 1000))
+
+    # 2023-04-18T18:47:45 or 2023-04-18 18:47:45
+    if (len(x) == 19 and (x[10] == "T" or x[10] == " ")):
+        return int(float(parser.parse(x + "+00:00").timestamp() * 1000))
+
+    # this seems to be a timestamp with second precision.
+    return int(datetime_to_utctimestamp(x) * 1000)
+
 # TODO. better naming
 def datetime_to_utctimestamp(x):
     # convert this to string first for failsafe
     x = str(x)
 
     # 2022-05-20T05:00:00+00:00
     if (x.endswith("UTC") or x.endswith("GMT") or x.endswith("Z") or x.endswith("+00:00")):
@@ -245,38 +321,58 @@
         if (x[10] == " "):
             x = x.replace(" ", "T")
         return int(parser.parse(x).timestamp())
     elif (len(x) == 26):
         # 2021-11-01T00:00:00.000000
         x = x + "Z"
         return int(parser.parse(x).timestamp())
-    elif (len(str(x)) == 10 and str(x).isnumeric() == True):
+    elif (len(x) == 27 and x[19] == "." and x.endswith("Z")):
+        # 2023-04-15T15:05:16.175000Z
+        return int(parser.parse(x).timestamp())
+    elif (len(x) == 29 and x[-6] == "+"):
+        # 2023-04-11T08:44:35.933+00:00
+        return int(parser.parse(x).timestamp())
+    elif (len(x) == 10 and str(x).isnumeric() == True):
         # this looks like a numeric timestamp
         return int(x)
-    elif (len(str(x)) == 13 and str(x).isnumeric() == True):
+    elif (len(x) == 13 and str(x).isnumeric() == True):
         # this looks like numeric timestamp in millis
         return int(int(x) / 1000)
+    elif (len(x) == 19 and (x[10] == "T" or x[10] == " ")):
+        # 2023-04-18T18:47:45 or 2023-04-18 18:47:45
+        return int(float(parser.parse(x + "+00:00").timestamp() * 1000))
     else:
         raise Exception("Unknown date format. Problem with UTC: '{}'".format(x))
 
 # TODO: Converts seconds format only
-def utctimestamp_to_datetime_str(x):
-    return utctimestamp_to_datetime(x).isoformat()
-
-# TODO: Converts seconds format only
 def utctimestamp_to_datetime(x):
-    # take it as int
-    x = int(x)
-    if (len(str(x)) == 10):
-        return datetime.datetime.utcfromtimestamp(x).replace(tzinfo = datetime.timezone.utc)
-    elif (len(str(x)) == 13):
-        return datetime.datetime.utcfromtimestamp(int(x)//1000).replace(tzinfo = datetime.timezone.utc)
+    # use the string form
+    x = str(x)
+    if (len(x) == 10 and x.isnumeric() == True):
+        return datetime.datetime.utcfromtimestamp(int(x)).replace(tzinfo = datetime.timezone.utc)
+    elif (len(x) == 13 and x.isnumeric() == True):
+        return datetime.datetime.utcfromtimestamp(int(x)/1000).replace(tzinfo = datetime.timezone.utc)
+    elif (len(x) > 10 and x.find(".") == 10 and utils.is_float(x)): 
+        return datetime.datetime.utcfromtimestamp(float(x)).replace(tzinfo = datetime.timezone.utc)
     else:
         raise Exception("Unknown timestamp format: {}".format(x))
 
+# TODO: Converts seconds format only
+def utctimestamp_millis_to_datetime(x):
+    return utctimestamp_to_datetime(x)
+
+# TODO: Converts seconds format only
+# Its utc so removed the last timezone
+def utctimestamp_to_datetime_str(x):
+    return utctimestamp_to_datetime(x).isoformat()[0:19]
+
+# Its utc so removed the last timezone
+def utctimestamp_millis_to_datetime_str(x):
+    return utctimestamp_to_datetime(x).isoformat()[0:23]
+
 def datetime_to_timestamp(x):
     raise Exception("Please use datetime_to_utctimestamp")
 
 def get_utctimestamp_sec():
     return int(datetime.datetime.now(datetime.timezone.utc).timestamp())
 
 def datestr_to_datetime(x):
@@ -444,7 +540,51 @@
         elif (diff < 30 * 24 * 60 * 60):
             result.append("{}d".format(int(diff / (24 * 60 * 60))))
         else:
             result.append("{}:s".format(diff))
 
     # return
     return ",".join(result)
+
+def simple_map_to_url_encoded_col_names(cols, url_encoded_cols = None):
+    # create result
+    results = []
+    if (url_encoded_cols is not None):
+        # iterate
+        for c in cols:
+            if (c in url_encoded_cols):
+                results.append("{}:url_encoded".format(c))
+            else:
+                results.append(c)
+    else:
+        results = cols
+
+    # return
+    return results
+
+def map_to_url_encoded_col_names(cols, prefix = None, url_encoded_cols = None):
+    results = []
+
+    # iterate
+    for c in cols:
+        col = c
+        # check if there is prefix 
+        if (col.find(":") != -1):
+            col = col.split(":")[-1]
+
+        # assign
+        result = c
+
+        # handle url_encoded suffix
+        if (url_encoded_cols is not None and col in url_encoded_cols):
+            result = "{}:url_encoded".format(c)
+
+        # handle prefix
+        if (prefix is not None):
+            result = "{}:{}".format(prefix, result)
+
+        # append
+        results.append(result)
+
+    # return
+    return results
+
```

### Comparing `omigo_core-0.5.0/src/omigo_core/local_fs_wrapper.py` & `omigo_core-0.5.1/src/omigo_core/local_fs_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.0/src/omigo_core/s3_wrapper.py` & `omigo_core-0.5.1/src/omigo_core/s3_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,25 +214,26 @@
         response = s3.list_objects_v2(**list_kwargs)
         yield from response.get('Contents', [])
         if not response.get('IsTruncated'):  # At the end of the list?
             break
         continuation_token = response.get('NextContinuationToken')
 
 # FIXME: This method is implemented using reverse engineering. Not so reliable
-def get_directory_listing(path, filter_func = None, fail_if_missing = True, region = None, profile = None):
+# TODO: ignore_if_missing should be FALSE by default
+def get_directory_listing(path, filter_func = None, ignore_if_missing = False, skip_exist_check = False, region = None, profile = None):
     region, profile = resolve_region_profile(region, profile)
     s3 = get_s3_client_cache(region, profile)
 
     # split the path
     bucket_name, object_key = utils.split_s3_path(path)
 
     filenames = []
     # validation
     if (check_path_exists(path, region, profile) == False):
-        if (fail_if_missing):
+        if (ignore_if_missing == False):
             raise Exception("Directory does not exist: " + path)
         else:
             if (utils.is_debug()):
                 print("Directory does not exist: " + path)
             return []
 
     # set the max keys as boto3 api are weird
@@ -274,46 +275,47 @@
     # print the number of object_keys found
     utils.trace("Number of entries found in directory listing: {}: {}".format(path, count))
 
     # dedup
     filenames = sorted(list(set(filenames)))
 
     # valid files as boto does a prefix search
-    filenames = list(filter(lambda t: check_path_exists(t), filenames))
+    if (skip_exist_check == False):
+        filenames = list(filter(lambda t: check_path_exists(t), filenames))
 
     # apply filter func if any
     if (filter_func is not None):
         filenames = list(filter(lambda t: filter_func(t), filenames))
 
     # return
     return filenames
 
-def delete_file(path, fail_if_missing = False, region = None, profile = None):
+def delete_file(path, ignore_if_missing = False, region = None, profile = None):
     region, profile = resolve_region_profile(region, profile)
     s3 = get_s3_client_cache(region, profile)
 
     # split the path
     bucket_name, object_key = utils.split_s3_path(path)
 
     # check if the file exists
     if (check_path_exists(path) == False):
-        if (fail_if_missing):
+        if (ignore_if_missing == False):
             raise Exception("delete_file: path doesnt exist: {}".format(path))
         else:
             utils.debug("delete_file: path doesnt exist: {}".format(path))
 
         return
 
     # delete
     s3.delete_object(Bucket = bucket_name, Key = object_key)
 
-def get_last_modified_time(path, fail_if_missing = False, region = None, profile = None):
+def get_last_modified_time(path, ignore_if_missing = False, region = None, profile = None):
     # check if exists
     if (check_path_exists(path) == False):
-        if (fail_if_missing):
+        if (ignore_if_missing == False):
             raise Exception("get_last_modified_time: path doesnt exist: {}".format(path))
         else:
             utils.debug("get_last_modified_time: path doesnt exist: {}".format(path))
 
         return None
 
     # parse
```

### Comparing `omigo_core-0.5.0/src/omigo_core/s3io_wrapper.py` & `omigo_core-0.5.1/src/omigo_core/s3io_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -125,43 +125,45 @@
             raise Exception("Multiple trailing '/' characters found: {}".format(path))
 
         return path
 
     def __simplify_dir_list__(self, path, listings, include_reserved_files = False):
         path = self.__normalize_path__(path)
 
+        # get index to simplify output
         index = len(path)
         result1 = list(filter(lambda t: include_reserved_files == True or t.endswith("/" + RESERVED_HIDDEN_FILE) == False, listings))
         result2 = list(map(lambda t: t[index + 1:], result1))
 
         # return
         return result2
 
     # TODO: this is a wait method and confusing
-    def ls(self, path, include_reserved_files = False, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS):
+    def ls(self, path, include_reserved_files = False, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS, skip_exist_check = False):
         path = self.__normalize_path__(path)
 
         # go into a wait loop for s3 to sync if the path is missing
         if (self.dir_exists(path) == False and attempts > 0):
             utils.info("ls: path: {} doesnt exist. waiting for {} seconds. attempts: {}".format(path, wait_sec, attempts))
             time.sleep(wait_sec)
             return self.ls(path, include_reserved_files = include_reserved_files, wait_sec = wait_sec, attempts = attempts - 1)
 
-        listings = self.get_directory_listing(path)
+        # get directory listings
+        listings = self.get_directory_listing(path, skip_exist_check = skip_exist_check)
         return self.__simplify_dir_list__(path, listings, include_reserved_files = include_reserved_files)
 
 
-    def get_directory_listing(self, path):
+    def get_directory_listing(self, path, skip_exist_check = False):
         if (self.__is_s3__(path)):
-            return self.__s3_get_directory_listing__(path)
+            return self.__s3_get_directory_listing__(path, skip_exist_check = skip_exist_check)
         else:
-            return self.__local_get_directory_listing__(path)
+            return self.__local_get_directory_listing__(path, skip_exist_check = skip_exist_check)
 
-    def __s3_get_directory_listing__(self, path):
-        return s3_wrapper.get_directory_listing(path)
+    def __s3_get_directory_listing__(self, path, skip_exist_check = False):
+        return s3_wrapper.get_directory_listing(path, skip_exist_check = skip_exist_check)
 
     def __local_get_directory_listing__(self, path): 
         return local_fs_wrapper.get_directory_listing(path)
 
     def list_dirs(self, path):
         path = self.__normalize_path__(path)
         result1 = self.ls(path)
@@ -177,74 +179,74 @@
     def is_file(self, path):
         return self.is_directory(path) == False
 
     def is_directory(self, path):
         return self.file_exists("{}/{}".format(path, RESERVED_HIDDEN_FILE))
 
     # TODO: confusing logic
-    def delete_file_with_wait(self, path, ignore_missing = True, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS):
+    def delete_file_with_wait(self, path, ignore_if_missing = True, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS):
         # check for ignore missing
         if (self.file_exists(path) == False):
-            if (ignore_missing == True):
-                utils.debug("delete_file_with_wait: path doesnt exist. ignore_missing: {}, returning".format(ignore_missing))
+            if (ignore_if_missing == True):
+                utils.debug("delete_file_with_wait: path doesnt exist. ignore_if_missing: {}, returning".format(ignore_if_missing))
                 return True
             else:
                 # check if attempts left
                 if (attempts > 0):
-                    utils.info("delete_file_with_wait: path: {} doesnt exists. ignore_missing is False. attempts: {}, sleep for : {} seconds".format(path, attempts, wait_sec))
+                    utils.info("delete_file_with_wait: path: {} doesnt exists. ignore_if_missing is False. attempts: {}, sleep for : {} seconds".format(path, attempts, wait_sec))
                     time.sleep(wait_sec)
-                    return self.delete_file_with_wait(path, ignore_missing = ignore_missing, wait_sec = wait_sec, attempts = attempts - 1)
+                    return self.delete_file_with_wait(path, ignore_if_missing = ignore_if_missing, wait_sec = wait_sec, attempts = attempts - 1)
                 else:
-                    utils.info("delete_file_with_wait: path doesnt exists. ignore_missing is False. attempts: over")
+                    utils.info("delete_file_with_wait: path doesnt exists. ignore_if_missing is False. attempts: over")
                     raise Exception("delete_file_with_wait: unable to delete file: {}".format(path))
         else:
             # file exists. call delete
-            self.delete_file(path, ignore_missing = ignore_missing)
+            self.delete_file(path, ignore_if_missing = ignore_if_missing)
 
             # verify that the file is deleted
             return self.file_not_exists_with_wait(path)
 
-    def delete_file(self, path, ignore_missing = None):
+    def delete_file(self, path, ignore_if_missing = None):
         if (self.__is_s3__(path)):
-            return self.__s3_delete_file__(path, ignore_missing = ignore_missing)
+            return self.__s3_delete_file__(path, ignore_if_missing = ignore_if_missing)
         else:
-            return self.__local_delete_file__(path, ignore_missing = ignore_missing)
+            return self.__local_delete_file__(path, ignore_if_missing = ignore_if_missing)
 
-    def __s3_delete_file__(self, path, ignore_missing = None):
-        return s3_wrapper.delete_file(path, fail_if_missing = ignore_missing)
+    def __s3_delete_file__(self, path, ignore_if_missing = None):
+        return s3_wrapper.delete_file(path, ignore_if_missing = ignore_if_missing)
 
-    def __local_delete_file__(self, path, ignore_missing = None):
+    def __local_delete_file__(self, path, ignore_if_missing = None):
         # delete file
-        local_fs_wrapper.delete_file(path, fail_if_missing = ignore_missing)
+        local_fs_wrapper.delete_file(path, fail_if_missing = ignore_if_missing)
 
         # check if this was the reserved file for directory
         if (path.endswith("/" + RESERVED_HIDDEN_FILE)):
             # delete the directory
             dir_path = path[0:path.rindex("/")]
             local_fs_wrapper.delete_dir(dir_path)
 
-    def delete_dir_with_wait(self, path, ignore_missing = True, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS):
+    def delete_dir_with_wait(self, path, ignore_if_missing = True, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS):
         path = self.__normalize_path__(path)
         file_path = "{}/{}".format(path, RESERVED_HIDDEN_FILE)
 
         # check for existence 
         if (self.file_exists(file_path) == False):
-            if (ignore_missing == True):
-                utils.warn("delete_dir: path doesnt exist: {}, ignore_missing: {}".format(path, ignore_missing))
+            if (ignore_if_missing == True):
+                utils.warn("delete_dir: path doesnt exist: {}, ignore_if_missing: {}".format(path, ignore_if_missing))
                 return
             else:
                 raise Exception("delete_dir: path doesnt exist: {}".format(path))
 
         # check if the directory is empty or not. to prevent race conditions
         if (len(self.ls(path)) > 0):
             utils.warn("delete_dir: directory not empty: {}".format(path))
             return False
 
         # delete the reserved file 
-        return self.delete_file_with_wait(file_path, ignore_missing = ignore_missing, wait_sec = wait_sec, attempts = attempts)
+        return self.delete_file_with_wait(file_path, ignore_if_missing = ignore_if_missing, wait_sec = wait_sec, attempts = attempts)
 
     def get_parent_directory(self, path):
         # normalize
         path = self.__normalize_path__(path)
 
         # get the last index
         index = path.rindex("/")
@@ -347,7 +349,55 @@
 
         # return
         return int(dt.replace(tzinfo = timezone.utc).timestamp())
 
     def __local_get_last_modified_timestamp__(self, path):
         return local_fs_wrapper.get_last_modified_timestamp(path)
 
+    def copy_leaf_dir(self, src_path, dest_path, overwrite = False, append = True):
+        # check if src exists
+        if (self.dir_exists(src_path) == False):
+            raise Exception("copy_leaf_dir: src_path doesnt exist: {}".format(src_path))
+
+        # # check if it is not a leaf dir
+        # if (len(self.list_dirs(dest_path)) > 0):
+        #     raise Exception("copy_leaf_dir: can not copy non leaf directories: {}".format(dest_path))
+
+        # check if dest exists
+        if (self.dir_exists(dest_path) == True):
+            # check if overwrite is False
+            if (overwrite == False):
+                raise Exception("copy_leaf_dir: dest_path exists and overwrite = False: {}".format(dest_path))
+
+        # create dir
+        self.create_dir(dest_path)
+
+        # gather the list of files to copy 
+        src_files = self.list_files(src_path)
+        dest_files = self.list_files(dest_path)
+
+        # check if there are files that will not be overwritten
+        files_not_in_src = list(set(dest_files).difference(set(src_files)))
+
+        # check for append flag
+        if (len(files_not_in_src) > 0):
+            if (append == False):
+                raise Exception("copy_leaf_dir: there are files in dest that will not be replaced and append = False: {}".format(files_not_in_src))
+            else:
+                # debug
+                utils.warn("copy_leaf_dir: there are files in dest that will not be replaced: {}".format(files_not_in_src))
+
+        # iterate
+        for f in src_files:
+            # debug
+            utils.info("copy_leaf_dir: copying: {}".format(f))
+
+            # if file exists in dest, warn
+            if (self.file_exists("{}/{}".format(dest_path, f))):
+                utils.warn("copy_leaf_dir: overwriting existing file: {}".format(f))
+
+            # copy
+            contents = self.read_file_contents_as_text("{}/{}".format(src_path, f))
+            self.write_text_file("{}/{}".format(dest_path, f), contents)
+
+    def list_leaf_dir(self, path, include_reserved_files = False, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS):
+        return self.ls(path, include_reserved_files = include_reserved_files, wait_sec = wait_sec, attempts = attempts, skip_exist_check = True)
```

### Comparing `omigo_core-0.5.0/src/omigo_core/tsv.py` & `omigo_core-0.5.1/src/omigo_core/tsv.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # validate xcol
         return col in self.header_map.keys()
 
     # cols is array of string
     def select(self, col_or_cols, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("select: empty tsv")
+            raise Exception("select: empty header tsv")
 
         # get matching column and indexes
         matching_cols = self.__get_matching_cols__(col_or_cols)
         indexes = self.__get_col_indexes__(matching_cols)
 
         # create new header
         new_header = "\t".join(matching_cols)
@@ -280,15 +280,15 @@
         return self.transform_inline(cols, lambda x: x.replace(old_str, new_str), ignore_if_missing = ignore_if_missing, dmsg = dmsg)
 
     def group_count(self, cols, prefix = "group", collapse = True, precision = 6, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "group_count")
 
         # check empty
         if (self.has_empty_header()):
-            raise Exception("group_count: empty tsv")
+            raise Exception("group_count: empty header tsv")
 
         # find the matching cols and indexes
         cols = self.__get_matching_cols__(cols)
 
         # define new columns
         new_count_col = prefix + ":count"
         new_ratio_col = prefix + ":ratio"
@@ -378,15 +378,15 @@
         return self.drop_cols(col_or_cols, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
 
     def drop_cols(self, col_or_cols, ignore_if_missing = False, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "drop_cols")
 
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("drop: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("drop: empty header tsv", ignore_if_missing)
             return self
 
         # get matching column and indexes
         matching_cols = self.__get_matching_cols__(col_or_cols, ignore_if_missing = ignore_if_missing)
 
         # find the columns that dont match
         non_matching_cols = []
@@ -413,19 +413,59 @@
         return self \
             .drop_cols(col_or_cols, ignore_if_missing = True, dmsg = dmsg)
 
     def drop_cols_if_exists(self, col_or_cols, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "drop_cols_if_exists")
         return self.drop_cols(col_or_cols, ignore_if_missing = True, dmsg = dmsg)
 
+    def drop_empty_cols(self, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "drop_empty_cols")
+
+        # check for empty data
+        if (self.num_rows() == 0):
+            return self
+
+        # iterate through each column and flag if there was a non empty value
+        fill_flags = list([0 for i in range(self.num_cols())])
+
+        # iterate and add
+        counter = 0
+        for line in self.get_data():
+            # report progress
+            counter = counter + 1
+            utils.report_progress("[1/1] calling function", dmsg, counter, self.num_rows())
+
+            # parse
+            fields = line.split("\t")
+            for i in range(self.num_cols()):
+                if (fields[i] != ""):
+                    fill_flags[i] = 1
+
+        # find the column indexes that didnt have any value
+        empty_cols = []
+        for i in range(len(fill_flags)):
+            if (fill_flags[i] == 0):
+                empty_cols.append(self.get_column(i))
+
+        # if there are empty cols, drop them
+        if (len(empty_cols) > 0):
+            if (len(empty_cols) == self.num_cols()):
+                return self \
+                    .get_columns()
+            else:
+                return self \
+                    .drop_cols(empty_cols, dmsg = dmsg)
+        else:
+            return self
+ 
     # TODO: the select_cols is not implemented properly
     def window_aggregate(self, win_col, agg_cols, agg_funcs, winsize, select_cols = None, sliding = False, collapse = True, suffix = "", precision = 2, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("window_aggregate: empty tsv")
+            raise Exception("window_aggregate: empty header tsv")
 
         # get the matching cols
         if (select_cols is None):
             select_cols = []
         select_cols = self.__get_matching_cols__(select_cols)
 
         # do validation on window column. All values should be unique
@@ -509,15 +549,15 @@
             return TSV(new_header, new_data) \
                 .aggregate(cols2, agg_cols, agg_funcs, collapse, precision)
 
     # The signature for agg_func is func(list_of_maps). Each map will get the agg_cols
     def group_by_key(self, grouping_cols, agg_cols, agg_func, suffix = "", collapse = True, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("group_by_key: empty tsv")
+            raise Exception("group_by_key: empty header tsv")
 
         # resolve grouping and agg_cols
         grouping_cols = self.__get_matching_cols__(grouping_cols)
         agg_cols = self.__get_matching_cols__(agg_cols)
 
         # check for validity
         if (len(grouping_cols) == 0):
@@ -751,15 +791,15 @@
     # TODO: this use_string_datatype is temporary and needs to be replaced with better design.
     def aggregate(self, grouping_col_or_cols, agg_cols, agg_funcs, collapse = True, precision = None, use_rolling = None, use_string_datatype = None,
 	string_datatype_cols = None, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "aggregate")
 
         # check empty
         if (self.has_empty_header()):
-            raise Exception("aggregate: empty tsv")
+            raise Exception("aggregate: empty header tsv")
 
         # check for usage of builtin functions
         for agg_func in agg_funcs:
             # raise warning if builtin functions are used
             if (__is_builtin_func__(agg_func)):
                 utils.warn("aggregate: builtin function used that has side effect. Please use funclib.* functions")
 
@@ -796,15 +836,15 @@
             if (agg_col not in self.header_map.keys()):
                 raise Exception("Column not found: {}, header: {}".format(agg_col, self.header_fields))
 
             new_cols.append(agg_col + ":" + get_func_name(agg_funcs[i]))
 
         # check for empty data
         if (self.num_rows() == 0):
-            utils.debug("aggregate: no data. Returning new header only")
+            utils.trace("aggregate: no data. Returning new header only")
 
         # take the indexes
         agg_col_indexes = []
         str_agg_col_indexes = []
 
         # for each agg col, add the index
         for i in range(len(agg_cols)):
@@ -844,15 +884,16 @@
 
         # compute the aggregation
         value_func_map_arr = [{} for i in range(len(agg_col_indexes))]
 
         # for each possible index, do aggregation
         for j in range(len(agg_col_indexes)):
             for k, vs in value_map_arr[j].items():
-                value_func_map_arr[j][k] = agg_funcs[j](vs)
+                agg_value = agg_funcs[j](vs)
+                value_func_map_arr[j][k] = agg_value if (agg_value) is not None else ""
 
         # create new header and data
         new_header = "\t".join(utils.merge_arrays([self.header_fields, new_cols]))
         new_data = []
 
         # for each output line, attach the new aggregate value
         counter = 0
@@ -895,15 +936,15 @@
         return result_xtsv
 
     def filter(self, cols, func, include_cond = True, use_array_notation = False, ignore_if_missing = False, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "filter")
 
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("filter: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("filter: empty header tsv", ignore_if_missing)
             return self
 
         # TODO: Filter should not use regex. Need to add warning as the order of fields matter
         cols = self.__get_matching_cols__(cols, ignore_if_missing = ignore_if_missing)
         indexes = self.__get_col_indexes__(cols)
 
         # count the number of columns
@@ -972,32 +1013,34 @@
         # return
         return TSV(self.header, new_data)
 
     def exclude_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "exclude_filter")
         return self.filter(cols, func, include_cond = False, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
 
-    def any_col_with_cond_exists_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
+    def __any_col_with_cond_exists_filter__(self, cols, func, exclude_flag = False, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "__any_col_with_cond_exists_filter__")
+
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("any_col_with_cond_exists_filter: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("__any_col_with_cond_exists_filter__: empty header tsv", ignore_if_missing)
             return self
 
         # find the matching cols and indexes
         matching_cols = self.__get_matching_cols__(cols, ignore_if_missing = ignore_if_missing)
         indexes = self.__get_col_indexes__(matching_cols)
 
         # check if there were any matching columns
         if (len(matching_cols) == 0):
-            utils.raise_exception_or_warn("any_col_with_cond_exists_filter: no matching columns", ignore_if_missing)
+            utils.raise_exception_or_warn("{}: no matching columns".format(dmsg), ignore_if_missing)
             return self
 
         # print which columns are going to be transformed
         if (len(matching_cols) != len(cols) and len(matching_cols) != 1):
-            utils.debug("any_col_with_cond_exists_filter: list of columns that will be checked: {}".format(str(matching_cols)))
+            utils.debug("{}: list of columns that will be checked: {}".format(dmsg, str(matching_cols)))
 
         # iterate
         new_data = []
         for line in self.get_data():
             # get fields
             fields = line.split("\t", -1)
 
@@ -1005,39 +1048,45 @@
             flag = False 
             for i in indexes:
                 # append to new data if any column matched
                 if (func(fields[i]) == True):
                     flag = True
                     break
 
-            # check if all conditions met
+            # check if all conditions met. apply exclude filter
             if (flag == True):
-                new_data.append(line)
+                if (exclude_flag == False):
+                    new_data.append(line)
+            else:
+                if (exclude_flag == True):
+                    new_data.append(line)
 
         # return
         return TSV(self.get_header(), new_data)
  
-    def all_cols_with_cond_exists_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
+    def __all_cols_with_cond_exists_filter__(self, cols, func, exclude_flag = False, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "__all_cols_with_cond_exists_filter__")
+
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("all_cols_with_cond_exists_filter: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("__all_cols_with_cond_exists_filter__: empty header tsv", ignore_if_missing)
             return self
 
         # find the matching cols and indexes
         matching_cols = self.__get_matching_cols__(cols, ignore_if_missing = ignore_if_missing)
         indexes = self.__get_col_indexes__(matching_cols)
 
         # check if there were any matching columns
         if (len(matching_cols) == 0):
-            utils.raise_exception_or_warn("any_col_with_cond_exists_filter: no matching columns", ignore_if_missing)
+            utils.raise_exception_or_warn("{}: no matching columns".format(dmsg), ignore_if_missing)
             return self
 
         # print which columns are going to be transformed
         if (len(matching_cols) != len(cols) and len(matching_cols) != 1):
-            utils.debug("any_col_with_cond_exists_filter: list of columns that will be checked: {}".format(str(matching_cols)))
+            utils.debug("{}: list of columns that will be checked: {}".format(dmsg, str(matching_cols)))
 
         # iterate
         new_data = []
         for line in self.get_data():
             # get fields
             fields = line.split("\t", -1)
 
@@ -1047,19 +1096,39 @@
                 # append to new data if any column matched
                 if (func(fields[i]) == False):
                     flag = False
                     break
 
             # check if all conditions met
             if (flag == True):
-                new_data.append(line)
+                if (exclude_flag == False):
+                    new_data.append(line)
+            else:
+                if (exclude_flag == True):
+                    new_data.append(line)
 
         # return
-        return TSV(self.get_header(), new_data) 
-        
+        return TSV(self.get_header(), new_data)
+
+    def any_col_with_cond_exists_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "any_col_with_cond_exists_filter")
+        return self.__any_col_with_cond_exists_filter__(cols, func, exclude_flag = False, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
+
+    def any_col_with_cond_exists_exclude_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "any_col_with_cond_exists_exclude_filter")
+        return self.__any_col_with_cond_exists_filter__(cols, func, exclude_flag = True, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
+
+    def all_col_with_cond_exists_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "all_col_with_cond_exists_filter")
+        return self.__all_col_with_cond_exists_filter__(cols, func, exclude_flag = False, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
+
+    def all_col_with_cond_exists_exclude_filter(self, cols, func, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "all_col_with_cond_exists_exclude_filter")
+        return self.__all_col_with_cond_exists_filter__(cols, func, exclude_flag = True, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
+
     def transform(self, cols, func, new_col_or_cols, use_array_notation = False, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "transform")
 
         # check empty
         if (self.has_empty_header()):
             raise Exception("transform: empty header tsv")
 
@@ -1153,14 +1222,18 @@
                 elif (num_cols == 15):
                     result = func(col_values[0], col_values[1], col_values[2], col_values[3], col_values[4], col_values[5], col_values[6], col_values[7], col_values[8], col_values[9], col_values[10], col_values[11], col_values[12], col_values[13], col_values[14])
                 else:
                     raise Exception("Number of columns is not supported beyond 15. Probably try to use use_array_notation approach: {}".format(str(cols)))
             else:
                 result = func(col_values)
 
+            # if result is None, convert to empty string
+            if (result is None):
+                result = ""
+
             # create new line and append to data. Do validation
             result_arr = []
             if (use_array_notation == False):
                 if (num_new_cols == 1):
                     if (isinstance(result, list)):
                         result_arr.append(str(result[0]))
                     else:
@@ -1209,15 +1282,15 @@
         return TSV(new_header, new_data)
 
     def transform_inline(self, cols, func, ignore_if_missing = False, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "transform_inline")
 
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("transform_inline: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("transform_inline: empty header tsv", ignore_if_missing)
             return self
 
         # find the matching cols and indexes
         matching_cols = self.__get_matching_cols__(cols, ignore_if_missing = ignore_if_missing)
         indexes = self.__get_col_indexes__(matching_cols)
 
         # check if there were any matching columns
@@ -1282,15 +1355,15 @@
     def transform_inline_log1p_base10(self, col_or_cols, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "transform_inline_log1p_base10")
         return self.transform_inline_log1p(col_or_cols, base = 10, dmsg = dmsg)
         
     def rename(self, col, new_col, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("rename: empty tsv")
+            raise Exception("rename: empty header tsv")
 
         # validation
         if (self.has_col(col) == False):
             raise Exception("Column: {} not found in {}".format(str(col), str(self.get_header_fields())))
 
         # validation
         if (self.has_col(new_col) == True):
@@ -1336,44 +1409,73 @@
 
     def get_header_fields(self):
         return self.header_fields
 
     def get_columns(self):
         return self.get_header_fields()
 
+    def get_column(self, index):
+        # validation
+        if (index < 0 or index >= self.num_cols()):
+            raise Exception("get_column: invalid index: {}".format(index))
+
+        # return
+        return self.get_header_fields()[index]
+
     def columns(self):
         utils.warn("Deprecated. Use get_columns() instead")
         return self.get_columns()
 
     def get_column_index(self, col):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("get_column_index: empty tsv")
+            raise Exception("get_column_index: empty header tsv")
 
         # validation
         if (col not in self.get_columns()):
             raise Exception("Column not found: {}, {}".format(col, self.get_columns()))
 
         # get index
         header_map = self.get_header_map()
         return header_map[col]
 
     def export_to_maps(self):
         utils.warn("Please use to_maps()")
         return self.to_maps()
 
-    def to_maps(self):
+    def to_maps(self, resolve_url_encoded_cols = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "to_maps")
+
+        # create maps
         mps = []
 
         # create a map for each row
         for line in self.get_data():
             fields = line.split("\t")
             mp = {}
             for i in range(len(self.get_header_fields())):
-                mp[self.header_fields[i]] = str(fields[i])
+                key = self.header_fields[i]
+                value = str(fields[i])
+
+                # check for resolving url encoded cols
+                if (resolve_url_encoded_cols == True):
+                    if (key.endswith(":url_encoded") == True):
+                        key = key[0:-len(":url_encoded")]
+                        value = utils.url_decode(value)
+                    elif (key.endswith(":url_encoded:uniq_mkstr") == True):
+                        key = key[0:-len(":url_encoded:uniq_mkstr")] + ":uniq_mkstr"
+                        value = ",".join([utils.url_decode(t) for t in value.split(",")])
+                    elif (key.endswith(":url_encoded:mkstr") == True):
+                        key = key[0:-len(":url_encoded:mkstr")] + ":mkstr"
+                        value = ",".join([utils.url_decode(t) for t in value.split(",")])
+
+                # set new value 
+                mp[key] = str(value)
+
+            # append
             mps.append(mp)
 
         # return
         return mps
 
     def __convert_to_numeric__(self, x, precision = 6):
         try:
@@ -1393,15 +1495,15 @@
     def to_numeric(self, cols, precision = 6, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "to_numeric")
         return self.transform_inline(cols, lambda x: self.__convert_to_numeric__(x, precision), dmsg = dmsg)
 
     def add_seq_num(self, new_col, start = 1, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("add_seq_num: empty tsv")
+            utils.warn("add_seq_num: empty header tsv")
             return self
 
         # validation
         if (new_col in self.header_map.keys()):
             raise Exception("Output column name: {} already exists in {}".format(new_col, self.header_fields))
 
         # create new header
@@ -1561,63 +1663,73 @@
 
         # print blank lines
         print("")
 
         # return self
         return self
 
-    def col_as_array(self, col):
+    def col_as_array(self, col, include_empty = True):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("col_as_array: empty tsv")
+            raise Exception("col_as_array: empty header tsv")
 
         # validation
         if (col not in self.header_map.keys()):
             raise Exception("Column not found: {}, {}".format(str(col), str(self.get_header_fields())))
 
+        # index
         index = self.header_map[col]
         ret_values = []
         for line in self.get_data():
             fields = line.split("\t")
-            ret_values.append(str(fields[index]))
+            value = str(fields[index])
+            if (value != ""):
+                ret_values.append(value)
+            else:
+                if (include_empty == True):
+                    ret_values.append(value)
 
+        # return
         return ret_values
 
     def col_as_float_array(self, col):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("col_as_float_array: empty tsv")
+            raise Exception("col_as_float_array: empty header tsv")
 
         values = self.col_as_array(col)
         float_values = [float(v) for v in values]
         return float_values
 
     def col_as_int_array(self, col):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("col_as_int_array: empty tsv")
+            raise Exception("col_as_int_array: empty header tsv")
 
         values = self.col_as_float_array(col)
         numeric_values = [int(v) for v in values]
         return numeric_values
 
     def col_as_array_uniq(self, col):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("col_as_array_uniq: empty tsv")
+            raise Exception("col_as_array_uniq: empty header tsv")
 
         values = self.col_as_array(col)
         return list(dict.fromkeys(values))
 
+    def col_as_array_uniq_non_empty(self, col):
+        return list(filter(lambda t: t != "", self.col_as_array_uniq(col)))
+
     # this method returns hashmap of key->map[k:v]
     # TODO: keys should be changed to single column
     def cols_as_map(self, key_cols, value_cols):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("cols_as_map: empty tsv")
+            raise Exception("cols_as_map: empty header tsv")
 
         # warn
         utils.debug_once("[OLD_WARN]: cols_as_map: This api has changed from prev implementation")
 
         # validation
         key_cols = self.__get_matching_cols__(key_cols)
 
@@ -1669,15 +1781,15 @@
 
         return tuple(values)
 
     # TODO: this api needs to remove the auto detection of all_numeric flag
     def sort(self, cols = None, reverse = False, reorder = False, all_numeric = None, ignore_if_missing = False, dmsg = ""):
         # check empty
         if (self.has_empty_header() and cols is None):
-            utils.raise_exception_or_warn("sort: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("sort: empty header tsv", ignore_if_missing)
             return self
 
         # if nothing is specified sort on all columns
         if (cols is None):
             cols = self.get_header_fields()
 
         # find the matching cols and indexes
@@ -1727,18 +1839,18 @@
         return self.reverse_sort(cols = cols, reorder = reorder, all_numeric = True, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
 
     # reorder the specific columns
     def reorder(self, cols, use_existing_order = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
             if (cols is None):
-                utils.warn("reorder: empty tsv")
+                utils.warn("reorder: empty header tsv")
                 return self
             else:
-                raise Exception("reorder: empty tsv")
+                raise Exception("reorder: empty header tsv")
 
         # get matching column and indexes
         matching_cols = self.__get_matching_cols__(cols)
         indexes = self.__get_col_indexes__(matching_cols)
 
         # do a full reorder if asked
         if (use_existing_order == False):
@@ -1779,15 +1891,15 @@
         utils.warn("Please use reverse_reorder instead")
         return self.reverse_reorder(cols, dmsg)
 
     # reorder for pushing the columns to the end
     def reverse_reorder(self, cols, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("reorder: empty tsv")
+            raise Exception("reorder: empty header tsv")
 
         # get matching column and indexes
         matching_cols = self.__get_matching_cols__(cols)
 
         # generate the list of cols that should be brought to front
         rcols = []
         for h in self.get_header_fields():
@@ -1909,19 +2021,39 @@
         dmsg = utils.extend_inherit_message(dmsg, "url_encode")
         return self.transform([col], lambda x: utils.url_encode(x), newcol, dmsg = dmsg)
 
     def url_decode(self, col, newcol, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "url_decode")
         return self.transform([col], lambda x: utils.url_decode(x), newcol, dmsg = dmsg)
 
-    def resolve_url_encoded_cols(self, suffix = "url_encoded", ignore_if_missing = True, dmsg = ""):
+    def resolve_url_encoded_cols(self, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "resolve_url_encoded_cols")
+
+        # return
         return self \
-            .url_decode_inline(".*:{}".format(suffix), ignore_if_missing = ignore_if_missing, dmsg = dmsg) \
-            .remove_suffix(suffix, ignore_if_missing = ignore_if_missing, dmsg = dmsg)
+            .transform_inline(".*:url_encoded", utils.url_decode, ignore_if_missing = True, dmsg = dmsg) \
+            .remove_suffix("url_encoded", ignore_if_missing = True, dmsg = dmsg)
+
+    def resolve_url_encoded_list_cols(self, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "resolve_url_encoded_list_cols")
+
+        # return
+        return self \
+            .transform_inline([".*:url_encoded:uniq_mkstr", ".*:url_encoded:mkstr"],
+                lambda t: ",".join([utils.url_decode(t1) for t1 in t.split(",")]) if (t != "") else t, ignore_if_missing = True, dmsg = dmsg) \
+            .replace_suffix("url_encoded:uniq_mkstr", "uniq_mkstr", ignore_if_missing = True, dmsg = dmsg) \
+            .replace_suffix("url_encoded:mkstr", "mkstr", ignore_if_missing = True, dmsg = dmsg)
+
+    def resolve_all_url_encoded_cols(self, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "resolve_all_url_encoded_cols")
+
+        # return
+        return self \
+            .resolve_url_encoded_cols(dmsg = dmsg) \
+            .resolve_url_encoded_list_cols(dmsg = dmsg)
 
     def union(self, tsv_or_that_arr):
         # check if this is a single element TSV or an array
         if (type(tsv_or_that_arr) == TSV):
             that_arr = [tsv_or_that_arr]
         else:
             that_arr = tsv_or_that_arr
@@ -2015,18 +2147,18 @@
         return self.transform([self.header_fields[0]], lambda x: str(value), col, dmsg = dmsg)
 
     def add_const_if_missing(self, col, value, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
             # checking empty value
             if (value == ""):
-                utils.warn("add_const_if_missing: empty tsv and empty value. extending just the header")
+                utils.warn("add_const_if_missing: empty header tsv and empty value. extending just the header")
                 return new_with_cols([col])
             else:
-                raise Exception("add_const_if_missing: empty tsv but non empty value")
+                raise Exception("add_const_if_missing: empty header tsv but non empty value")
 
         # check for presence
         if (col in self.header_fields):
             return self
         else:
             dmsg = utils.extend_inherit_message(dmsg, "add_const_if_missing")
             return self.add_const(col, value, dmsg = dmsg)
@@ -2083,15 +2215,15 @@
 
         # return
         return TSV(new_header, new_data)
 
     def add_row(self, row_fields):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("{}: add_row: empty tsv".format(dmsg))
+            raise Exception("{}: add_row: empty header tsv".format(dmsg))
 
         # validation
         if (len(row_fields) != self.num_cols()):
             raise Exception("{}: Number of fields is not matching with number of columns: {} != {}".format(dmsg, len(row_fields), self.num_cols()))
 
         # create new row
         new_line = "\t".join(row_fields)
@@ -2104,15 +2236,15 @@
 
         # return
         return TSV(self.header, new_data)
 
     def add_map_as_row(self, mp, default_val = None):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("add_map_as_row: empty tsv")
+            raise Exception("add_map_as_row: empty header tsv")
 
         # validation
         for k in mp.keys():
             if (k not in self.header_fields):
                 raise Exception("Column not in existing data: {}, {}".format(k, str(self.get_header_fields())))
 
         # check for default values
@@ -2137,15 +2269,15 @@
     def assign_value(self, col_or_cols, value, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "assign_value")
         return self.transform_inline(col_or_cols, lambda x: value, dmsg = dmsg)
 
     def concat_as_cols(self, that, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("concat_as_cols: empty tsv")
+            utils.warn("concat_as_cols: empty header tsv")
             return that
 
         # validation
         if (self.num_rows() != that.num_rows()):
             raise Exception("Mismatch in number of rows: {}, {}".format(self.num_rows(), that.num_rows()))
 
         # check for complete disjoint set of columns
@@ -2173,17 +2305,19 @@
         return TSV(new_header, new_data)
 
     def add_col_prefix(self, cols, prefix, dmsg = ""):
         utils.warn("Deprecated: Use add_prefix instead")
         return self.add_prefix(self, prefix, cols)
 
     def remove_suffix(self, suffix, prefix = None, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "remove_suffix")
+
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("remove_suffix: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("{}: empty header tsv".format(dmsg), ignore_if_missing)
             return self
 
         # create a map
         mp = {}
 
         # validation
         if (suffix.startswith(":") == False):
@@ -2192,29 +2326,30 @@
         # check for matching cols
         for c in self.get_header_fields():
             if (c.endswith(suffix)):
                 # check if the prefix is defined and matcing
                 if (prefix is None or c.startswith(prefix + ":") == True):
                     new_col =  c[0:-len(suffix)]
                     if (new_col in self.header_fields or len(new_col) == 0):
-                        utils.warn("remove_suffix: Duplicate names found. Ignoring removal of prefix for col: {} to new_col: {}".format(c, new_col))
+                        utils.warn("{}: Duplicate names found. Ignoring removal of suffix for col: {} to new_col: {}".format(dmsg, c, new_col))
                     else:
                         mp[c] = new_col
 
         # validation
         if (len(mp) == 0):
-            utils.raise_exception_or_warn("suffix didnt match any of the columns: {}, {}".format(suffix, str(self.get_header_fields())), ignore_if_missing)
+            utils.raise_exception_or_warn("{}: suffix didnt match any of the columns: {}, {}".format(dmsg, suffix, str(self.get_header_fields())), ignore_if_missing)
 
+        # return
         new_header = "\t".join(list([h if (h not in mp.keys()) else mp[h] for h in self.header_fields]))
         return TSV(new_header, self.data)
 
     def add_prefix(self, prefix, cols = None, ignore_if_missing = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("add_prefix: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("add_prefix: empty header tsv", ignore_if_missing)
             return self
 
         # by default all columns are renamed
         if (cols is None):
             cols = self.header_fields
 
         # resolve columns
@@ -2232,15 +2367,15 @@
 
         # return
         return TSV("\t".join(new_header_fields), self.data)
 
     def add_suffix(self, suffix, cols = None, ignore_if_missing = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("add_suffix: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("add_suffix: empty header tsv", ignore_if_missing)
             return self
 
         # by default all columns are renamed
         if (cols is None):
             cols = self.header_fields
 
         # resolve columns
@@ -2258,15 +2393,15 @@
 
         # return
         return TSV("\t".join(new_header_fields), self.data)
 
     def rename_prefix(self, old_prefix, new_prefix, cols = None, ignore_if_missing = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("rename_prefix: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("rename_prefix: empty header tsv", ignore_if_missing)
             return self
 
         # either selective columns can be renamed or all matching ones
         if (cols is None):
             # use the prefix patterns for determing cols
             cols = "{}:.*".format(old_prefix)
 
@@ -2285,15 +2420,15 @@
 
         # return
         return TSV("\t".join(new_header_fields), self.data)
 
     def rename_suffix(self, old_suffix, new_suffix, cols = None, ignore_if_missing = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("rename_suffix: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("rename_suffix: empty header tsv", ignore_if_missing)
             return self
 
         # either selective columns can be renamed or all matching ones
         if (cols is None):
             # use the prefix patterns for determing cols
             cols = ".*:{}".format(old_suffix)
 
@@ -2310,45 +2445,113 @@
             else:
                 new_header_fields.append(h)
 
         # return
         return TSV("\t".join(new_header_fields), self.data)
 
     def remove_prefix(self, prefix, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "remove_prefix")
+
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("remove_prefix: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("{}: empty header tsv".format(dmsg), ignore_if_missing)
             return self
 
         # create a map
         mp = {}
 
         # validation
         if (prefix.endswith(":") == False):
             prefix = prefix + ":"
 
         # check for matching cols
         for c in self.get_header_fields():
             if (c.startswith(prefix)):
                 new_col = c[len(prefix):]
+                # validation
                 if (new_col in self.get_header_fields() or len(new_col) == 0):
-                    raise Exception("Duplicate names. Cant do the prefix: {}, {}, {}".format(c, new_col, str(self.get_header_fields())))
+                    raise Exception("{}: Duplicate names. Cant do the prefix: {}, {}, {}".format(dmsg, c, new_col, str(self.get_header_fields())))
+
+                # assign new col
                 mp[c] = new_col
 
         # validation
         if (len(mp) == 0):
-            utils.raise_exception_or_warn("prefix didnt match any of the columns: {}, {}".format(prefix, str(self.get_header_fields())), ignore_if_missing)
+            utils.raise_exception_or_warn("{}: prefix didnt match any of the columns: {}, {}".format(dmsg, prefix, str(self.get_header_fields())), ignore_if_missing)
 
+        # return
+        new_header = "\t".join(list([h if (h not in mp.keys()) else mp[h] for h in self.get_header_fields()]))
+        return TSV(new_header, self.data)
+
+    def replace_prefix(self, old_prefix, new_prefix, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "replace_prefix")
+
+        # check empty
+        if (self.has_empty_header()):
+            utils.raise_exception_or_warn("{}: empty header tsv".format(dmsg), ignore_if_missing)
+            return self
+
+        # create a map
+        mp = {}
+
+        # validation
+        if (old_prefix.endswith(":") == False):
+            old_prefix = prefix + ":"
+
+        # check for matching cols
+        for c in self.get_header_fields():
+            if (c.startswith(old_prefix)):
+                new_col = "{}:{}".format(new_prefix, c[len(old_prefix):])
+                if (new_col in self.get_header_fields() or len(new_col) == 0):
+                    raise Exception("{}: Duplicate names. Cant do the prefix: {}, {}, {}".format(dmsg, c, new_col, str(self.get_header_fields())))
+                mp[c] = new_col
+
+        # validation
+        if (len(mp) == 0):
+            utils.raise_exception_or_warn("{}: prefix didnt match any of the columns: {}, {}".format(dmsg, prefix, str(self.get_header_fields())), ignore_if_missing)
+
+        # return
+        new_header = "\t".join(list([h if (h not in mp.keys()) else mp[h] for h in self.get_header_fields()]))
+        return TSV(new_header, self.data)
+
+    def replace_suffix(self, old_suffix, new_suffix, ignore_if_missing = False, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "replace_suffix")
+
+        # check empty
+        if (self.has_empty_header()):
+            utils.raise_exception_or_warn("{}: empty header tsv".format(dmsg), ignore_if_missing)
+            return self
+
+        # create a map
+        mp = {}
+
+        # validation
+        if (old_suffix.startswith(":") == False):
+            old_suffix = ":" + old_suffix
+
+        # check for matching cols
+        for c in self.get_header_fields():
+            if (c.endswith(old_suffix)):
+                new_col = "{}:{}".format(c[0:-len(old_suffix)], new_suffix)
+                if (new_col in self.get_header_fields() or len(new_col) == 0):
+                    raise Exception("{}: Duplicate names. Cant do the suffix: {}, {}, {}".format(dmsg, c, new_col, str(self.get_header_fields())))
+                mp[c] = new_col
+
+        # validation
+        if (len(mp) == 0):
+            utils.raise_exception_or_warn("{}: suffix didnt match any of the columns: {}, {}".format(dmsg, old_suffix, str(self.get_header_fields())), ignore_if_missing)
+
+        # return
         new_header = "\t".join(list([h if (h not in mp.keys()) else mp[h] for h in self.get_header_fields()]))
         return TSV(new_header, self.data)
 
     def sample(self, sampling_ratio, seed = 0, with_replacement = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample: empty tsv")
+            utils.warn("sample: empty header tsv")
             return self
 
         # TODO
         if (with_replacement == True):
             raise Exception("sampling with replacement not implemented yet.")
 
         # set seed
@@ -2381,15 +2584,15 @@
         utils.warn("Please use sample_n")
         dmsg = utils.extend_inherit_message(dmsg, "sample_rows")
         return self.sample_n(n, seed, dmsg = dmsg)
 
     def sample_n(self, n, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_n: empty tsv")
+            utils.warn("sample_n: empty header tsv")
             return self
 
         # validation
         if (n < 0):
             raise Exception("n cant be negative: {}".format(n))
 
         # check if n == 0
@@ -2467,15 +2670,15 @@
         return self.transform([col], lambda x: x, newcol, dmsg = dmsg)
 
     # sampling method to do class rebalancing where the class is defined by a specific col-value. As best practice,
     # the sampling ratios should be determined externally.
     def sample_class(self, col, col_value, sampling_ratio, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_class: empty tsv")
+            utils.warn("sample_class: empty header tsv")
             return self
 
         # Validation
         if (col not in self.header_map.keys()):
             raise Exception("Column not found: {}, {}".format(str(col), str(self.get_header_fields())))
 
         # cap the sampling ratio to 1
@@ -2536,15 +2739,15 @@
         # return
         return __sample_group_by_col_value_agg_func_inner__
 
     # sampling method where each sample group is restricted by the max values for a specific col-value. Useful for reducing skewness in dataset
     def sample_group_by_col_value(self, grouping_cols, col, col_value, sampling_ratio, seed = 0, use_numeric = False, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_group_by_col_value: empty tsv")
+            utils.warn("sample_group_by_col_value: empty header tsv")
             return self
 
         # resolve grouping_cols
         grouping_cols = self.__get_matching_cols__(grouping_cols)
 
         # validation
         if (col not in self.header_map.keys()):
@@ -2583,15 +2786,15 @@
             return result_mp
         
         return __sample_group_by_max_uniq_values_exact_group_by_inner__
 
     def sample_group_by_max_uniq_values_exact(self, grouping_cols, col, max_uniq_values, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_group_by_max_uniq_values_exact: empty tsv")
+            utils.warn("sample_group_by_max_uniq_values_exact: empty header tsv")
             return self
 
         # check for no data
         if (self.num_rows() == 0):
             return self
 
         # resolve grouping_cols
@@ -2621,15 +2824,15 @@
     def __sample_group_by_max_uniq_values_approx_uniq_count__(self, vs):
         return len(set(vs))
 
     # sampling method to take a grouping key, and a column where the number of unique values for column are capped. this uses approximate sampling technique
     def sample_group_by_max_uniq_values_approx(self, grouping_cols, col, max_uniq_values, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_group_by_max_uniq_values_approx: empty tsv")
+            utils.warn("sample_group_by_max_uniq_values_approx: empty header tsv")
             return self
 
         # check seed
         if (seed is None or seed < 0):
             raise Exception("Invalid seed: {}".format(seed))
 
         # resolve grouping_cols
@@ -2677,15 +2880,15 @@
     def __sample_group_by_max_uniq_values_per_class_uniq_count__(self, vs):
         return len(set(vs))
 
     # sampling method to take a grouping key, and a column where the number of unique values for column are capped.
     def sample_group_by_max_uniq_values_per_class(self, grouping_cols, class_col, col, max_uniq_values_map, def_max_uniq_values = None , seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_group_by_max_uniq_values_per_class: empty tsv")
+            utils.warn("sample_group_by_max_uniq_values_per_class: empty header tsv")
             return self
 
         # resolve grouping_cols
         grouping_cols = self.__get_matching_cols__(grouping_cols)
 
         # validation
         if (col not in self.header_map.keys()):
@@ -2723,15 +2926,15 @@
         # return
         return agg_result
 
     # random sampling within a group
     def sample_group_by_key(self, grouping_cols, sampling_ratio, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_group_by_key: empty tsv")
+            utils.warn("sample_group_by_key: empty header tsv")
             return self
 
         # resolve grouping_cols
         grouping_cols = self.__get_matching_cols__(grouping_cols)
 
         # check sampling ratio
         if (sampling_ratio < 0 or sampling_ratio > 1):
@@ -2758,15 +2961,15 @@
         # return
         return TSV(self.header, new_data)
 
     # sample by taking only n number of unique values for a specific column
     def sample_column_by_max_uniq_values(self, col, max_uniq_values, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("sample_column_by_max_uniq_values: empty tsv")
+            utils.warn("sample_column_by_max_uniq_values: empty header tsv")
             return self
 
         # get unique values
         uniq_values = self.col_as_array_uniq(col)
 
         # this random number is only for basic sampling and not for doing anything sensitive.
         random.seed(seed)  # nosec
@@ -3082,15 +3285,15 @@
         # return
         return result 
 
     # method to do map join. The right side is stored in a hashmap. only applicable to inner joins
     def natural_join(self, that, dmsg = ""):
         # check for empty
         if (self.has_empty_header()):
-            utils.warn("natural_join: empty tsv")
+            utils.warn("natural_join: empty header tsv")
             return that
 
         # find the list of common cols
         keys = sorted(list(set(self.get_header_fields()).intersection(set(that.get_header_fields()))))
 
         # create hashmap
         rmap = {}
@@ -3215,15 +3418,15 @@
                 rvalue_indexes.append(that.get_header_map()[h])
 
         # check the lengths
         if (len(lkeys) != len(rkeys)):
             raise Exception("Length mismatch in lkeys and rkeys: {}, {}".format(lkeys, rkeys))
 
         # print stats for left and right side
-        utils.debug("__map_join__: left num_rows: {}, right num_rows: {}".format(self.num_rows(), that.num_rows()))
+        utils.trace("__map_join__: left num_rows: {}, right num_rows: {}".format(self.num_rows(), that.num_rows()))
 
         # Check for num_par. TODO: Experimental
         if (num_par > 0):
             # split left and right sides
             left_batches = self.__split_batches_by_cols__(num_par, lkeys, seed = seed)
             right_batches = that.__split_batches_by_cols__(num_par, rkeys, seed = seed)
 
@@ -3375,22 +3578,22 @@
 
     # public method handling both random and cols based splitting
     def split_batches(self, num_batches, cols = None, preserve_order = False, seed = None, dmsg = ""):
         # check for empty
         if (self.has_empty_header()):
             # check for cols
             if (cols is None):
-                utils.warn("split_batches: empty tsv")
+                utils.warn("split_batches: empty header tsv")
                 return [self]
             else:
-                raise Exception("split_batches: empty tsv")
+                raise Exception("split_batches: empty header tsv")
 
         # check for empty rows
         if (self.num_rows() == 0):
-            utils.warn("split_batches: empty tsv")
+            utils.warn("split_batches: empty data tsv")
             return [self]
 
         # check if cols are defined or not
         dmsg = utils.extend_inherit_message(dmsg, "split_batches")
         if (cols is None):
             return self.__split_batches_randomly__(num_batches, preserve_order = preserve_order, seed = seed, dmsg = dmsg)
         else:
@@ -3500,15 +3703,15 @@
         # return
         return new_tsvs
 
     # method to generate a hash for a given set of columns
     def generate_key_hash(self, cols, new_col, seed = 0, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("generate_key_hash: empty tsv")
+            raise Exception("generate_key_hash: empty header tsv")
 
         # resolve cols
         cols = self.__get_matching_cols__(cols)
         indexes = self.__get_col_indexes__(cols)
 
         # validation
         if (new_col in self.get_columns()):
@@ -3536,15 +3739,15 @@
 
         # return
         return TSV(new_header, new_data)
 
     def cumulative_sum(self, col, new_col, as_int = True):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("cumulative_sum: empty tsv")
+            raise Exception("cumulative_sum: empty header tsv")
 
         # check for presence of col
         if (col not in self.header_map.keys()):
             raise Exception("Column not found: {}, {}".format(str(col), str(self.get_header_fields())))
 
         # check for validity of new col
         if (new_col in self.header_map.keys()):
@@ -3575,15 +3778,15 @@
 
         # return
         return TSV(new_header, new_data)
 
     def replicate_rows(self, col, new_col = None, max_repl = 0):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("replicate_rows: empty tsv")
+            raise Exception("replicate_rows: empty header tsv")
 
         # check for presence of col
         if (col not in self.header_map.keys()):
             raise Exception("Column not found: {}, {}".format(str(col), str(self.get_header_fields())))
 
         # create new column if it is not existing
         if (new_col is None):
@@ -3613,15 +3816,15 @@
     # default_val should be empty string
     # This doesnt handle empty data correctly. the output cols need add_empty_cols_if_missing
     def explode(self, cols, exp_func, prefix, default_val = None, collapse = True, ignore_if_missing = False, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "explode")
 
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("{}: empty tsv".format(dmsg), ignore_if_missing)
+            utils.raise_exception_or_warn("{}: empty header tsv".format(dmsg), ignore_if_missing)
             return self
 
         # get matching column and indexes
         matching_cols = self.__get_matching_cols__(cols, ignore_if_missing = ignore_if_missing)
         indexes = self.__get_col_indexes__(matching_cols)
 
         # check for no matching cols
@@ -3737,63 +3940,64 @@
                 new_data.append("\t".join(utils.merge_arrays([new_fields, new_vals])))
 
         # result. json expansion needs to be validated because of potential noise in the data.
         return TSV(new_header, new_data) \
             .validate()
 
     def __explode_json_transform_func__(self, col, accepted_cols, excluded_cols, single_value_list_cols, transpose_col_groups, merge_list_method, url_encoded_cols,
-        nested_cols, collapse_primitive_list, max_results = None, join_col = ","):
+        nested_cols, collapse_primitive_list, max_results = None, join_col = ",", dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "__explode_json_transform_func__")
 
         # constant
         json_explode_index = "__explode_json_index__"
 
         # inner function that is returned
         def __explode_json_transform_func_inner__(mp):
             # some validation.
             if (col not in mp.keys() or mp[col] == "" or mp[col] is None):
-                utils.trace_once("__explode_json_transform_func_inner__: potentially invalid json response found. Usually it is okay. But better to check: {}, {}".format(col, mp))
+                utils.trace_once("{}: __explode_json_transform_func_inner__: potentially invalid json response found. Usually it is okay. But better to check: {}, {}".format(dmsg, col, mp))
                 mp = {"__explode_json_len__": "0"}
                 return [mp]
 
             # fetch the json string, it might be url encoded or not though recommendation is to use url encoding.
             json_str = mp[col]
             json_mp = None
 
             # best effort in detecting the type and parsing for robustness
             if (json_str.startswith("%7B") == False and json_str.startswith("%5B") == False):
                 if (json_str.startswith("{") or json_str.startswith("[")):
-                    utils.warn_once("explode_json called with column that is not url encoded json. Assuming plain json string")
+                    utils.warn_once("{}: called with column that is not url encoded json. Assuming plain json string".format(dmsg))
                     json_mp = json.loads(json_str)
                 else:
                     json_str10 = json_str[0:10] + "..." if (len(json_str) > 10) else json_str
-                    utils.warn("explode_json called with invalid value in the string. Ignoring parsing: {}".format(json_str10))
+                    utils.warn("{}: called with invalid value in the string. Ignoring parsing: {}".format(dmsg, json_str10))
                     mp = {"__explode_json_len__": "0"}
                     return [mp]
             else:
                 json_mp = json.loads(utils.url_decode(json_str))
 
             # call internal methods
             results = __explode_json_transform_func_inner_helper__(json_mp)
 
             # Check if the number of results need to be capped
             if (max_results is not None and len(results) > max_results):
-                utils.warn("__explode_json_transform_func__: capping the number of results from {} to {}".format(len(results), max_results))
+                utils.warn("{}: capping the number of results from {} to {}".format(dmsg, len(results), max_results))
                 results = results[0:max_results]
 
             # return
             return results
 
         def __explode_json_transform_func_inner_helper__(json_mp):
             # validation
             if (transpose_col_groups is not None and merge_list_method == "join"):
                 raise Exception("transpose_col_groups can not be used with join method. Please use cogroup or unset transpose_col_groups")
 
             # check if top level is a list
             if (isinstance(json_mp, list)):
-                utils.debug("top level is a list. converting to a map")
+                utils.debug("{}: top level is a list. converting to a map".format(dmsg))
                 return __explode_json_transform_func_inner_helper__({col: json_mp})
 
             # use inner functions to parse the json
             results = __explode_json_transform_func_expand_json__(json_mp)
 
             # return
             return results
@@ -3819,15 +4023,15 @@
 
                 # get value
                 v = json_mp[k]
 
                 # handle null scenario. json string can have a special value called null to represent empty or null value, which is converted to None in json parser.
                 # such null value should be okay to read as empty string
                 if (v is None):
-                    utils.warn_once("__explode_json_transform_func_expand_json__: None type value found. Taking it as empty string. Key: {}".format(k))
+                    utils.debug_once("{}: __explode_json_transform_func_expand_json__: None type value found. Taking it as empty string. Key: {}".format(dmsg, k))
                     v = ""
 
                 # handle nested_cols scenario where the entire value is to be set as url encoded json blob
                 if (nested_cols is not None and k in nested_cols):
                     single_results[k + ":json:url_encoded"] = utils.url_encode(json.dumps(v))
                 # for each data type, there is a different kind of handling
                 elif (isinstance(v, (str, int, float))):
@@ -3839,15 +4043,15 @@
                     else:
                         single_results[k] = v1
                 else:
                     # TODO :Added on 2021-11-27. Need the counts for arrays and dict to handle 0 count errors. Splitting the single if-elif-else to two level
                     if (isinstance(v, list) and len(v) > 0):
                         single_results[k + ":__explode_json_len__"] = str(len(v))
                         if (len(list_results_arr) > 0 and utils.is_debug()):
-                            utils.warn_once("explode_json: multiple lists are not fully supported. Confirm data parsing or Use accepted_cols or excluded_cols: {}".format(str(k)))
+                            utils.warn_once("{}: multiple lists are not fully supported. Confirm data parsing or Use accepted_cols or excluded_cols: {}".format(dmsg, str(k)))
 
                         # create a new entry for holding the list array
                         list_results_arr.append([])
 
                         # check for base data types
                         if (isinstance(v[0], (str,int,float))):
                             # treat primitive lists as single value or as yet another list
@@ -3908,15 +4112,15 @@
                             else:
                                 raise Exception("Inner lists are not supported. Use accepted_cols or excluded_cols: {}".format(str(k)))
                         else:
                             raise Exception("Unknown data type: {}".format(type(v[0])))
                     elif (isinstance(v, dict) and len(v) > 0):
                         # warn for non trivial case
                         if (len(dict_results) > 0 and utils.is_debug()):
-                            utils.warn_once("explode_json: multiple maps are not fully supported. Confirm data parsing or Use accepted_cols or excluded_cols: {}".format(str(k)))
+                            utils.warn_once("{}: multiple maps are not fully supported. Confirm data parsing or Use accepted_cols or excluded_cols: {}".format(dmsg, str(k)))
 
                         # recursive call
                         mp2_list = __explode_json_transform_func_expand_json__(v, parent_prefix = parent_with_child_key)
 
                         # check if it was a flat hashmap or a nested. if flat, use dict_list else use list_results_arr
                         if (len(mp2_list) > 1):
                             list_results_arr.append([])
@@ -4024,15 +4228,16 @@
                          mp_new[k] = str(combined_map[k])
                      results.append(mp_new)
             else:
                 results.append(combined_map)
 
             # trace
             if (len(results) >= 100):
-                utils.trace("__explode_json_transform_func_expand_json__: with count: {} >= 10, parent_prefix: {}, results[0]: {}".format(len(results), parent_prefix, results[0]))
+                utils.trace("{}: __explode_json_transform_func_expand_json__: with count: {} >= 100, parent_prefix: {}, results[0]: {}".format(dmsg, len(results),
+                    parent_prefix, results[0]))
 
             # return
             return results
 
         def __explode_json_transform_func_join_lists__(list_results_arr):
             if (len(list_results_arr) == 0):
                 return {}
@@ -4062,50 +4267,50 @@
     # TODO: the json col is expected to be in url_encoded form otherwise does best effort guess
     # TODO: url_encoded_cols, excluded_cols, accepted_cols are actually json hashmap keys and not xpath
     # TODO: __explode_json_index__ needs to be tested and confirmed
     # TODO: need proper xpath based exclusion to better handle noise
     def explode_json(self, col, prefix = None, accepted_cols = None, excluded_cols = None, single_value_list_cols = None, transpose_col_groups = None,
         merge_list_method = "cogroup", collapse_primitive_list = True, url_encoded_cols = None, nested_cols = None, collapse = True, max_results = None, ignore_if_missing = False,
         default_val = "", dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "explode_json")
 
         # validation
         if (prefix is None):
-            utils.warn("explode_json: prefix = None is deprecated. Using the original column name as prefix: {}".format(col))
+            utils.warn("{}: prefix = None is deprecated. Using the original column name as prefix: {}".format(dmsg, col))
             prefix = col
 
         # check empty
         if (self.has_empty_header()):
-            utils.raise_exception_or_warn("explode_json: empty tsv", ignore_if_missing)
+            utils.raise_exception_or_warn("{}: empty header tsv".format(dmsg), ignore_if_missing)
             return self
 
         # warn
         if (excluded_cols is not None):
-            utils.print_code_todo_warning("explode_json: excluded_cols is work in progress and may not work in all scenarios")
+            utils.print_code_todo_warning("{}: excluded_cols is work in progress and may not work in all scenarios".format(dmsg))
 
         # validation
         if (col not in self.header_map.keys()):
-            utils.raise_exception_or_warn("Column not found: {}, {}".format(str(col), str(self.get_header_fields())), ignore_if_missing)
+            utils.raise_exception_or_warn("{}: Column not found: {}, {}".format(dmsg, str(col), str(self.get_header_fields())), ignore_if_missing)
             return self
 
         # warn on risky combinations
         if (merge_list_method == "cogroup"):
-            utils.print_code_todo_warning("explode_json: merge_list_method = cogroup is only meant for data exploration. Use merge_list_method = join for generating all combinations for multiple list values")
+            utils.print_code_todo_warning("{}: merge_list_method = cogroup is only meant for data exploration. Use merge_list_method = join for generating all combinations for multiple list values".format(dmsg))
 
         # name prefix
         if (prefix is None):
-            utils.warn("explode_json: prefix is None. Using col as the name prefix")
+            utils.warn("{}: prefix is None. Using col as the name prefix".format(dmsg))
             prefix = col
 
         # check for explode function
         exp_func = self.__explode_json_transform_func__(col, accepted_cols = accepted_cols, excluded_cols = excluded_cols, single_value_list_cols = single_value_list_cols,
             transpose_col_groups = transpose_col_groups, merge_list_method = merge_list_method, url_encoded_cols = url_encoded_cols, nested_cols = nested_cols,
-            collapse_primitive_list = collapse_primitive_list, max_results = max_results)
+            collapse_primitive_list = collapse_primitive_list, max_results = max_results, dmsg = dmsg)
 
         # use explode to do this parsing
-        dmsg = utils.extend_inherit_message(dmsg, "explode_json")
         return self \
             .add_seq_num(prefix + ":__json_index__", dmsg = dmsg) \
             .explode([col], exp_func, prefix = prefix, default_val = default_val, collapse = collapse, dmsg = dmsg) \
             .validate()
 
     def transpose(self, n = 1, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "transpose")
@@ -4131,15 +4336,15 @@
         # return
         return TSV(new_header, new_data)
 
     # this method converts the rows into columns. very inefficient
     def reverse_transpose(self, grouping_cols, transpose_key, transpose_cols, default_val = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("reverse_transpose empty tsv")
+            raise Exception("reverse_transpose empty header tsv")
 
         utils.print_code_todo_warning("reverse_transpose: is not implemented efficiently")
         # resolve the grouping and transpose_cols
         grouping_cols = self.__get_matching_cols__(grouping_cols)
         transpose_cols = self.__get_matching_cols__(transpose_cols)
 
         # get the columns to be selected for each tsv
@@ -4160,15 +4365,15 @@
 
         # return result
         return result
 
     def flatmap(self, col, func, new_col):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("flatmap: empty tsv")
+            raise Exception("flatmap: empty header tsv")
 
         # validation
         if (col not in self.header_map.keys()):
             raise Exception("Column not found: {}, {}".format(str(col), str(self.get_header_fields())))
 
         # check for new column
         if (new_col in self.header_map.keys()):
@@ -4187,15 +4392,15 @@
                 new_data.append(line + "\t" + new_val)
 
         return TSV(new_header, new_data)
 
     def to_tuples(self, cols, dmsg = ""):
         # check empty
         if (self.has_empty_header()):
-            raise Exception("to_tuples: empty tsv")
+            raise Exception("to_tuples: empty header tsv")
 
         # validate cols
         for col in cols:
             if (self.has_col(col) == False):
                 raise Exception("col doesnt exist: {}, {}".format(col, str(self.get_header_fields())))
 
         # select the cols
@@ -4299,28 +4504,28 @@
         raise Exception("Not implemented yet")
 
     def get_col_index(self, col):
         utils.warn("Use get_column_index and remove this function")
 
         # check empty
         if (self.has_empty_header()):
-            raise Exception("get_col_index: empty tsv")
+            raise Exception("get_col_index: empty header tsv")
 
         # validation
         if (col not in self.get_columns()):
             raise Exception("Column not found: {}".format(col))
 
         # return
         return self.header_map[col]
 
     # method to return a unique hash for the tsv objet
     def get_hash(self):
         # check empty
         if (self.has_empty_header()):
-            utils.warn("get_hash: empty tsv")
+            utils.warn("get_hash: empty header tsv")
 
         # create array
         hashes = []
 
         # hash of header
         hashes.append("{}".format(utils.compute_hash(self.header)))
 
@@ -4348,26 +4553,31 @@
         self \
             .custom_func(func, *args, **kwargs) \
             .show(n = n, title = title)
 
         # return self
         return self
 
-    def show_group_count(self, col_or_cols, n = 20, title = "Group Count", max_col_width = 40, sort_by_key = False, dmsg = ""):
+    def show_group_count(self, col_or_cols, n = 20, title = "Group Count", max_col_width = 40, sort_by_key = False, seq_col = "sno", dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "show_group_count")
 
         # call show transpose after custom func
         result = self \
             .group_count(col_or_cols, dmsg = dmsg)
 
         # sorting
         if (sort_by_key == True):
             result = result \
                 .sort(col_or_cols)
 
+        # add seq num 
+        if (seq_col is not None):
+            result = result \
+                .add_seq_num(seq_col)
+
         # show
         result \
             .show(n = n, title = title, max_col_width = max_col_width, dmsg = dmsg)
 
         # return self
         return self
 
@@ -4422,14 +4632,15 @@
 
         # return
         return True
 
     # this is a utility function that takes list of column names that support regular expression.
     # col_or_cols is a special variable that can be either single column name or an array. python
     # treats a string as an array of characters, so little hacky but a more intuitive api wise
+    # TODO: mp.keys() doesnt return a list and can break the string matching
     def __get_matching_cols__(self, col_or_cols, ignore_if_missing = False):
         # handle boundary conditions
         if (col_or_cols is None or len(col_or_cols) == 0):
             return []
 
         # check for wild card
         if (col_or_cols == ".*" or col_or_cols[0] == ".*"):
```

### Comparing `omigo_core-0.5.0/src/omigo_core/tsvutils.py` & `omigo_core-0.5.1/src/omigo_core/tsvutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return tsv.create_empty()
 
     # warn if a huge tsv is found 
     for i in range(len(tsv_list)):
         if (tsv_list[i].size_in_gb() >= 1):
             utils.warn("merge: Found a very big tsv: {} / {}, num_rows: {}, size (GB): {}. max_size_cols_stats: {}".format(
                 i + 1, len(tsv_list), tsv_list[i].num_rows(), tsv_list[i].size_in_gb(), str(tsv_list[i].get_max_size_cols_stats())))
-            # tsv_list[i].show_transpose(1, title = "merge: big tsv")
+            tsv_list[i].show_transpose(1, title = "merge: big tsv")
 
     # check for valid headers
     header = tsv_list[0].get_header()
     header_fields = tsv_list[0].get_header_fields()
 
     # iterate to check mismatch in header
     index = 0
```

### Comparing `omigo_core-0.5.0/src/omigo_core/utils.py` & `omigo_core-0.5.1/src/omigo_core/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -519,7 +519,125 @@
      return "{}: {}".format(old_msg, new_msg) if (old_msg is not None and len(old_msg) > 0) else "{}".format(new_msg)
 
 def max_dmsg_str(dmsg, max_len = 300):
     if (dmsg is None or len(dmsg) <= max_len):
         return dmsg
     else:
         return "{}... ".format(dmsg[0:max_len - 4])
+
+def is_tsv_file_extension(path):
+    # check extensions
+    if (path.endswith(".tsv") or path.endswith(".tsv.gz") or path.endswith(".csv") or path.endswith(".csv.gz")):
+        return True
+    else:
+        return False
+
+# TODO: Move this to proper package 
+class CombGenerator:
+    def __init__(self):
+        self.comb1_cache = {}
+        self.comb2_cache = {}
+        self.comb3_cache = {}
+        self.comb4_cache = {}
+        self.comb5_cache = {}
+        self.comb6_cache = {}
+        self.comb7_cache = {}
+
+    def gen_comb1(self, n):
+        if (n not in self.comb1_cache.keys()):
+            self.comb1_cache[n] = self.__gen_comb1__(n)
+        return self.comb1_cache[n]
+
+    def gen_comb2(self, n):
+        if (n not in self.comb2_cache.keys()):
+            self.comb2_cache[n] = self.__gen_comb2__(n)
+        return self.comb2_cache[n]
+
+    def gen_comb3(self, n):
+        if (n not in self.comb3_cache.keys()):
+            self.comb3_cache[n] = self.__gen_comb3__(n)
+        return self.comb3_cache[n]
+
+    def gen_comb4(self, n):
+        if (n not in self.comb4_cache.keys()):
+            self.comb4_cache[n] = self.__gen_comb4__(n)
+        return self.comb4_cache[n]
+
+    def gen_comb5(self, n):
+        if (n not in self.comb5_cache.keys()):
+            self.comb5_cache[n] = self.__gen_comb5__(n)
+        return self.comb5_cache[n]
+
+    def gen_comb6(self, n):
+        if (n not in self.comb6_cache.keys()):
+            self.comb6_cache[n] = self.__gen_comb6__(n)
+        return self.comb6_cache[n]
+
+    def gen_comb7(self, n):
+        if (n not in self.comb7_cache.keys()):
+            self.comb7_cache[n] = self.__gen_comb7__(n)
+        return self.comb7_cache[n]
+
+    def __gen_comb1__(self, n):
+       result = []
+       for i1 in range(0, n):
+           result.append([i1])
+       return result
+    
+    def __gen_comb2__(self, n):
+       result = []
+       for i2 in range(0, n-1):
+           for i1 in range(i2+1, n):
+               result.append([i2, i1])
+       return result
+    
+    def __gen_comb3__(self, n):
+       result = []
+       for i3 in range(0, n-2):
+           for i2 in range(i3+1, n-1):
+               for i1 in range(i2+1, n):
+                   result.append([i3, i2, i1])
+       return result
+    
+    def __gen_comb4__(self, n):
+       result = []
+       for i4 in range(0, n-3):
+           for i3 in range(i4+1, n-2):
+               for i2 in range(i3+1, n-1):
+                   for i1 in range(i2+1, n):
+                       result.append([i4, i3, i2, i1])
+       return result
+    
+    def __gen_comb5__(self, n):
+       result = []
+       for i5 in range(0, n-4):
+           for i4 in range(i5+1, n-3):
+               for i3 in range(i4+1, n-2):
+                   for i2 in range(i3+1, n-1):
+                       for i1 in range(i2+1, n):
+                           result.append([i5, i4, i3, i2, i1])
+       return result
+    
+    def __gen_comb6__(self, n):
+       result = []
+       for i6 in range(0, n-5):
+           for i5 in range(i6+1, n-4):
+               for i4 in range(i5+1, n-3):
+                   for i3 in range(i4+1, n-2):
+                       for i2 in range(i3+1, n-1):
+                           for i1 in range(i2+1, n):
+                               result.append([i6, i5, i4, i3, i2, i1])
+       return result
+    
+    def __gen_comb7__(self, n):
+       result = []
+       for i7 in range(0, n-6):
+           for i6 in range(i7+1, n-5):
+               for i5 in range(i6+1, n-4):
+                   for i4 in range(i5+1, n-3):
+                       for i3 in range(i4+1, n-2):
+                           for i2 in range(i3+1, n-1):
+                               for i1 in range(i2+1, n):
+                                   result.append([i7, i6, i5, i4, i3, i2, i1])
+       return result
+
+
```

### Comparing `omigo_core-0.5.0/src/omigo_core.egg-info/PKG-INFO` & `omigo_core-0.5.1/src/omigo_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo-core
-Version: 0.5.0
+Version: 0.5.1
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.0/src/omigo_core.egg-info/SOURCES.txt` & `omigo_core-0.5.1/src/omigo_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

