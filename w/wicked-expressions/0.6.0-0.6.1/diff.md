# Comparing `tmp/wicked_expressions-0.6.0.tar.gz` & `tmp/wicked_expressions-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.6.0.tar", max compression
+gzip compressed data, was "wicked_expressions-0.6.1.tar", max compression
```

## Comparing `wicked_expressions-0.6.0.tar` & `wicked_expressions-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-05-15 18:09:05.160196 wicked_expressions-0.6.0/LICENSE
--rw-r--r--   0        0        0     2119 2023-05-15 18:09:05.160196 wicked_expressions-0.6.0/README.md
--rw-r--r--   0        0        0     1219 2023-05-15 18:10:36.521298 wicked_expressions-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-15 18:10:36.501288 wicked_expressions-0.6.0/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      819 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     7975 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     8309 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/datastash.bolt
--rw-r--r--   0        0        0     1850 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      341 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8524 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1221 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     5253 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-05-15 18:09:05.168197 wicked_expressions-0.6.0/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-25 20:58:54.292242 wicked_expressions-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2119 2023-05-25 20:58:54.292242 wicked_expressions-0.6.1/README.md
+-rw-r--r--   0        0        0     1219 2023-05-25 21:00:52.877227 wicked_expressions-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-25 21:00:52.853227 wicked_expressions-0.6.1/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-25 20:58:54.300243 wicked_expressions-0.6.1/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     7975 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      341 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8524 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1221 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     5253 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.1/PKG-INFO
```

### Comparing `wicked_expressions-0.6.0/LICENSE` & `wicked_expressions-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/README.md` & `wicked_expressions-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/pyproject.toml` & `wicked_expressions-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.6.0"
+version = "0.6.1"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/api.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from bolt_expressions import Expression
 
 from ./sources import ScoreSource, DataSource
 from ./comparison import ExpressionComparison
 from ./raw_operations import StoreExpressionValue, GetExpressionValue
 from ./var import Var, StaticVar
 from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List
-from ./datastash import DataStash
+# from ./datastash import DataStash
 from ./rebindable import Rebindable
 
 import ./internal_api as internal_api
 
 
 Scoreboard = ctx.inject(internal_api.Scoreboard)
 Data = ctx.inject(internal_api.Data)
 
 this = Data.entity('@s')
 
 
 ExpressionComparison.monkeypatch(Scoreboard, Data, ScoreSource, DataSource)
 StoreExpressionValue.monkeypatch(ScoreSource, DataSource)
 GetExpressionValue.monkeypatch(ScoreSource, DataSource)
-DataStash.monkeypatch(Scoreboard, Data)
+# DataStash.monkeypatch(Scoreboard, Data)
```

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.6.1/wicked_expressions/modules/var_sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.0/PKG-INFO` & `wicked_expressions-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.6.0
+Version: 0.6.1
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

