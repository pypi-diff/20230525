# Comparing `tmp/dfmodule-0.0.4.2.tar.gz` & `tmp/dfmodule-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.4.2.tar", last modified: Thu May 25 13:44:55 2023, max compression
+gzip compressed data, was "dfmodule-0.0.5.1.tar", last modified: Thu May 25 14:30:07 2023, max compression
```

## Comparing `dfmodule-0.0.4.2.tar` & `dfmodule-0.0.5.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:44:55.537639 dfmodule-0.0.4.2/
--rw-rw-rw-   0        0        0      491 2023-05-25 13:44:55.536642 dfmodule-0.0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-25 13:38:17.000000 dfmodule-0.0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:44:55.514616 dfmodule-0.0.4.2/common/
--rw-rw-rw-   0        0        0      310 2023-05-25 13:44:46.000000 dfmodule-0.0.4.2/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:44:55.515616 dfmodule-0.0.4.2/common/aws_/
--rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.4.2/common/aws_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:44:55.516616 dfmodule-0.0.4.2/common/b64uuid_/
--rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.4.2/common/b64uuid_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:44:55.518617 dfmodule-0.0.4.2/common/compress_/
--rw-rw-rw-   0        0        0     3702 2023-05-25 13:38:02.000000 dfmodule-0.0.4.2/common/compress_/__init__.py
--rw-rw-rw-   0        0        0      463 2023-05-25 13:37:03.000000 dfmodule-0.0.4.2/common/compress_/gzip_.py
--rw-rw-rw-   0        0        0      463 2023-04-26 23:23:30.000000 dfmodule-0.0.4.2/common/compress_/lzma_.py
--rw-rw-rw-   0        0        0      480 2023-04-26 23:23:30.000000 dfmodule-0.0.4.2/common/compress_/zlib_.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:44:55.536642 dfmodule-0.0.4.2/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-25 13:44:55.000000 dfmodule-0.0.4.2/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-05-25 13:44:55.000000 dfmodule-0.0.4.2/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:44:55.000000 dfmodule-0.0.4.2/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.4.2/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-05-25 13:44:55.000000 dfmodule-0.0.4.2/dfmodule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 13:44:55.000000 dfmodule-0.0.4.2/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:44:55.537639 dfmodule-0.0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-05-25 13:44:43.000000 dfmodule-0.0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.971144 dfmodule-0.0.5.1/
+-rw-rw-rw-   0        0        0      491 2023-05-25 14:30:07.971144 dfmodule-0.0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-05-25 14:14:12.000000 dfmodule-0.0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.939937 dfmodule-0.0.5.1/common/
+-rw-rw-rw-   0        0        0      310 2023-05-25 14:13:54.000000 dfmodule-0.0.5.1/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.940938 dfmodule-0.0.5.1/common/aws_/
+-rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.5.1/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.940938 dfmodule-0.0.5.1/common/b64uuid_/
+-rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.5.1/common/b64uuid_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.943937 dfmodule-0.0.5.1/common/compress_/
+-rw-rw-rw-   0        0        0     3702 2023-05-25 13:38:02.000000 dfmodule-0.0.5.1/common/compress_/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-05-25 13:37:03.000000 dfmodule-0.0.5.1/common/compress_/gzip_.py
+-rw-rw-rw-   0        0        0      463 2023-04-26 23:23:30.000000 dfmodule-0.0.5.1/common/compress_/lzma_.py
+-rw-rw-rw-   0        0        0      480 2023-04-26 23:23:30.000000 dfmodule-0.0.5.1/common/compress_/zlib_.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.944940 dfmodule-0.0.5.1/common/cryptography_/
+-rw-rw-rw-   0        0        0      751 2023-05-25 13:52:18.000000 dfmodule-0.0.5.1/common/cryptography_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:30:07.970154 dfmodule-0.0.5.1/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.5.1/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 14:30:07.000000 dfmodule-0.0.5.1/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:30:07.971144 dfmodule-0.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-05-25 14:13:49.000000 dfmodule-0.0.5.1/setup.py
```

### Comparing `dfmodule-0.0.4.2/common/aws_/__init__.py` & `dfmodule-0.0.5.1/common/aws_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.4.2/common/b64uuid_/__init__.py` & `dfmodule-0.0.5.1/common/b64uuid_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.4.2/common/compress_/__init__.py` & `dfmodule-0.0.5.1/common/compress_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.4.2/setup.py` & `dfmodule-0.0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.4.2',
+    version='0.0.5.1',
     description='data management project common features module',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
-    install_requires=['boto3', 'b64uuid'],
+    install_requires=['boto3', 'b64uuid', 'cryptography'],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
```

