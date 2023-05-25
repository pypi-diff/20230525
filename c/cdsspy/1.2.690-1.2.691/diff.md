# Comparing `tmp/cdsspy-1.2.690.tar.gz` & `tmp/cdsspy-1.2.691.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsspy-1.2.690.tar", last modified: Wed May 24 17:35:55 2023, max compression
+gzip compressed data, was "cdsspy-1.2.691.tar", last modified: Wed May 24 17:53:26 2023, max compression
```

## Comparing `cdsspy-1.2.690.tar` & `cdsspy-1.2.691.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 17:35:55.519964 cdsspy-1.2.690/
--rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.690/LICENSE
--rw-rw-rw-   0        0        0    19402 2023-05-24 17:35:55.519964 cdsspy-1.2.690/PKG-INFO
--rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.690/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 17:35:55.482965 cdsspy-1.2.690/cdsspy/
--rw-rw-rw-   0        0        0      294 2023-05-24 17:35:42.000000 cdsspy-1.2.690/cdsspy/__init__.py
--rw-rw-rw-   0        0        0     5075 2023-05-24 17:35:14.000000 cdsspy-1.2.690/cdsspy/admin_calls.py
--rw-rw-rw-   0        0        0    34256 2023-05-24 17:34:52.000000 cdsspy-1.2.690/cdsspy/analysis_services.py
--rw-rw-rw-   0        0        0    23273 2023-05-24 17:35:03.000000 cdsspy-1.2.690/cdsspy/climate.py
--rw-rw-rw-   0        0        0    15842 2023-05-24 17:34:51.000000 cdsspy-1.2.690/cdsspy/gw.py
--rw-rw-rw-   0        0        0    25370 2023-05-24 17:34:49.000000 cdsspy-1.2.690/cdsspy/reference_tbl.py
--rw-rw-rw-   0        0        0    34631 2023-05-24 17:34:50.000000 cdsspy-1.2.690/cdsspy/structures.py
--rw-rw-rw-   0        0        0    24836 2023-05-24 17:34:18.000000 cdsspy-1.2.690/cdsspy/sw.py
--rw-rw-rw-   0        0        0    11244 2023-05-24 17:34:21.000000 cdsspy-1.2.690/cdsspy/telemetry.py
--rw-rw-rw-   0        0        0    33575 2023-05-24 14:30:00.000000 cdsspy-1.2.690/cdsspy/utils.py
--rw-rw-rw-   0        0        0     9956 2023-05-24 17:34:33.000000 cdsspy-1.2.690/cdsspy/water_rights.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:35:55.516962 cdsspy-1.2.690/cdsspy.egg-info/
--rw-rw-rw-   0        0        0    19402 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 17:35:55.520964 cdsspy-1.2.690/setup.cfg
--rw-rw-rw-   0        0        0     1357 2023-05-24 17:35:44.000000 cdsspy-1.2.690/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:53:26.556854 cdsspy-1.2.691/
+-rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.691/LICENSE
+-rw-rw-rw-   0        0        0    19402 2023-05-24 17:53:26.556854 cdsspy-1.2.691/PKG-INFO
+-rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.691/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 17:53:26.535853 cdsspy-1.2.691/cdsspy/
+-rw-rw-rw-   0        0        0      276 2023-05-24 17:51:53.000000 cdsspy-1.2.691/cdsspy/__init__.py
+-rw-rw-rw-   0        0        0     5075 2023-05-24 17:35:14.000000 cdsspy-1.2.691/cdsspy/admin_calls.py
+-rw-rw-rw-   0        0        0    34256 2023-05-24 17:34:52.000000 cdsspy-1.2.691/cdsspy/analysis_services.py
+-rw-rw-rw-   0        0        0    23273 2023-05-24 17:53:19.000000 cdsspy-1.2.691/cdsspy/climate.py
+-rw-rw-rw-   0        0        0    15842 2023-05-24 17:34:51.000000 cdsspy-1.2.691/cdsspy/gw.py
+-rw-rw-rw-   0        0        0    25370 2023-05-24 17:34:49.000000 cdsspy-1.2.691/cdsspy/reference_tbl.py
+-rw-rw-rw-   0        0        0    34631 2023-05-24 17:34:50.000000 cdsspy-1.2.691/cdsspy/structures.py
+-rw-rw-rw-   0        0        0    24836 2023-05-24 17:34:18.000000 cdsspy-1.2.691/cdsspy/sw.py
+-rw-rw-rw-   0        0        0    11244 2023-05-24 17:34:21.000000 cdsspy-1.2.691/cdsspy/telemetry.py
+-rw-rw-rw-   0        0        0    33575 2023-05-24 14:30:00.000000 cdsspy-1.2.691/cdsspy/utils.py
+-rw-rw-rw-   0        0        0     9956 2023-05-24 17:34:33.000000 cdsspy-1.2.691/cdsspy/water_rights.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:53:26.554853 cdsspy-1.2.691/cdsspy.egg-info/
+-rw-rw-rw-   0        0        0    19402 2023-05-24 17:53:26.000000 cdsspy-1.2.691/cdsspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-24 17:53:26.000000 cdsspy-1.2.691/cdsspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 17:53:26.000000 cdsspy-1.2.691/cdsspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 17:53:26.000000 cdsspy-1.2.691/cdsspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 17:53:26.000000 cdsspy-1.2.691/cdsspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 17:53:26.557853 cdsspy-1.2.691/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-05-24 17:52:05.000000 cdsspy-1.2.691/setup.py
```

### Comparing `cdsspy-1.2.690/LICENSE` & `cdsspy-1.2.691/LICENSE`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/PKG-INFO` & `cdsspy-1.2.691/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.690
+Version: 1.2.691
 Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
 Author: Angus Watters
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.690 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.691 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.690/README.md` & `cdsspy-1.2.691/README.md`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/admin_calls.py` & `cdsspy-1.2.691/cdsspy/admin_calls.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/analysis_services.py` & `cdsspy-1.2.691/cdsspy/analysis_services.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/climate.py` & `cdsspy-1.2.691/cdsspy/climate.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/gw.py` & `cdsspy-1.2.691/cdsspy/gw.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/reference_tbl.py` & `cdsspy-1.2.691/cdsspy/reference_tbl.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/structures.py` & `cdsspy-1.2.691/cdsspy/structures.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/sw.py` & `cdsspy-1.2.691/cdsspy/sw.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/telemetry.py` & `cdsspy-1.2.691/cdsspy/telemetry.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/utils.py` & `cdsspy-1.2.691/cdsspy/utils.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy/water_rights.py` & `cdsspy-1.2.691/cdsspy/water_rights.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.690/cdsspy.egg-info/PKG-INFO` & `cdsspy-1.2.691/cdsspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.690
+Version: 1.2.691
 Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
 Author: Angus Watters
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.690 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.691 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.690/setup.py` & `cdsspy-1.2.691/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdsspy",                     # This is the name of the package
-    version="1.2.690",                        # The initial release version
+    version="1.2.691",                        # The initial release version
     author="Angus Watters",                     # Full name of the author
     description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     # packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
     classifiers=[
```

