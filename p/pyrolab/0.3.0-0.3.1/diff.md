# Comparing `tmp/PyroLab-0.3.0.tar.gz` & `tmp/PyroLab-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroLab-0.3.0.tar", last modified: Wed Mar  1 00:41:43 2023, max compression
+gzip compressed data, was "PyroLab-0.3.1.tar", last modified: Thu May 11 03:11:18 2023, max compression
```

## Comparing `PyroLab-0.3.0.tar` & `PyroLab-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-01 00:41:14.000000 PyroLab-0.3.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-01 00:41:14.000000 PyroLab-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-01 00:41:14.000000 PyroLab-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-01 00:41:14.000000 PyroLab-0.3.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    49794 2023-03-01 00:41:43.448003 PyroLab-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-01 00:41:14.000000 PyroLab-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-01 00:41:14.000000 PyroLab-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 00:41:43.448003 PyroLab-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/PyroLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49794 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/pyrolab/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/pyrolabd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/pyromonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/lister.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:11:18.851460 PyroLab-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-11 03:10:43.000000 PyroLab-0.3.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 03:10:43.000000 PyroLab-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 03:10:43.000000 PyroLab-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-11 03:10:43.000000 PyroLab-0.3.1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-05-11 03:11:18.851460 PyroLab-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-11 03:10:43.000000 PyroLab-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-11 03:10:43.000000 PyroLab-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 03:11:18.851460 PyroLab-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:11:18.847460 PyroLab-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:11:18.851460 PyroLab-0.3.1/src/PyroLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-05-11 03:11:18.000000 PyroLab-0.3.1/src/PyroLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-11 03:11:18.000000 PyroLab-0.3.1/src/PyroLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 03:11:18.000000 PyroLab-0.3.1/src/PyroLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 03:11:18.000000 PyroLab-0.3.1/src/PyroLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 03:11:18.000000 PyroLab-0.3.1/src/PyroLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 03:11:18.000000 PyroLab-0.3.1/src/PyroLab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:11:18.851460 PyroLab-0.3.1/src/pyrolab/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/pyrolabd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyrolab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:11:18.851460 PyroLab-0.3.1/src/pyromonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyromonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyromonitor/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyromonitor/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-11 03:10:43.000000 PyroLab-0.3.1/src/pyromonitor/lister.py
```

### Comparing `PyroLab-0.3.0/AUTHORS.txt` & `PyroLab-0.3.1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/LICENSE` & `PyroLab-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/NOTICE.txt` & `PyroLab-0.3.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/PKG-INFO` & `PyroLab-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroLab
-Version: 0.3.0
+Version: 0.3.1
 Summary: A framework for using remote lab instruments as local resources built on Pyro5
 Author-email: Sequoia Ploeg <sequoiap4@gmail.com>, BYU CamachoLab <camacho@byu.edu>
 Maintainer-email: Sequoia Ploeg <sequoiap4@gmail.com>, BYU CamachoLab <camacho@byu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -707,24 +707,25 @@
 Provides-Extra: tsl550
 Provides-Extra: ppcl55x
 Provides-Extra: rto
 Provides-Extra: arduino
 Provides-Extra: monitor
 Provides-Extra: test
 License-File: LICENSE
+License-File: NOTICE.txt
 License-File: AUTHORS.txt
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/BYUCamachoLab/pyrolab/master/docs/_static/images/pyrolab_logo.svg" width="40%" alt="PyroLab">
 </p>
 
 ---
 
 <p align="center">
-<img alt="Development version" src="https://img.shields.io/badge/master-v0.3.0-informational">
+<img alt="Development version" src="https://img.shields.io/badge/master-v0.3.1-informational">
 <a href="https://pypi.python.org/pypi/pyrolab"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/pyrolab.svg"></a>
 <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pyrolab">
 <a href="https://pyrolab.readthedocs.io/"><img alt="Documentation Status" src="https://readthedocs.org/projects/pyrolab/badge/?version=latest"></a>
 <a href="https://pypi.python.org/pypi/pyrolab/"><img alt="License" src="https://img.shields.io/pypi/l/pyrolab.svg"></a>
 <a href="https://github.com/BYUCamachoLab/pyrolab/commits/master"><img alt="Latest Commit" src="https://img.shields.io/github/last-commit/BYUCamachoLab/pyrolab.svg"></a>
 </p>
 
