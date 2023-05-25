# Comparing `tmp/lesscode_tag-0.0.0.tar.gz` & `tmp/lesscode_tag-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tag-0.0.0.tar", last modified: Thu May 25 02:56:17 2023, max compression
+gzip compressed data, was "dist/lesscode_tag-0.0.1.tar", last modified: Thu May 25 07:46:49 2023, max compression
```

## Comparing `lesscode_tag-0.0.0.tar` & `lesscode_tag-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/
--rw-r--r--   0 baai       (501) staff       (20)      379 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.0/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.0/lesscode_tag/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1807 2023-05-25 02:53:36.000000 lesscode_tag-0.0.0/lesscode_tag/aes.py
--rw-r--r--   0 baai       (501) staff       (20)     4610 2023-05-25 01:48:21.000000 lesscode_tag-0.0.0/lesscode_tag/business.py
--rw-r--r--   0 baai       (501) staff       (20)     9603 2023-05-25 02:53:36.000000 lesscode_tag-0.0.0/lesscode_tag/es_util.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-25 01:31:34.000000 lesscode_tag-0.0.0/lesscode_tag/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      379 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      315 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       20 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag.egg-info/requires.txt
--rw-r--r--   0 baai       (501) staff       (20)       13 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/lesscode_tag.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-25 02:56:17.000000 lesscode_tag-0.0.0/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1257 2023-05-25 01:34:02.000000 lesscode_tag-0.0.0/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.1/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/lesscode_tag/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.1/lesscode_tag/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1807 2023-05-25 02:53:36.000000 lesscode_tag-0.0.1/lesscode_tag/aes.py
+-rw-r--r--   0 baai       (501) staff       (20)     4610 2023-05-25 01:48:21.000000 lesscode_tag-0.0.1/lesscode_tag/business.py
+-rw-r--r--   0 baai       (501) staff       (20)     9603 2023-05-25 02:53:36.000000 lesscode_tag-0.0.1/lesscode_tag/es_util.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-25 07:46:43.000000 lesscode_tag-0.0.1/lesscode_tag/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/lesscode_tag.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/lesscode_tag.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      280 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/lesscode_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/lesscode_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       13 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/lesscode_tag.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-25 07:46:49.000000 lesscode_tag-0.0.1/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1273 2023-05-25 07:46:43.000000 lesscode_tag-0.0.1/setup.py
```

### Comparing `lesscode_tag-0.0.0/lesscode_tag/aes.py` & `lesscode_tag-0.0.1/lesscode_tag/aes.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.0/lesscode_tag/business.py` & `lesscode_tag-0.0.1/lesscode_tag/business.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.0/lesscode_tag/es_util.py` & `lesscode_tag-0.0.1/lesscode_tag/es_util.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.0/setup.py` & `lesscode_tag-0.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     platforms='python',
-    install_requires=["pycryptodomex==3.17"]
+    install_requires=[
+        # "pycryptodomex==3.17"
+    ]
 
 )
 
 """
 1、打包流程
 打包过程中也可以多增加一些额外的操作，减少上传中的错误
```

