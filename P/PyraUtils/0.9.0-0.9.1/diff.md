# Comparing `tmp/PyraUtils-0.9.0.tar.gz` & `tmp/PyraUtils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyraUtils-0.9.0.tar", last modified: Mon Apr 10 08:09:34 2023, max compression
+gzip compressed data, was "PyraUtils-0.9.1.tar", last modified: Fri May 12 07:01:37 2023, max compression
```

## Comparing `PyraUtils-0.9.0.tar` & `PyraUtils-0.9.1.tar`

### file list

```diff
@@ -1,56 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.707033 PyraUtils-0.9.0/
--rw-rw-rw-   0        0        0    11558 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     1661 2023-04-10 08:09:34.707033 PyraUtils-0.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.655030 PyraUtils-0.9.0/PyraUtils/
--rw-rw-rw-   0        0        0      814 2023-04-10 06:59:47.000000 PyraUtils-0.9.0/PyraUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.689030 PyraUtils-0.9.0/PyraUtils/common/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/common/__init__.py
--rw-rw-rw-   0        0        0     5136 2023-04-10 08:06:47.000000 PyraUtils-0.9.0/PyraUtils/common/_file.py
--rw-rw-rw-   0        0        0     1331 2022-07-28 11:34:05.000000 PyraUtils-0.9.0/PyraUtils/common/_ipaddress.py
--rw-rw-rw-   0        0        0     2604 2023-04-10 08:06:59.000000 PyraUtils-0.9.0/PyraUtils/common/_json.py
--rw-rw-rw-   0        0        0     1624 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/common/_shelve.py
--rw-rw-rw-   0        0        0     5737 2023-04-10 07:44:37.000000 PyraUtils-0.9.0/PyraUtils/common/_strings.py
--rw-rw-rw-   0        0        0     2789 2023-04-10 08:01:53.000000 PyraUtils-0.9.0/PyraUtils/common/_time.py
--rw-rw-rw-   0        0        0     3636 2023-04-10 07:43:32.000000 PyraUtils-0.9.0/PyraUtils/common/cert.py
--rw-rw-rw-   0        0        0     3794 2023-04-10 07:43:31.000000 PyraUtils-0.9.0/PyraUtils/common/download.py
--rw-rw-rw-   0        0        0     2042 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/common/password.py
--rw-rw-rw-   0        0        0     3187 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/common/rsync.py
--rw-rw-rw-   0        0        0     2298 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/common/signature.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.690031 PyraUtils-0.9.0/PyraUtils/db/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/db/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-04-10 07:32:29.000000 PyraUtils-0.9.0/PyraUtils/db/_sqlite3.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.693031 PyraUtils-0.9.0/PyraUtils/hash/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/hash/__init__.py
--rw-rw-rw-   0        0        0     4181 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/hash/_hashlib.py
--rw-rw-rw-   0        0        0     1585 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/hash/_hmac.py
--rw-rw-rw-   0        0        0     1651 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/hash/_xxhash.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.695032 PyraUtils-0.9.0/PyraUtils/http/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/http/__init__.py
--rw-rw-rw-   0        0        0     4179 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/http/_httpx.py
--rw-rw-rw-   0        0        0     5231 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/http/_request.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.696032 PyraUtils-0.9.0/PyraUtils/log/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.697032 PyraUtils-0.9.0/PyraUtils/log/filelogger/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/log/filelogger/__init__.py
--rw-rw-rw-   0        0        0     3207 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/log/filelogger/_logging.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.700037 PyraUtils-0.9.0/PyraUtils/log/logger/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/log/logger/__init__.py
--rw-rw-rw-   0        0        0     3777 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/log/logger/_logging.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.701036 PyraUtils-0.9.0/PyraUtils/service/
--rw-rw-rw-   0        0        0      754 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.706036 PyraUtils-0.9.0/PyraUtils/service/work_wechat/
--rw-rw-rw-   0        0        0     3079 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/service/work_wechat/AbstractApi.py
--rw-rw-rw-   0        0        0     3313 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/service/work_wechat/CorpApi.py
--rw-rw-rw-   0        0        0     7057 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/service/work_wechat/CorpApiType.py
--rw-rw-rw-   0        0        0    11253 2023-04-10 07:08:41.000000 PyraUtils-0.9.0/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/PyraUtils/service/work_wechat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:09:34.678029 PyraUtils-0.9.0/PyraUtils.egg-info/
--rw-rw-rw-   0        0        0     1661 2023-04-10 08:09:34.000000 PyraUtils-0.9.0/PyraUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-04-10 08:09:34.000000 PyraUtils-0.9.0/PyraUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:09:34.000000 PyraUtils-0.9.0/PyraUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 08:09:34.000000 PyraUtils-0.9.0/PyraUtils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      281 2023-04-10 08:09:34.000000 PyraUtils-0.9.0/PyraUtils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 08:09:34.000000 PyraUtils-0.9.0/PyraUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      419 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/README.rst
--rw-rw-rw-   0        0        0     1812 2023-04-10 08:09:34.715036 PyraUtils-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1663 2022-04-21 03:55:13.000000 PyraUtils-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.568222 PyraUtils-0.9.1/
+-rw-rw-rw-   0        0        0      161 2023-05-11 08:15:40.000000 PyraUtils-0.9.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3666 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/HISTORY.rst
+-rw-rw-rw-   0        0        0    11558 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1689 2023-05-12 07:01:37.568222 PyraUtils-0.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.525774 PyraUtils-0.9.1/PyraUtils/
+-rw-rw-rw-   0        0        0      884 2023-05-11 09:55:49.000000 PyraUtils-0.9.1/PyraUtils/__init__.py
+-rw-rw-rw-   0        0        0      427 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/PyraUtils/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.548222 PyraUtils-0.9.1/PyraUtils/common/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/common/__init__.py
+-rw-rw-rw-   0        0        0     5136 2023-04-10 08:06:47.000000 PyraUtils-0.9.1/PyraUtils/common/_file.py
+-rw-rw-rw-   0        0        0     1372 2023-05-11 08:50:17.000000 PyraUtils-0.9.1/PyraUtils/common/_ipaddress.py
+-rw-rw-rw-   0        0        0     2604 2023-04-10 08:06:59.000000 PyraUtils-0.9.1/PyraUtils/common/_json.py
+-rw-rw-rw-   0        0        0     1624 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/common/_shelve.py
+-rw-rw-rw-   0        0        0     5724 2023-05-11 08:57:30.000000 PyraUtils-0.9.1/PyraUtils/common/_strings.py
+-rw-rw-rw-   0        0        0     2789 2023-04-10 08:01:53.000000 PyraUtils-0.9.1/PyraUtils/common/_time.py
+-rw-rw-rw-   0        0        0     3636 2023-04-10 07:43:32.000000 PyraUtils-0.9.1/PyraUtils/common/cert.py
+-rw-rw-rw-   0        0        0     4445 2023-05-11 09:18:20.000000 PyraUtils-0.9.1/PyraUtils/common/download.py
+-rw-rw-rw-   0        0        0     2031 2023-05-11 09:37:39.000000 PyraUtils-0.9.1/PyraUtils/common/password.py
+-rw-rw-rw-   0        0        0     3187 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/common/rsync.py
+-rw-rw-rw-   0        0        0     2298 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/common/signature.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.549224 PyraUtils-0.9.1/PyraUtils/db/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/db/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-04-10 07:32:29.000000 PyraUtils-0.9.1/PyraUtils/db/_sqlite3.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.551224 PyraUtils-0.9.1/PyraUtils/hash/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/hash/__init__.py
+-rw-rw-rw-   0        0        0     4181 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/hash/_hashlib.py
+-rw-rw-rw-   0        0        0     1585 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/hash/_hmac.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.553222 PyraUtils-0.9.1/PyraUtils/http/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/http/__init__.py
+-rw-rw-rw-   0        0        0     4254 2023-05-11 09:35:29.000000 PyraUtils-0.9.1/PyraUtils/http/_httpx.py
+-rw-rw-rw-   0        0        0     5295 2023-05-11 09:35:04.000000 PyraUtils-0.9.1/PyraUtils/http/_request.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.553222 PyraUtils-0.9.1/PyraUtils/log/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.555222 PyraUtils-0.9.1/PyraUtils/log/filelogger/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/log/filelogger/__init__.py
+-rw-rw-rw-   0        0        0     3207 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/log/filelogger/_logging.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.556225 PyraUtils-0.9.1/PyraUtils/log/logger/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/log/logger/__init__.py
+-rw-rw-rw-   0        0        0     3777 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/log/logger/_logging.py
+-rw-rw-rw-   0        0        0     1701 2023-05-11 09:53:45.000000 PyraUtils-0.9.1/PyraUtils/log/logger/_loguru.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.557225 PyraUtils-0.9.1/PyraUtils/service/
+-rw-rw-rw-   0        0        0      754 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.560222 PyraUtils-0.9.1/PyraUtils/service/work_wechat/
+-rw-rw-rw-   0        0        0     3079 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/service/work_wechat/AbstractApi.py
+-rw-rw-rw-   0        0        0     3313 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/service/work_wechat/CorpApi.py
+-rw-rw-rw-   0        0        0     7057 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/service/work_wechat/CorpApiType.py
+-rw-rw-rw-   0        0        0    11253 2023-04-10 07:08:41.000000 PyraUtils-0.9.1/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/PyraUtils/service/work_wechat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.537223 PyraUtils-0.9.1/PyraUtils.egg-info/
+-rw-rw-rw-   0        0        0     1689 2023-05-12 07:01:37.000000 PyraUtils-0.9.1/PyraUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1536 2023-05-12 07:01:37.000000 PyraUtils-0.9.1/PyraUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:01:37.000000 PyraUtils-0.9.1/PyraUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 07:00:26.000000 PyraUtils-0.9.1/PyraUtils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      296 2023-05-12 07:01:37.000000 PyraUtils-0.9.1/PyraUtils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-12 07:01:37.000000 PyraUtils-0.9.1/PyraUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      419 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.566222 PyraUtils-0.9.1/docs/
+-rw-rw-rw-   0        0        0      632 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4961 2023-05-11 08:11:29.000000 PyraUtils-0.9.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/history.rst
+-rw-rw-rw-   0        0        0      328 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1173 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       84 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/docs/usage.rst
+-rw-rw-rw-   0        0        0      209 2023-05-12 07:01:34.000000 PyraUtils-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1839 2023-05-12 07:01:37.570222 PyraUtils-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2022-04-21 03:55:13.000000 PyraUtils-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:01:37.567225 PyraUtils-0.9.1/tests/
+-rw-rw-rw-   0        0        0       42 2023-04-13 07:49:46.000000 PyraUtils-0.9.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      238 2023-05-12 02:55:42.000000 PyraUtils-0.9.1/tests/test_download.py
```

### Comparing `PyraUtils-0.9.0/LICENSE` & `PyraUtils-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PKG-INFO` & `PyraUtils-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyraUtils
-Version: 0.9.0
+Version: 0.9.1
 Summary: Common development utils.
 Home-page: https://www.920430.com/
 Author: pyra
 Author-email: ops@920430.com
 License: APACHE LICENSE, VERSION 2.0
 Project-URL: Documentation, https://www.920430.com/
 Project-URL: Release notes, https://www.920430.com/
