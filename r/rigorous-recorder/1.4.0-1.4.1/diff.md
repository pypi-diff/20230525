# Comparing `tmp/rigorous_recorder-1.4.0.tar.gz` & `tmp/rigorous_recorder-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigorous_recorder-1.4.0.tar", last modified: Mon Apr 24 14:15:45 2023, max compression
+gzip compressed data, was "rigorous_recorder-1.4.1.tar", last modified: Thu May 25 20:56:13 2023, max compression
```

## Comparing `rigorous_recorder-1.4.0.tar` & `rigorous_recorder-1.4.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 14:15:45.533557 rigorous_recorder-1.4.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-24 14:15:45.533414 rigorous_recorder-1.4.0/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 14:15:45.532658 rigorous_recorder-1.4.0/rigorous_recorder/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.4.0/rigorous_recorder/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    35695 2023-04-24 14:13:02.000000 rigorous_recorder-1.4.0/rigorous_recorder/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 14:15:45.533182 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 14:15:45.533597 rigorous_recorder-1.4.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1104 2023-04-24 13:58:53.000000 rigorous_recorder-1.4.0/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:56:13.321543 rigorous_recorder-1.4.1/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-25 20:56:13.321283 rigorous_recorder-1.4.1/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:56:13.320345 rigorous_recorder-1.4.1/rigorous_recorder/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    35674 2023-05-25 20:48:40.000000 rigorous_recorder-1.4.1/rigorous_recorder/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:56:13.321134 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-25 20:56:12.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      202 2023-05-25 20:56:13.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-25 20:56:13.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-05-25 20:56:13.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-25 20:56:13.321619 rigorous_recorder-1.4.1/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1104 2023-04-24 13:58:53.000000 rigorous_recorder-1.4.1/setup.py
```

### Comparing `rigorous_recorder-1.4.0/PKG-INFO` & `rigorous_recorder-1.4.1/rigorous_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rigorous_recorder
-Version: 1.4.0
+Name: rigorous-recorder
+Version: 1.4.1
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.4.0/rigorous_recorder/main.py` & `rigorous_recorder-1.4.1/rigorous_recorder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,12 +948,8 @@
                 print(f'This happend on:\n    dict(experiment_number={experiment_number}, error_number={error_number})')
                 print(traceback.format_exc())
                 raise error
         
         return Experiment(
             internal_experiment_info=self.current_experiment,
             save_experiment=save_experiment,
-        )
-    
-    
-    
-    
+        )
```

### Comparing `rigorous_recorder-1.4.0/rigorous_recorder.egg-info/PKG-INFO` & `rigorous_recorder-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rigorous-recorder
-Version: 1.4.0
+Name: rigorous_recorder
+Version: 1.4.1
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.4.0/setup.py` & `rigorous_recorder-1.4.1/setup.py`

 * *Files identical despite different names*

