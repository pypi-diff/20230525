# Comparing `tmp/samarium62-0.0.2.tar.gz` & `tmp/samarium62-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samarium62-0.0.2.tar", last modified: Thu May 25 18:39:35 2023, max compression
+gzip compressed data, was "samarium62-0.0.3.tar", last modified: Thu May 25 18:46:41 2023, max compression
```

## Comparing `samarium62-0.0.2.tar` & `samarium62-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.820840 samarium62-0.0.2/
--rw-r--r--   0 samarthshastry   (501) staff       (20)     1073 2023-05-24 07:57:59.000000 samarium62-0.0.2/LICENSE
--rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:39:35.817957 samarium62-0.0.2/PKG-INFO
--rw-r--r--   0 samarthshastry   (501) staff       (20)      104 2023-05-24 08:21:01.000000 samarium62-0.0.2/README.md
--rw-r--r--   0 samarthshastry   (501) staff       (20)      569 2023-05-25 18:38:49.000000 samarium62-0.0.2/pyproject.toml
--rw-r--r--   0 samarthshastry   (501) staff       (20)       38 2023-05-25 18:39:35.821375 samarium62-0.0.2/setup.cfg
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.693254 samarium62-0.0.2/src/
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.731071 samarium62-0.0.2/src/samarium62/
--rw-r--r--   0 samarthshastry   (501) staff       (20)      299 2023-05-24 03:20:40.000000 samarium62-0.0.2/src/samarium62/__init__.py
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.815573 samarium62-0.0.2/src/samarium62/discord/
--rw-r--r--   0 samarthshastry   (501) staff       (20)       78 2023-05-23 23:49:35.000000 samarium62-0.0.2/src/samarium62/discord/__init__.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     4488 2023-05-25 18:35:26.000000 samarium62-0.0.2/src/samarium62/discord/component.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     7820 2023-05-25 18:31:37.000000 samarium62-0.0.2/src/samarium62/discord/embed.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     1025 2023-05-23 23:58:01.000000 samarium62-0.0.2/src/samarium62/discord/image_processing.py
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.796677 samarium62-0.0.2/src/samarium62.egg-info/
--rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/PKG-INFO
--rw-r--r--   0 samarthshastry   (501) staff       (20)      394 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/SOURCES.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)        1 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/dependency_links.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)       14 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/requires.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)       11 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/top_level.txt
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.255041 samarium62-0.0.3/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     1073 2023-05-24 07:57:59.000000 samarium62-0.0.3/LICENSE
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:46:41.254065 samarium62-0.0.3/PKG-INFO
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      104 2023-05-24 08:21:01.000000 samarium62-0.0.3/README.md
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      569 2023-05-25 18:46:18.000000 samarium62-0.0.3/pyproject.toml
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       38 2023-05-25 18:46:41.255214 samarium62-0.0.3/setup.cfg
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.227403 samarium62-0.0.3/src/
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.233432 samarium62-0.0.3/src/samarium62/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      298 2023-05-25 18:46:00.000000 samarium62-0.0.3/src/samarium62/__init__.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.251405 samarium62-0.0.3/src/samarium62/discord/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       78 2023-05-23 23:49:35.000000 samarium62-0.0.3/src/samarium62/discord/__init__.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     4488 2023-05-25 18:35:26.000000 samarium62-0.0.3/src/samarium62/discord/component.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     7820 2023-05-25 18:31:37.000000 samarium62-0.0.3/src/samarium62/discord/embed.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     1025 2023-05-23 23:58:01.000000 samarium62-0.0.3/src/samarium62/discord/image_processing.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.244630 samarium62-0.0.3/src/samarium62.egg-info/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/PKG-INFO
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      394 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/SOURCES.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)        1 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/dependency_links.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       14 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/requires.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       11 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/top_level.txt
```

### Comparing `samarium62-0.0.2/LICENSE` & `samarium62-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.2/PKG-INFO` & `samarium62-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium62
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper package for creating custom discord embed
 Author-email: GitYACC <shastrysamarth@gmail.com>
 Project-URL: Homepage, https://home.page
 Project-URL: Bug Tracker, https://github.com/Future-Lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `samarium62-0.0.2/pyproject.toml` & `samarium62-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samarium62"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="GitYACC", email="shastrysamarth@gmail.com" },
 ]
 description = "A wrapper package for creating custom discord embed"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `samarium62-0.0.2/src/samarium62/discord/component.py` & `samarium62-0.0.3/src/samarium62/discord/component.py`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.2/src/samarium62/discord/embed.py` & `samarium62-0.0.3/src/samarium62/discord/embed.py`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.2/src/samarium62/discord/image_processing.py` & `samarium62-0.0.3/src/samarium62/discord/image_processing.py`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.2/src/samarium62.egg-info/PKG-INFO` & `samarium62-0.0.3/src/samarium62.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium62
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper package for creating custom discord embed
 Author-email: GitYACC <shastrysamarth@gmail.com>
 Project-URL: Homepage, https://home.page
 Project-URL: Bug Tracker, https://github.com/Future-Lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

