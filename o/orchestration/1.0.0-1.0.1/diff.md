# Comparing `tmp/orchestration-1.0.0.tar.gz` & `tmp/orchestration-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orchestration-1.0.0.tar", last modified: Thu May 25 17:54:46 2023, max compression
+gzip compressed data, was "dist/orchestration-1.0.1.tar", last modified: Thu May 25 18:12:51 2023, max compression
```

## Comparing `orchestration-1.0.0.tar` & `orchestration-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 17:54:46.000000 orchestration-1.0.0/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 17:54:46.000000 orchestration-1.0.0/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3197 2023-05-25 17:46:38.000000 orchestration-1.0.0/README.md
--rw-r--r--   0 henrytazewell   (501) staff       (20)      639 2023-05-25 17:54:32.000000 orchestration-1.0.0/setup.py
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration.egg-info/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration.egg-info/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration.egg-info/requires.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration.egg-info/top_level.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration.egg-info/dependency_links.txt
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 17:54:46.000000 orchestration-1.0.0/orchestration/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     2961 2023-05-25 17:46:02.000000 orchestration-1.0.0/orchestration/task.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)        0 2023-05-25 17:45:07.000000 orchestration-1.0.0/orchestration/__init__.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)     1074 2023-05-25 17:46:13.000000 orchestration-1.0.0/orchestration/orchestrator.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 17:54:46.000000 orchestration-1.0.0/setup.cfg
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 18:12:51.000000 orchestration-1.0.1/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 18:12:51.000000 orchestration-1.0.1/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3197 2023-05-25 17:46:38.000000 orchestration-1.0.1/README.md
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      652 2023-05-25 18:12:48.000000 orchestration-1.0.1/setup.py
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration.egg-info/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration.egg-info/requires.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration.egg-info/top_level.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration.egg-info/dependency_links.txt
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 18:12:51.000000 orchestration-1.0.1/orchestration/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     2961 2023-05-25 17:46:02.000000 orchestration-1.0.1/orchestration/task.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        0 2023-05-25 17:45:07.000000 orchestration-1.0.1/orchestration/__init__.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     1074 2023-05-25 17:46:13.000000 orchestration-1.0.1/orchestration/orchestrator.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 18:12:51.000000 orchestration-1.0.1/setup.cfg
```

### Comparing `orchestration-1.0.0/PKG-INFO` & `orchestration-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.0.0
+Version: 1.0.1
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazwell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestrator
```

### Comparing `orchestration-1.0.0/README.md` & `orchestration-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `orchestration-1.0.0/setup.py` & `orchestration-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='orchestration',
-    version='1.0.0',
+    version='1.0.1',
     description='This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Henry Tazewell',
     author_email='htazewell@gmail.com',
     url='https://github.com/htazwell/orchestration',
-    packages=['orchestration'],
+    packages=find_packages(),
     install_requires=[
         'croniter',
         'pytz',
     ],
 )
```

### Comparing `orchestration-1.0.0/orchestration.egg-info/PKG-INFO` & `orchestration-1.0.1/orchestration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.0.0
+Version: 1.0.1
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazwell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestrator
```

### Comparing `orchestration-1.0.0/orchestration/task.py` & `orchestration-1.0.1/orchestration/task.py`

 * *Files identical despite different names*

### Comparing `orchestration-1.0.0/orchestration/orchestrator.py` & `orchestration-1.0.1/orchestration/orchestrator.py`

 * *Files identical despite different names*

