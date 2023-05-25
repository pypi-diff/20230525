# Comparing `tmp/pymender-0.0.3.tar.gz` & `tmp/pymender-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymender-0.0.3.tar", last modified: Thu May 25 19:42:14 2023, max compression
+gzip compressed data, was "pymender-0.0.4.tar", last modified: Thu May 25 19:46:45 2023, max compression
```

## Comparing `pymender-0.0.3.tar` & `pymender-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:14.627253 pymender-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 19:42:14.627253 pymender-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 19:42:05.000000 pymender-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:14.627253 pymender-0.0.3/pymender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:14.627253 pymender-0.0.3/pymender/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/commands/fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:14.627253 pymender-0.0.3/pymender/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-25 19:42:05.000000 pymender-0.0.3/pymender/commands/tests/test_fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:14.627253 pymender-0.0.3/pymender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 19:42:14.000000 pymender-0.0.3/pymender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 19:42:14.000000 pymender-0.0.3/pymender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:42:14.000000 pymender-0.0.3/pymender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 19:42:14.000000 pymender-0.0.3/pymender.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:42:14.000000 pymender-0.0.3/pymender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 19:42:14.000000 pymender-0.0.3/pymender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 19:42:05.000000 pymender-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 19:42:05.000000 pymender-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:42:14.627253 pymender-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.675695 pymender-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 19:46:45.671695 pymender-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 19:46:36.000000 pymender-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/tests/test_fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 19:46:36.000000 pymender-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 19:46:36.000000 pymender-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:46:45.675695 pymender-0.0.4/setup.cfg
```

### Comparing `pymender-0.0.3/PKG-INFO` & `pymender-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pymender
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 
 # PyMender
 
 Uses the excellent [libCST](https://github.com/Instagram/LibCST) to perform entire codebase refactors.
 
 ## Usage
 
 ```bash
-pip install pymender==0.0.3
+pip install pymender==0.0.4
 
 
 # Run a particular codemod
 python3 -m pymender <codemod> <path_to_project>
 # e.g.
 python3 -m pymender FastAPIAnnotated <path_to_project>
```

### Comparing `pymender-0.0.3/pymender/cli.py` & `pymender-0.0.4/pymender/cli.py`

 * *Files identical despite different names*

### Comparing `pymender-0.0.3/pymender/commands/fastapi_annotated.py` & `pymender-0.0.4/pymender/commands/fastapi_annotated.py`

 * *Files identical despite different names*

### Comparing `pymender-0.0.3/pymender/commands/tests/test_fastapi_annotated.py` & `pymender-0.0.4/pymender/commands/tests/test_fastapi_annotated.py`

 * *Files identical despite different names*

### Comparing `pymender-0.0.3/pymender.egg-info/PKG-INFO` & `pymender-0.0.4/pymender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pymender
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 
 # PyMender
 
 Uses the excellent [libCST](https://github.com/Instagram/LibCST) to perform entire codebase refactors.
 
 ## Usage
 
 ```bash
-pip install pymender==0.0.3
+pip install pymender==0.0.4
 
 
 # Run a particular codemod
 python3 -m pymender <codemod> <path_to_project>
 # e.g.
 python3 -m pymender FastAPIAnnotated <path_to_project>
```

### Comparing `pymender-0.0.3/pyproject.toml` & `pymender-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymender"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = ["dependencies", "readme"]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
@@ -12,18 +12,18 @@
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 
 [project.scripts]
-cli-name = "pymender:__main__"
+pymender = "pymender.cli:main"
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

