# Comparing `tmp/aish-0.1.4.tar.gz` & `tmp/aish-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aish-0.1.4.tar", last modified: Tue May 23 17:04:24 2023, max compression
+gzip compressed data, was "aish-0.1.5.tar", last modified: Thu May 25 17:14:24 2023, max compression
```

## Comparing `aish-0.1.4.tar` & `aish-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 17:04:24.891083 aish-0.1.4/
--rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.4/LICENCE
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 17:04:24.890759 aish-0.1.4/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.4/README.md
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 17:04:24.888050 aish-0.1.4/aish/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.4/aish/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)     8387 2023-05-23 16:49:03.000000 aish-0.1.4/aish/aish.py
--rw-r--r--   0 toni       (501) staff       (20)     2395 2023-05-22 11:56:07.000000 aish-0.1.4/aish/proxy.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 17:04:24.890006 aish-0.1.4/aish.egg-info/
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 17:04:24.000000 aish-0.1.4/aish.egg-info/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)      258 2023-05-23 17:04:24.000000 aish-0.1.4/aish.egg-info/SOURCES.txt
--rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-23 17:04:24.000000 aish-0.1.4/aish.egg-info/dependency_links.txt
--rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-23 17:04:24.000000 aish-0.1.4/aish.egg-info/entry_points.txt
--rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-23 17:04:24.000000 aish-0.1.4/aish.egg-info/requires.txt
--rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-23 17:04:24.000000 aish-0.1.4/aish.egg-info/top_level.txt
--rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-23 17:04:24.891190 aish-0.1.4/setup.cfg
--rw-r--r--   0 toni       (501) staff       (20)      570 2023-05-23 17:03:37.000000 aish-0.1.4/setup.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 17:04:24.890325 aish-0.1.4/tests/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.4/tests/__init__.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.683937 aish-0.1.5/
+-rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.5/LICENCE
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-25 17:14:24.683490 aish-0.1.5/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.5/README.md
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.679848 aish-0.1.5/aish/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.5/aish/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)    11594 2023-05-25 17:03:57.000000 aish-0.1.5/aish/aish.py
+-rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.5/aish/proxy.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.682029 aish-0.1.5/aish.egg-info/
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/SOURCES.txt
+-rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/dependency_links.txt
+-rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/entry_points.txt
+-rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/requires.txt
+-rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/top_level.txt
+-rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-25 17:14:24.684069 aish-0.1.5/setup.cfg
+-rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-25 16:28:27.000000 aish-0.1.5/setup.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.682841 aish-0.1.5/tests/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.5/tests/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)     6008 2023-05-25 17:12:37.000000 aish-0.1.5/tests/test_chat.py
```

### Comparing `aish-0.1.4/LICENCE` & `aish-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `aish-0.1.4/PKG-INFO` & `aish-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.4
+Version: 0.1.5
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.4/README.md` & `aish-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aish-0.1.4/aish.egg-info/PKG-INFO` & `aish-0.1.5/aish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.4
+Version: 0.1.5
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.4/setup.py` & `aish-0.1.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='aish',
-    version='0.1.4',
+    name="aish",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
-        'rich',
-        'flask',
-        'requests',
-        'distro',
+        "rich",
+        "flask",
+        "requests",
+        "distro",
     ],
     entry_points={
-        'console_scripts': [
-            'aish=aish.aish:main'
-       ],
+        "console_scripts": ["aish=aish.aish:main"],
     },
-    author='Toni Leino',
-    author_email='toni@leino.net',
-    description='A command-line application that interacts with the OpenAI ChatGPT API.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
+    author="Toni Leino",
+    author_email="toni@leino.net",
+    description="A command-line application that interacts with the OpenAI "
+    "ChatGPT API.",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
 )
```

