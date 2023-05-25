# Comparing `tmp/mlopspython-inference-93446164921611003430826400.tar.gz` & `tmp/mlopspython-inference-9685412409802298096004.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlopspython-inference-93446164921611003430826400.tar", last modified: Mon Apr  3 14:20:15 2023, max compression
+gzip compressed data, was "mlopspython-inference-9685412409802298096004.tar", last modified: Fri Mar 17 16:53:36 2023, max compression
```

## Comparing `mlopspython-inference-93446164921611003430826400.tar` & `mlopspython-inference-9685412409802298096004.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:20:15.045027 mlopspython-inference-93446164921611003430826400/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-03 14:20:15.045027 mlopspython-inference-93446164921611003430826400/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:20:15.045027 mlopspython-inference-93446164921611003430826400/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-03 14:17:22.000000 mlopspython-inference-93446164921611003430826400/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:20:15.041027 mlopspython-inference-93446164921611003430826400/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:20:15.041027 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 14:17:22.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-03 14:17:22.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference/model_pillow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:20:15.045027 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-03 14:20:15.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-03 14:20:15.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:20:15.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-03 14:20:15.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 14:20:15.000000 mlopspython-inference-93446164921611003430826400/src/mlopspython_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:53:36.364317 mlopspython-inference-9685412409802298096004/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-17 16:53:36.364317 mlopspython-inference-9685412409802298096004/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 16:53:36.364317 mlopspython-inference-9685412409802298096004/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-17 16:51:49.000000 mlopspython-inference-9685412409802298096004/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:53:36.360317 mlopspython-inference-9685412409802298096004/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:53:36.360317 mlopspython-inference-9685412409802298096004/src/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 16:51:49.000000 mlopspython-inference-9685412409802298096004/src/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:53:36.364317 mlopspython-inference-9685412409802298096004/src/mlopspython_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-17 16:53:36.000000 mlopspython-inference-9685412409802298096004/src/mlopspython_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-17 16:53:36.000000 mlopspython-inference-9685412409802298096004/src/mlopspython_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 16:53:36.000000 mlopspython-inference-9685412409802298096004/src/mlopspython_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-17 16:53:36.000000 mlopspython-inference-9685412409802298096004/src/mlopspython_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-17 16:53:36.000000 mlopspython-inference-9685412409802298096004/src/mlopspython_inference.egg-info/top_level.txt
```

### Comparing `mlopspython-inference-93446164921611003430826400/setup.py` & `mlopspython-inference-9685412409802298096004/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="mlopspython-inference",
     version=version.VERSION,
-    packages=["mlopspython_inference"],
+    packages=["inference"],
     package_dir={"": "src"},
-    package_data={"mlopspython_inference": ["*"]},
+    package_data={"inference": ["*"]},
     install_requires=requirements,
     author="Guillaume Chervet",
     include_package_data=True,
     python_requires=">=3.8",
     author_email="guillaume.chervet@gmail.com",
     url='https://github.com/guillaume-chervet/MLOpsPython',
     description="Inference package for MLOpsPython project",
```