@@ -895,15 +896,15 @@
 ```
 
 This will automatically create a git tag in the repository with the 
 corrresponding version number and commit the modified files (where version
 numbers were updated). Pushing the tags (a manual process) to the remote will 
 automatically create a new release. Releases are automatically published to 
 PyPI and GitHub when git tags matching the "v*" pattern are created 
-(e.g. "v0.3.0"), as bumpversion does.
+(e.g. "v0.3.1"), as bumpversion does.
 
 After bumping version, you can view the tags on the local machine by running 
 ``git tag``. To push the tags to the remote server and trigger the release
 workflow, you can run ``git push origin <tagname>``.
 
 For code quality, please run isort and black before committing (note that the
 latest release of isort may not work through VSCode's integrated terminal, and
```

### Comparing `PyroLab-0.3.0/README.md` & `PyroLab-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <p align="center">
 <img src="https://raw.githubusercontent.com/BYUCamachoLab/pyrolab/master/docs/_static/images/pyrolab_logo.svg" width="40%" alt="PyroLab">
 </p>
 
 ---
 
 <p align="center">
-<img alt="Development version" src="https://img.shields.io/badge/master-v0.3.0-informational">
+<img alt="Development version" src="https://img.shields.io/badge/master-v0.3.1-informational">
 <a href="https://pypi.python.org/pypi/pyrolab"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/pyrolab.svg"></a>
 <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pyrolab">
 <a href="https://pyrolab.readthedocs.io/"><img alt="Documentation Status" src="https://readthedocs.org/projects/pyrolab/badge/?version=latest"></a>
 <a href="https://pypi.python.org/pypi/pyrolab/"><img alt="License" src="https://img.shields.io/pypi/l/pyrolab.svg"></a>
 <a href="https://github.com/BYUCamachoLab/pyrolab/commits/master"><img alt="Latest Commit" src="https://img.shields.io/github/last-commit/BYUCamachoLab/pyrolab.svg"></a>
 </p>
 
@@ -180,15 +180,15 @@
 ```
 
 This will automatically create a git tag in the repository with the 
 corrresponding version number and commit the modified files (where version
 numbers were updated). Pushing the tags (a manual process) to the remote will 
 automatically create a new release. Releases are automatically published to 
 PyPI and GitHub when git tags matching the "v*" pattern are created 
-(e.g. "v0.3.0"), as bumpversion does.
+(e.g. "v0.3.1"), as bumpversion does.
 
 After bumping version, you can view the tags on the local machine by running 
 ``git tag``. To push the tags to the remote server and trigger the release
 workflow, you can run ``git push origin <tagname>``.
 
 For code quality, please run isort and black before committing (note that the
 latest release of isort may not work through VSCode's integrated terminal, and
```

### Comparing `PyroLab-0.3.0/pyproject.toml` & `PyroLab-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [project]
 name = "PyroLab"
-version = "0.3.0"
+version = "0.3.1"
 description = "A framework for using remote lab instruments as local resources built on Pyro5"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
