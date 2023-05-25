# Comparing `tmp/cq23-0.1.4.tar.gz` & `tmp/cq23-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-0.1.4.tar", last modified: Sat May 20 10:53:39 2023, max compression
+gzip compressed data, was "cq23-1.0.0.tar", last modified: Thu May 25 04:42:05 2023, max compression
```

## Comparing `cq23-0.1.4.tar` & `cq23-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:53:39.694452 cq23-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-20 10:53:39.694452 cq23-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 10:53:32.000000 cq23-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-20 10:53:32.000000 cq23-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-20 10:53:39.694452 cq23-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:53:39.694452 cq23-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:53:39.694452 cq23-0.1.4/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-20 10:53:39.000000 cq23-0.1.4/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-20 10:53:39.000000 cq23-0.1.4/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:53:39.000000 cq23-0.1.4/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 10:53:39.000000 cq23-0.1.4/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:53:39.694452 cq23-0.1.4/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:53:32.000000 cq23-0.1.4/src/run_game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.631007 cq23-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 04:42:05.631007 cq23-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 04:41:56.000000 cq23-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 04:41:56.000000 cq23-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-25 04:42:05.631007 cq23-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.627007 cq23-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.627007 cq23-1.0.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.631007 cq23-1.0.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 04:41:56.000000 cq23-1.0.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 04:41:56.000000 cq23-1.0.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 04:41:56.000000 cq23-1.0.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.631007 cq23-1.0.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/gcs.py
```

### Comparing `cq23-0.1.4/PKG-INFO` & `cq23-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 0.1.4
+Version: 1.0.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-0.1.4/setup.cfg` & `cq23-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 0.1.4
+version = 1.0.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls = 
@@ -16,18 +16,24 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
+install_requires = 
+	docker>=6.0.1
 
 [options.packages.find]
 where = src
 
+[options.entry_points]
+console_scripts = 
+	cq23 = main.command:route_command
+
 [flake8]
 max-line-length = 120
 exclude = .tox,.git,*/static/CACHE/*,docs,node_modules,venv
 
 [pycodestyle]
 max-line-length = 120
 exclude = .tox,.git,*/static/CACHE/*,docs,node_modules,venv
```

### Comparing `cq23-0.1.4/src/cq23.egg-info/PKG-INFO` & `cq23-1.0.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 0.1.4
+Version: 1.0.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

