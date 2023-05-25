# Comparing `tmp/dfmodule-0.0.2.4.tar.gz` & `tmp/dfmodule-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.2.4.tar", last modified: Thu May 25 13:09:54 2023, max compression
+gzip compressed data, was "dfmodule-0.0.3.1.tar", last modified: Thu May 25 13:30:58 2023, max compression
```

## Comparing `dfmodule-0.0.2.4.tar` & `dfmodule-0.0.3.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.563883 dfmodule-0.0.2.4/
--rw-rw-rw-   0        0        0      480 2023-05-25 13:09:54.563883 dfmodule-0.0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       80 2023-05-25 13:03:51.000000 dfmodule-0.0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.544584 dfmodule-0.0.2.4/common/
--rw-rw-rw-   0        0        0      310 2023-05-25 13:09:41.000000 dfmodule-0.0.2.4/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.544584 dfmodule-0.0.2.4/common/aws_/
--rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.2.4/common/aws_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.562886 dfmodule-0.0.2.4/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      480 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2.4/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:09:54.563883 dfmodule-0.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-05-25 13:09:42.000000 dfmodule-0.0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:30:58.953099 dfmodule-0.0.3.1/
+-rw-rw-rw-   0        0        0      491 2023-05-25 13:30:58.952099 dfmodule-0.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-25 13:29:16.000000 dfmodule-0.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:30:58.926074 dfmodule-0.0.3.1/common/
+-rw-rw-rw-   0        0        0      310 2023-05-25 13:30:16.000000 dfmodule-0.0.3.1/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:30:58.927073 dfmodule-0.0.3.1/common/aws_/
+-rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.3.1/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:30:58.928074 dfmodule-0.0.3.1/common/b64uuid_/
+-rw-rw-rw-   0        0        0      656 2023-05-25 13:24:03.000000 dfmodule-0.0.3.1/common/b64uuid_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:30:58.952099 dfmodule-0.0.3.1/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-25 13:30:58.000000 dfmodule-0.0.3.1/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-25 13:30:58.000000 dfmodule-0.0.3.1/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:30:58.000000 dfmodule-0.0.3.1/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.3.1/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-05-25 13:30:58.000000 dfmodule-0.0.3.1/dfmodule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 13:30:58.000000 dfmodule-0.0.3.1/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 13:30:58.953099 dfmodule-0.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-05-25 13:30:34.000000 dfmodule-0.0.3.1/setup.py
```

### Comparing `dfmodule-0.0.2.4/common/aws_/__init__.py` & `dfmodule-0.0.3.1/common/aws_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.2.4/setup.py` & `dfmodule-0.0.3.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.2.4',
-    description='PYPI tutorial package by howardHamm',
+    version='0.0.3.1',
+    description='data management project common features module',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
-    install_requires=['boto3'],
+    install_requires=['boto3', 'b64uuid'],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
```

