# Comparing `tmp/FFHT-unofficial-0.2.tar.gz` & `tmp/FFHT-unofficial-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFHT-unofficial-0.2.tar", last modified: Fri May 19 16:04:27 2023, max compression
+gzip compressed data, was "FFHT-unofficial-0.3.tar", last modified: Thu May 25 09:33:22 2023, max compression
```

## Comparing `FFHT-unofficial-0.2.tar` & `FFHT-unofficial-0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:04:27.094532 FFHT-unofficial-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:04:27.090532 FFHT-unofficial-0.2/FFHT_unofficial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-19 16:04:27.000000 FFHT-unofficial-0.2/FFHT_unofficial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-19 16:04:27.000000 FFHT-unofficial-0.2/FFHT_unofficial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:04:27.000000 FFHT-unofficial-0.2/FFHT_unofficial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 16:04:27.000000 FFHT-unofficial-0.2/FFHT_unofficial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-19 16:04:27.094532 FFHT-unofficial-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:04:27.094532 FFHT-unofficial-0.2/ffht/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/_ffht_2.c
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/_ffht_3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fast_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fast_copy.h
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht-pybind11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht.c
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht.h
--rw-r--r--   0 runner    (1001) docker     (123)   875212 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht_header_only.h
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)  1006554 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/ffht/fht_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:04:27.094532 FFHT-unofficial-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-19 16:04:19.000000 FFHT-unofficial-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:33:22.425577 FFHT-unofficial-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:33:22.417577 FFHT-unofficial-0.3/FFHT_unofficial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-25 09:33:22.000000 FFHT-unofficial-0.3/FFHT_unofficial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 09:33:22.000000 FFHT-unofficial-0.3/FFHT_unofficial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:33:22.000000 FFHT-unofficial-0.3/FFHT_unofficial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 09:33:22.000000 FFHT-unofficial-0.3/FFHT_unofficial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 09:33:22.000000 FFHT-unofficial-0.3/FFHT_unofficial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-25 09:33:22.425577 FFHT-unofficial-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:33:22.421577 FFHT-unofficial-0.3/ffht/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/_ffht_2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/_ffht_3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fast_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fast_copy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht-pybind11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht.c
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht.h
+-rw-r--r--   0 runner    (1001) docker     (123)   875212 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht_header_only.h
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)  1006554 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/ffht/fht_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:33:22.425577 FFHT-unofficial-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-25 09:33:11.000000 FFHT-unofficial-0.3/setup.py
```

### Comparing `FFHT-unofficial-0.2/ffht/_ffht_2.c` & `FFHT-unofficial-0.3/ffht/_ffht_2.c`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/_ffht_3.c` & `FFHT-unofficial-0.3/ffht/_ffht_3.c`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fast_copy.c` & `FFHT-unofficial-0.3/ffht/fast_copy.c`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fht-pybind11.cpp` & `FFHT-unofficial-0.3/ffht/fht-pybind11.cpp`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fht.h` & `FFHT-unofficial-0.3/ffht/fht.h`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fht_avx.c` & `FFHT-unofficial-0.3/ffht/fht_avx.c`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fht_header_only.h` & `FFHT-unofficial-0.3/ffht/fht_header_only.h`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fht_impl.h` & `FFHT-unofficial-0.3/ffht/fht_impl.h`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/ffht/fht_sse.c` & `FFHT-unofficial-0.3/ffht/fht_sse.c`

 * *Files identical despite different names*

### Comparing `FFHT-unofficial-0.2/setup.py` & `FFHT-unofficial-0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     sources=["ffht/fht-pybind11.cpp", "ffht/fht.c", "ffht/fast_copy.c"],
     extra_compile_args=extra_compile_args,
     extra_link_args=['-fopenmp'],
     include_dirs=[np.get_include()] + ['ffht-unofficial/ffht']
     )
 
 setup(name='FFHT-unofficial',
-      version='0.2',
+      version='0.3',
       author='Alexandre Pasco',
       url='https://github.com/alexandre-pasco/FFHT-unofficial',
       description='Fast implementation of the Fast Hadamard Transform (FHT)',
       long_description=long_description,
       long_description_content_type='text/markdown',
       license='MIT',
       keywords='fast Fourier Hadamard transform butterfly',
       packages=find_packages(),
+      install_requires=['numpy ','pybind11'],
       include_package_data=True,
       ext_modules=[module])
```

