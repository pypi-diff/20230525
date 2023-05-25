# Comparing `tmp/ronnytest-0.0.9.tar.gz` & `tmp/ronnytest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.0.9.tar", last modified: Wed May 24 12:54:00 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.1.0.tar", last modified: Thu May 25 02:40:46 2023, max compression
```

## Comparing `ronnytest-0.0.9.tar` & `ronnytest-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:54:00.000000 ronnytest-0.0.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:54:00.000000 ronnytest-0.0.9/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:54:00.000000 ronnytest-0.0.9/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:54:00.000000 ronnytest-0.0.9/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 12:54:00.000000 ronnytest-0.0.9/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:54:00.000000 ronnytest-0.0.9/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:54:00.000000 ronnytest-0.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:54:00.000000 ronnytest-0.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      970 2023-05-24 12:53:34.000000 ronnytest-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 02:40:46.000000 ronnytest-0.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 02:40:46.000000 ronnytest-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 02:40:46.000000 ronnytest-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-25 02:40:23.000000 ronnytest-0.1.0/setup.py
```

### Comparing `ronnytest-0.0.9/ronnytest.egg-info/PKG-INFO` & `ronnytest-0.1.0/ronnytest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.0.9
+Version: 0.1.0
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.0.9/LICENSE` & `ronnytest-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.0.9/PKG-INFO` & `ronnytest-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.0.9
+Version: 0.1.0
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.0.9/setup.py` & `ronnytest-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+'''
+Author: ronnyrzyang
+Date: 2023-05-15 19:30:45
+LastEditors: ronnyrzyang@tencent.com
+LastEditTime: 2023-05-25 10:34:19
+FilePath: /ronnyrzyang/upload_pypi/ronnytest/setup.py
+Description: 
+'''
 import setuptools
 from setuptools.command.install import install as _install
 
-try:
-  from pip.commands.install import logger
-except Exception as e:
-   print('don not install!')
+from pip.commands.install import logger
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 notice = \
     "[!!!] NOTICE: mynotice"
 
@@ -18,22 +23,24 @@
         logger.warning(notice)
         logger.error(notice)
 
 logger.error(notice)
 
 setuptools.setup(
   name="ronnytest",
-  version="0.0.9",
+  version="0.1.0",
   author="wxpay_sec_team",
   author_email="wxpay_sec_team@tencent.com",
   description="ronnytest",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypi/ronnytest",
   packages=setuptools.find_packages(),
   cmdclass={'install': install_with_warning},
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
-)
+)
+
+raise RuntimeError('do not install!')
```

