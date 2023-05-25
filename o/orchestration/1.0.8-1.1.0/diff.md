# Comparing `tmp/orchestration-1.0.8.tar.gz` & `tmp/orchestration-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orchestration-1.0.8.tar", last modified: Thu May 25 19:40:26 2023, max compression
+gzip compressed data, was "dist/orchestration-1.1.0.tar", last modified: Thu May 25 19:47:21 2023, max compression
```

## Comparing `orchestration-1.0.8.tar` & `orchestration-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:40:26.000000 orchestration-1.0.8/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 19:40:26.000000 orchestration-1.0.8/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3197 2023-05-25 17:46:38.000000 orchestration-1.0.8/README.md
--rw-r--r--   0 henrytazewell   (501) staff       (20)      652 2023-05-25 19:23:33.000000 orchestration-1.0.8/setup.py
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4519 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/requires.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/top_level.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration.egg-info/dependency_links.txt
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:40:26.000000 orchestration-1.0.8/orchestration/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3082 2023-05-25 19:40:08.000000 orchestration-1.0.8/orchestration/task.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-25 19:23:22.000000 orchestration-1.0.8/orchestration/__init__.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)     1088 2023-05-25 18:34:30.000000 orchestration-1.0.8/orchestration/orchestrator.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 19:40:26.000000 orchestration-1.0.8/setup.cfg
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:47:21.000000 orchestration-1.1.0/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4425 2023-05-25 19:47:21.000000 orchestration-1.1.0/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.0/README.md
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      652 2023-05-25 19:46:47.000000 orchestration-1.1.0/setup.py
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4425 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/requires.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/top_level.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration.egg-info/dependency_links.txt
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:47:21.000000 orchestration-1.1.0/orchestration/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3082 2023-05-25 19:40:08.000000 orchestration-1.1.0/orchestration/task.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-25 19:23:22.000000 orchestration-1.1.0/orchestration/__init__.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     1138 2023-05-25 19:46:26.000000 orchestration-1.1.0/orchestration/orchestrator.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 19:47:21.000000 orchestration-1.1.0/setup.cfg
```

### Comparing `orchestration-1.0.8/setup.py` & `orchestration-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='orchestration',
-    version='1.0.8',
+    version='1.1.0',
     description='This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Henry Tazewell',
     author_email='htazewell@gmail.com',
     url='https://github.com/htazwell/orchestration',
     packages=find_packages(),
```

### Comparing `orchestration-1.0.8/orchestration/task.py` & `orchestration-1.1.0/orchestration/task.py`

 * *Files identical despite different names*

### Comparing `orchestration-1.0.8/orchestration/orchestrator.py` & `orchestration-1.1.0/orchestration/orchestrator.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,9 +23,10 @@
                 if task.should_execute():
                     for script in task.scripts:
                         if isinstance(script, tuple) and len(script) == 2:
                             script_path, parameters_list = script
                             task.repeat(script_path, parameters_list)
                         else:
                             task.execute_script(script)
+                        time.sleep(task.interval)
 
             time.sleep(task.interval)  # Sleep for 1 second
```

