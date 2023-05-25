# Comparing `tmp/inha_cloud-0.1.tar.gz` & `tmp/inha_cloud-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inha_cloud-0.1.tar", last modified: Thu May 25 20:17:13 2023, max compression
+gzip compressed data, was "inha_cloud-0.1.1.tar", last modified: Thu May 25 20:34:22 2023, max compression
```

## Comparing `inha_cloud-0.1.tar` & `inha_cloud-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:17:13.047702 inha_cloud-0.1/
--rw-r--r--   0 leejongyoung   (501) staff       (20)     1081 2023-05-25 20:12:18.000000 inha_cloud-0.1/LICENSE
--rw-r--r--   0 leejongyoung   (501) staff       (20)      585 2023-05-25 20:17:13.047597 inha_cloud-0.1/PKG-INFO
--rw-r--r--   0 leejongyoung   (501) staff       (20)     1872 2023-05-25 20:12:18.000000 inha_cloud-0.1/README.md
-drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:17:13.047421 inha_cloud-0.1/inha_cloud.egg-info/
--rw-r--r--   0 leejongyoung   (501) staff       (20)      585 2023-05-25 20:17:13.000000 inha_cloud-0.1/inha_cloud.egg-info/PKG-INFO
--rw-r--r--   0 leejongyoung   (501) staff       (20)      195 2023-05-25 20:17:13.000000 inha_cloud-0.1/inha_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)        1 2023-05-25 20:17:13.000000 inha_cloud-0.1/inha_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)       28 2023-05-25 20:17:13.000000 inha_cloud-0.1/inha_cloud.egg-info/requires.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)        1 2023-05-25 20:17:13.000000 inha_cloud-0.1/inha_cloud.egg-info/top_level.txt
--rw-r--r--   0 leejongyoung   (501) staff       (20)       38 2023-05-25 20:17:13.047740 inha_cloud-0.1/setup.cfg
--rw-r--r--   0 leejongyoung   (501) staff       (20)      768 2023-05-25 20:14:13.000000 inha_cloud-0.1/setup.py
+drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:34:22.412726 inha_cloud-0.1.1/
+-rw-r--r--   0 leejongyoung   (501) staff       (20)     1081 2023-05-25 20:12:18.000000 inha_cloud-0.1.1/LICENSE
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      587 2023-05-25 20:34:22.412599 inha_cloud-0.1.1/PKG-INFO
+-rw-r--r--   0 leejongyoung   (501) staff       (20)     1883 2023-05-25 20:33:57.000000 inha_cloud-0.1.1/README.md
+drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:34:22.411758 inha_cloud-0.1.1/inha_cloud/
+-rw-r--r--   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:33:57.000000 inha_cloud-0.1.1/inha_cloud/__init__.py
+-rw-r--r--   0 leejongyoung   (501) staff       (20)     2663 2023-05-25 20:12:18.000000 inha_cloud-0.1.1/inha_cloud/inha_cloud.py
+drwxr-xr-x   0 leejongyoung   (501) staff       (20)        0 2023-05-25 20:34:22.412410 inha_cloud-0.1.1/inha_cloud.egg-info/
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      587 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      243 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)        1 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       28 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/requires.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       11 2023-05-25 20:34:22.000000 inha_cloud-0.1.1/inha_cloud.egg-info/top_level.txt
+-rw-r--r--   0 leejongyoung   (501) staff       (20)       38 2023-05-25 20:34:22.412794 inha_cloud-0.1.1/setup.cfg
+-rw-r--r--   0 leejongyoung   (501) staff       (20)      770 2023-05-25 20:33:57.000000 inha_cloud-0.1.1/setup.py
```

### Comparing `inha_cloud-0.1/LICENSE` & `inha_cloud-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inha_cloud-0.1/PKG-INFO` & `inha_cloud-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inha_cloud
-Version: 0.1
+Version: 0.1.1
 Summary: A simple fetcher for Inha University login
 Home-page: https://github.com/inha-fc/inha-login-fetcher
 Author: Lee Jongyoung
 Author-email: leejongyoung98@inha.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inha_cloud-0.1/README.md` & `inha_cloud-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```
 
 If the login is successful, the user's name and student ID will be displayed. If it fails, "Login failed." will be displayed.
 
 ## Example
 
 ``` python
-from inha_cloud import InhaCloud
+from inha_cloud.inha_cloud import InhaCloud
 
 def main():
     # Instantiate an InhaCloud object
     inha = InhaCloud()
 
     # Login to the InhaCloud with the username and password stored in the .env file
     inha.login()
```

### Comparing `inha_cloud-0.1/inha_cloud.egg-info/PKG-INFO` & `inha_cloud-0.1.1/inha_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inha-cloud
-Version: 0.1
+Version: 0.1.1
 Summary: A simple fetcher for Inha University login
 Home-page: https://github.com/inha-fc/inha-login-fetcher
 Author: Lee Jongyoung
 Author-email: leejongyoung98@inha.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inha_cloud-0.1/setup.py` & `inha_cloud-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="inha_cloud",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     description="A simple fetcher for Inha University login",
     author="Lee Jongyoung",
     author_email="leejongyoung98@inha.edu",
     url="https://github.com/inha-fc/inha-login-fetcher",
     install_requires=[
         'python-dotenv',
```

