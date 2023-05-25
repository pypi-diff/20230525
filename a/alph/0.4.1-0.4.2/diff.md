# Comparing `tmp/alph-0.4.1.tar.gz` & `tmp/alph-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alph-0.4.1.tar", last modified: Wed Feb  1 17:20:05 2023, max compression
+gzip compressed data, was "alph-0.4.2.tar", last modified: Thu May 25 12:41:51 2023, max compression
```

## Comparing `alph-0.4.1.tar` & `alph-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 17:20:05.333301 alph-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-01 17:18:05.000000 alph-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-02-01 17:20:05.333301 alph-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-02-01 17:18:05.000000 alph-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 17:20:05.333301 alph-0.4.1/alph/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 17:18:05.000000 alph-0.4.1/alph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-01 17:20:04.000000 alph-0.4.1/alph/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-02-01 17:18:05.000000 alph-0.4.1/alph/combo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-02-01 17:18:05.000000 alph-0.4.1/alph/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-02-01 17:18:05.000000 alph-0.4.1/alph/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-02-01 17:18:05.000000 alph-0.4.1/alph/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-01 17:18:05.000000 alph-0.4.1/alph/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-01 17:18:05.000000 alph-0.4.1/alph/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 17:20:05.333301 alph-0.4.1/alph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-02-01 17:20:05.000000 alph-0.4.1/alph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-01 17:20:05.000000 alph-0.4.1/alph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 17:20:05.000000 alph-0.4.1/alph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-01 17:20:05.000000 alph-0.4.1/alph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-01 17:20:05.000000 alph-0.4.1/alph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 17:20:05.333301 alph-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-01 17:18:05.000000 alph-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:41:51.334094 alph-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 12:39:46.000000 alph-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-25 12:41:51.334094 alph-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-05-25 12:39:46.000000 alph-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:41:51.330093 alph-0.4.2/alph/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 12:39:46.000000 alph-0.4.2/alph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 12:41:50.000000 alph-0.4.2/alph/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-25 12:39:46.000000 alph-0.4.2/alph/combo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-25 12:39:46.000000 alph-0.4.2/alph/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-25 12:39:46.000000 alph-0.4.2/alph/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-25 12:39:46.000000 alph-0.4.2/alph/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-25 12:39:46.000000 alph-0.4.2/alph/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-25 12:39:46.000000 alph-0.4.2/alph/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:41:51.334094 alph-0.4.2/alph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:41:51.334094 alph-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 12:39:46.000000 alph-0.4.2/setup.py
```

### Comparing `alph-0.4.1/LICENSE` & `alph-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/PKG-INFO` & `alph-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alph
-Version: 0.4.1
+Version: 0.4.2
 Summary: alph
 Home-page: https://github.com/connectedcompany/alph
 Author: Uros Rapajic
 License: UNKNOWN
 Description: # **alph** - <b>al</b>tair for your gra<b>ph</b>
         
         A Python library using [Altair](https://altair-viz.github.io/) for declarative, data-driven network visualisation.
```

### Comparing `alph-0.4.1/README.md` & `alph-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/alph/combo.py` & `alph-0.4.2/alph/combo.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/alph/core.py` & `alph-0.4.2/alph/core.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/alph/layers.py` & `alph-0.4.2/alph/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 def _wrap_altair_str_value(val):
     if isinstance(val, str):
         return alt.value(val)
     return val
 
 
 def _nx_nodes_to_pandas(G, pos):
-    attributes = set(["x", "y"] + [k for n in G.nodes() for k in G.nodes[n].keys()])
+    attributes = list(
+        set(["x", "y"] + [k for n in G.nodes() for k in G.nodes[n].keys()])
+    )
 
     df = pd.DataFrame(index=G.nodes(), columns=attributes)
 
     for n in G.nodes:
         data = dict(x=pos[n][0], y=pos[n][1], **G.nodes[n])
         df.loc[n] = data
```

### Comparing `alph-0.4.1/alph/layout.py` & `alph-0.4.2/alph/layout.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/alph/preproc.py` & `alph-0.4.2/alph/preproc.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/alph/util.py` & `alph-0.4.2/alph/util.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.1/alph.egg-info/PKG-INFO` & `alph-0.4.2/alph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alph
-Version: 0.4.1
+Version: 0.4.2
 Summary: alph
 Home-page: https://github.com/connectedcompany/alph
 Author: Uros Rapajic
 License: UNKNOWN
 Description: # **alph** - <b>al</b>tair for your gra<b>ph</b>
         
         A Python library using [Altair](https://altair-viz.github.io/) for declarative, data-driven network visualisation.
```

### Comparing `alph-0.4.1/setup.py` & `alph-0.4.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     author="Uros Rapajic",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/connectedcompany/alph",
     license_files=["LICENSE"],
     install_requires=[
         "altair>=4.1.0",
-        "jsonschema<4.17",  # TEMPORARY - until fix for this is merged into altair: https://github.com/altair-viz/altair/issues/2705, either via 5.0 or via intermediate release - https://github.com/altair-viz/altair/pull/2827
+        "jsonschema<4.17",  # TEMPORARY - only required for altair < 5, due to https://github.com/altair-viz/altair/issues/2705
         "networkx>=2.6.3",
-        "pandas<1.5.0",  # 1.5.0 causes ValueError: columns cannot be a set when plotting altair facets
+        "pandas>=1.3.5",
         "scikit-network>=0.27.1",
-        # "cython fa2 @ git+https://github.com/connectedcompany/forceatlas2.git",
+        # also cython, fa2, @ git+https://github.com/connectedcompany/forceatlas2.git"
     ],
     extras_require={
         "graphviz": [
             "pygraphviz>=1.10",
         ],
     },
     python_requires=">=3.8",
```

