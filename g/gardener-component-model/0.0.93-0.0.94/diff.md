# Comparing `tmp/gardener-component-model-0.0.93.tar.gz` & `tmp/gardener-component-model-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-component-model-0.0.93.tar", last modified: Fri May 19 05:47:01 2023, max compression
+gzip compressed data, was "gardener-component-model-0.0.94.tar", last modified: Thu May 25 10:25:45 2023, max compression
```

## Comparing `gardener-component-model-0.0.93.tar` & `gardener-component-model-0.0.94.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/gardener_component_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/gci/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/gci/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-05-19 05:44:43.000000 gardener-component-model-0.0.93/gci/component-descriptor.json-schema.yaml
--rw-r--r--   0 root         (0) root         (0)    17784 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/gci/componentmodel.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/gci/oci.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      942 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:25:45.886357 gardener-component-model-0.0.94/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-25 10:25:45.882357 gardener-component-model-0.0.94/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:25:45.882357 gardener-component-model-0.0.94/gardener_component_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-25 10:25:45.000000 gardener-component-model-0.0.94/gardener_component_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-25 10:25:45.000000 gardener-component-model-0.0.94/gardener_component_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:25:45.000000 gardener-component-model-0.0.94/gardener_component_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-25 10:25:45.000000 gardener-component-model-0.0.94/gardener_component_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-25 10:25:45.000000 gardener-component-model-0.0.94/gardener_component_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:25:45.882357 gardener-component-model-0.0.94/gci/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-25 10:24:22.000000 gardener-component-model-0.0.94/gci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-05-25 10:24:23.000000 gardener-component-model-0.0.94/gci/component-descriptor.json-schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    17784 2023-05-25 10:24:22.000000 gardener-component-model-0.0.94/gci/componentmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-05-25 10:24:22.000000 gardener-component-model-0.0.94/gci/oci.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:25:45.886357 gardener-component-model-0.0.94/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      942 2023-05-25 10:24:22.000000 gardener-component-model-0.0.94/setup.py
```

### Comparing `gardener-component-model-0.0.93/gci/component-descriptor.json-schema.yaml` & `gardener-component-model-0.0.94/gci/component-descriptor.json-schema.yaml`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.93/gci/componentmodel.py` & `gardener-component-model-0.0.94/gci/componentmodel.py`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.93/gci/oci.py` & `gardener-component-model-0.0.94/gci/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.93/setup.py` & `gardener-component-model-0.0.94/setup.py`

 * *Files identical despite different names*

