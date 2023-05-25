# Comparing `tmp/thztools-0.1.tar.gz` & `tmp/thztools-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thztools-0.1.tar", last modified: Thu May 25 12:11:03 2023, max compression
+gzip compressed data, was "thztools-1.0.tar", last modified: Thu May 25 12:47:26 2023, max compression
```

## Comparing `thztools-0.1.tar` & `thztools-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:11:03.934108 thztools-0.1/
--rw-rw-rw-   0        0        0       63 2023-05-25 12:10:26.000000 thztools-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      313 2023-05-25 12:11:03.931108 thztools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1823 2023-05-25 12:08:36.000000 thztools-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 12:11:03.935108 thztools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-05-25 10:43:57.000000 thztools-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:11:03.862104 thztools-0.1/thztools/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-0.1/thztools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:11:03.928108 thztools-0.1/thztools/jiami/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-0.1/thztools/jiami/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-05-25 10:02:38.000000 thztools-0.1/thztools/jiami/aes.py
--rw-rw-rw-   0        0        0     1170 2023-05-25 09:55:51.000000 thztools-0.1/thztools/jiami/kaisa.py
--rw-rw-rw-   0        0        0     1404 2023-05-25 11:52:52.000000 thztools-0.1/thztools/jiami/rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:11:03.912107 thztools-0.1/thztools.egg-info/
--rw-rw-rw-   0        0        0      313 2023-05-25 12:11:03.000000 thztools-0.1/thztools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-25 12:11:03.000000 thztools-0.1/thztools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:11:03.000000 thztools-0.1/thztools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-25 12:11:03.000000 thztools-0.1/thztools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 12:11:03.000000 thztools-0.1/thztools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 12:47:26.065919 thztools-1.0/
+-rw-rw-rw-   0        0        0       63 2023-05-25 12:10:26.000000 thztools-1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2243 2023-05-25 12:47:26.064919 thztools-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1823 2023-05-25 12:08:36.000000 thztools-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:47:26.066919 thztools-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-05-25 12:47:20.000000 thztools-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:47:26.018916 thztools-1.0/thztools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0/thztools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:47:26.058918 thztools-1.0/thztools/jiami/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0/thztools/jiami/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-05-25 10:02:38.000000 thztools-1.0/thztools/jiami/aes.py
+-rw-rw-rw-   0        0        0     1170 2023-05-25 09:55:51.000000 thztools-1.0/thztools/jiami/kaisa.py
+-rw-rw-rw-   0        0        0     1404 2023-05-25 11:52:52.000000 thztools-1.0/thztools/jiami/rsa.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:47:26.040917 thztools-1.0/thztools.egg-info/
+-rw-rw-rw-   0        0        0     2243 2023-05-25 12:47:25.000000 thztools-1.0/thztools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-25 12:47:25.000000 thztools-1.0/thztools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:47:25.000000 thztools-1.0/thztools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 12:47:25.000000 thztools-1.0/thztools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 12:47:25.000000 thztools-1.0/thztools.egg-info/top_level.txt
```

### Comparing `thztools-0.1/README.md` & `thztools-1.0/README.md`

 * *Files identical despite different names*

### Comparing `thztools-0.1/setup.py` & `thztools-1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from setuptools import setup
+with open("./README.md",mode='r',encoding='utf-8') as f:
+    des = f.read()
 setup(
     name="thztools",      # 包名，用于安装和调用该包
-    version="0.1",               # 版本号
+    version="1.0",               # 版本号
     author="Sen",
+    description="由天狐宗开发的工具，方便开发时使用",
+    long_description=des,
+    long_description_content_type='text/markdown',
     author_email="tianhuzong@qq.com",
     url="https://github.com/tianhuzong/thztools",
     license="MIT",
     packages=["thztools"],     # 需要打包的包，可以是单个或多个包
     package_data={"thztools": ["*.py","jiami/*.py"]},  # 包需要包含的数据文件（可选）
     install_requires=[           # 安装依赖，可以是单个或多个依赖项
         "rsa",
```

### Comparing `thztools-0.1/thztools/jiami/aes.py` & `thztools-1.0/thztools/jiami/aes.py`

 * *Files identical despite different names*

### Comparing `thztools-0.1/thztools/jiami/kaisa.py` & `thztools-1.0/thztools/jiami/kaisa.py`

 * *Files identical despite different names*

### Comparing `thztools-0.1/thztools/jiami/rsa.py` & `thztools-1.0/thztools/jiami/rsa.py`

 * *Files identical despite different names*

