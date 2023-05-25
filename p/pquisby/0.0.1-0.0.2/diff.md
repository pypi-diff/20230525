# Comparing `tmp/pquisby-0.0.1.tar.gz` & `tmp/pquisby-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pquisby-0.0.1.tar", last modified: Thu May 18 05:11:29 2023, max compression
+gzip compressed data, was "pquisby-0.0.2.tar", last modified: Thu May 25 01:25:11 2023, max compression
```

## Comparing `pquisby-0.0.1.tar` & `pquisby-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,46 @@
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-18 05:11:29.701835 pquisby-0.0.1/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)    35149 2023-05-18 03:42:45.000000 pquisby-0.0.1/LICENSE
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       39 2023-05-18 05:09:46.000000 pquisby-0.0.1/MANIFEST.in
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      798 2023-05-18 05:11:29.701835 pquisby-0.0.1/PKG-INFO
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      474 2023-05-18 05:09:46.000000 pquisby-0.0.1/README.md
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-18 05:11:29.700835 pquisby-0.0.1/pquisby/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-18 05:09:46.000000 pquisby-0.0.1/pquisby/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      277 2023-05-18 05:09:46.000000 pquisby-0.0.1/pquisby/__main__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-18 05:11:29.701835 pquisby-0.0.1/pquisby.egg-info/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      798 2023-05-18 05:11:29.000000 pquisby-0.0.1/pquisby.egg-info/PKG-INFO
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      283 2023-05-18 05:11:29.000000 pquisby-0.0.1/pquisby.egg-info/SOURCES.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        1 2023-05-18 05:11:29.000000 pquisby-0.0.1/pquisby.egg-info/dependency_links.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       49 2023-05-18 05:11:29.000000 pquisby-0.0.1/pquisby.egg-info/entry_points.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1990 2023-05-18 05:11:29.000000 pquisby-0.0.1/pquisby.egg-info/requires.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        8 2023-05-18 05:11:29.000000 pquisby-0.0.1/pquisby.egg-info/top_level.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3903 2023-05-18 05:09:46.000000 pquisby-0.0.1/requirements.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       38 2023-05-18 05:11:29.701835 pquisby-0.0.1/setup.cfg
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      918 2023-05-18 05:10:22.000000 pquisby-0.0.1/setup.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.166885 pquisby-0.0.2/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)    35149 2023-05-24 16:14:46.000000 pquisby-0.0.2/LICENSE
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       39 2023-05-24 16:16:23.000000 pquisby-0.0.2/MANIFEST.in
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      798 2023-05-25 01:25:11.165885 pquisby-0.0.2/PKG-INFO
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      474 2023-05-24 16:16:23.000000 pquisby-0.0.2/README.md
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3903 2023-05-24 16:16:23.000000 pquisby-0.0.2/requirements.txt
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       38 2023-05-25 01:25:11.166885 pquisby-0.0.2/setup.cfg
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      950 2023-05-25 01:24:19.000000 pquisby-0.0.2/setup.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.159885 pquisby-0.0.2/src/
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.161885 pquisby-0.0.2/src/pquisby/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:14:46.000000 pquisby-0.0.2/src/pquisby/__init__.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.163885 pquisby-0.0.2/src/pquisby/command/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 00:29:29.000000 pquisby-0.0.2/src/pquisby/command/__init__.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      488 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/command/compare_benchmark.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      300 2023-05-25 00:29:57.000000 pquisby-0.0.2/src/pquisby/command/main.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     2513 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/command/process_benchmark.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.163885 pquisby-0.0.2/src/pquisby/lib/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/__init__.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.164885 pquisby-0.0.2/src/pquisby/lib/benchmarks/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/__init__.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.164885 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/__init__.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1214 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/comparison.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5175 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/graph.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5344 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/uperf.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1639 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/compare_result.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.164885 pquisby-0.0.2/src/pquisby/lib/credentials/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/credentials/__init__.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1119 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/credentials/creds.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3699 2023-05-24 16:18:25.000000 pquisby-0.0.2/src/pquisby/lib/get_data.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.165885 pquisby-0.0.2/src/pquisby/lib/pricing/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/pricing/__init__.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     4728 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/pricing/cloud_pricing.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5927 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/process_result.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.165885 pquisby-0.0.2/src/pquisby/lib/sheet/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/sheet/__init__.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5692 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/sheet/sheet_util.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      783 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/sheet/sheetapi.py
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     2202 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/util.py
+drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.162885 pquisby-0.0.2/src/pquisby.egg-info/
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      798 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/PKG-INFO
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1054 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/SOURCES.txt
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        1 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/dependency_links.txt
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       54 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/entry_points.txt
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1990 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/requires.txt
+-rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        8 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/top_level.txt
```

### Comparing `pquisby-0.0.1/LICENSE` & `pquisby-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.1/PKG-INFO` & `pquisby-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pquisby
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pquisby-0.0.1/pquisby.egg-info/PKG-INFO` & `pquisby-0.0.2/src/pquisby.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pquisby
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pquisby-0.0.1/pquisby.egg-info/requires.txt` & `pquisby-0.0.2/src/pquisby.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.1/requirements.txt` & `pquisby-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.1/setup.py` & `pquisby-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from setuptools import setup, find_namespace_packages
+from setuptools import setup, find_packages
 from importlib.metadata import entry_points
 import pathlib
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # The text of the README file
 REQUIRE = (HERE / "requirements.txt").read_text()
 
 setup(
     name="pquisby",
-    version="0.0.1",
+    version="0.0.2",
     description="Quisby is a data processing and visualization tool for benchmark testing.",
     url = 'https://github.com/sousinha1997/Quisby',
     author = 'Soumya Sinha',
     author_email = 'sinhasoumya97@gmail.com',
     license = 'GPL v3.0',
-    packages=["pquisby"],
+    packages=find_packages("src"),
+    package_dir={"":"src"},
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires = REQUIRE,
     entry_points={
         "console_scripts": [
-            "pquisby = pquisby.__main__:cli",
+            "pquisby = pquisby.command.main:main",
         ]
     },
     include_package_data=True,
 )
```

