# Comparing `tmp/hashkern-0.3.0.tar.gz` & `tmp/hashkern-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashkern-0.3.0.tar", last modified: Thu May 25 21:34:52 2023, max compression
+gzip compressed data, was "hashkern-0.3.1.tar", last modified: Thu May 25 21:41:58 2023, max compression
```

## Comparing `hashkern-0.3.0.tar` & `hashkern-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.610741 hashkern-0.3.0/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    11344 2023-01-13 23:42:17.000000 hashkern-0.3.0/LICENSE
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14845 2023-05-25 21:34:52.610741 hashkern-0.3.0/PKG-INFO
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14112 2023-05-25 21:09:44.000000 hashkern-0.3.0/README.md
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       38 2023-05-25 21:34:52.610741 hashkern-0.3.0/setup.cfg
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     1230 2023-05-25 21:01:42.000000 hashkern-0.3.0/setup.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.606741 hashkern-0.3.0/src/
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.606741 hashkern-0.3.0/src/hash/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      239 2023-05-10 20:44:27.000000 hashkern-0.3.0/src/hash/__init__.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.606741 hashkern-0.3.0/src/hash/cli/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       23 2023-01-14 12:45:56.000000 hashkern-0.3.0/src/hash/cli/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5912 2023-05-25 20:39:35.000000 hashkern-0.3.0/src/hash/cli/main.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7189 2023-01-13 23:42:17.000000 hashkern-0.3.0/src/hash/dag.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     2148 2023-05-14 21:16:53.000000 hashkern-0.3.0/src/hash/errors.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.610741 hashkern-0.3.0/src/hash/kern/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      148 2023-05-25 21:01:54.000000 hashkern-0.3.0/src/hash/kern/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    10412 2023-05-15 21:31:58.000000 hashkern-0.3.0/src/hash/kern/action.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7361 2023-05-25 20:39:35.000000 hashkern-0.3.0/src/hash/kern/execute.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      931 2023-01-26 22:20:41.000000 hashkern-0.3.0/src/hash/kern/hash.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3196 2023-05-25 20:39:35.000000 hashkern-0.3.0/src/hash/kern/main.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    16126 2023-05-25 20:39:35.000000 hashkern-0.3.0/src/hash/kern/planner.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     4181 2023-05-21 16:39:22.000000 hashkern-0.3.0/src/hash/kern/secrets.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    19277 2023-05-10 20:44:27.000000 hashkern-0.3.0/src/hash/kern/state.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5952 2023-05-15 21:31:58.000000 hashkern-0.3.0/src/hash/kern/templates.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3461 2023-01-13 23:42:17.000000 hashkern-0.3.0/src/hash/logs.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.610741 hashkern-0.3.0/src/hash/resources/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       69 2023-05-14 22:02:35.000000 hashkern-0.3.0/src/hash/resources/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    97796 2023-05-25 20:39:36.000000 hashkern-0.3.0/src/hash/resources/base.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    22702 2023-05-15 21:31:58.000000 hashkern-0.3.0/src/hash/resources/targets.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.610741 hashkern-0.3.0/src/hash/store/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       59 2023-01-13 23:42:17.000000 hashkern-0.3.0/src/hash/store/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    28132 2023-05-25 20:39:35.000000 hashkern-0.3.0/src/hash/store/base.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    12523 2023-05-21 16:41:33.000000 hashkern-0.3.0/src/hash/utils.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:34:52.610741 hashkern-0.3.0/src/hashkern.egg-info/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14845 2023-05-25 21:34:52.000000 hashkern-0.3.0/src/hashkern.egg-info/PKG-INFO
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      738 2023-05-25 21:34:52.000000 hashkern-0.3.0/src/hashkern.egg-info/SOURCES.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        1 2023-05-25 21:34:52.000000 hashkern-0.3.0/src/hashkern.egg-info/dependency_links.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       39 2023-05-25 21:34:52.000000 hashkern-0.3.0/src/hashkern.egg-info/entry_points.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      199 2023-05-25 21:34:52.000000 hashkern-0.3.0/src/hashkern.egg-info/requires.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        5 2023-05-25 21:34:52.000000 hashkern-0.3.0/src/hashkern.egg-info/top_level.txt
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.656200 hashkern-0.3.1/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    11344 2023-01-13 23:42:17.000000 hashkern-0.3.1/LICENSE
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14840 2023-05-25 21:41:58.656200 hashkern-0.3.1/PKG-INFO
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14107 2023-05-25 21:38:34.000000 hashkern-0.3.1/README.md
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       38 2023-05-25 21:41:58.656200 hashkern-0.3.1/setup.cfg
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     1230 2023-05-25 21:40:19.000000 hashkern-0.3.1/setup.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.648200 hashkern-0.3.1/src/
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.652200 hashkern-0.3.1/src/hash/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      239 2023-05-10 20:44:27.000000 hashkern-0.3.1/src/hash/__init__.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.652200 hashkern-0.3.1/src/hash/cli/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       23 2023-01-14 12:45:56.000000 hashkern-0.3.1/src/hash/cli/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5912 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/cli/main.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7189 2023-01-13 23:42:17.000000 hashkern-0.3.1/src/hash/dag.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     2148 2023-05-14 21:16:53.000000 hashkern-0.3.1/src/hash/errors.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.652200 hashkern-0.3.1/src/hash/kern/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      148 2023-05-25 21:40:09.000000 hashkern-0.3.1/src/hash/kern/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    10412 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/action.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7361 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/execute.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      931 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/hash.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3196 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/main.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    16126 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/planner.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     4181 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/secrets.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    19277 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/state.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5952 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/kern/templates.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3461 2023-01-13 23:42:17.000000 hashkern-0.3.1/src/hash/logs.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.652200 hashkern-0.3.1/src/hash/resources/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       69 2023-05-14 22:02:35.000000 hashkern-0.3.1/src/hash/resources/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    97796 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/resources/base.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    22702 2023-05-15 21:31:58.000000 hashkern-0.3.1/src/hash/resources/targets.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.652200 hashkern-0.3.1/src/hash/store/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       59 2023-01-13 23:42:17.000000 hashkern-0.3.1/src/hash/store/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    28132 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/store/base.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    12523 2023-05-25 21:36:32.000000 hashkern-0.3.1/src/hash/utils.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:41:58.656200 hashkern-0.3.1/src/hashkern.egg-info/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14840 2023-05-25 21:41:58.000000 hashkern-0.3.1/src/hashkern.egg-info/PKG-INFO
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      738 2023-05-25 21:41:58.000000 hashkern-0.3.1/src/hashkern.egg-info/SOURCES.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        1 2023-05-25 21:41:58.000000 hashkern-0.3.1/src/hashkern.egg-info/dependency_links.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       39 2023-05-25 21:41:58.000000 hashkern-0.3.1/src/hashkern.egg-info/entry_points.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      199 2023-05-25 21:41:58.000000 hashkern-0.3.1/src/hashkern.egg-info/requires.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        5 2023-05-25 21:41:58.000000 hashkern-0.3.1/src/hashkern.egg-info/top_level.txt
```

### Comparing `hashkern-0.3.0/LICENSE` & `hashkern-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/PKG-INFO` & `hashkern-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashkern
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool for managing resources in a mono repository
 Author: Mouhsen Ibrahim
 Author-email: mouhsen.ibrahim@gmail.com
 Project-URL: Documentation, https://hashkern.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://gitlab.com/hash-platform/hashkern
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -29,15 +29,15 @@
 Hash kern achieves all of this using well designed kern package, Dependency Graph and a set of plugins for defining
 resources, state storage backends and targets for executing some actions in enviornments (more about these later).
 
 ## Quick Architecture Introduction
 
 The following diagram shows the most important packages and modules in Hash kern and their interactions
 
