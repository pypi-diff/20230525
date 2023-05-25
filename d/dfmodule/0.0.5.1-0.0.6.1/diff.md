# Comparing `tmp/dfmodule-0.0.5.1.tar.gz` & `tmp/dfmodule-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.5.1.tar", last modified: Thu May 25 14:30:07 2023, max compression
+gzip compressed data, was "dfmodule-0.0.6.1.tar", last modified: Thu May 25 14:35:15 2023, max compression
```

## Comparing `dfmodule-0.0.5.1.tar` & `dfmodule-0.0.6.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.971144 dfmodule-0.0.5.1/
--rw-rw-rw-   0        0        0      491 2023-05-25 14:30:07.971144 dfmodule-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-05-25 14:14:12.000000 dfmodule-0.0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.939937 dfmodule-0.0.5.1/common/
--rw-rw-rw-   0        0        0      310 2023-05-25 14:13:54.000000 dfmodule-0.0.5.1/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.940938 dfmodule-0.0.5.1/common/aws_/
--rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.5.1/common/aws_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.940938 dfmodule-0.0.5.1/common/b64uuid_/
--rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.5.1/common/b64uuid_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.943937 dfmodule-0.0.5.1/common/compress_/
--rw-rw-rw-   0        0        0     3702 2023-05-25 13:38:02.000000 dfmodule-0.0.5.1/common/compress_/__init__.py
--rw-rw-rw-   0        0        0      463 2023-05-25 13:37:03.000000 dfmodule-0.0.5.1/common/compress_/gzip_.py
--rw-rw-rw-   0        0        0      463 2023-04-26 23:23:30.000000 dfmodule-0.0.5.1/common/compress_/lzma_.py
--rw-rw-rw-   0        0        0      480 2023-04-26 23:23:30.000000 dfmodule-0.0.5.1/common/compress_/zlib_.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.944940 dfmodule-0.0.5.1/common/cryptography_/
--rw-rw-rw-   0        0        0      751 2023-05-25 13:52:18.000000 dfmodule-0.0.5.1/common/cryptography_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.970154 dfmodule-0.0.5.1/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.5.1/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:30:07.971144 dfmodule-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-05-25 14:13:49.000000 dfmodule-0.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.514068 dfmodule-0.0.6.1/
+-rw-rw-rw-   0        0        0      491 2023-05-25 14:35:15.514068 dfmodule-0.0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-25 14:35:13.000000 dfmodule-0.0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.486310 dfmodule-0.0.6.1/common/
+-rw-rw-rw-   0        0        0      310 2023-05-25 14:34:44.000000 dfmodule-0.0.6.1/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.487311 dfmodule-0.0.6.1/common/aws_/
+-rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.6.1/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.487311 dfmodule-0.0.6.1/common/b64uuid_/
+-rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.6.1/common/b64uuid_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.490309 dfmodule-0.0.6.1/common/compress_/
+-rw-rw-rw-   0        0        0     3702 2023-05-25 13:38:02.000000 dfmodule-0.0.6.1/common/compress_/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-05-25 13:37:03.000000 dfmodule-0.0.6.1/common/compress_/gzip_.py
+-rw-rw-rw-   0        0        0      463 2023-04-26 23:23:30.000000 dfmodule-0.0.6.1/common/compress_/lzma_.py
+-rw-rw-rw-   0        0        0      480 2023-04-26 23:23:30.000000 dfmodule-0.0.6.1/common/compress_/zlib_.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.491309 dfmodule-0.0.6.1/common/cryptography_/
+-rw-rw-rw-   0        0        0      751 2023-05-25 13:52:18.000000 dfmodule-0.0.6.1/common/cryptography_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.491309 dfmodule-0.0.6.1/common/json_/
+-rw-rw-rw-   0        0        0      770 2023-05-25 14:34:30.000000 dfmodule-0.0.6.1/common/json_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:35:15.513547 dfmodule-0.0.6.1/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-25 14:35:15.000000 dfmodule-0.0.6.1/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-05-25 14:35:15.000000 dfmodule-0.0.6.1/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:35:15.000000 dfmodule-0.0.6.1/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.6.1/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-25 14:35:15.000000 dfmodule-0.0.6.1/dfmodule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 14:35:15.000000 dfmodule-0.0.6.1/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:35:15.515066 dfmodule-0.0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-05-25 14:34:47.000000 dfmodule-0.0.6.1/setup.py
```

### Comparing `dfmodule-0.0.5.1/common/aws_/__init__.py` & `dfmodule-0.0.6.1/common/aws_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.5.1/common/b64uuid_/__init__.py` & `dfmodule-0.0.6.1/common/b64uuid_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.5.1/common/compress_/__init__.py` & `dfmodule-0.0.6.1/common/compress_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.5.1/common/cryptography_/__init__.py` & `dfmodule-0.0.6.1/common/cryptography_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.5.1/setup.py` & `dfmodule-0.0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.5.1',
+    version='0.0.6.1',
     description='data management project common features module',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
     install_requires=['boto3', 'b64uuid', 'cryptography'],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
```

