# Comparing `tmp/corby-0.0.7.tar.gz` & `tmp/corby-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.0.7.tar", last modified: Wed May 24 15:31:11 2023, max compression
+gzip compressed data, was "corby-0.0.8.tar", last modified: Thu May 25 09:24:33 2023, max compression
```

## Comparing `corby-0.0.7.tar` & `corby-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:31:11.348651 corby-0.0.7/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:31:11.348217 corby-0.0.7/PKG-INFO
--rw-r--r--   0 ji.hervas   (504) staff       (20)        9 2023-05-24 14:54:54.000000 corby-0.0.7/README.md
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:31:11.342704 corby-0.0.7/corby/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      244 2023-05-24 15:21:28.000000 corby-0.0.7/corby/__init__.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)      244 2023-05-24 15:30:37.000000 corby-0.0.7/corby/__main__.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:31:11.345917 corby-0.0.7/corby/generator/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:56.000000 corby-0.0.7/corby/generator/__init__.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:31:11.347509 corby-0.0.7/corby/generator/chatbot/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:59.000000 corby-0.0.7/corby/generator/chatbot/__init__.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)     2028 2023-05-24 14:28:51.000000 corby-0.0.7/corby/generator/chatbot/cli.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)      392 2023-05-24 13:28:19.000000 corby-0.0.7/corby/generator/chatbot/index.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)     1186 2023-05-24 15:30:49.000000 corby-0.0.7/corby/index.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:31:11.345441 corby-0.0.7/corby.egg-info/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:31:11.000000 corby-0.0.7/corby.egg-info/PKG-INFO
--rw-r--r--   0 ji.hervas   (504) staff       (20)      341 2023-05-24 15:31:11.000000 corby-0.0.7/corby.egg-info/SOURCES.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)        1 2023-05-24 15:31:11.000000 corby-0.0.7/corby.egg-info/dependency_links.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)       26 2023-05-24 15:31:11.000000 corby-0.0.7/corby.egg-info/requires.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)        6 2023-05-24 15:31:11.000000 corby-0.0.7/corby.egg-info/top_level.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)       38 2023-05-24 15:31:11.348816 corby-0.0.7/setup.cfg
--rw-r--r--   0 ji.hervas   (504) staff       (20)      518 2023-05-24 15:30:54.000000 corby-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.139398 corby-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 09:24:14.000000 corby-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-25 09:24:33.139398 corby-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-25 09:24:14.000000 corby-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.135398 corby-0.0.8/corby/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 09:24:14.000000 corby-0.0.8/corby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 09:24:14.000000 corby-0.0.8/corby/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.139398 corby-0.0.8/corby/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.139398 corby-0.0.8/corby/generator/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/chatbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/chatbot/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 09:24:14.000000 corby-0.0.8/corby/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.135398 corby-0.0.8/corby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:24:33.139398 corby-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 09:24:14.000000 corby-0.0.8/setup.py
```

### Comparing `corby-0.0.7/setup.py` & `corby-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from setuptools import setup, find_packages
+'''Pypi setup file for corby'''
 
-python_requires='>=3.6',
+from setuptools import setup, find_packages
 
 setup(
     name="corby",
-    version="0.0.7",
+    version="0.0.8",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
-    long_description=open("README.md").read(),
+    # pylint: disable=consider-using-with
+    long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         "inquirer",
```