-![Hash kern Archirecture](assets/hash-kern.jpg "Hash kern Archirecture")
+![Hash kern Archirecture](assets/hashkern.jpg "Hash kern Archirecture")
 
 * **kern Package** It contains modules for defining state, hash templates, actions, planning actions and executing them.
 It is designed to be independent from resources and it interacts with resources and store packages to manage resources and store their state.
 
 * **Resources Package** It contains the base class for all resources and it also defines the Environment resource, along with some built in resources and the targets used by resources to execute some actions in some environments.
 
 * **Store Package** This package contains the base for all store plugins and some built in plugins, it is used to store the state which results from running actions on resources in its own store which can be local file, GCP buckets, Digital Ocean spaces, etc....
@@ -79,16 +79,16 @@
 ```bash
 sudo apt install git make python3 python3-venv python3-apt
 ```
 
 Now clone the repository and cd into its directory
 
 ```bash
-git clone https://gitlab.com/hash-platform/hash-kern.git
-cd hash-kern
+git clone https://gitlab.com/hash-platform/hashkern.git
+cd hashkern
 ```
 
 Create a virtual env and activate it with these commands
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
@@ -272,15 +272,15 @@
 * Test hash kern in real world use cases and add more features accordingly.
 * Evaluate our graph implementation and add more tests to it.
 
 ## Contribution Guide
 
 We highly welcome any contributions to Hash kern as it helps us to improve it and test it more before it is declared as production ready.
 
