# Comparing `tmp/py-partiql-parser-0.3.0.tar.gz` & `tmp/py-partiql-parser-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.3.0.tar", last modified: Sun Apr 16 13:50:03 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.3.1.tar", last modified: Thu May 25 12:46:16 2023, max compression
```

## Comparing `py-partiql-parser-0.3.0.tar` & `py-partiql-parser-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.470916 py-partiql-parser-0.3.0/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-16 13:49:56.000000 py-partiql-parser-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.603204 py-partiql-parser-0.3.1/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.603204 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-25 12:46:06.000000 py-partiql-parser-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 12:46:16.611204 py-partiql-parser-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.3.0/LICENSE` & `py-partiql-parser-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/PKG-INFO` & `py-partiql-parser-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.3.0/README.md` & `py-partiql-parser-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/json_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from json import JSONEncoder
 from typing import Dict, Any, List, Union
 
 from .clause_tokenizer import ClauseTokenizer
 from .case_insensitive_dict import CaseInsensitiveDict
 
 ACCEPTED_QUOTES = ["'", '"', "’"]
 NEW_LINE = "\n"
@@ -189,7 +190,14 @@
                 tokenizer.skip_white_space()
             elif not section:
                 current_phrase += c
                 section = "VAR_VALUE"
             elif section in ["VALUE", "VAR_VALUE"]:
                 current_phrase += c
         return result
+
+
+class SelectEncoder(JSONEncoder):
+    def default(self, o):
+        if isinstance(o, Variable) and o.value is None:
+            return None
+        return o
```

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.3.1/py_partiql_parser/_internal/where_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.3.1/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.3.0/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.3.1/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_csv_converter.py` & `py-partiql-parser-0.3.1/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.3.1/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_from_parser.py` & `py-partiql-parser-0.3.1/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_json_parser.py` & `py-partiql-parser-0.3.1/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_query_metadata.py` & `py-partiql-parser-0.3.1/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_s3_examples.py` & `py-partiql-parser-0.3.1/tests/test_s3_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import pytest
 import sure  # noqa
-from py_partiql_parser import S3SelectParser
+from py_partiql_parser import S3SelectParser, SelectEncoder
 from . import input_json_list, json_as_lines
 
 
 # https://aws.amazon.com/blogs/storage/querying-data-without-servers-or-databases-using-amazon-s3-select/
 
 
 input_data_csv = """Name,PhoneNumber,City,Occupation
@@ -159,7 +159,23 @@
         + "\n"
         + json.dumps({"Name": "Vinod", "City": "Los Angeles"})
     )
     parser = S3SelectParser(source_data={"s3object": all_rows})
     assert parser.parse(query, parameters=None) == [
         {"Name": "Vinod", "City": "Los Angeles"}
     ]
+
+
+def test_json_output_can_be_dumped():
+    query = "select * from s3object s"
+    input_with_none = json.dumps(
+        [
+            {
+                "name": "Janelyn M",
+                "date": "2020-02-23T00:00:00",
+                "city": "Chicago",
+                "kids": None,
+            },
+        ]
+    )
+    result = S3SelectParser(source_data={"s3object": input_with_none}).parse(query)
+    assert input_with_none == json.dumps(result, cls=SelectEncoder)
```

### Comparing `py-partiql-parser-0.3.0/tests/test_select_functions.py` & `py-partiql-parser-0.3.1/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_select_parser.py` & `py-partiql-parser-0.3.1/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_utils.py` & `py-partiql-parser-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.0/tests/test_where_parser.py` & `py-partiql-parser-0.3.1/tests/test_where_parser.py`

 * *Files identical despite different names*

