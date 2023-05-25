# Comparing `tmp/dfmodule-0.0.2.3.tar.gz` & `tmp/dfmodule-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.2.3.tar", last modified: Thu May 25 13:04:26 2023, max compression
+gzip compressed data, was "dfmodule-0.0.2.4.tar", last modified: Thu May 25 13:09:54 2023, max compression
```

## Comparing `dfmodule-0.0.2.3.tar` & `dfmodule-0.0.2.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:04:26.793932 dfmodule-0.0.2.3/
--rw-rw-rw-   0        0        0      480 2023-05-25 13:04:26.793932 dfmodule-0.0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       80 2023-05-25 13:03:51.000000 dfmodule-0.0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:04:26.782932 dfmodule-0.0.2.3/common/
--rw-rw-rw-   0        0        0      310 2023-05-25 13:04:21.000000 dfmodule-0.0.2.3/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:04:26.783931 dfmodule-0.0.2.3/common/aws_/
--rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.2.3/common/aws_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:04:26.792931 dfmodule-0.0.2.3/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      480 2023-05-25 13:04:26.000000 dfmodule-0.0.2.3/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-25 13:04:26.000000 dfmodule-0.0.2.3/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:04:26.000000 dfmodule-0.0.2.3/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2.3/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-25 13:04:26.000000 dfmodule-0.0.2.3/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:04:26.793932 dfmodule-0.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-05-25 13:04:22.000000 dfmodule-0.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.563883 dfmodule-0.0.2.4/
+-rw-rw-rw-   0        0        0      480 2023-05-25 13:09:54.563883 dfmodule-0.0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2023-05-25 13:03:51.000000 dfmodule-0.0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.544584 dfmodule-0.0.2.4/common/
+-rw-rw-rw-   0        0        0      310 2023-05-25 13:09:41.000000 dfmodule-0.0.2.4/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.544584 dfmodule-0.0.2.4/common/aws_/
+-rw-rw-rw-   0        0        0     1159 2023-05-25 13:02:04.000000 dfmodule-0.0.2.4/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:09:54.562886 dfmodule-0.0.2.4/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2.4/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 13:09:54.000000 dfmodule-0.0.2.4/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 13:09:54.563883 dfmodule-0.0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-05-25 13:09:42.000000 dfmodule-0.0.2.4/setup.py
```

### Comparing `dfmodule-0.0.2.3/common/aws_/__init__.py` & `dfmodule-0.0.2.4/common/aws_/__init__.py`

 * *Files identical despite different names*

### Comparing `dfmodule-0.0.2.3/setup.py` & `dfmodule-0.0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.2.3',
+    version='0.0.2.4',
     description='PYPI tutorial package by howardHamm',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
-    install_requires=[],
+    install_requires=['boto3'],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
```

