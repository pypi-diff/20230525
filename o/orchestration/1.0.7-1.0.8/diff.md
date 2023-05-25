# Comparing `tmp/orchestration-1.0.7.tar.gz` & `tmp/orchestration-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orchestration-1.0.7.tar", last modified: Thu May 25 18:34:47 2023, max compression
+gzip compressed data, was "dist/orchestration-1.0.8.tar", last modified: Thu May 25 19:40:26 2023, max compression
```

## Comparing `orchestration-1.0.7.tar` & `orchestration-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 18:34:47.000000 orchestration-1.0.7/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 18:34:47.000000 orchestration-1.0.7/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3197 2023-05-25 17:46:38.000000 orchestration-1.0.7/README.md
--rw-r--r--   0 henrytazewell   (501) staff       (20)      652 2023-05-25 18:34:40.000000 orchestration-1.0.7/setup.py
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration.egg-info/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration.egg-info/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration.egg-info/requires.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration.egg-info/top_level.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration.egg-info/dependency_links.txt
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 18:34:47.000000 orchestration-1.0.7/orchestration/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     2961 2023-05-25 17:46:02.000000 orchestration-1.0.7/orchestration/task.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       87 2023-05-25 18:32:38.000000 orchestration-1.0.7/orchestration/__init__.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)     1088 2023-05-25 18:34:30.000000 orchestration-1.0.7/orchestration/orchestrator.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 18:34:47.000000 orchestration-1.0.7/setup.cfg
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:40:26.000000 orchestration-1.0.8/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 19:40:26.000000 orchestration-1.0.8/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3197 2023-05-25 17:46:38.000000 orchestration-1.0.8/README.md
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      652 2023-05-25 19:23:33.000000 orchestration-1.0.8/setup.py
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/requires.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/top_level.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/dependency_links.txt
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3082 2023-05-25 19:40:08.000000 orchestration-1.0.8/orchestration/task.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-25 19:23:22.000000 orchestration-1.0.8/orchestration/__init__.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     1088 2023-05-25 18:34:30.000000 orchestration-1.0.8/orchestration/orchestrator.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 19:40:26.000000 orchestration-1.0.8/setup.cfg
```

### Comparing `orchestration-1.0.7/PKG-INFO` & `orchestration-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.0.7
+Version: 1.0.8
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazwell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestrator
```

### Comparing `orchestration-1.0.7/README.md` & `orchestration-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `orchestration-1.0.7/setup.py` & `orchestration-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='orchestration',
-    version='1.0.7',
+    version='1.0.8',
     description='This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Henry Tazewell',
     author_email='htazewell@gmail.com',
     url='https://github.com/htazwell/orchestration',
     packages=find_packages(),
```

### Comparing `orchestration-1.0.7/orchestration.egg-info/PKG-INFO` & `orchestration-1.0.8/orchestration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.0.7
+Version: 1.0.8
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazwell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestrator
```

### Comparing `orchestration-1.0.7/orchestration/task.py` & `orchestration-1.0.8/orchestration/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         self.script_type = script_type
         self.cron_expression = cron_expression
         self.interval = interval
         self.scripts = []
         self.skips = []
         self.parameters = {}
 
+    def add_repeat(self, script_path, script_parameters):
+        self.scripts.append((script_path, script_parameters))
+
     def add_script(self, script_path, script_parameters=None):
         self.scripts.append(script_path)
         if script_parameters:
             self.parameters.update(script_parameters)
 
     def add_skip(self, skip_condition):
         self.skips.append(skip_condition)
```

### Comparing `orchestration-1.0.7/orchestration/orchestrator.py` & `orchestration-1.0.8/orchestration/orchestrator.py`

 * *Files identical despite different names*

