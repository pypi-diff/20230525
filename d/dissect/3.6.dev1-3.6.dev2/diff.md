# Comparing `tmp/dissect-3.6.dev1.tar.gz` & `tmp/dissect-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect-3.6.dev1.tar", last modified: Tue May 16 13:25:36 2023, max compression
+gzip compressed data, was "dissect-3.6.dev2.tar", last modified: Thu May 25 08:03:54 2023, max compression
```

## Comparing `dissect-3.6.dev1.tar` & `dissect-3.6.dev2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:36.714911 dissect-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-16 13:25:21.000000 dissect-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:21.000000 dissect-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:21.000000 dissect-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-16 13:25:36.710911 dissect-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-16 13:25:21.000000 dissect-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:36.710911 dissect-3.6.dev1/dissect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 13:25:26.000000 dissect-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:36.714911 dissect-3.6.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 13:25:21.000000 dissect-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:03:54.308419 dissect-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 08:03:36.000000 dissect-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 08:03:36.000000 dissect-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 08:03:36.000000 dissect-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-25 08:03:54.308419 dissect-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-25 08:03:36.000000 dissect-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:03:54.308419 dissect-3.6.dev2/dissect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-25 08:03:42.000000 dissect-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:03:54.312419 dissect-3.6.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-25 08:03:36.000000 dissect-3.6.dev2/tox.ini
```

### Comparing `dissect-3.6.dev1/LICENSE` & `dissect-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect-3.6.dev1/PKG-INFO` & `dissect-3.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect-3.6.dev1/README.md` & `dissect-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect-3.6.dev1/dissect.egg-info/PKG-INFO` & `dissect-3.6.dev2/dissect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect-3.6.dev1/pyproject.toml` & `dissect-3.6.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 authors = [
   {name = "Dissect Team", email = "dissect@fox-it.com"}
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "dissect.cim==3.5",
-    "dissect.clfs==1.4",
-    "dissect.cstruct==3.6",
-    "dissect.esedb==3.6",
-    "dissect.etl==3.4",
-    "dissect.eventlog==3.4",
-    "dissect.evidence==3.4",
-    "dissect.executable==1.2",
-    "dissect.extfs==3.4",
-    "dissect.fat==3.4",
-    "dissect.ffs==3.4",
-    "dissect.hypervisor==3.6",
-    "dissect.ntfs==3.4",
-    "dissect.ole==3.4",
-    "dissect.regf==3.4",
-    "dissect.shellitem==3.4",
-    "dissect.sql==3.4",
-    "dissect.squashfs==1.1",
-    "dissect.target[full]==3.8",
-    "dissect.thumbcache==1.3",
-    "dissect.util==3.7",
-    "dissect.vmfs==3.4",
-    "dissect.volume==3.4",
-    "dissect.xfs==3.4",
+    "dissect.cim==3.6",
+    "dissect.clfs==1.5",
+    "dissect.cstruct==3.7",
+    "dissect.esedb==3.7",
+    "dissect.etl==3.5",
+    "dissect.eventlog==3.5",
+    "dissect.evidence==3.5",
+    "dissect.executable==1.3",
+    "dissect.extfs==3.5",
+    "dissect.fat==3.5",
+    "dissect.ffs==3.5",
+    "dissect.hypervisor==3.7",
+    "dissect.ntfs==3.5",
+    "dissect.ole==3.5",
+    "dissect.regf==3.5",
+    "dissect.shellitem==3.5",
+    "dissect.sql==3.5",
+    "dissect.squashfs==1.2",
+    "dissect.target[full]==3.9",
+    "dissect.thumbcache==1.4",
+    "dissect.util==3.8",
+    "dissect.vmfs==3.5",
+    "dissect.volume==3.5",
+    "dissect.xfs==3.5",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://dissect.tools"
 documentation = "https://docs.dissect.tools"
 repository = "https://github.com/fox-it/dissect"
```

### Comparing `dissect-3.6.dev1/tox.ini` & `dissect-3.6.dev2/tox.ini`

 * *Files identical despite different names*

