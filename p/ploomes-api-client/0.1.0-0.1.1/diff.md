# Comparing `tmp/ploomes-api-client-0.1.0.tar.gz` & `tmp/ploomes-api-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.0.tar", last modified: Thu May 25 21:12:32 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.1.tar", last modified: Thu May 25 21:21:14 2023, max compression
```

## Comparing `ploomes-api-client-0.1.0.tar` & `ploomes-api-client-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:12:32.431108 ploomes-api-client-0.1.0/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.0/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     1001 2023-05-25 21:12:32.430854 ploomes-api-client-0.1.0/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      255 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.0/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:12:32.427109 ploomes-api-client-0.1.0/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1001 2023-05-25 21:12:32.000000 ploomes-api-client-0.1.0/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-25 21:12:32.000000 ploomes-api-client-0.1.0/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-25 21:12:32.000000 ploomes-api-client-0.1.0/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-25 21:12:32.000000 ploomes-api-client-0.1.0/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-25 21:12:32.000000 ploomes-api-client-0.1.0/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:12:32.429174 ploomes-api-client-0.1.0/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-25 21:10:14.000000 ploomes-api-client-0.1.0/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    21748 2023-05-25 21:10:21.000000 ploomes-api-client-0.1.0/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-25 21:12:32.433452 ploomes-api-client-0.1.0/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-25 21:12:12.000000 ploomes-api-client-0.1.0/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:21:14.664690 ploomes-api-client-0.1.1/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.1/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2301 2023-05-25 21:21:14.664125 ploomes-api-client-0.1.1/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1139 2023-05-25 21:19:00.000000 ploomes-api-client-0.1.1/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:21:14.662996 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2301 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:21:14.663399 ploomes-api-client-0.1.1/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-25 21:10:14.000000 ploomes-api-client-0.1.1/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    21748 2023-05-25 21:10:21.000000 ploomes-api-client-0.1.1/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-25 21:21:14.664777 ploomes-api-client-0.1.1/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-25 21:19:52.000000 ploomes-api-client-0.1.1/setup.py
```

### Comparing `ploomes-api-client-0.1.0/LICENSE` & `ploomes-api-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.0/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.1/ploomes_client/ploomes_client.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.0/setup.py` & `ploomes-api-client-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

