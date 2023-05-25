# Comparing `tmp/dfmodule-0.0.1.tar.gz` & `tmp/dfmodule-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.1.tar", last modified: Tue May 23 02:49:51 2023, max compression
+gzip compressed data, was "dfmodule-0.0.2.1.tar", last modified: Thu May 25 12:44:58 2023, max compression
```

## Comparing `dfmodule-0.0.1.tar` & `dfmodule-0.0.2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:49:51.562770 dfmodule-0.0.1/
--rw-rw-rw-   0        0        0      426 2023-05-23 02:49:51.562770 dfmodule-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-05-23 02:43:44.000000 dfmodule-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 02:49:51.546767 dfmodule-0.0.1/common/
--rw-rw-rw-   0        0        0       21 2023-05-23 02:38:36.000000 dfmodule-0.0.1/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:49:51.561765 dfmodule-0.0.1/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      426 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 02:49:51.563766 dfmodule-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      643 2023-05-23 02:36:00.000000 dfmodule-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.098922 dfmodule-0.0.2.1/
+-rw-rw-rw-   0        0        0      480 2023-05-25 12:44:58.098922 dfmodule-0.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1434 2023-05-23 08:39:22.000000 dfmodule-0.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.087922 dfmodule-0.0.2.1/common/
+-rw-rw-rw-   0        0        0      310 2023-05-25 12:44:49.000000 dfmodule-0.0.2.1/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.087922 dfmodule-0.0.2.1/common/aws_/
+-rw-rw-rw-   0        0        0     1009 2023-05-25 12:38:15.000000 dfmodule-0.0.2.1/common/aws_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:44:58.097921 dfmodule-0.0.2.1/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2.1/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-25 12:44:58.000000 dfmodule-0.0.2.1/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:44:58.098922 dfmodule-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-05-25 12:44:42.000000 dfmodule-0.0.2.1/setup.py
```

### Comparing `dfmodule-0.0.1/setup.py` & `dfmodule-0.0.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.1',
+    version='0.0.2.1',
     description='PYPI tutorial package by howardHamm',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
     install_requires=[],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
@@ -14,9 +14,10 @@
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

