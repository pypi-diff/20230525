# Comparing `tmp/dfmodule-0.0.7.tar.gz` & `tmp/dfmodule-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.7.tar", last modified: Thu May 25 14:40:09 2023, max compression
+gzip compressed data, was "dfmodule-0.0.8.tar", last modified: Thu May 25 14:48:12 2023, max compression
```

## Comparing `dfmodule-0.0.7.tar` & `dfmodule-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.612998 dfmodule-0.0.7/
--rw-rw-rw-   0        0        0      489 2023-05-25 14:40:09.611997 dfmodule-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-25 14:35:13.000000 dfmodule-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.588997 dfmodule-0.0.7/common/
--rw-rw-rw-   0        0        0      308 2023-05-25 14:39:51.000000 dfmodule-0.0.7/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.589996 dfmodule-0.0.7/common/aws_/
--rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.7/common/aws_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.590998 dfmodule-0.0.7/common/b64uuid_/
--rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.7/common/b64uuid_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.592998 dfmodule-0.0.7/common/compress_/
--rw-rw-rw-   0        0        0     3702 2023-05-25 13:38:02.000000 dfmodule-0.0.7/common/compress_/__init__.py
--rw-rw-rw-   0        0        0      463 2023-05-25 13:37:03.000000 dfmodule-0.0.7/common/compress_/gzip_.py
--rw-rw-rw-   0        0        0      463 2023-04-26 23:23:30.000000 dfmodule-0.0.7/common/compress_/lzma_.py
--rw-rw-rw-   0        0        0      480 2023-04-26 23:23:30.000000 dfmodule-0.0.7/common/compress_/zlib_.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.593997 dfmodule-0.0.7/common/cryptography_/
--rw-rw-rw-   0        0        0      751 2023-05-25 13:52:18.000000 dfmodule-0.0.7/common/cryptography_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.594484 dfmodule-0.0.7/common/json_/
--rw-rw-rw-   0        0        0      770 2023-05-25 14:34:30.000000 dfmodule-0.0.7/common/json_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.595997 dfmodule-0.0.7/common/requests_/
--rw-rw-rw-   0        0        0      474 2023-05-25 14:39:58.000000 dfmodule-0.0.7/common/requests_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:40:09.611997 dfmodule-0.0.7/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      489 2023-05-25 14:40:09.000000 dfmodule-0.0.7/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-05-25 14:40:09.000000 dfmodule-0.0.7/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:40:09.000000 dfmodule-0.0.7/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.7/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2023-05-25 14:40:09.000000 dfmodule-0.0.7/dfmodule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 14:40:09.000000 dfmodule-0.0.7/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:40:09.612998 dfmodule-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-05-25 14:39:47.000000 dfmodule-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.746018 dfmodule-0.0.8/
+-rw-rw-rw-   0        0        0      489 2023-05-25 14:48:12.745018 dfmodule-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-05-25 14:44:02.000000 dfmodule-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.724017 dfmodule-0.0.8/common/
+-rw-rw-rw-   0        0        0      308 2023-05-25 14:44:14.000000 dfmodule-0.0.8/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.725018 dfmodule-0.0.8/common/aws_/
+-rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.8/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.725018 dfmodule-0.0.8/common/b64uuid_/
+-rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.8/common/b64uuid_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.728019 dfmodule-0.0.8/common/compress_/
+-rw-rw-rw-   0        0        0     3702 2023-05-25 13:38:02.000000 dfmodule-0.0.8/common/compress_/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-05-25 13:37:03.000000 dfmodule-0.0.8/common/compress_/gzip_.py
+-rw-rw-rw-   0        0        0      463 2023-04-26 23:23:30.000000 dfmodule-0.0.8/common/compress_/lzma_.py
+-rw-rw-rw-   0        0        0      480 2023-04-26 23:23:30.000000 dfmodule-0.0.8/common/compress_/zlib_.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.729018 dfmodule-0.0.8/common/cryptography_/
+-rw-rw-rw-   0        0        0      751 2023-05-25 13:52:18.000000 dfmodule-0.0.8/common/cryptography_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.729018 dfmodule-0.0.8/common/json_/
+-rw-rw-rw-   0        0        0      770 2023-05-25 14:34:30.000000 dfmodule-0.0.8/common/json_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.730016 dfmodule-0.0.8/common/requests_/
+-rw-rw-rw-   0        0        0      474 2023-05-25 14:39:58.000000 dfmodule-0.0.8/common/requests_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.731017 dfmodule-0.0.8/common/times_/
+-rw-rw-rw-   0        0        0     1078 2023-05-25 14:43:26.000000 dfmodule-0.0.8/common/times_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:48:12.745018 dfmodule-0.0.8/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-25 14:48:12.000000 dfmodule-0.0.8/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-05-25 14:48:12.000000 dfmodule-0.0.8/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:48:12.000000 dfmodule-0.0.8/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.8/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-05-25 14:48:12.000000 dfmodule-0.0.8/dfmodule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 14:48:12.000000 dfmodule-0.0.8/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:48:12.746018 dfmodule-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-05-25 14:44:10.000000 dfmodule-0.0.8/setup.py
```

### Comparing `dfmodule-0.0.7/common/aws_/__init__.py` & `dfmodule-0.0.8/common/aws_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.7/common/b64uuid_/__init__.py` & `dfmodule-0.0.8/common/b64uuid_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.7/common/compress_/__init__.py` & `dfmodule-0.0.8/common/compress_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.7/common/cryptography_/__init__.py` & `dfmodule-0.0.8/common/cryptography_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.7/common/json_/__init__.py` & `dfmodule-0.0.8/common/json_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.7/setup.py` & `dfmodule-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.7',
+    version='0.0.8',
     description='data management project common features module',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
     install_requires=['boto3', 'b64uuid', 'cryptography', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
```

