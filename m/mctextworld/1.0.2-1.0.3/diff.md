# Comparing `tmp/mctextworld-1.0.2.tar.gz` & `tmp/mctextworld-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctextworld-1.0.2.tar", last modified: Thu May 25 14:42:47 2023, max compression
+gzip compressed data, was "mctextworld-1.0.3.tar", last modified: Thu May 25 15:00:34 2023, max compression
```

## Comparing `mctextworld-1.0.2.tar` & `mctextworld-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 zhwang     (501) staff       (20)        0 2023-05-25 14:42:47.850448 mctextworld-1.0.2/
--rw-r--r--   0 zhwang     (501) staff       (20)      586 2023-05-25 14:42:47.850344 mctextworld-1.0.2/PKG-INFO
--rw-r--r--   0 zhwang     (501) staff       (20)       52 2023-05-24 16:00:36.000000 mctextworld-1.0.2/README.md
-drwxr-xr-x   0 zhwang     (501) staff       (20)        0 2023-05-25 14:42:47.850180 mctextworld-1.0.2/mctextworld.egg-info/
--rw-r--r--   0 zhwang     (501) staff       (20)      586 2023-05-25 14:42:47.000000 mctextworld-1.0.2/mctextworld.egg-info/PKG-INFO
--rw-r--r--   0 zhwang     (501) staff       (20)      192 2023-05-25 14:42:47.000000 mctextworld-1.0.2/mctextworld.egg-info/SOURCES.txt
--rw-r--r--   0 zhwang     (501) staff       (20)        1 2023-05-25 14:42:47.000000 mctextworld-1.0.2/mctextworld.egg-info/dependency_links.txt
--rw-r--r--   0 zhwang     (501) staff       (20)        4 2023-05-25 14:42:47.000000 mctextworld-1.0.2/mctextworld.egg-info/requires.txt
--rw-r--r--   0 zhwang     (501) staff       (20)       12 2023-05-25 14:42:47.000000 mctextworld-1.0.2/mctextworld.egg-info/top_level.txt
--rw-r--r--   0 zhwang     (501) staff       (20)       38 2023-05-25 14:42:47.850489 mctextworld-1.0.2/setup.cfg
--rw-r--r--   0 zhwang     (501) staff       (20)      842 2023-05-25 14:42:30.000000 mctextworld-1.0.2/setup.py
+drwxr-xr-x   0 zhwang     (501) staff       (20)        0 2023-05-25 15:00:34.677991 mctextworld-1.0.3/
+-rw-r--r--   0 zhwang     (501) staff       (20)      586 2023-05-25 15:00:34.677859 mctextworld-1.0.3/PKG-INFO
+-rw-r--r--   0 zhwang     (501) staff       (20)       52 2023-05-24 16:00:36.000000 mctextworld-1.0.3/README.md
+drwxr-xr-x   0 zhwang     (501) staff       (20)        0 2023-05-25 15:00:34.677599 mctextworld-1.0.3/mctextworld.egg-info/
+-rw-r--r--   0 zhwang     (501) staff       (20)      586 2023-05-25 15:00:34.000000 mctextworld-1.0.3/mctextworld.egg-info/PKG-INFO
+-rw-r--r--   0 zhwang     (501) staff       (20)      192 2023-05-25 15:00:34.000000 mctextworld-1.0.3/mctextworld.egg-info/SOURCES.txt
+-rw-r--r--   0 zhwang     (501) staff       (20)        1 2023-05-25 15:00:34.000000 mctextworld-1.0.3/mctextworld.egg-info/dependency_links.txt
+-rw-r--r--   0 zhwang     (501) staff       (20)        4 2023-05-25 15:00:34.000000 mctextworld-1.0.3/mctextworld.egg-info/requires.txt
+-rw-r--r--   0 zhwang     (501) staff       (20)       12 2023-05-25 15:00:34.000000 mctextworld-1.0.3/mctextworld.egg-info/top_level.txt
+-rw-r--r--   0 zhwang     (501) staff       (20)       38 2023-05-25 15:00:34.678033 mctextworld-1.0.3/setup.cfg
+-rw-r--r--   0 zhwang     (501) staff       (20)      842 2023-05-25 15:00:32.000000 mctextworld-1.0.3/setup.py
```

### Comparing `mctextworld-1.0.2/PKG-INFO` & `mctextworld-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctextworld
-Version: 1.0.2
+Version: 1.0.3
 Summary: A text world based on Minecraft rules.
 Home-page: https://zhwang4ai.github.io/
 Author: wangzihao
 Author-email: zhwang@stu.pku.edu.cn
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mctextworld-1.0.2/mctextworld.egg-info/PKG-INFO` & `mctextworld-1.0.3/mctextworld.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctextworld
-Version: 1.0.2
+Version: 1.0.3
 Summary: A text world based on Minecraft rules.
 Home-page: https://zhwang4ai.github.io/
 Author: wangzihao
 Author-email: zhwang@stu.pku.edu.cn
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mctextworld-1.0.2/setup.py` & `mctextworld-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mctextworld',
-    version='1.0.2',
+    version='1.0.3',
     description='A text world based on Minecraft rules.',
     long_description='',
     # The project's main homepage.
     url='https://zhwang4ai.github.io/',
     # Author details
     author='wangzihao',
     author_email='zhwang@stu.pku.edu.cn',
```

