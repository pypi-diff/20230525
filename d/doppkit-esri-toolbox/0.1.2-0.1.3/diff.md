# Comparing `tmp/doppkit-esri-toolbox-0.1.2.tar.gz` & `tmp/doppkit-esri-toolbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-esri-toolbox-0.1.2.tar", last modified: Mon May 22 16:13:15 2023, max compression
+gzip compressed data, was "doppkit-esri-toolbox-0.1.3.tar", last modified: Thu May 25 21:11:33 2023, max compression
```

## Comparing `doppkit-esri-toolbox-0.1.2.tar` & `doppkit-esri-toolbox-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/arcpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.373572 doppkit-esri-toolbox-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.373572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/arcpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.373572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/gp/Fetch_Export_grid access.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.Fetch_Export.pyt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt.xml
```

### Comparing `doppkit-esri-toolbox-0.1.2/LICENSE` & `doppkit-esri-toolbox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.2/PKG-INFO` & `doppkit-esri-toolbox-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit-esri-toolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-esri-toolbox-0.1.2/README.md` & `doppkit-esri-toolbox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.2/pyproject.toml` & `doppkit-esri-toolbox-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -18,17 +18,22 @@
     { name = "Ognyan Moore", email = "ogi@hobu.co" },
 ]
 
 [project.urls]
 homepage = "https://github.com/hobuinc/doppkit-esri-toolbox"
 repository = "https://github.com/hobuinc/doppkit-esri-toolbox"
 
-[tool.setuptools]
-package-dir = {"" =  "src"}
-zip-safe = false
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+doppkit_toolbox = ["*.xml"]
+"doppkit_toolbox.esri.help.gp" = ["*.xml"]
+"doppkit_toolbox.esri.help.gp.toolboxes" = ["*.xml"]
+"doppkit_toolbox.esri.toolboxes" = ["*.pyt", "*.xml"]
 
 [tool.setuptools.dynamic]
 version = { attr = "doppkit_toolbox.__version__" }
 readme = { file = "README.md", content-type = "text/markdown" }
 
 [build-system]
 requires = ["setuptools>=64.0"]
```

### Comparing `doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/PKG-INFO` & `doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit-esri-toolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py` & `doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py`

 * *Files identical despite different names*

