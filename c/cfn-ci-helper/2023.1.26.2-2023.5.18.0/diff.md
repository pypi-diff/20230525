# Comparing `tmp/cfn-ci-helper-2023.1.26.2.tar.gz` & `tmp/cfn-ci-helper-2023.5.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-ci-helper-2023.1.26.2.tar", last modified: Fri Jan 27 00:52:39 2023, max compression
+gzip compressed data, was "cfn-ci-helper-2023.5.18.0.tar", last modified: Thu May 25 21:42:14 2023, max compression
```

## Comparing `cfn-ci-helper-2023.1.26.2.tar` & `cfn-ci-helper-2023.5.18.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:52:39.487297 cfn-ci-helper-2023.1.26.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-27 00:52:39.487297 cfn-ci-helper-2023.1.26.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:52:39.483297 cfn-ci-helper-2023.1.26.2/cfnStack/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/cfnStack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/cfnStack/default_stack.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/cfnStack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:52:39.487297 cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-27 00:52:39.000000 cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-27 00:52:39.000000 cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 00:52:39.000000 cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-27 00:52:39.000000 cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-27 00:52:39.000000 cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/deploy_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-27 00:52:23.000000 cfn-ci-helper-2023.1.26.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-27 00:52:39.487297 cfn-ci-helper-2023.1.26.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:42:14.317302 cfn-ci-helper-2023.5.18.0/cfnStack/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/cfnStack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/cfnStack/default_stack.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/cfnStack/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/deploy_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/setup.cfg
```

### Comparing `cfn-ci-helper-2023.1.26.2/LICENSE` & `cfn-ci-helper-2023.5.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.1.26.2/PKG-INFO` & `cfn-ci-helper-2023.5.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.1.26.2
+Version: 2023.5.18.0
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.1.26.2/cfnStack/default_stack.yaml.jinja` & `cfn-ci-helper-2023.5.18.0/cfnStack/default_stack.yaml.jinja`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.1.26.2/cfnStack/stack.py` & `cfn-ci-helper-2023.5.18.0/cfnStack/stack.py`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.1.26.2/cfn_ci_helper.egg-info/PKG-INFO` & `cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.1.26.2
+Version: 2023.5.18.0
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.1.26.2/deploy_cf.py` & `cfn-ci-helper-2023.5.18.0/deploy_cf.py`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.1.26.2/setup.cfg` & `cfn-ci-helper-2023.5.18.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cfn-ci-helper
-version = 2023.01.26.2
+version = 2023.05.18.0
 author = Chris Halbersma
 author_email = chris@halbersma.us
 description = A Cloudformation CI Helper System
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chalbersma/cfn-ci-helper
 classifiers =
```

