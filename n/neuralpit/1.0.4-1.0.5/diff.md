# Comparing `tmp/neuralpit-1.0.4.tar.gz` & `tmp/neuralpit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-1.0.4.tar", last modified: Tue May  9 09:01:44 2023, max compression
+gzip compressed data, was "neuralpit-1.0.5.tar", last modified: Wed May 24 13:49:02 2023, max compression
```

## Comparing `neuralpit-1.0.4.tar` & `neuralpit-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:01:44.380716 neuralpit-1.0.4/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 09:01:09.000000 neuralpit-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-09 09:01:44.380716 neuralpit-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-09 09:01:09.000000 neuralpit-1.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)      982 2023-05-09 09:01:09.000000 neuralpit-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 09:01:44.380716 neuralpit-1.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:01:44.380716 neuralpit-1.0.4/src/
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-09 09:01:09.000000 neuralpit-1.0.4/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:01:44.380716 neuralpit-1.0.4/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 09:01:09.000000 neuralpit-1.0.4/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:01:44.380716 neuralpit-1.0.4/src/neuralpit/explore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 09:01:09.000000 neuralpit-1.0.4/src/neuralpit/explore/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-09 09:01:09.000000 neuralpit-1.0.4/src/neuralpit/explore/data.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-09 09:01:09.000000 neuralpit-1.0.4/src/neuralpit/explore/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:01:44.380716 neuralpit-1.0.4/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-09 09:01:44.000000 neuralpit-1.0.4/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      360 2023-05-09 09:01:44.000000 neuralpit-1.0.4/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 09:01:44.000000 neuralpit-1.0.4/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-09 09:01:44.000000 neuralpit-1.0.4/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-09 09:01:44.000000 neuralpit-1.0.4/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:49:01.998288 neuralpit-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 13:48:27.000000 neuralpit-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-24 13:49:01.998288 neuralpit-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-24 13:48:27.000000 neuralpit-1.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-24 13:48:27.000000 neuralpit-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 13:49:01.998288 neuralpit-1.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:49:01.994288 neuralpit-1.0.5/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:49:01.994288 neuralpit-1.0.5/src/neuralpit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:49:01.998288 neuralpit-1.0.5/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/neuralpit/services/api.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/neuralpit/services/convert.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/neuralpit/services/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:49:01.998288 neuralpit-1.0.5/src/neuralpit/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/neuralpit/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-24 13:48:27.000000 neuralpit-1.0.5/src/neuralpit/tools/chat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:49:01.998288 neuralpit-1.0.5/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-24 13:49:01.000000 neuralpit-1.0.5/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2023-05-24 13:49:01.000000 neuralpit-1.0.5/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:49:01.000000 neuralpit-1.0.5/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-24 13:49:01.000000 neuralpit-1.0.5/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-24 13:49:01.000000 neuralpit-1.0.5/src/neuralpit.egg-info/top_level.txt
```

### Comparing `neuralpit-1.0.4/PKG-INFO` & `neuralpit-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.4
+Version: 1.0.5
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.4/pyproject.toml` & `neuralpit-1.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "1.0.4"
+version = "1.0.5"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["api", "neural", "neuralpit"]
 dependencies = [
+    "requests",
+    "lxml",
+    "toml",
+    "langchain",
+    "openai",
+    "bs4"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
@@ -30,8 +36,7 @@
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/__init__.py" = ["{version}"]
```

### Comparing `neuralpit-1.0.4/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-1.0.5/src/neuralpit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.4
+Version: 1.0.5
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

