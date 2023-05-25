# Comparing `tmp/orchestration-1.1.0.tar.gz` & `tmp/orchestration-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orchestration-1.1.0.tar", last modified: Thu May 25 19:47:21 2023, max compression
+gzip compressed data, was "dist/orchestration-1.1.1.tar", last modified: Thu May 25 19:50:34 2023, max compression
```

## Comparing `orchestration-1.1.0.tar` & `orchestration-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:47:21.000000 orchestration-1.1.0/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4425 2023-05-25 19:47:21.000000 orchestration-1.1.0/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.0/README.md
--rw-r--r--   0 henrytazewell   (501) staff       (20)      652 2023-05-25 19:46:47.000000 orchestration-1.1.0/setup.py
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4425 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/requires.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/top_level.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/dependency_links.txt
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3082 2023-05-25 19:40:08.000000 orchestration-1.1.0/orchestration/task.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-25 19:23:22.000000 orchestration-1.1.0/orchestration/__init__.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)     1138 2023-05-25 19:46:26.000000 orchestration-1.1.0/orchestration/orchestrator.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 19:47:21.000000 orchestration-1.1.0/setup.cfg
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:50:34.000000 orchestration-1.1.1/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-25 19:50:34.000000 orchestration-1.1.1/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.1/README.md
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      653 2023-05-25 19:50:21.000000 orchestration-1.1.1/setup.py
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/requires.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/top_level.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/dependency_links.txt
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3082 2023-05-25 19:40:08.000000 orchestration-1.1.1/orchestration/task.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-25 19:23:22.000000 orchestration-1.1.1/orchestration/__init__.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     1138 2023-05-25 19:46:26.000000 orchestration-1.1.1/orchestration/orchestrator.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 19:50:34.000000 orchestration-1.1.1/setup.cfg
```

### Comparing `orchestration-1.1.0/PKG-INFO` & `orchestration-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.1.0
+Version: 1.1.1
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
-Home-page: https://github.com/htazwell/orchestration
+Home-page: https://github.com/htazewell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestration
         
         The Orchestration library provides functionality to schedule and execute tasks based on cron expressions. It allows you to add skip conditions and dynamically generate script parameters. This library is designed to simplify the process of automating script execution.
```

### Comparing `orchestration-1.1.0/README.md` & `orchestration-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `orchestration-1.1.0/setup.py` & `orchestration-1.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='orchestration',
-    version='1.1.0',
+    version='1.1.1',
     description='This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Henry Tazewell',
     author_email='htazewell@gmail.com',
-    url='https://github.com/htazwell/orchestration',
+    url='https://github.com/htazewell/orchestration',
     packages=find_packages(),
     install_requires=[
         'croniter',
         'pytz',
     ],
 )
```

### Comparing `orchestration-1.1.0/orchestration.egg-info/PKG-INFO` & `orchestration-1.1.1/orchestration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.1.0
+Version: 1.1.1
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
-Home-page: https://github.com/htazwell/orchestration
+Home-page: https://github.com/htazewell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestration
         
         The Orchestration library provides functionality to schedule and execute tasks based on cron expressions. It allows you to add skip conditions and dynamically generate script parameters. This library is designed to simplify the process of automating script execution.
```

### Comparing `orchestration-1.1.0/orchestration/task.py` & `orchestration-1.1.1/orchestration/task.py`

 * *Files identical despite different names*

### Comparing `orchestration-1.1.0/orchestration/orchestrator.py` & `orchestration-1.1.1/orchestration/orchestrator.py`

 * *Files identical despite different names*