@@ -21,16 +21,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 License-File: LICENSE
+License-File: AUTHORS.rst
 
 PyraUtils
 ====================
 
 This project will collect General-purpose utilities used in development.
 
 What is the main function??
```

### Comparing `PyraUtils-0.9.0/PyraUtils/__init__.py` & `PyraUtils-0.9.1/PyraUtils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+ * Top-level package for PyraUtils.
+ *
  *                    .::::.
  *                  .::::::::.
  *                 :::::::::::
  *             ..:::::::::::'
  *           '::::::::::::'
  *             .::::::::::
  *        '::::::::::::::..
@@ -15,9 +17,11 @@
  *       .::'        :::::.:::::::::'      ':::::.
  *      .::'         ::::::::::::::'         ``::::.
  *  ...:::           ::::::::::::'              ``::.
  * ```` ':.          ':::::::::'                  ::::..
  *                    '.:::::'                    ':'````..
 """
 
-VERSION = (0, 9, 0, 'alpha', 0)
-__version__ = '0.9.0'
+
+__author__ = """PyraUtils"""
+__email__ = 'ops@920430.com'
+__version__ = '0.9.1'
```

### Comparing `PyraUtils-0.9.0/PyraUtils/common/__init__.py` & `PyraUtils-0.9.1/PyraUtils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/_file.py` & `PyraUtils-0.9.1/PyraUtils/common/_file.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/_ipaddress.py` & `PyraUtils-0.9.1/PyraUtils/common/_ipaddress.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 """
 created by：2022-07-28 16:17:47
 modify by: 2022-07-28 19:34:04
 
 功能：ipaddress函数的封装。
 """
 import ipaddress
+from loguru import logger
 
 
 class IpaddressUtils:
     """IpaddressUtils"""
     def __init__(self) -> None:
         pass
 
     def _ip_network(self, network):
         '''
         验证network是否合法；如果输入值异常，一律按照127.0.0.1处理。
         '''
         try:
             return ipaddress.ip_network(network)
         except ValueError as e:
-            print(e)
+            logger.error(e)
             return ipaddress.ip_network("127.0.0.1")
 
     def _ip_address(self, address):
         '''
         验证address是否合法；如果输入值异常，一律按照127.0.0.1处理。
         '''
         try:
             return ipaddress.ip_address(address)
         except ValueError as e:
-            print(e)
+            logger.error(e)
             return ipaddress.ip_address("127.0.0.1")
 
     def check_ipaddress(self, address:str, network_list:list="") -> bool:
         '''
         验证address是否在network_list内
         '''
         address = self._ip_address(address)
```

### Comparing `PyraUtils-0.9.0/PyraUtils/common/_json.py` & `PyraUtils-0.9.1/PyraUtils/common/_json.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/_shelve.py` & `PyraUtils-0.9.1/PyraUtils/common/_shelve.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/_strings.py` & `PyraUtils-0.9.1/PyraUtils/common/_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,20 @@
         trailing whitespace, dashes, and underscores.
 
         https://github.com/django/django/blob/main/django/utils/text.py
 
         In [20]: slugify("陈 ll%.jpg")  --> In [20]: slugify("陈 ll%.jpg")
         In [22]: slugify("aaa ll%.jpg", allow_unicode=True)  --> Out[23]: '陈aaa-lljpg'
         """
