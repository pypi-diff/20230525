# Comparing `tmp/pysdot-0.2.7.tar.gz` & `tmp/pysdot-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdot-0.2.7.tar", last modified: Mon Apr 17 09:39:15 2023, max compression
+gzip compressed data, was "pysdot-0.2.8.tar", last modified: Fri May  5 12:52:12 2023, max compression
```

## Comparing `pysdot-0.2.7.tar` & `pysdot-0.2.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.694103 pysdot-0.2.7/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       29 2022-10-12 11:21:09.000000 pysdot-0.2.7/MANIFEST.in
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      490 2023-04-17 09:39:15.694103 pysdot-0.2.7/PKG-INFO
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.690103 pysdot-0.2.7/pysdot/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     5944 2023-04-17 09:30:02.000000 pysdot-0.2.7/pysdot/OptimalTransport.py
--rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)    16769 2022-10-19 07:05:57.000000 pysdot-0.2.7/pysdot/PowerDiagram.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       86 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.694103 pysdot-0.2.7/pysdot/cpp/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       25 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/cpp/__init__.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      204 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/cpp/comb_types.h
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      295 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/cpp/cpp_module.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    14376 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/cpp/inferno_color_map.h
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    44123 2023-04-17 09:34:00.000000 pysdot-0.2.7/pysdot/cpp/pybind_sdot.cpp
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      719 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/cpp/pybind_sdot_Arfd.cpp
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.694103 pysdot-0.2.7/pysdot/domain_types/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     3094 2022-10-12 11:35:06.000000 pysdot-0.2.7/pysdot/domain_types/ConvexPolyhedraAssembly.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1230 2022-10-19 07:05:57.000000 pysdot-0.2.7/pysdot/domain_types/ScaledImage.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       98 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/domain_types/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.694103 pysdot-0.2.7/pysdot/radial_funcs/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      592 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/RadialFuncArfd.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      253 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/RadialFuncEntropy.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      264 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/RadialFuncInBall.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      256 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/RadialFuncPpWmR2.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      224 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/RadialFuncR2.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      222 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/RadialFuncUnit.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      268 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/radial_funcs/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.694103 pysdot-0.2.7/pysdot/solvers/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      630 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/solvers/CuPyx.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      929 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/solvers/Petsc.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      493 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/solvers/Scipy.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        0 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/solvers/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.694103 pysdot-0.2.7/pysdot/util/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     2557 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/util/FastMarching.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       39 2022-10-12 11:21:09.000000 pysdot-0.2.7/pysdot/util/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-17 09:39:15.690103 pysdot-0.2.7/pysdot.egg-info/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      490 2023-04-17 09:39:15.000000 pysdot-0.2.7/pysdot.egg-info/PKG-INFO
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      930 2023-04-17 09:39:15.000000 pysdot-0.2.7/pysdot.egg-info/SOURCES.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        1 2023-04-17 09:39:15.000000 pysdot-0.2.7/pysdot.egg-info/dependency_links.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        6 2023-04-17 09:39:15.000000 pysdot-0.2.7/pysdot.egg-info/requires.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       68 2023-04-17 09:39:15.000000 pysdot-0.2.7/pysdot.egg-info/top_level.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       38 2023-04-17 09:39:15.694103 pysdot-0.2.7/setup.cfg
--rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)     3372 2023-04-17 09:35:55.000000 pysdot-0.2.7/setup.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.809024 pysdot-0.2.8/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       29 2023-01-20 07:48:21.000000 pysdot-0.2.8/MANIFEST.in
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      454 2023-05-05 12:52:12.809024 pysdot-0.2.8/PKG-INFO
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     7281 2023-05-05 12:51:53.000000 pysdot-0.2.8/pysdot/OptimalTransport.py
+-rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)    16769 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/PowerDiagram.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       86 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/cpp/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       25 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/__init__.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      204 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/comb_types.h
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      295 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/cpp_module.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    14376 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/inferno_color_map.h
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    44123 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/pybind_sdot.cpp
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      719 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/pybind_sdot_Arfd.cpp
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/domain_types/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     3094 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/domain_types/ConvexPolyhedraAssembly.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1230 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/domain_types/ScaledImage.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       98 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/domain_types/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/radial_funcs/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      592 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncArfd.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      253 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncEntropy.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      264 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncInBall.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      256 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncPpWmR2.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      224 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncR2.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      222 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncUnit.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      268 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/solvers/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      630 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/CuPyx.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      929 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/Petsc.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      493 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/Scipy.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        0 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.809024 pysdot-0.2.8/pysdot/util/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     2557 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/util/FastMarching.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       39 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/util/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot.egg-info/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      454 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/PKG-INFO
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      930 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/SOURCES.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        1 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/dependency_links.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        6 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/requires.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       68 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/top_level.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       38 2023-05-05 12:52:12.809024 pysdot-0.2.8/setup.cfg
+-rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)     3372 2023-05-05 12:51:24.000000 pysdot-0.2.8/setup.py
```

### Comparing `pysdot-0.2.7/pysdot/PowerDiagram.py` & `pysdot-0.2.8/pysdot/PowerDiagram.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/cpp/inferno_color_map.h` & `pysdot-0.2.8/pysdot/cpp/inferno_color_map.h`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/cpp/pybind_sdot.cpp` & `pysdot-0.2.8/pysdot/cpp/pybind_sdot.cpp`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/cpp/pybind_sdot_Arfd.cpp` & `pysdot-0.2.8/pysdot/cpp/pybind_sdot_Arfd.cpp`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/domain_types/ConvexPolyhedraAssembly.py` & `pysdot-0.2.8/pysdot/domain_types/ConvexPolyhedraAssembly.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/domain_types/ScaledImage.py` & `pysdot-0.2.8/pysdot/domain_types/ScaledImage.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/radial_funcs/RadialFuncArfd.py` & `pysdot-0.2.8/pysdot/radial_funcs/RadialFuncArfd.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/solvers/CuPyx.py` & `pysdot-0.2.8/pysdot/solvers/CuPyx.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/solvers/Petsc.py` & `pysdot-0.2.8/pysdot/solvers/Petsc.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot/util/FastMarching.py` & `pysdot-0.2.8/pysdot/util/FastMarching.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/pysdot.egg-info/SOURCES.txt` & `pysdot-0.2.8/pysdot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.7/setup.py` & `pysdot-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             subprocess.check_call(['git', 'clone', 'https://github.com/eigenteam/eigen-git-mirror.git', 'ext/eigen3'])
         if not os.path.isdir('./ext/pybind11'):
             subprocess.check_call(['git', 'clone', 'https://github.com/pybind/pybind11.git', 'ext/pybind11'])
         setuptools.command.build_py.build_py.run(self)
 
 setup(
     name='pysdot',
-    version='0.2.7',
+    version='0.2.8',
     packages=find_packages(exclude=[
         'hugo', 'ext', 'build', 'dist',
         'examples', 'results', 'tests'
     ]),
     cmdclass={
         'build_py': BuildPyCommand,
     },
```

