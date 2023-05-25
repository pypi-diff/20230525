# Comparing `tmp/TimePrintOnPYPI-1.1.0.tar.gz` & `tmp/TimePrintOnPYPI-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.1.0.tar", last modified: Thu May 18 18:18:48 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.2.0.tar", last modified: Thu May 25 20:39:50 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.1.0.tar` & `TimePrintOnPYPI-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 18:18:48.475342 TimePrintOnPYPI-1.1.0/
--rw-rw-rw-   0        0        0      445 2023-05-18 18:18:48.474341 TimePrintOnPYPI-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 18:18:48.453697 TimePrintOnPYPI-1.1.0/TimePrint/
--rw-rw-rw-   0        0        0     1064 2023-05-18 18:16:21.000000 TimePrintOnPYPI-1.1.0/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:18:48.472337 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0      445 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 18:18:48.475342 TimePrintOnPYPI-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-05-18 18:16:57.000000 TimePrintOnPYPI-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:39:50.542334 TimePrintOnPYPI-1.2.0/
+-rw-rw-rw-   0        0        0      445 2023-05-25 20:39:50.540760 TimePrintOnPYPI-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 20:39:50.519175 TimePrintOnPYPI-1.2.0/TimePrint/
+-rw-rw-rw-   0        0        0     1140 2023-05-25 20:38:40.000000 TimePrintOnPYPI-1.2.0/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:39:50.539759 TimePrintOnPYPI-1.2.0/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0      445 2023-05-25 20:39:50.000000 TimePrintOnPYPI-1.2.0/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-05-25 20:39:50.000000 TimePrintOnPYPI-1.2.0/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 20:39:50.000000 TimePrintOnPYPI-1.2.0/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 20:39:50.000000 TimePrintOnPYPI-1.2.0/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 20:39:50.543309 TimePrintOnPYPI-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-25 20:37:21.000000 TimePrintOnPYPI-1.2.0/setup.py
```

### Comparing `TimePrintOnPYPI-1.1.0/TimePrint/__init__.py` & `TimePrintOnPYPI-1.2.0/TimePrint/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,8 +18,10 @@
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.1.0")
+    print("Version: 1.2.0")
+def timetag(format):
+    return time.strftime(format, time.localtime())
```

### Comparing `TimePrintOnPYPI-1.1.0/setup.py` & `TimePrintOnPYPI-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='TimePrintOnPYPI',
-    version='1.1.0',
+    version='1.2.0',
     description='A package for printing text with time delay between characters',
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
     packages=['TimePrint'],
     classifiers=[
```