-You can check open issues [here](https://gitlab.com/hash-platform/hash-kern/-/issues), you can follow the installation guide
+You can check open issues [here](https://gitlab.com/hash-platform/hashkern/-/issues), you can follow the installation guide
 above to get sarted with development, hash kern is written in python so you can install it in development mode and get started
 quickly, it is tested using python 3.7, 3.8, 3.9, 3.10 and 3.11.
 
 Make sure to install the latest version of python, create the virtual env and get started with one of the issues.
 
 You can run the test suite after you are finished implemneting the feature or fix using this command
 
@@ -292,10 +292,10 @@
 
 We use a tag based releases, the versions correspond to the tags. [Semantic versioning](https://semver.org) is used to create tags, all
 versions before the first stable release `1.0.0` might include backward incompatible changes.
 
 To create a new version you simply increase the version argument in setup.py, create a merge request to merge it with main
 and then create a tag that corresponds to the new version number.
 
-The [CHANGLOG.md](https://gitlab.com/hash-platform/hash-kern/-/blob/main/CHANGELOG.md) contains all changes between releases and their release dates.
+The [CHANGLOG.md](https://gitlab.com/hash-platform/hashkern/-/blob/main/CHANGELOG.md) contains all changes between releases and their release dates.
 
 More detailed contribution guide will be shared later :)
```

### Comparing `hashkern-0.3.0/README.md` & `hashkern-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Hash kern achieves all of this using well designed kern package, Dependency Graph and a set of plugins for defining
 resources, state storage backends and targets for executing some actions in enviornments (more about these later).
 
 ## Quick Architecture Introduction
 
 The following diagram shows the most important packages and modules in Hash kern and their interactions
 
-![Hash kern Archirecture](assets/hash-kern.jpg "Hash kern Archirecture")
+![Hash kern Archirecture](assets/hashkern.jpg "Hash kern Archirecture")
 
 * **kern Package** It contains modules for defining state, hash templates, actions, planning actions and executing them.
 It is designed to be independent from resources and it interacts with resources and store packages to manage resources and store their state.
 
 * **Resources Package** It contains the base class for all resources and it also defines the Environment resource, along with some built in resources and the targets used by resources to execute some actions in some environments.
 
 * **Store Package** This package contains the base for all store plugins and some built in plugins, it is used to store the state which results from running actions on resources in its own store which can be local file, GCP buckets, Digital Ocean spaces, etc....
@@ -60,16 +60,16 @@
 ```bash
 sudo apt install git make python3 python3-venv python3-apt
 ```
 
 Now clone the repository and cd into its directory
 
 ```bash
-git clone https://gitlab.com/hash-platform/hash-kern.git
-cd hash-kern
+git clone https://gitlab.com/hash-platform/hashkern.git
+cd hashkern
 ```
 
 Create a virtual env and activate it with these commands
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
@@ -253,15 +253,15 @@
 * Test hash kern in real world use cases and add more features accordingly.
 * Evaluate our graph implementation and add more tests to it.
 
 ## Contribution Guide
 
 We highly welcome any contributions to Hash kern as it helps us to improve it and test it more before it is declared as production ready.
 
-You can check open issues [here](https://gitlab.com/hash-platform/hash-kern/-/issues), you can follow the installation guide
+You can check open issues [here](https://gitlab.com/hash-platform/hashkern/-/issues), you can follow the installation guide
 above to get sarted with development, hash kern is written in python so you can install it in development mode and get started
 quickly, it is tested using python 3.7, 3.8, 3.9, 3.10 and 3.11.
 
 Make sure to install the latest version of python, create the virtual env and get started with one of the issues.
 
 You can run the test suite after you are finished implemneting the feature or fix using this command
 
@@ -273,10 +273,10 @@
 
 We use a tag based releases, the versions correspond to the tags. [Semantic versioning](https://semver.org) is used to create tags, all
 versions before the first stable release `1.0.0` might include backward incompatible changes.
 
 To create a new version you simply increase the version argument in setup.py, create a merge request to merge it with main
 and then create a tag that corresponds to the new version number.
 
-The [CHANGLOG.md](https://gitlab.com/hash-platform/hash-kern/-/blob/main/CHANGELOG.md) contains all changes between releases and their release dates.
+The [CHANGLOG.md](https://gitlab.com/hash-platform/hashkern/-/blob/main/CHANGELOG.md) contains all changes between releases and their release dates.
 
 More detailed contribution guide will be shared later :)
```

### Comparing `hashkern-0.3.0/setup.py` & `hashkern-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         return f.read().splitlines()
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name="hashkern",
-    version="0.3.0",
+    version="0.3.1",
     author="Mouhsen Ibrahim",
     author_email="mouhsen.ibrahim@gmail.com",
     description="A tool for managing resources in a mono repository",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `hashkern-0.3.0/src/hash/cli/main.py` & `hashkern-0.3.1/src/hash/cli/main.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/dag.py` & `hashkern-0.3.1/src/hash/dag.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/errors.py` & `hashkern-0.3.1/src/hash/errors.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/action.py` & `hashkern-0.3.1/src/hash/kern/action.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/execute.py` & `hashkern-0.3.1/src/hash/kern/execute.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/hash.py` & `hashkern-0.3.1/src/hash/kern/hash.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/main.py` & `hashkern-0.3.1/src/hash/kern/main.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/planner.py` & `hashkern-0.3.1/src/hash/kern/planner.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/secrets.py` & `hashkern-0.3.1/src/hash/kern/secrets.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/state.py` & `hashkern-0.3.1/src/hash/kern/state.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/kern/templates.py` & `hashkern-0.3.1/src/hash/kern/templates.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/logs.py` & `hashkern-0.3.1/src/hash/logs.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/resources/base.py` & `hashkern-0.3.1/src/hash/resources/base.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/resources/targets.py` & `hashkern-0.3.1/src/hash/resources/targets.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/store/base.py` & `hashkern-0.3.1/src/hash/store/base.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hash/utils.py` & `hashkern-0.3.1/src/hash/utils.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.0/src/hashkern.egg-info/PKG-INFO` & `hashkern-0.3.1/src/hashkern.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashkern
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool for managing resources in a mono repository
 Author: Mouhsen Ibrahim
 Author-email: mouhsen.ibrahim@gmail.com
 Project-URL: Documentation, https://hashkern.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://gitlab.com/hash-platform/hashkern
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -29,15 +29,15 @@
 Hash kern achieves all of this using well designed kern package, Dependency Graph and a set of plugins for defining
 resources, state storage backends and targets for executing some actions in enviornments (more about these later).
 
 ## Quick Architecture Introduction
 
 The following diagram shows the most important packages and modules in Hash kern and their interactions
 
-![Hash kern Archirecture](assets/hash-kern.jpg "Hash kern Archirecture")
+![Hash kern Archirecture](assets/hashkern.jpg "Hash kern Archirecture")
 
 * **kern Package** It contains modules for defining state, hash templates, actions, planning actions and executing them.
 It is designed to be independent from resources and it interacts with resources and store packages to manage resources and store their state.
 
 * **Resources Package** It contains the base class for all resources and it also defines the Environment resource, along with some built in resources and the targets used by resources to execute some actions in some environments.
 
 * **Store Package** This package contains the base for all store plugins and some built in plugins, it is used to store the state which results from running actions on resources in its own store which can be local file, GCP buckets, Digital Ocean spaces, etc....
@@ -79,16 +79,16 @@
 ```bash
 sudo apt install git make python3 python3-venv python3-apt
 ```
 
 Now clone the repository and cd into its directory
 
 ```bash
-git clone https://gitlab.com/hash-platform/hash-kern.git
-cd hash-kern
+git clone https://gitlab.com/hash-platform/hashkern.git
+cd hashkern
 ```
 
 Create a virtual env and activate it with these commands
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
@@ -272,15 +272,15 @@
 * Test hash kern in real world use cases and add more features accordingly.
 * Evaluate our graph implementation and add more tests to it.
 
 ## Contribution Guide
 
 We highly welcome any contributions to Hash kern as it helps us to improve it and test it more before it is declared as production ready.
 
-You can check open issues [here](https://gitlab.com/hash-platform/hash-kern/-/issues), you can follow the installation guide
+You can check open issues [here](https://gitlab.com/hash-platform/hashkern/-/issues), you can follow the installation guide
 above to get sarted with development, hash kern is written in python so you can install it in development mode and get started
 quickly, it is tested using python 3.7, 3.8, 3.9, 3.10 and 3.11.
 
 Make sure to install the latest version of python, create the virtual env and get started with one of the issues.
 
 You can run the test suite after you are finished implemneting the feature or fix using this command
 
@@ -292,10 +292,10 @@
 
 We use a tag based releases, the versions correspond to the tags. [Semantic versioning](https://semver.org) is used to create tags, all
 versions before the first stable release `1.0.0` might include backward incompatible changes.
 
 To create a new version you simply increase the version argument in setup.py, create a merge request to merge it with main
 and then create a tag that corresponds to the new version number.
 
-The [CHANGLOG.md](https://gitlab.com/hash-platform/hash-kern/-/blob/main/CHANGELOG.md) contains all changes between releases and their release dates.
+The [CHANGLOG.md](https://gitlab.com/hash-platform/hashkern/-/blob/main/CHANGELOG.md) contains all changes between releases and their release dates.
 
 More detailed contribution guide will be shared later :)
```

### Comparing `hashkern-0.3.0/src/hashkern.egg-info/SOURCES.txt` & `hashkern-0.3.1/src/hashkern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

