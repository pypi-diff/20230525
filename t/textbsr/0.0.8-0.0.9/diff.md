# Comparing `tmp/textbsr-0.0.8.tar.gz` & `tmp/textbsr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.0.8.tar", last modified: Thu May 25 13:38:27 2023, max compression
+gzip compressed data, was "textbsr-0.0.9.tar", last modified: Thu May 25 13:54:59 2023, max compression
```

## Comparing `textbsr-0.0.8.tar` & `textbsr-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:38:27.000000 textbsr-0.0.8/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-25 13:38:27.000000 textbsr-0.0.8/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-25 13:38:27.000000 textbsr-0.0.8/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1276 2023-05-25 13:37:51.000000 textbsr-0.0.8/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:16:08.000000 textbsr-0.0.8/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.8/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.8/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.8/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6128 2023-05-25 13:35:18.000000 textbsr-0.0.8/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.8/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.8/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      383 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       40 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/entry_points.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-25 13:38:27.000000 textbsr-0.0.8/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:54:59.000000 textbsr-0.0.9/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-25 13:54:59.000000 textbsr-0.0.9/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-25 13:54:59.000000 textbsr-0.0.9/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1276 2023-05-25 13:54:47.000000 textbsr-0.0.9/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       21 2023-05-25 13:53:54.000000 textbsr-0.0.9/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.9/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.9/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.9/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6128 2023-05-25 13:35:18.000000 textbsr-0.0.9/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.9/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.9/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      383 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       40 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/entry_points.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-25 13:54:59.000000 textbsr-0.0.9/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.0.8/setup.py` & `textbsr-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     here = os.path.dirname(os.path.realpath(__file__))
     with open(os.path.join(here, filename), 'r') as f:
         requires = [line.replace('\n', '') for line in f.readlines()]
     return requires
 
 
 setup(name='textbsr',
-      version='0.0.8',
+      version='0.0.9',
       description='a simple version for blind text image super-resolution (current version is only for English and Chinese)',
       author='Xiaoming Li',
       author_email='csxmli@gmail.com',
       #requires= ['numpy','torch','cv2','time','argparse','torchvision'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

### Comparing `textbsr-0.0.8/textbsr/models/TextEnhancement.py` & `textbsr-0.0.9/textbsr/models/TextEnhancement.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.0.8/textbsr/textbsr.py` & `textbsr-0.0.9/textbsr/textbsr.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.0.8/textbsr/utils/utils_image.py` & `textbsr-0.0.9/textbsr/utils/utils_image.py`

 * *Files identical despite different names*

