# Comparing `tmp/ronnytest-0.1.0.tar.gz` & `tmp/ronnytest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.1.0.tar", last modified: Thu May 25 02:40:46 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.1.1.tar", last modified: Thu May 25 02:44:25 2023, max compression
```

## Comparing `ronnytest-0.1.0.tar` & `ronnytest-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 02:40:46.000000 ronnytest-0.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 02:40:46.000000 ronnytest-0.1.0/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 02:40:46.000000 ronnytest-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 02:40:46.000000 ronnytest-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-25 02:40:23.000000 ronnytest-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 02:44:25.000000 ronnytest-0.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 02:44:25.000000 ronnytest-0.1.1/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 02:44:25.000000 ronnytest-0.1.1/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 02:44:25.000000 ronnytest-0.1.1/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 02:44:25.000000 ronnytest-0.1.1/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 02:44:25.000000 ronnytest-0.1.1/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 02:44:25.000000 ronnytest-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 02:44:25.000000 ronnytest-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-05-25 02:43:46.000000 ronnytest-0.1.1/setup.py
```

### Comparing `ronnytest-0.1.0/ronnytest.egg-info/PKG-INFO` & `ronnytest-0.1.1/ronnytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.1.0
+Version: 0.1.1
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.1.0/LICENSE` & `ronnytest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.1.0/PKG-INFO` & `ronnytest-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.1.0
+Version: 0.1.1
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.1.0/setup.py` & `ronnytest-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 '''
 Author: ronnyrzyang
 Date: 2023-05-15 19:30:45
 LastEditors: ronnyrzyang@tencent.com
-LastEditTime: 2023-05-25 10:34:19
+LastEditTime: 2023-05-25 10:43:46
 FilePath: /ronnyrzyang/upload_pypi/ronnytest/setup.py
 Description: 
 '''
 import setuptools
 from setuptools.command.install import install as _install
 
-from pip.commands.install import logger
+# from pip.commands.install import logger
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
-notice = \
-    "[!!!] NOTICE: mynotice"
+# notice = \
+#     "[!!!] NOTICE: mynotice"
 
-class install_with_warning(_install):
-    def run(self):
-        _install.run(self)
-        logger.warning(notice)
-        logger.error(notice)
+# class install_with_warning(_install):
+#     def run(self):
+#         _install.run(self)
+#         logger.warning(notice)
+#         logger.error(notice)
 
-logger.error(notice)
+# logger.error(notice)
 
 setuptools.setup(
   name="ronnytest",
-  version="0.1.0",
+  version="0.1.1",
   author="wxpay_sec_team",
   author_email="wxpay_sec_team@tencent.com",
   description="ronnytest",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypi/ronnytest",
   packages=setuptools.find_packages(),
-  cmdclass={'install': install_with_warning},
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
 )
```

