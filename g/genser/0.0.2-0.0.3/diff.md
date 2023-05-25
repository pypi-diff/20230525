# Comparing `tmp/genser-0.0.2.tar.gz` & `tmp/genser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genser-0.0.2.tar", last modified: Thu May 25 15:19:07 2023, max compression
+gzip compressed data, was "genser-0.0.3.tar", last modified: Thu May 25 15:37:01 2023, max compression
```

## Comparing `genser-0.0.2.tar` & `genser-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 15:19:07.570429 genser-0.0.2/
--rw-r--r--   0 sergejzuev   (501) staff       (20)    35350 2023-05-25 13:24:49.000000 genser-0.0.2/LICENSE
--rw-r--r--   0 sergejzuev   (501) staff       (20)     1988 2023-05-25 15:19:07.570606 genser-0.0.2/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)     1637 2023-05-25 14:59:24.000000 genser-0.0.2/README.md
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 15:19:07.567763 genser-0.0.2/genser/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 genser-0.0.2/genser/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)     3457 2023-05-25 12:53:06.000000 genser-0.0.2/genser/main.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 15:19:07.569999 genser-0.0.2/genser.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)     1988 2023-05-25 15:19:07.000000 genser-0.0.2/genser.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      190 2023-05-25 15:19:07.000000 genser-0.0.2/genser.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-25 15:19:07.000000 genser-0.0.2/genser.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-25 15:19:07.000000 genser-0.0.2/genser.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-25 15:19:07.571445 genser-0.0.2/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      519 2023-05-25 15:18:31.000000 genser-0.0.2/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 15:37:01.082211 genser-0.0.3/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    35350 2023-05-25 13:24:49.000000 genser-0.0.3/LICENSE
+-rw-r--r--   0 sergejzuev   (501) staff       (20)     1988 2023-05-25 15:37:01.082390 genser-0.0.3/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)     1637 2023-05-25 14:59:24.000000 genser-0.0.3/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 15:37:01.078929 genser-0.0.3/genser/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 genser-0.0.3/genser/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)     3457 2023-05-25 12:53:06.000000 genser-0.0.3/genser/main.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 15:37:01.081750 genser-0.0.3/genser.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)     1988 2023-05-25 15:37:00.000000 genser-0.0.3/genser.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      190 2023-05-25 15:37:00.000000 genser-0.0.3/genser.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-25 15:37:00.000000 genser-0.0.3/genser.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-25 15:37:00.000000 genser-0.0.3/genser.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-25 15:37:01.083274 genser-0.0.3/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      519 2023-05-25 15:36:26.000000 genser-0.0.3/setup.py
```

### Comparing `genser-0.0.2/LICENSE` & `genser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genser-0.0.2/PKG-INFO` & `genser-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of functions for dataset dimension transformations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `genser-0.0.2/README.md` & `genser-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `genser-0.0.2/genser/main.py` & `genser-0.0.3/genser/main.py`

 * *Files identical despite different names*

### Comparing `genser-0.0.2/genser.egg-info/PKG-INFO` & `genser-0.0.3/genser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of functions for dataset dimension transformations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `genser-0.0.2/setup.py` & `genser-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(name="genser",
-	version="0.0.2",
+	version="0.0.3",
 	author="Sergei Zuev",
 	author_email="shoukhov@mail.ru",
 	description="A set of functions for dataset dimension transformations",
 	packages=setuptools.find_packages(),
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	classifiers=[
```

