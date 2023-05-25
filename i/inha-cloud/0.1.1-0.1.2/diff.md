# Comparing `tmp/inha_cloud-0.1.1.tar.gz` & `tmp/inha_cloud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inha_cloud-0.1.1.tar", last modified: Thu May 25 20:34:22 2023, max compression
+gzip compressed data, was "inha_cloud-0.1.2.tar", last modified: Thu May 25 20:41:09 2023, max compression
```

## Comparing `inha_cloud-0.1.1.tar` & `inha_cloud-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:34:22.412726 inha_cloud-0.1.1/
--rw-r--r--   0 leejongyoung   (501) staff       (20)     1081 2023-05-25 20:12:18.000000 inha_cloud-0.1.1/LICENSE
--rw-r--r--   0 leejongyoung   (501) staff       (20)      587 2023-05-25 20:34:22.412599 inha_cloud-0.1.1/PKG-INFO
--rw-r--r--   0 leejongyoung   (501) staff       (20)     1883 2023-05-25 20:33:57.000000 inha_cloud-0.1.1/README.md
-drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:34:22.411758 inha_cloud-0.1.1/inha_cloud/
--rw-r--r--   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:33:57.000000 inha_cloud-0.1.1/inha_cloud/__init__.py
--rw-r--r--   0 leejongyoung   (501) staff       (20)     2663 2023-05-25 20:12:18.000000 inha_cloud-0.1.1/inha_cloud/inha_cloud.py
-drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:34:22.412410 inha_cloud-0.1.1/inha_cloud.egg-info/
--rw-r--r--   0 leejongyoung   (501) staff       (20)      587 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/PKG-INFO
--rw-r--r--   0 leejongyoung   (501) staff       (20)      243 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)        1 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)       28 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/requires.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)       11 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/top_level.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)       38 2023-05-25 20:34:22.412794 inha_cloud-0.1.1/setup.cfg
--rw-r--r--   0 leejongyoung   (501) staff       (20)      770 2023-05-25 20:33:57.000000 inha_cloud-0.1.1/setup.py
+drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:41:09.476219 inha_cloud-0.1.2/
+-rw-r--r--   0 leejongyoung   (501) staff       (20)     1081 2023-05-25 20:12:18.000000 inha_cloud-0.1.2/LICENSE
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      587 2023-05-25 20:41:09.476103 inha_cloud-0.1.2/PKG-INFO
+-rw-r--r--   0 leejongyoung   (501) staff       (20)     1883 2023-05-25 20:33:57.000000 inha_cloud-0.1.2/README.md
+drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:41:09.475356 inha_cloud-0.1.2/inha_cloud/
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       25 2023-05-25 20:39:43.000000 inha_cloud-0.1.2/inha_cloud/__init__.py
+-rw-r--r--   0 leejongyoung   (501) staff       (20)     2663 2023-05-25 20:12:18.000000 inha_cloud-0.1.2/inha_cloud/inha_cloud.py
+drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:41:09.475937 inha_cloud-0.1.2/inha_cloud.egg-info/
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      587 2023-05-25 20:41:09.000000 inha_cloud-0.1.2/inha_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      243 2023-05-25 20:41:09.000000 inha_cloud-0.1.2/inha_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)        1 2023-05-25 20:41:09.000000 inha_cloud-0.1.2/inha_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       28 2023-05-25 20:41:09.000000 inha_cloud-0.1.2/inha_cloud.egg-info/requires.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       11 2023-05-25 20:41:09.000000 inha_cloud-0.1.2/inha_cloud.egg-info/top_level.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       38 2023-05-25 20:41:09.476257 inha_cloud-0.1.2/setup.cfg
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      770 2023-05-25 20:40:57.000000 inha_cloud-0.1.2/setup.py
```

### Comparing `inha_cloud-0.1.1/LICENSE` & `inha_cloud-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inha_cloud-0.1.1/PKG-INFO` & `inha_cloud-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inha_cloud
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple fetcher for Inha University login
 Home-page: https://github.com/inha-fc/inha-login-fetcher
 Author: Lee Jongyoung
 Author-email: leejongyoung98@inha.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inha_cloud-0.1.1/README.md` & `inha_cloud-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `inha_cloud-0.1.1/inha_cloud/inha_cloud.py` & `inha_cloud-0.1.2/inha_cloud/inha_cloud.py`

 * *Files identical despite different names*

### Comparing `inha_cloud-0.1.1/inha_cloud.egg-info/PKG-INFO` & `inha_cloud-0.1.2/inha_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inha-cloud
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple fetcher for Inha University login
 Home-page: https://github.com/inha-fc/inha-login-fetcher
 Author: Lee Jongyoung
 Author-email: leejongyoung98@inha.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inha_cloud-0.1.1/setup.py` & `inha_cloud-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="inha_cloud",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     description="A simple fetcher for Inha University login",
     author="Lee Jongyoung",
     author_email="leejongyoung98@inha.edu",
     url="https://github.com/inha-fc/inha-login-fetcher",
     install_requires=[
         'python-dotenv',
```

