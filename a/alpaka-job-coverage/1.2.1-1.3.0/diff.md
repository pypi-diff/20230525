# Comparing `tmp/alpaka-job-coverage-1.2.1.tar.gz` & `tmp/alpaka-job-coverage-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.2.1.tar", last modified: Tue Aug 23 14:29:27 2022, max compression
+gzip compressed data, was "alpaka-job-coverage-1.3.0.tar", last modified: Wed May 24 16:38:01 2023, max compression
```

## Comparing `alpaka-job-coverage-1.2.1.tar` & `alpaka-job-coverage-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 14:29:27.445088 alpaka-job-coverage-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2022-08-23 14:29:27.445088 alpaka-job-coverage-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5983 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-23 14:29:27.445088 alpaka-job-coverage-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 14:29:27.445088 alpaka-job-coverage-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 14:29:27.445088 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9305 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 14:29:27.445088 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2022-08-23 14:29:27.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-08-23 14:29:27.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 14:29:27.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-23 14:29:27.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-23 14:29:27.000000 alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-23 14:29:12.000000 alpaka-job-coverage-1.2.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:38:01.766342 alpaka-job-coverage-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-24 16:38:01.766342 alpaka-job-coverage-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:38:01.766342 alpaka-job-coverage-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:38:01.758342 alpaka-job-coverage-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:38:01.766342 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:38:01.766342 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-24 16:38:01.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 16:38:01.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:38:01.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 16:38:01.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 16:38:01.000000 alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:37:41.000000 alpaka-job-coverage-1.3.0/version.txt
```

### Comparing `alpaka-job-coverage-1.2.1/LICENSE` & `alpaka-job-coverage-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/PKG-INFO` & `alpaka-job-coverage-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.2.1
+Version: 1.3.0
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.2.1/README.md` & `alpaka-job-coverage-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/setup.py` & `alpaka-job-coverage-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
         bool: True, if combination is valid, otherwise False.
     """
     ###########################
     ## gcc device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", GCC):
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
             return False
 
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             return False
 
     ###########################
     ## clang device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG):
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
             return False
 
         # clang cannot compile with enabled HIP backend
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             return False
 
     ###########################
     ## nvcc device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", NVCC):
@@ -58,32 +58,32 @@
             ALPAKA_ACC_GPU_CUDA_ENABLE,
             "!=",
             row[param_map[DEVICE_COMPILER]][VERSION],
         ):
             return False
 
         # it is not allowed to enable the HIP and CUDA backend on the same time
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             return False
 
     ###########################
     ## clang-cuda device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA):
         # the CUDA backend needs to be defined
         if backend_is_not_in_row(row, ALPAKA_ACC_GPU_CUDA_ENABLE):
             return False
 
         # the CUDA backend needs to be enabled
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "==", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "==", OFF_VER):
             return False
 
         # it is not allowed to enable the HIP and CUDA backend on the same time
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             return False
 
         if row_check_version(
             row, DEVICE_COMPILER, "<=", "7"
         ) and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">", "9.2"):
             return False
 
@@ -127,11 +127,11 @@
             ALPAKA_ACC_GPU_HIP_ENABLE,
             "!=",
             row[param_map[DEVICE_COMPILER]][VERSION],
         ):
             return False
 
         # it is not allowed to enable the HIP and CUDA backend on the same time
-        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
             return False
 
     return True
```

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,29 +88,29 @@
                 row, HOST_COMPILER, "==", compiler_name
             ) and row_check_version(row, HOST_COMPILER, "<=", "9"):
                 return False
 
     # ubuntu 18.04 containers are not available for CUDA 11.0 and later
     if (
         row_check_version(row, UBUNTU, "==", "18.04")
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF)
+        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER)
         and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">=", "11.0")
     ):
         return False
 
     # ubuntu 20.04 containers are not available for CUDA 10.2 and before
     if (
         row_check_version(row, UBUNTU, "==", "20.04")
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF)
+        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER)
         and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "<", "11.0")
     ):
         return False
 
     # all rocm images are Ubuntu 20.04 based
     if (
         row_check_version(row, UBUNTU, "!=", "20.04")
         and row_check_name(row, DEVICE_COMPILER, "==", HIPCC)
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF)
+        and row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER)
     ):
         return False
 
     return True
```

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/globals.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,18 +37,22 @@
     ALPAKA_ACC_CPU_B_OMP2_T_SEQ_ENABLE,
     ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE,
     ALPAKA_ACC_ANY_BT_OMP5_ENABLE,
     ALPAKA_ACC_GPU_CUDA_ENABLE,
     ALPAKA_ACC_GPU_HIP_ENABLE,
 ]
 
-# backend states
+# if want to use version comparison functions from util.py, you need to use ON_VER and OFF_VER
 ON: str = "on"
 OFF: str = "off"
 
+# backend states
+ON_VER: str = "1.0.0"
+OFF_VER: str = "0.0.0"
+
 # additional parameters, like alpaka software dependencies, compiler configurations and so one
 UBUNTU: str = "ubuntu"
 CMAKE: str = "cmake"
 BOOST: str = "boost"
 CXX_STANDARD: str = "cxx_standard"
 
 # Is required because allpairspy uses a List for each row. The ordering of the entries in a row
```

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.2.1
+Version: 1.3.0
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.2.1/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.3.0/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

