# Comparing `tmp/dfmodule-0.0.2.1.tar.gz` & `tmp/dfmodule-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.2.1.tar", last modified: Thu May 25 12:44:58 2023, max compression
+gzip compressed data, was "dfmodule-0.0.2.2.tar", last modified: Thu May 25 12:48:13 2023, max compression
```

## Comparing `dfmodule-0.0.2.1.tar` & `dfmodule-0.0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.098922 dfmodule-0.0.2.1/
--rw-rw-rw-   0        0        0      480 2023-05-25 12:44:58.098922 dfmodule-0.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1434 2023-05-23 08:39:22.000000 dfmodule-0.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.087922 dfmodule-0.0.2.1/common/
--rw-rw-rw-   0        0        0      310 2023-05-25 12:44:49.000000 dfmodule-0.0.2.1/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.087922 dfmodule-0.0.2.1/common/aws_/
--rw-rw-rw-   0        0        0     1009 2023-05-25 12:38:15.000000 dfmodule-0.0.2.1/common/aws_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.097921 dfmodule-0.0.2.1/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      480 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2.1/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 12:44:58.098922 dfmodule-0.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-05-25 12:44:42.000000 dfmodule-0.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:48:13.145054 dfmodule-0.0.2.2/
+-rw-rw-rw-   0        0        0      480 2023-05-25 12:48:13.145054 dfmodule-0.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1434 2023-05-23 08:39:22.000000 dfmodule-0.0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:48:13.132055 dfmodule-0.0.2.2/common/
+-rw-rw-rw-   0        0        0      310 2023-05-25 12:47:59.000000 dfmodule-0.0.2.2/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:48:13.133057 dfmodule-0.0.2.2/common/aws_/
+-rw-rw-rw-   0        0        0     1015 2023-05-25 12:47:45.000000 dfmodule-0.0.2.2/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:48:13.144054 dfmodule-0.0.2.2/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-05-25 12:48:13.000000 dfmodule-0.0.2.2/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-25 12:48:13.000000 dfmodule-0.0.2.2/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:48:13.000000 dfmodule-0.0.2.2/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2.2/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-25 12:48:13.000000 dfmodule-0.0.2.2/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:48:13.145054 dfmodule-0.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-05-25 12:48:01.000000 dfmodule-0.0.2.2/setup.py
```

### Comparing `dfmodule-0.0.2.1/README.md` & `dfmodule-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.2.1/common/aws_/__init__.py` & `dfmodule-0.0.2.2/common/aws_/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-def test():
+def debug_text():
     print('this is modules/aws_ __init__.py')
 
 def send_to_aws_s3_path(data, file_path, accessParams):
     """ 데이터를 AWS S3에 전송하는 함수 """
     import boto3
 
     # AWS S3에 접근하기 위한 클라이언트를 생성한다.
```

### Comparing `dfmodule-0.0.2.1/setup.py` & `dfmodule-0.0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.2.1',
+    version='0.0.2.2',
     description='PYPI tutorial package by howardHamm',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
     install_requires=[],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
```