-        value = str(value)
         if allow_unicode:
-            value = unicodedata.normalize('NFKC', value)
+            value_1 = unicodedata.normalize('NFKC', str(value))
         else:
-            value = unicodedata.normalize('NFKD', value).encode('ascii', 'ignore').decode('ascii')
-        value = re.sub(r'[^\w\s-]', '', value.lower())
-        return re.sub(r'[-\s]+', '-', value).strip('-_')
+            value_1 = unicodedata.normalize('NFKD', value).encode('ascii', 'ignore').decode('ascii')
+        value_2 = re.sub(r'[^\w\s-]', '', value_1.lower())
+        return re.sub(r'[-\s]+', '-', value_2).strip('-_')
 
     @staticmethod
     def natural_sort(value:list) -> list: 
         """自然排序
         
         https://blog.codinghorror.com/sorting-for-humans-natural-sort-order/
         """
```

### Comparing `PyraUtils-0.9.0/PyraUtils/common/_time.py` & `PyraUtils-0.9.1/PyraUtils/common/_time.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/cert.py` & `PyraUtils-0.9.1/PyraUtils/common/cert.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/password.py` & `PyraUtils-0.9.1/PyraUtils/common/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-import os
 import secrets
 import string
 
 
 class PasswordMake:
     @staticmethod
     def make_random_password(length:int=10,
```

### Comparing `PyraUtils-0.9.0/PyraUtils/common/rsync.py` & `PyraUtils-0.9.1/PyraUtils/common/rsync.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/common/signature.py` & `PyraUtils-0.9.1/PyraUtils/common/signature.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/db/__init__.py` & `PyraUtils-0.9.1/PyraUtils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/db/_sqlite3.py` & `PyraUtils-0.9.1/PyraUtils/db/_sqlite3.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/hash/__init__.py` & `PyraUtils-0.9.1/PyraUtils/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/hash/_hashlib.py` & `PyraUtils-0.9.1/PyraUtils/hash/_hashlib.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/hash/_hmac.py` & `PyraUtils-0.9.1/PyraUtils/hash/_hmac.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/http/__init__.py` & `PyraUtils-0.9.1/PyraUtils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/http/_httpx.py` & `PyraUtils-0.9.1/PyraUtils/http/_httpx.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 参考文档:
     https://github.com/encode/httpx
     https://www.python-httpx.org/
 """
 
 import httpx
 
-
 class httpxBasiceUtil:
     """httpx二次封装，常用的get,post,head,delete方法封装，工具类。"""
 
     @staticmethod
-    def httpx_method(method, url, **kwargs):
+    def httpx_method(method:str, url:str, **kwargs) -> httpx.Response:
         """Sends a request.
 
         参数:
 
             method: - ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
             url – 新建 Request 对象的URL
             params – (可选) Request 对象的查询字符中要发送的字典或字节内容
@@ -44,26 +43,26 @@
             Response object
 
         返回类型:
             httpx.Response
         """
 
         try:
-            req = httpx.Request(method, url, **kwargs)
+            resp = httpx.Request(method, url, **kwargs)
         except (httpx.ConnectError, httpx.HTTPError, httpx.ProtocolError,
                 httpx.InvalidURL, httpx.TimeoutException, httpx.NetworkError,
                 httpx.ProxyError) as err:
-            print("Error", err)
-        return req
+            raise RuntimeError(err)
+        return resp
 
 
 class httpxClientUtil:
     """httpx连接池二次封装，异步支持;常用的get,post,head,delete方法封装，工具类。"""
 
-    def __init__(self, http2=False, proxies=None,  timeout=5.0,
+    def __init__(self, http2:bool=False, proxies=None,  timeout=5.0,
                 max_keepalive=20, max_connections=100, keepalive_expiry:float=5.0) -> None:
         """
         http2: 启用 HTTP/2 支持的客户端
         proxies： 代理地址
         max_keepalive，允许保持活动连接的数量，或None始终允许。（默认 20）
         max_connections、最大允许连接数或None无限制。（默认 100）
         keepalive_expiry: 浮点， 默认为5.0
@@ -72,20 +71,20 @@
         self.http2 = http2
         self.proxies = proxies
         self.timeout = timeout
         self.limits = httpx.Limits(max_keepalive_connections=max_keepalive,
                                    max_connections=max_connections,
                                    keepalive_expiry=keepalive_expiry)
 
-    def httpx_method(self, method, url, **kwargs):
+    def httpx_method(self, method, url, **kwargs) -> httpx.Response:
         with httpx.Client(http2=self.http2, proxies=self.proxies,
                           timeout=self.timeout, limits=self.limits) as client:
-            req = client.request(method, url, **kwargs)
-        return req
+            resp = client.request(method, url, **kwargs)
+        return resp
 
 
-    async def async_method(self, method, url, **kwargs):
+    async def async_method(self, method, url, **kwargs) -> httpx.Response:
         async with httpx.AsyncClient(http2=self.http2, proxies=self.proxies,
                                      timeout=self.timeout, limits=self.limits) as client:
-            req = await client.request(method, url, **kwargs)
-        return req
+            resp = await client.request(method, url, **kwargs)
+        return resp
```

### Comparing `PyraUtils-0.9.0/PyraUtils/http/_request.py` & `PyraUtils-0.9.1/PyraUtils/http/_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import requests
 
 
 class RequestsBasiceUtil:
     """requests二次封装，常用的get,post,head,delete方法封装，工具类。"""
 
     @staticmethod
-    def req_method(method, url, **kwargs):
+    def req_method(method:str, url:str, **kwargs) -> requests.Response:
         """Sends request.
 
         参数:
 
             method: - ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
             url – 新建 Request 对象的URL
             params – (可选) Request 对象的查询字符中要发送的字典或字节内容
@@ -45,33 +45,33 @@
         返回:
             Response object
 
         返回类型:
             requests.Response
         """
         try:
-            req = requests.request(method, url, **kwargs)
+            resp = requests.request(method, url, **kwargs)
         except (requests.ConnectionError, requests.HTTPError,
                 requests.Timeout, requests.URLRequired) as err:
-            print("error", err)
-        return req
+            raise RuntimeError(err)
+        return resp
 
 
 class RequestsSessionUtil:
     """Request ssession方法封装，额外提供 cookie 的存储，连接池和配置"""
 
     def __init__(self, max_retries:int=5, proxies:any={}):
         """
         max_retries: 最大重试次数
         proxies： 代理池
         """
         self.max_retries = max_retries
         self.proxies = proxies
 
-    def session_method(self, method, url, **kwargs):
+    def session_method(self, method:str, url:str, **kwargs) -> requests.Response:
         """Sends request.
 
         参数:
 
             url – 新建 Request 对象的URL.
             method: - ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
             params – (可选) Request 对象的查询字符中要发送的字典或字节内容。
```

### Comparing `PyraUtils-0.9.0/PyraUtils/log/__init__.py` & `PyraUtils-0.9.1/PyraUtils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/log/filelogger/__init__.py` & `PyraUtils-0.9.1/PyraUtils/log/filelogger/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/log/filelogger/_logging.py` & `PyraUtils-0.9.1/PyraUtils/log/filelogger/_logging.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/log/logger/__init__.py` & `PyraUtils-0.9.1/PyraUtils/log/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/log/logger/_logging.py` & `PyraUtils-0.9.1/PyraUtils/log/logger/_logging.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/service/__init__.py` & `PyraUtils-0.9.1/PyraUtils/service/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/service/work_wechat/AbstractApi.py` & `PyraUtils-0.9.1/PyraUtils/service/work_wechat/AbstractApi.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/service/work_wechat/CorpApi.py` & `PyraUtils-0.9.1/PyraUtils/service/work_wechat/CorpApi.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/service/work_wechat/CorpApiType.py` & `PyraUtils-0.9.1/PyraUtils/service/work_wechat/CorpApiType.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py` & `PyraUtils-0.9.1/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils/service/work_wechat/__init__.py` & `PyraUtils-0.9.1/PyraUtils/service/work_wechat/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.0/PyraUtils.egg-info/PKG-INFO` & `PyraUtils-0.9.1/PyraUtils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyraUtils
-Version: 0.9.0
+Version: 0.9.1
 Summary: Common development utils.
 Home-page: https://www.920430.com/
 Author: pyra
 Author-email: ops@920430.com
 License: APACHE LICENSE, VERSION 2.0
 Project-URL: Documentation, https://www.920430.com/
 Project-URL: Release notes, https://www.920430.com/
@@ -21,16 +21,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 License-File: LICENSE
+License-File: AUTHORS.rst
 
 PyraUtils
 ====================
 
 This project will collect General-purpose utilities used in development.
 
 What is the main function??
```

### Comparing `PyraUtils-0.9.0/setup.cfg` & `PyraUtils-0.9.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -63,52 +63,53 @@
 000003e0: 6365 203d 2068 7474 7073 3a2f 2f62 6974  ce = https://bit
 000003f0: 6275 636b 6574 2e6f 7267 2f70 7972 6175  bucket.org/pyrau
 00000400: 7469 6c73 2e67 6974 0d0a 0954 7261 636b  tils.git...Track
 00000410: 6572 203d 2068 7474 7073 3a2f 2f77 7777  er = https://www
 00000420: 2e39 3230 3433 302e 636f 6d2f 0d0a 0d0a  .920430.com/....
 00000430: 5b6f 7074 696f 6e73 5d0d 0a70 7974 686f  [options]..pytho
 00000440: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000450: 2e39 0d0a 7061 636b 6167 6573 203d 2066  .9..packages = f
-00000460: 696e 643a 0d0a 696e 636c 7564 655f 7061  ind:..include_pa
-00000470: 636b 6167 655f 6461 7461 203d 2074 7275  ckage_data = tru
-00000480: 650d 0a7a 6970 5f73 6166 6520 3d20 6661  e..zip_safe = fa
-00000490: 6c73 650d 0a69 6e73 7461 6c6c 5f72 6571  lse..install_req
-000004a0: 7569 7265 7320 3d20 0d0a 0968 7474 7078  uires = ...httpx
-000004b0: 3d3d 302e 3231 2e31 0d0a 0970 7970 696e  ==0.21.1...pypin
-000004c0: 7969 6e3d 3d30 2e34 342e 303b 2070 7974  yin==0.44.0; pyt
-000004d0: 686f 6e5f 7665 7273 696f 6e20 3e3d 2027  hon_version >= '
-000004e0: 322e 3627 2061 6e64 2070 7974 686f 6e5f  2.6' and python_
-000004f0: 7665 7273 696f 6e20 6e6f 7420 696e 2027  version not in '
-00000500: 332e 302c 2033 2e31 2c20 332e 322c 2033  3.0, 3.1, 3.2, 3
-00000510: 2e33 2720 616e 6420 7079 7468 6f6e 5f76  .3' and python_v
-00000520: 6572 7369 6f6e 203c 2027 3427 0d0a 0970  ersion < '4'...p
-00000530: 7974 7a3d 3d32 3032 312e 330d 0a09 7265  ytz==2021.3...re
-00000540: 7175 6573 7473 3d3d 322e 3236 2e30 3b20  quests==2.26.0; 
-00000550: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-00000560: 3d20 2732 2e37 2720 616e 6420 7079 7468  = '2.7' and pyth
-00000570: 6f6e 5f76 6572 7369 6f6e 206e 6f74 2069  on_version not i
-00000580: 6e20 2733 2e30 2c20 332e 312c 2033 2e32  n '3.0, 3.1, 3.2
-00000590: 2c20 332e 332c 2033 2e34 2c20 332e 3527  , 3.3, 3.4, 3.5'
-000005a0: 0d0a 0970 7963 7279 7074 6f64 6f6d 653d  ...pycryptodome=
-000005b0: 3d33 2e31 322e 300d 0a09 7878 6861 7368  =3.12.0...xxhash
-000005c0: 3d3d 322e 302e 320d 0a0d 0a5b 666c 616b  ==2.0.2....[flak
-000005d0: 6538 5d0d 0a65 7863 6c75 6465 203d 2062  e8]..exclude = b
-000005e0: 7569 6c64 2c2e 6769 742c 2e74 6f78 2c2e  uild,.git,.tox,.
-000005f0: 2f74 6573 7473 2f2e 656e 762c 5069 7066  /tests/.env,Pipf
-00000600: 696c 652c 5069 7066 696c 652e 6c6f 636b  ile,Pipfile.lock
-00000610: 0d0a 6967 6e6f 7265 203d 2057 3530 342c  ..ignore = W504,
-00000620: 5736 3031 0d0a 6d61 782d 6c69 6e65 2d6c  W601..max-line-l
-00000630: 656e 6774 6820 3d20 3131 390d 0a0d 0a5b  ength = 119....[
-00000640: 6973 6f72 745d 0d0a 636f 6d62 696e 655f  isort]..combine_
-00000650: 6173 5f69 6d70 6f72 7473 203d 2074 7275  as_imports = tru
-00000660: 650d 0a64 6566 6175 6c74 5f73 6563 7469  e..default_secti
-00000670: 6f6e 203d 2054 4849 5244 5041 5254 590d  on = THIRDPARTY.
-00000680: 0a69 6e63 6c75 6465 5f74 7261 696c 696e  .include_trailin
-00000690: 675f 636f 6d6d 6120 3d20 7472 7565 0d0a  g_comma = true..
-000006a0: 6b6e 6f77 6e5f 6669 7273 745f 7061 7274  known_first_part
-000006b0: 7920 3d20 5079 7261 5574 696c 730d 0a6c  y = PyraUtils..l
-000006c0: 696e 655f 6c65 6e67 7468 203d 2037 390d  ine_length = 79.
-000006d0: 0a6d 756c 7469 5f6c 696e 655f 6f75 7470  .multi_line_outp
-000006e0: 7574 203d 2035 0d0a 0d0a 5b65 6767 5f69  ut = 5....[egg_i
-000006f0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000700: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000710: 0d0a 0d0a                                ....
+00000450: 2e31 300d 0a70 6163 6b61 6765 7320 3d20  .10..packages = 
+00000460: 6669 6e64 3a0d 0a69 6e63 6c75 6465 5f70  find:..include_p
+00000470: 6163 6b61 6765 5f64 6174 6120 3d20 7472  ackage_data = tr
+00000480: 7565 0d0a 7a69 705f 7361 6665 203d 2066  ue..zip_safe = f
+00000490: 616c 7365 0d0a 696e 7374 616c 6c5f 7265  alse..install_re
+000004a0: 7175 6972 6573 203d 200d 0a09 6874 7470  quires = ...http
+000004b0: 783d 3d30 2e32 342e 300d 0a09 7079 7069  x==0.24.0...pypi
+000004c0: 6e79 696e 3d3d 302e 3434 2e30 3b20 7079  nyin==0.44.0; py
+000004d0: 7468 6f6e 5f76 6572 7369 6f6e 203e 3d20  thon_version >= 
+000004e0: 2732 2e36 2720 616e 6420 7079 7468 6f6e  '2.6' and python
+000004f0: 5f76 6572 7369 6f6e 206e 6f74 2069 6e20  _version not in 
+00000500: 2733 2e30 2c20 332e 312c 2033 2e32 2c20  '3.0, 3.1, 3.2, 
+00000510: 332e 3327 2061 6e64 2070 7974 686f 6e5f  3.3' and python_
+00000520: 7665 7273 696f 6e20 3c20 2734 270d 0a09  version < '4'...
+00000530: 7079 747a 3d3d 3230 3233 2e33 0d0a 0972  pytz==2023.3...r
+00000540: 6571 7565 7374 733d 3d32 2e33 302e 303b  equests==2.30.0;
+00000550: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
+00000560: 3e3d 2027 322e 3727 2061 6e64 2070 7974  >= '2.7' and pyt
+00000570: 686f 6e5f 7665 7273 696f 6e20 6e6f 7420  hon_version not 
+00000580: 696e 2027 332e 302c 2033 2e31 2c20 332e  in '3.0, 3.1, 3.
+00000590: 322c 2033 2e33 2c20 332e 342c 2033 2e35  2, 3.3, 3.4, 3.5
+000005a0: 270d 0a09 7079 6372 7970 746f 646f 6d65  '...pycryptodome
+000005b0: 3d3d 332e 3132 2e30 0d0a 0975 726c 6c69  ==3.12.0...urlli
+000005c0: 6233 3d3d 322e 302e 320d 0a09 6c6f 6775  b3==2.0.2...logu
+000005d0: 7275 3d3d 302e 372e 300d 0a0d 0a5b 666c  ru==0.7.0....[fl
+000005e0: 616b 6538 5d0d 0a65 7863 6c75 6465 203d  ake8]..exclude =
+000005f0: 2062 7569 6c64 2c2e 6769 742c 2e74 6f78   build,.git,.tox
+00000600: 2c2e 2f74 6573 7473 2f2e 656e 762c 5069  ,./tests/.env,Pi
+00000610: 7066 696c 652c 5069 7066 696c 652e 6c6f  pfile,Pipfile.lo
+00000620: 636b 2c2e 656e 762c 746d 700d 0a69 676e  ck,.env,tmp..ign
+00000630: 6f72 6520 3d20 5735 3034 2c57 3630 310d  ore = W504,W601.
+00000640: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+00000650: 203d 2031 3139 0d0a 0d0a 5b69 736f 7274   = 119....[isort
+00000660: 5d0d 0a63 6f6d 6269 6e65 5f61 735f 696d  ]..combine_as_im
+00000670: 706f 7274 7320 3d20 7472 7565 0d0a 6465  ports = true..de
+00000680: 6661 756c 745f 7365 6374 696f 6e20 3d20  fault_section = 
+00000690: 5448 4952 4450 4152 5459 0d0a 696e 636c  THIRDPARTY..incl
+000006a0: 7564 655f 7472 6169 6c69 6e67 5f63 6f6d  ude_trailing_com
+000006b0: 6d61 203d 2074 7275 650d 0a6b 6e6f 776e  ma = true..known
+000006c0: 5f66 6972 7374 5f70 6172 7479 203d 2050  _first_party = P
+000006d0: 7972 6155 7469 6c73 0d0a 6c69 6e65 5f6c  yraUtils..line_l
+000006e0: 656e 6774 6820 3d20 3739 0d0a 6d75 6c74  ength = 79..mult
+000006f0: 695f 6c69 6e65 5f6f 7574 7075 7420 3d20  i_line_output = 
+00000700: 350d 0a0d 0a5b 6567 675f 696e 666f 5d0d  5....[egg_info].
+00000710: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000720: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `PyraUtils-0.9.0/setup.py` & `PyraUtils-0.9.1/setup.py`

 * *Files identical despite different names*

