# Comparing `tmp/IMCtermite-2.0.7.tar.gz` & `tmp/IMCtermite-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMCtermite-2.0.7.tar", last modified: Fri Feb 17 14:14:54 2023, max compression
+gzip compressed data, was "IMCtermite-2.0.8.tar", last modified: Thu May 25 18:28:14 2023, max compression
```

## Comparing `IMCtermite-2.0.7.tar` & `IMCtermite-2.0.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:14:54.906091 IMCtermite-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)   250385 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/IMCtermite.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:14:54.906091 IMCtermite-2.0.7/IMCtermite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/IMCtermite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/IMCtermite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/IMCtermite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/IMCtermite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/IMCtermite.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/IMCtermite.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-02-17 14:14:54.906091 IMCtermite-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:14:54.906091 IMCtermite-2.0.7/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/lib/endian.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   214552 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/lib/half.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/lib/half_precision_floating_point.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/lib/hexshow.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/lib/imc_block.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_channel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_conversion.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_datatype.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_key.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_parameter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_raw.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/imc_result.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/raweat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-02-17 14:14:54.000000 IMCtermite-2.0.7/lib/rawmerge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-17 14:14:54.906091 IMCtermite-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-17 14:14:53.000000 IMCtermite-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:28:14.132177 IMCtermite-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)   250385 2023-05-25 18:28:14.000000 IMCtermite-2.0.8/IMCtermite.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:28:14.132177 IMCtermite-2.0.8/IMCtermite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-25 18:28:14.000000 IMCtermite-2.0.8/IMCtermite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-25 18:28:14.000000 IMCtermite-2.0.8/IMCtermite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:28:14.000000 IMCtermite-2.0.8/IMCtermite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 18:28:14.000000 IMCtermite-2.0.8/IMCtermite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/IMCtermite.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/IMCtermite.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-25 18:28:14.132177 IMCtermite-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:28:14.132177 IMCtermite-2.0.8/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/endian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   214552 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/half.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/half_precision_floating_point.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/hexshow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_block.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_channel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_conversion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_datatype.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_key.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_parameter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_raw.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/imc_result.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/raweat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-25 18:28:13.000000 IMCtermite-2.0.8/lib/rawmerge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-25 18:28:14.132177 IMCtermite-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 18:28:12.000000 IMCtermite-2.0.8/setup.py
```

### Comparing `IMCtermite-2.0.7/IMCtermite.cpp` & `IMCtermite-2.0.8/IMCtermite.cpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/IMCtermite.egg-info/PKG-INFO` & `IMCtermite-2.0.8/IMCtermite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMCtermite
-Version: 2.0.7
+Version: 2.0.8
 Summary: Enables extraction of measurement data from binary files with extension 'raw' used by proprietary software imcFAMOS and imcSTUDIO and facilitates its storage in open source file formats
 Home-page: https://github.com/RecordEvolution/IMCtermite.git
 Author: Record Evolution GmbH
 Author-email: mario.fink@record-evolution.de
 Maintainer: Record Evolution GmbH
 License: MIT License
 Keywords: IMC,raw,imcFAMOS,imcSTUDIO,imcCRONOS
```

### Comparing `IMCtermite-2.0.7/IMCtermite.egg-info/SOURCES.txt` & `IMCtermite-2.0.8/IMCtermite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 IMCtermite.cpp
 IMCtermite.pxd
 IMCtermite.pyx
 LICENSE
 MANIFEST.in
 README.md
+VERSION
 pyproject.toml
 setup.cfg
 setup.py
 IMCtermite.egg-info/PKG-INFO
 IMCtermite.egg-info/SOURCES.txt
 IMCtermite.egg-info/dependency_links.txt
 IMCtermite.egg-info/top_level.txt
```

### Comparing `IMCtermite-2.0.7/IMCtermite.pxd` & `IMCtermite-2.0.8/IMCtermite.pxd`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/IMCtermite.pyx` & `IMCtermite-2.0.8/IMCtermite.pyx`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/LICENSE` & `IMCtermite-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/PKG-INFO` & `IMCtermite-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMCtermite
-Version: 2.0.7
+Version: 2.0.8
 Summary: Enables extraction of measurement data from binary files with extension 'raw' used by proprietary software imcFAMOS and imcSTUDIO and facilitates its storage in open source file formats
 Home-page: https://github.com/RecordEvolution/IMCtermite.git
 Author: Record Evolution GmbH
 Author-email: mario.fink@record-evolution.de
 Maintainer: Record Evolution GmbH
 License: MIT License
 Keywords: IMC,raw,imcFAMOS,imcSTUDIO,imcCRONOS
```

### Comparing `IMCtermite-2.0.7/README.md` & `IMCtermite-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/endian.hpp` & `IMCtermite-2.0.8/lib/endian.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/half.hpp` & `IMCtermite-2.0.8/lib/half.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/half_precision_floating_point.hpp` & `IMCtermite-2.0.8/lib/half_precision_floating_point.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/hexshow.hpp` & `IMCtermite-2.0.8/lib/hexshow.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_block.hpp` & `IMCtermite-2.0.8/lib/imc_block.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_channel.hpp` & `IMCtermite-2.0.8/lib/imc_channel.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_conversion.hpp` & `IMCtermite-2.0.8/lib/imc_conversion.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_datatype.hpp` & `IMCtermite-2.0.8/lib/imc_datatype.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_key.hpp` & `IMCtermite-2.0.8/lib/imc_key.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_object.hpp` & `IMCtermite-2.0.8/lib/imc_object.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_parameter.hpp` & `IMCtermite-2.0.8/lib/imc_parameter.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_raw.hpp` & `IMCtermite-2.0.8/lib/imc_raw.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/imc_result.hpp` & `IMCtermite-2.0.8/lib/imc_result.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/raweat.hpp` & `IMCtermite-2.0.8/lib/raweat.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/lib/rawmerge.hpp` & `IMCtermite-2.0.8/lib/rawmerge.hpp`

 * *Files identical despite different names*

### Comparing `IMCtermite-2.0.7/setup.cfg` & `IMCtermite-2.0.8/setup.cfg`

 * *Files identical despite different names*

