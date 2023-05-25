# Comparing `tmp/RobustifyToolkit-0.0.7a0.tar.gz` & `tmp/RobustifyToolkit-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobustifyToolkit-0.0.7a0.tar", last modified: Thu May 25 16:11:55 2023, max compression
+gzip compressed data, was "RobustifyToolkit-0.0.8a0.tar", last modified: Thu May 25 16:48:02 2023, max compression
```

## Comparing `RobustifyToolkit-0.0.7a0.tar` & `RobustifyToolkit-0.0.8a0.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-25 16:11:55.000000 RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-25 16:11:55.000000 RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:11:55.000000 RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 16:11:55.000000 RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 16:11:55.000000 RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/robustify/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/robustify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/robustify/noise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/robustify/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/robustify/noise/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/robustify/noise/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/robustify/noiseCorruptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-25 16:11:45.000000 RobustifyToolkit-0.0.7a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:11:55.179866 RobustifyToolkit-0.0.7a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-25 16:11:46.000000 RobustifyToolkit-0.0.7a0/tests/test_gaussianNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 16:11:46.000000 RobustifyToolkit-0.0.7a0/tests/test_poissonNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 16:11:46.000000 RobustifyToolkit-0.0.7a0/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-25 16:11:46.000000 RobustifyToolkit-0.0.7a0/tests/test_scikt-learn_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-25 16:11:46.000000 RobustifyToolkit-0.0.7a0/tests/test_tensorflow_keras_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.794044 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.794044 RobustifyToolkit-0.0.8a0/robustify/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.794044 RobustifyToolkit-0.0.8a0/robustify/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noise/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noise/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noiseCorruptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/robustify/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_gaussianNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_poissonNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_scikt-learn_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_tensorflow_keras_compatibility.py
```

### Comparing `RobustifyToolkit-0.0.7a0/LICENSE` & `RobustifyToolkit-0.0.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/PKG-INFO` & `RobustifyToolkit-0.0.8a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobustifyToolkit
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: Robustify:
 Author: Isabel Foster
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `RobustifyToolkit-0.0.7a0/README.md` & `RobustifyToolkit-0.0.8a0/README.md`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/RobustifyToolkit.egg-info/PKG-INFO` & `RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobustifyToolkit
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: Robustify:
 Author: Isabel Foster
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `RobustifyToolkit-0.0.7a0/robustify/noise/continuous.py` & `RobustifyToolkit-0.0.8a0/robustify/noise/continuous.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/robustify/noise/discrete.py` & `RobustifyToolkit-0.0.8a0/robustify/noise/discrete.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/robustify/noiseCorruptions.py` & `RobustifyToolkit-0.0.8a0/robustify/noiseCorruptions.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/setup.py` & `RobustifyToolkit-0.0.8a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 from setuptools import find_packages, setup
 setup(
     name='RobustifyToolkit',
-    packages=find_packages(include=['robustify', 'robustify.noise', 'robustify.utils' 'tests']),
-    version='0.0.7-alpha',
+    packages=find_packages(include=['robustify', 'robustify.noise', 'robustify.utils', 'tests']),
+    version='0.0.8-alpha',
     readme="README.md",
     description="Robustify:" ,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Isabel Foster',
     license='MIT',
     classifiers=[
```

### Comparing `RobustifyToolkit-0.0.7a0/tests/test_gaussianNoise.py` & `RobustifyToolkit-0.0.8a0/tests/test_gaussianNoise.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/tests/test_poissonNoise.py` & `RobustifyToolkit-0.0.8a0/tests/test_poissonNoise.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/tests/test_scikt-learn_compatibility.py` & `RobustifyToolkit-0.0.8a0/tests/test_scikt-learn_compatibility.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.7a0/tests/test_tensorflow_keras_compatibility.py` & `RobustifyToolkit-0.0.8a0/tests/test_tensorflow_keras_compatibility.py`

 * *Files identical despite different names*

