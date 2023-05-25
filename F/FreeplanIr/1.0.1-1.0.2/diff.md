# Comparing `tmp/FreeplanIr-1.0.1.tar.gz` & `tmp/FreeplanIr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeplanIr-1.0.1.tar", last modified: Wed May 24 09:01:50 2023, max compression
+gzip compressed data, was "FreeplanIr-1.0.2.tar", last modified: Thu May 25 02:34:12 2023, max compression
```

## Comparing `FreeplanIr-1.0.1.tar` & `FreeplanIr-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:01:50.235269 FreeplanIr-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-24 09:01:50.225269 FreeplanIr-1.0.1/FreeplanIr/
--rw-rw-rw-   0        0        0       28 2023-05-24 08:55:37.000000 FreeplanIr-1.0.1/FreeplanIr/__init__.py
--rw-rw-rw-   0        0        0     1262 2023-05-24 08:15:17.000000 FreeplanIr-1.0.1/FreeplanIr/main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:01:50.232269 FreeplanIr-1.0.1/FreeplanIr.egg-info/
--rw-rw-rw-   0        0        0     1265 2023-05-24 09:01:50.000000 FreeplanIr-1.0.1/FreeplanIr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-05-24 09:01:50.000000 FreeplanIr-1.0.1/FreeplanIr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:01:50.000000 FreeplanIr-1.0.1/FreeplanIr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 09:01:50.000000 FreeplanIr-1.0.1/FreeplanIr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2023-05-24 08:32:25.000000 FreeplanIr-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1265 2023-05-24 09:01:50.234269 FreeplanIr-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-05-24 09:00:22.000000 FreeplanIr-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 09:01:50.235269 FreeplanIr-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-05-24 08:59:50.000000 FreeplanIr-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:34:12.327485 FreeplanIr-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-25 02:34:12.319486 FreeplanIr-1.0.2/FreeplanIr/
+-rw-rw-rw-   0        0        0       47 2023-05-24 09:10:22.000000 FreeplanIr-1.0.2/FreeplanIr/__init__.py
+-rw-rw-rw-   0        0        0     3324 2023-05-25 02:17:24.000000 FreeplanIr-1.0.2/FreeplanIr/main.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:34:12.325485 FreeplanIr-1.0.2/FreeplanIr.egg-info/
+-rw-rw-rw-   0        0        0     1484 2023-05-25 02:34:12.000000 FreeplanIr-1.0.2/FreeplanIr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-25 02:34:12.000000 FreeplanIr-1.0.2/FreeplanIr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 02:34:12.000000 FreeplanIr-1.0.2/FreeplanIr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 02:34:12.000000 FreeplanIr-1.0.2/FreeplanIr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2023-05-24 08:32:25.000000 FreeplanIr-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1484 2023-05-25 02:34:12.326484 FreeplanIr-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-05-25 02:26:52.000000 FreeplanIr-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 02:34:12.327485 FreeplanIr-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-05-25 02:33:40.000000 FreeplanIr-1.0.2/setup.py
```

### Comparing `FreeplanIr-1.0.1/LICENSE.txt` & `FreeplanIr-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeplanIr-1.0.1/README.md` & `FreeplanIr-1.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,19 @@
             [a, d, e],
             [a, f, g],
             [h, i, j],
             [h, k, l]
         ]
 ## 使用方法
     安装相关模块后
-    导入模块和类
+    导入模块和类 form FreeplanIr import FreeplanIr
     file_path = r"XXXX.mm" # 你的文件路径
     test_plan = FreeplanIr(file_path) # 实例化类
-    datas = test_plan.plan_test() # 调用plan_test方法即可
+### 获取转换数据
+    datas = test_plan.plan_test() # 调用plan_test方法即可，返回为转换好数据
+    print(datas)  
+### 下载为xlxs
+    path = test_plan.download() # 调用plan_test方法即可，返回为文件保存地址
     print(datas)  
   此方法返回的结果就是如上所说，需要注意次方返回目前仅支持所有节点的长度一致。
+
```

### Comparing `FreeplanIr-1.0.1/setup.py` & `FreeplanIr-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="FreeplanIr",
-    version="1.0.1",
+    version="1.0.2",
     author="wangdashuai",
     author_email="hanchaodaming@outlook.com",
     description="一个可以解析freeplan *.mm格式文件的工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leslie110",
     packages=setuptools.find_packages(),
```

