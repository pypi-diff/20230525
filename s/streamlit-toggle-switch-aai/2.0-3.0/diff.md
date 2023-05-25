# Comparing `tmp/streamlit_toggle_switch_aai-2.0.tar.gz` & `tmp/streamlit_toggle_switch_aai-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_toggle_switch_aai-2.0.tar", last modified: Thu May 25 21:01:58 2023, max compression
+gzip compressed data, was "streamlit_toggle_switch_aai-3.0.tar", last modified: Thu May 25 21:18:40 2023, max compression
```

## Comparing `streamlit_toggle_switch_aai-2.0.tar` & `streamlit_toggle_switch_aai-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:58.062912 streamlit_toggle_switch_aai-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:01:41.000000 streamlit_toggle_switch_aai-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:01:41.000000 streamlit_toggle_switch_aai-2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 21:01:58.062912 streamlit_toggle_switch_aai-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:01:41.000000 streamlit_toggle_switch_aai-2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:01:58.062912 streamlit_toggle_switch_aai-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-25 21:01:41.000000 streamlit_toggle_switch_aai-2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:58.062912 streamlit_toggle_switch_aai-2.0/streamlit_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-25 21:01:41.000000 streamlit_toggle_switch_aai-2.0/streamlit_toggle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:58.062912 streamlit_toggle_switch_aai-2.0/streamlit_toggle_switch_aai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 21:01:58.000000 streamlit_toggle_switch_aai-2.0/streamlit_toggle_switch_aai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 21:01:58.000000 streamlit_toggle_switch_aai-2.0/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:01:58.000000 streamlit_toggle_switch_aai-2.0/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:01:58.000000 streamlit_toggle_switch_aai-2.0/streamlit_toggle_switch_aai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:01:58.000000 streamlit_toggle_switch_aai-2.0/streamlit_toggle_switch_aai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:40.313310 streamlit_toggle_switch_aai-3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:18:28.000000 streamlit_toggle_switch_aai-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:18:28.000000 streamlit_toggle_switch_aai-3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 21:18:40.313310 streamlit_toggle_switch_aai-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:18:28.000000 streamlit_toggle_switch_aai-3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:18:40.313310 streamlit_toggle_switch_aai-3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-25 21:18:28.000000 streamlit_toggle_switch_aai-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:40.313310 streamlit_toggle_switch_aai-3.0/streamlit_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-25 21:18:28.000000 streamlit_toggle_switch_aai-3.0/streamlit_toggle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:40.313310 streamlit_toggle_switch_aai-3.0/streamlit_toggle_switch_aai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 21:18:40.000000 streamlit_toggle_switch_aai-3.0/streamlit_toggle_switch_aai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 21:18:40.000000 streamlit_toggle_switch_aai-3.0/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:18:40.000000 streamlit_toggle_switch_aai-3.0/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:18:40.000000 streamlit_toggle_switch_aai-3.0/streamlit_toggle_switch_aai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:18:40.000000 streamlit_toggle_switch_aai-3.0/streamlit_toggle_switch_aai.egg-info/top_level.txt
```

### Comparing `streamlit_toggle_switch_aai-2.0/LICENSE` & `streamlit_toggle_switch_aai-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-2.0/README.md` & `streamlit_toggle_switch_aai-3.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-2.0/setup.py` & `streamlit_toggle_switch_aai-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_toggle_switch_aai",
-    version="2.0",
+    version="3.0",
     author="Carlos D. Serrano",
     author_email="sqlinsights@gmail.com",
     description="Creates a customizable toggle",
     long_description="",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/streamlit-toggle-switch",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_toggle_switch_aai-2.0/streamlit_toggle/__init__.py` & `streamlit_toggle_switch_aai-3.0/streamlit_toggle/__init__.py`

 * *Files identical despite different names*

