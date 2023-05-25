# Comparing `tmp/gscdash-0.0.1.tar.gz` & `tmp/gscdash-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscdash-0.0.1.tar", last modified: Thu May 25 21:51:52 2023, max compression
+gzip compressed data, was "gscdash-0.0.2.tar", last modified: Thu May 25 21:56:06 2023, max compression
```

## Comparing `gscdash-0.0.1.tar` & `gscdash-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:51:52.660620 gscdash-0.0.1/
--rw-r--r--   0 zives      (501) staff       (20)    34523 2023-04-14 14:43:14.000000 gscdash-0.0.1/LICENSE.TXT
--rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 21:51:52.660676 gscdash-0.0.1/PKG-INFO
--rw-r--r--   0 zives      (501) staff       (20)     4831 2023-05-25 21:44:35.000000 gscdash-0.0.1/README.md
-drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:51:52.658884 gscdash-0.0.1/gscdash/
-drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:51:52.660478 gscdash-0.0.1/gscdash/gscdash.egg-info/
--rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 21:51:52.000000 gscdash-0.0.1/gscdash/gscdash.egg-info/PKG-INFO
--rw-r--r--   0 zives      (501) staff       (20)      249 2023-05-25 21:51:52.000000 gscdash-0.0.1/gscdash/gscdash.egg-info/SOURCES.txt
--rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 21:51:52.000000 gscdash-0.0.1/gscdash/gscdash.egg-info/dependency_links.txt
--rw-r--r--   0 zives      (501) staff       (20)       62 2023-05-25 21:51:52.000000 gscdash-0.0.1/gscdash/gscdash.egg-info/requires.txt
--rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 21:51:52.000000 gscdash-0.0.1/gscdash/gscdash.egg-info/top_level.txt
--rw-r--r--   0 zives      (501) staff       (20)      255 2023-05-25 21:35:46.000000 gscdash-0.0.1/pyproject.toml
--rw-r--r--   0 zives      (501) staff       (20)      185 2023-05-25 21:51:52.660897 gscdash-0.0.1/setup.cfg
--rw-r--r--   0 zives      (501) staff       (20)      944 2023-05-25 21:51:38.000000 gscdash-0.0.1/setup.py
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:56:06.243268 gscdash-0.0.2/
+-rw-r--r--   0 zives      (501) staff       (20)    34523 2023-04-14 14:43:14.000000 gscdash-0.0.2/LICENSE.TXT
+-rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 21:56:06.243338 gscdash-0.0.2/PKG-INFO
+-rw-r--r--   0 zives      (501) staff       (20)     4831 2023-05-25 21:44:35.000000 gscdash-0.0.2/README.md
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:56:06.243068 gscdash-0.0.2/gscdash.egg-info/
+-rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/PKG-INFO
+-rw-r--r--   0 zives      (501) staff       (20)      209 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/SOURCES.txt
+-rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/dependency_links.txt
+-rw-r--r--   0 zives      (501) staff       (20)       62 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/requires.txt
+-rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/top_level.txt
+-rw-r--r--   0 zives      (501) staff       (20)      255 2023-05-25 21:55:55.000000 gscdash-0.0.2/pyproject.toml
+-rw-r--r--   0 zives      (501) staff       (20)      185 2023-05-25 21:56:06.243600 gscdash-0.0.2/setup.cfg
+-rw-r--r--   0 zives      (501) staff       (20)      951 2023-05-25 21:55:51.000000 gscdash-0.0.2/setup.py
```

### Comparing `gscdash-0.0.1/LICENSE.TXT` & `gscdash-0.0.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `gscdash-0.0.1/PKG-INFO` & `gscdash-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscdash
-Version: 0.0.1
+Version: 0.0.2
 Summary: Gradescope-Canvas Dashboard support
 Home-page: https://github.com/upenn/gradescope-canvas-dashboard
 Author: Zack Ives
 Author-email: zives@cis.upenn.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `gscdash-0.0.1/README.md` & `gscdash-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gscdash-0.0.1/gscdash/gscdash.egg-info/PKG-INFO` & `gscdash-0.0.2/gscdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscdash
-Version: 0.0.1
+Version: 0.0.2
 Summary: Gradescope-Canvas Dashboard support
 Home-page: https://github.com/upenn/gradescope-canvas-dashboard
 Author: Zack Ives
 Author-email: zives@cis.upenn.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `gscdash-0.0.1/setup.py` & `gscdash-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "gscdash",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Zack Ives",
     author_email = "zives@cis.upenn.edu",
     description = "Gradescope-Canvas Dashboard support",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/upenn/gradescope-canvas-dashboard",
     classifiers = [
@@ -22,11 +22,11 @@
         "html5lib",
         "beautifulsoup4",
         "canvasapi",
         "pandas",
         "pytz",
         "pyyaml",
     ],
-    package_dir = {"": "gscdash"},
+    package_dir = {"gscdash": "gscdash"},
     packages = setuptools.find_packages(where="gscdash"),
     python_requires = ">=3.9"
 )
```

