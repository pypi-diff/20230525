# Comparing `tmp/numalogic_prometheus-0.4.0.tar.gz` & `tmp/numalogic_prometheus-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.4.0.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.4.1.tar", max compression
```

## Comparing `numalogic_prometheus-0.4.0.tar` & `numalogic_prometheus-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/LICENSE
--rw-r--r--   0        0        0      839 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/__init__.py
--rw-r--r--   0        0        0     1395 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1316 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2515 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4483 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/factory.py
--rw-r--r--   0        0        0     7002 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      747 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4339 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/inference.py
--rw-r--r--   0        0        0     6836 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     2768 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     4193 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4148 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     6965 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udsink/train.py
--rw-r--r--   0        0        0     8095 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5935 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/watcher.py
--rw-r--r--   0        0        0     1550 2023-05-24 21:36:52.443238 numalogic_prometheus-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 17:27:12.581593 numalogic_prometheus-0.4.1/LICENSE
+-rw-r--r--   0        0        0      839 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3565 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1316 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2515 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4483 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/factory.py
+-rw-r--r--   0        0        0     7002 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4339 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     6836 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     2768 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     4193 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4148 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     6965 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     8095 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5935 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/numaprom/watcher.py
+-rw-r--r--   0        0        0     1550 2023-05-25 17:27:12.585593 numalogic_prometheus-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.1/PKG-INFO
```

### Comparing `numalogic_prometheus-0.4.0/LICENSE` & `numalogic_prometheus-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/__init__.py` & `numalogic_prometheus-0.4.1/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/_config.py` & `numalogic_prometheus-0.4.1/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/_constants.py` & `numalogic_prometheus-0.4.1/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.4.1/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/clients/redis.py` & `numalogic_prometheus-0.4.1/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.4.1/numaprom/clients/sentinel.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/configs/config.yaml` & `numalogic_prometheus-0.4.1/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.4.1/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/entities.py` & `numalogic_prometheus-0.4.1/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/factory.py` & `numalogic_prometheus-0.4.1/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/tools.py` & `numalogic_prometheus-0.4.1/numaprom/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udf/filter.py` & `numalogic_prometheus-0.4.1/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udf/inference.py` & `numalogic_prometheus-0.4.1/numaprom/udf/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.4.1/numaprom/udf/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.4.1/numaprom/udf/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udf/threshold.py` & `numalogic_prometheus-0.4.1/numaprom/udf/threshold.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udf/window.py` & `numalogic_prometheus-0.4.1/numaprom/udf/window.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udsink/train.py` & `numalogic_prometheus-0.4.1/numaprom/udsink/train.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.4.1/numaprom/udsink/train_rollout.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/numaprom/watcher.py` & `numalogic_prometheus-0.4.1/numaprom/watcher.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.0/pyproject.toml` & `numalogic_prometheus-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.4.0"
+version = "0.4.1"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
```

### Comparing `numalogic_prometheus-0.4.0/PKG-INFO` & `numalogic_prometheus-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.4.0
+Version: 0.4.1
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
```