-    "PyroLab", 
-    "Pyro5", 
-    "Pyro", 
-    "lab", 
-    "instrument", 
-    "remote", 
-    "resources", 
-    "framework", 
-    "laboratory", 
-    "instrumentation", 
-    "hardware", 
-    "science", 
-    "remote", 
-    "network", 
-    "integration"
+  "PyroLab", 
+  "Pyro5", 
+  "Pyro", 
+  "lab", 
+  "instrument", 
+  "remote", 
+  "resources", 
+  "framework", 
+  "laboratory", 
+  "instrumentation", 
+  "hardware", 
+  "science", 
+  "remote", 
+  "network", 
+  "integration",
 ]
 
 # This should be your name or the name of the organization who originally
 # authored the project, and a valid email address corresponding to the name
 # listed.
 authors = [
   {name = "Sequoia Ploeg", email = "sequoiap4@gmail.com" },
@@ -62,15 +62,14 @@
 dependencies = [
   "numpy",
   "scipy",
   "Pyro5",
   "pydantic",
   "pyyaml",
   "deprecation",
-  "appnope",
   "typer",
   "colorama",
   "tabulate",
   "requests",
   "packaging>=23.0",
 ]
```

### Comparing `PyroLab-0.3.0/src/PyroLab.egg-info/PKG-INFO` & `PyroLab-0.3.1/src/PyroLab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroLab
-Version: 0.3.0
+Version: 0.3.1
 Summary: A framework for using remote lab instruments as local resources built on Pyro5
 Author-email: Sequoia Ploeg <sequoiap4@gmail.com>, BYU CamachoLab <camacho@byu.edu>
 Maintainer-email: Sequoia Ploeg <sequoiap4@gmail.com>, BYU CamachoLab <camacho@byu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -707,24 +707,25 @@
 Provides-Extra: tsl550
 Provides-Extra: ppcl55x
 Provides-Extra: rto
 Provides-Extra: arduino
 Provides-Extra: monitor
 Provides-Extra: test
 License-File: LICENSE
+License-File: NOTICE.txt
 License-File: AUTHORS.txt
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/BYUCamachoLab/pyrolab/master/docs/_static/images/pyrolab_logo.svg" width="40%" alt="PyroLab">
 </p>
 
 ---
 
 <p align="center">
-<img alt="Development version" src="https://img.shields.io/badge/master-v0.3.0-informational">
+<img alt="Development version" src="https://img.shields.io/badge/master-v0.3.1-informational">
 <a href="https://pypi.python.org/pypi/pyrolab"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/pyrolab.svg"></a>
 <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pyrolab">
 <a href="https://pyrolab.readthedocs.io/"><img alt="Documentation Status" src="https://readthedocs.org/projects/pyrolab/badge/?version=latest"></a>
 <a href="https://pypi.python.org/pypi/pyrolab/"><img alt="License" src="https://img.shields.io/pypi/l/pyrolab.svg"></a>
 <a href="https://github.com/BYUCamachoLab/pyrolab/commits/master"><img alt="Latest Commit" src="https://img.shields.io/github/last-commit/BYUCamachoLab/pyrolab.svg"></a>
 </p>
 
@@ -895,15 +896,15 @@
 ```
 
 This will automatically create a git tag in the repository with the 
 corrresponding version number and commit the modified files (where version
 numbers were updated). Pushing the tags (a manual process) to the remote will 
 automatically create a new release. Releases are automatically published to 
 PyPI and GitHub when git tags matching the "v*" pattern are created 
-(e.g. "v0.3.0"), as bumpversion does.
+(e.g. "v0.3.1"), as bumpversion does.
 
 After bumping version, you can view the tags on the local machine by running 
 ``git tag``. To push the tags to the remote server and trigger the release
 workflow, you can run ``git push origin <tagname>``.
 
 For code quality, please run isort and black before committing (note that the
 latest release of isort may not work through VSCode's integrated terminal, and
```

### Comparing `PyroLab-0.3.0/src/PyroLab.egg-info/SOURCES.txt` & `PyroLab-0.3.1/src/PyroLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/__init__.py` & `PyroLab-0.3.1/src/pyrolab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     )
 
 
 # Metadata
 __name__ = "PyroLab"
 __author__ = "CamachoLab"
 __copyright__ = "Copyright 2020, The PyroLab Project"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __license__ = "GPLv3+"
 __maintainer__ = "Sequoia Ploeg"
 __maintainer_email__ = "sequoia.ploeg@byu.edu"
 __status__ = "Development" # "Production"
 __project_url__ = "https://github.com/sequoiap/pyrolab"
 __forum_url__ = "https://github.com/sequoiap/pyrolab/issues"
 __website_url__ = "https://camacholab.byu.edu/"
```

### Comparing `PyroLab-0.3.0/src/pyrolab/api.py` & `PyroLab-0.3.1/src/pyrolab/api.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/cli.py` & `PyroLab-0.3.1/src/pyrolab/cli.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/configure.py` & `PyroLab-0.3.1/src/pyrolab/configure.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/manager.py` & `PyroLab-0.3.1/src/pyrolab/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,17 +214,14 @@
         daemon = self.daemonconfig._get_daemon()
         daemon = daemon()
 
         uris = {}
         for sname, sconfig in self.serviceconfigs.items():
             log.info(f"Registering service '{sname}'")
             service = sconfig._get_service()
-
-            log.debug("Preparing daemon class")
-            service = daemon.prepare_class(service)
             
             log.debug("Getting service uri")
             uri = daemon.register(service)
             uris[sname] = uri
         
         if self.daemonconfig.nameservers:
             log.debug("Self-registering daemon")
```

### Comparing `PyroLab-0.3.0/src/pyrolab/nameserver.py` & `PyroLab-0.3.1/src/pyrolab/nameserver.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/pyrolabd.py` & `PyroLab-0.3.1/src/pyrolab/pyrolabd.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/server.py` & `PyroLab-0.3.1/src/pyrolab/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -167,23 +167,42 @@
         server socket.
     """
     # TODO: Implement methods that allow a client to view and forcibly close 
     # connections to this Daemon.
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
+    def register(self, obj_or_class, objectId=None, force=False, weak=False):
+        """
+        Register a Pyro object under the given id. 
+        
+        Note that this object is now only known inside this daemon, it is not
+        automatically available in a name server. This method returns a URI for
+        the registered object. Pyro checks if an object is already registered,
+        unless you set force=True. You can register a class or an object
+        (instance) directly. For a class, Pyro will create instances of it to
+        handle the remote calls according to the instance_mode (set via @expose
+        on the class). The default there is one object per session (=proxy
+        connection). If you register an object directly, Pyro will use that
+        single object for all remote calls. With weak=True, only weak reference
+        to the object will be stored, and the object will get unregistered from
+        the daemon automatically when garbage-collected.
+        """
+        obj_or_class = self._prepare_class(obj_or_class)
+        return super().register(obj_or_class, objectId=objectId, force=force, weak=weak)
+
     @staticmethod
-    def prepare_class(cls) -> Type[Service]:
+    def _prepare_class(cls) -> Type[Service]:
         """
         Performs any actions on the class required for the given Daemon.
 
         Some classes require mixins to be added in order for certain 
-        functionality to work. When the ProcessManager prepares to run a Daemon,
-        the child process will call this method on the class before registering
-        the class.
+        functionality to work. This method is called by 
+        :py:meth:`pyrolab.server.Daemon.register` before passing the 
+        registration on to the Pyro5 daemon.
 
         Parameters
         ----------
         cls : class
             The class to prepare.
         
         Returns
@@ -256,36 +275,40 @@
         server socket.
     """
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.locked_instances = {}
 
     @staticmethod
-    def prepare_class(cls) -> Type[Service]:
+    def _prepare_class(cls) -> Type[Service]:
         """
         Dynamically create a new class that is also based on Lockable.
 
         Parameters
         ----------
         cls : class
             The class to be used as a template while dynamically creating a new
             class.
         
         Returns
         -------
         class
             A subclass that inherits from the original class and ``Lockable``.
         """
+        if issubclass(type(cls), Daemon):
+            return cls
+        
         DynamicLockable = type(
             cls.__name__ + "Lockable",
             (cls, Lockable, ),
             {}
         )
         return DynamicLockable
 
+
     def _lock(self, pyroId: str, conn: SocketConnection, user: str="") -> bool:
         """
         Logs a "lock" action on a Pyro object.
         
         LockableDaemon tracks which connection owns the lock over a given Pyro
         object.
 
@@ -407,14 +430,15 @@
         obj = super()._getInstance(clazz, conn)
         if issubclass(obj.__class__, Lockable):
             lock_owner, username = self.locked_instances.get(obj._pyroId, (None, ""))
             if lock_owner is None or lock_owner == conn:
                 return obj
             if lock_owner != conn:
                 raise ConnectionRefusedError(f"Pyro object is locked (by '{username or lock_owner}')")
+        return obj
 
     def clientDisconnect(self, conn):
         """
         Automatically releases any locked resources in the event of a client 
         disconnect.
 
         Parameters
```

### Comparing `PyroLab-0.3.0/src/pyrolab/service.py` & `PyroLab-0.3.1/src/pyrolab/service.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyrolab/utils.py` & `PyroLab-0.3.1/src/pyrolab/utils.py`

 * *Files identical despite different names*

### Comparing `PyroLab-0.3.0/src/pyromonitor/__init__.py` & `PyroLab-0.3.1/src/pyromonitor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     )
 
 
 # Metadata
 __name__ = "pyromonitor"
 __author__ = "BYU CamachoLab"
 __copyright__ = "Copyright 2023, The PyroLab Project"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __license__ = "GPLv3+"
 __maintainer__ = "Sequoia Ploeg"
 __maintainer_email__ = "sequoiac@byu.edu"
 __status__ = "Development" # "Production"
 __project_url__ = "https://github.com/sequoiap/pyrolab"
 __forum_url__ = "https://github.com/sequoiap/pyrolab/issues"
 __website_url__ = "https://camacholab.byu.edu/"
```

### Comparing `PyroLab-0.3.0/src/pyromonitor/cli.py` & `PyroLab-0.3.1/src/pyromonitor/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,11 +67,11 @@
     
     from pyromonitor import create_app
     webapp = create_app()
 
     from waitress import serve
     uri = f'{CONFIG.host}:{CONFIG.port}'
     
-    print(f"\n    Serving on http://{uri}")
+    print(f"\n    Serving on http://{uri}/{CONFIG.subfolder}")
     print(f"    (press CTRL+C to quit)\n")
 
     serve(webapp, listen=uri, threads=4, clear_untrusted_proxy_headers=True)
```

### Comparing `PyroLab-0.3.0/src/pyromonitor/lister.py` & `PyroLab-0.3.1/src/pyromonitor/lister.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,15 +92,18 @@
 
     with locate_ns(CONFIG.nameserver) as ns:
         instruments: dict = ns.list(return_metadata=True) # {name: (uri, description)}
         instruments.pop("Pyro.NameServer") # no need to display the nameserver
         
     status = []
     for name, (uri, description) in instruments.items():
-        description = list(description)[0]
+        try:
+            description = list(description)[0]
+        except:
+            description = 'Not available'
         if len(description) > 80:
             description = description[:77] + "..."
         try:
             with Proxy(ns.lookup(name)) as p:
                 version = p.pyrolab_version()
                 status.append(InstrumentStatus(name, uri, description, version, AVAILABLE))
         except ConnectionRefusedError as e:
@@ -109,21 +112,20 @@
             status.append(InstrumentStatus(name, uri, description, "", UNREACHABLE))
 
     _last_updated = datetime.now()
     _status = status
     reset_timer()
 
 
-@bp.route('/', methods=["GET"])
+@bp.route(f'/{CONFIG.subfolder}', methods=["GET"])
 def listall():
     global _last_updated
     global _status
 
     updated = f"{time_elapsed_human_readable(_last_updated)} ago"
-    status = sorted([stat for stat in _status if stat.status == AVAILABLE], key=lambda x: x.name) + \
-             sorted([stat for stat in _status if stat.status == LOCKED], key=lambda x: x.name) + \
+    status = sorted([stat for stat in _status if stat.status in [AVAILABLE, LOCKED]], key=lambda x: x.name) + \
              sorted([stat for stat in _status if stat.status == UNREACHABLE], key=lambda x: x.name)
 
     return render_template('base.html', status=status, update_time=updated)
 
 
 refresh_status()
```

