# Comparing `tmp/ronnytest-0.2.1.tar.gz` & `tmp/ronnytest-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.2.1.tar", last modified: Thu May 25 08:11:14 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.2.2.tar", last modified: Thu May 25 08:24:10 2023, max compression
```

## Comparing `ronnytest-0.2.1.tar` & `ronnytest-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:11:14.000000 ronnytest-0.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:11:14.000000 ronnytest-0.2.1/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:11:13.000000 ronnytest-0.2.1/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:11:13.000000 ronnytest-0.2.1/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 08:11:13.000000 ronnytest-0.2.1/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:11:13.000000 ronnytest-0.2.1/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:11:14.000000 ronnytest-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:11:14.000000 ronnytest-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-25 08:11:11.000000 ronnytest-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:24:10.000000 ronnytest-0.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:24:10.000000 ronnytest-0.2.2/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:24:10.000000 ronnytest-0.2.2/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:24:10.000000 ronnytest-0.2.2/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 08:24:10.000000 ronnytest-0.2.2/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:24:10.000000 ronnytest-0.2.2/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:24:10.000000 ronnytest-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:24:10.000000 ronnytest-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      976 2023-05-25 08:24:07.000000 ronnytest-0.2.2/setup.py
```

### Comparing `ronnytest-0.2.1/LICENSE` & `ronnytest-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.2.1/setup.py` & `ronnytest-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup,find_packages
 from setuptools.command.install import install
 
 def _post_install(setup):
     def _post_actions():
-        print('\033[91m腾讯安全团队发现您当前试图从pypi官方源下载公司内部的私有包！\033[0m'.encode('utf-8').decode('latin1'))
-        print('\033[91m按照腾讯公司安全规范，不得下载未经安全评估和确认的第三方私有包，已阻止您本次下载行为!\033[0m'.encode('utf-8').decode('latin1'))
-        print('\033[91m请使用pip intall your_package_name --index-url=https://mirrors.tencent.com/#/private/pypi 强制指定公司内部源进行私有包下载！\033[0m'.encode('utf-8').decode('latin1'))
+        print('腾讯安全团队发现您当前试图从pypi官方源下载公司内部的私有包！'.encode('utf-8').decode('latin1'))
+        print('按照腾讯公司安全规范，不得下载未经安全评估和确认的第三方私有包，已阻止您本次下载行为!'.encode('utf-8').decode('latin1'))
+        print('请使用pip intall your_package_name --index-url=https://mirrors.tencent.com/#/private/pypi 强制指定公司内部源进行私有包下载！'.encode('utf-8').decode('latin1'))
         raise RuntimeError('do not install!')
     _post_actions()
     return setup
 
 setup(
     name = 'ronnytest',
-    version = '0.2.1',
+    version = '0.2.2',
     author = 'wxpay_sec_team',
     author_email = 'wxpay_sec_team@tencent.com',
     packages = find_packages(),
     install_requires=[""],
     tests_require=[],
 )
```

