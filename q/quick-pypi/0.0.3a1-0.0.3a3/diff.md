# Comparing `tmp/quick-pypi-0.0.3a1.tar.gz` & `tmp/quick-pypi-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-0.0.3a1.tar", last modified: Wed May 24 14:06:33 2023, max compression
+gzip compressed data, was "quick-pypi-0.0.3a3.tar", last modified: Thu May 25 01:43:20 2023, max compression
```

## Comparing `quick-pypi-0.0.3a1.tar` & `quick-pypi-0.0.3a3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:06:33.919108 quick-pypi-0.0.3a1/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.3a1/LICENSE
--rw-rw-rw-   0        0        0      252 2022-01-17 11:10:09.000000 quick-pypi-0.0.3a1/MANIFEST.in
--rw-rw-rw-   0        0        0     4916 2023-05-24 14:06:33.919108 quick-pypi-0.0.3a1/PKG-INFO
--rw-rw-rw-   0        0        0     3709 2023-05-24 10:36:19.000000 quick-pypi-0.0.3a1/README.md
--rw-rw-rw-   0        0        0       81 2023-05-24 14:06:33.919108 quick-pypi-0.0.3a1/setup.cfg
--rw-rw-rw-   0        0        0     8548 2023-05-24 10:36:19.000000 quick-pypi-0.0.3a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:06:33.687944 quick-pypi-0.0.3a1/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:06:33.766092 quick-pypi-0.0.3a1/src/quick_pypi/
--rw-rw-rw-   0        0        0       21 2022-01-28 20:43:51.000000 quick-pypi-0.0.3a1/src/quick_pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:06:33.781720 quick-pypi-0.0.3a1/src/quick_pypi/__pycache__/
--rw-rw-rw-   0        0        0      208 2022-01-28 18:44:01.000000 quick-pypi-0.0.3a1/src/quick_pypi/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0     6124 2022-01-28 19:04:43.000000 quick-pypi-0.0.3a1/src/quick_pypi/__pycache__/deploy.cpython-36.pyc
--rw-rw-rw-   0        0        0     9920 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/deploy.py
--rw-rw-rw-   0        0        0    10376 2023-05-24 14:06:10.000000 quick-pypi-0.0.3a1/src/quick_pypi/deploy_toml.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:06:33.919108 quick-pypi-0.0.3a1/src/quick_pypi/template/
--rw-rw-rw-   0        0        0     1106 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/LICENSE
--rw-rw-rw-   0        0        0      292 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2022-01-28 19:03:49.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/README.md
--rw-rw-rw-   0        0        0     6300 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/pyproject.toml
--rw-rw-rw-   0        0        0     6308 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/pyproject_no_urls.toml
--rw-rw-rw-   0        0        0     6318 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/pyproject_only_project_url.toml
--rw-rw-rw-   0        0        0      205 2022-01-28 16:39:43.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/setup.cfg
--rw-rw-rw-   0        0        0     8606 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/setup.py
--rw-rw-rw-   0        0        0     8591 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/setup_no_urls.py
--rw-rw-rw-   0        0        0     8590 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a1/src/quick_pypi/template/setup_with_only_project_url.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:06:33.781720 quick-pypi-0.0.3a1/src/quick_pypi.egg-info/
--rw-rw-rw-   0        0        0     4916 2023-05-24 14:06:33.000000 quick-pypi-0.0.3a1/src/quick_pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-05-24 14:06:33.000000 quick-pypi-0.0.3a1/src/quick_pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:06:33.000000 quick-pypi-0.0.3a1/src/quick_pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-24 14:06:33.000000 quick-pypi-0.0.3a1/src/quick_pypi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 14:06:33.000000 quick-pypi-0.0.3a1/src/quick_pypi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.3a3/LICENSE
+-rw-rw-rw-   0        0        0      252 2022-01-17 11:10:09.000000 quick-pypi-0.0.3a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4916 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/PKG-INFO
+-rw-rw-rw-   0        0        0     3709 2023-05-24 10:36:19.000000 quick-pypi-0.0.3a3/README.md
+-rw-rw-rw-   0        0        0       81 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/setup.cfg
+-rw-rw-rw-   0        0        0     8548 2023-05-25 01:42:59.000000 quick-pypi-0.0.3a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.777375 quick-pypi-0.0.3a3/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.823202 quick-pypi-0.0.3a3/src/quick_pypi/
+-rw-rw-rw-   0        0        0       21 2022-01-28 20:43:51.000000 quick-pypi-0.0.3a3/src/quick_pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.867552 quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/
+-rw-rw-rw-   0        0        0      208 2022-01-28 18:44:01.000000 quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0     6124 2022-01-28 19:04:43.000000 quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/deploy.cpython-36.pyc
+-rw-rw-rw-   0        0        0     9920 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/deploy.py
+-rw-rw-rw-   0        0        0    10376 2023-05-24 14:06:10.000000 quick-pypi-0.0.3a3/src/quick_pypi/deploy_toml.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/src/quick_pypi/template/
+-rw-rw-rw-   0        0        0     1106 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/LICENSE
+-rw-rw-rw-   0        0        0      292 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2022-01-28 19:03:49.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/README.md
+-rw-rw-rw-   0        0        0     6548 2023-05-25 01:40:08.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject.toml
+-rw-rw-rw-   0        0        0     6558 2023-05-25 01:40:08.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_no_urls.toml
+-rw-rw-rw-   0        0        0     6568 2023-05-25 01:40:08.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_only_project_url.toml
+-rw-rw-rw-   0        0        0      205 2022-01-28 16:39:43.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup.cfg
+-rw-rw-rw-   0        0        0     8606 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup.py
+-rw-rw-rw-   0        0        0     8591 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup_no_urls.py
+-rw-rw-rw-   0        0        0     8590 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup_with_only_project_url.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.866546 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/
+-rw-rw-rw-   0        0        0     4916 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/top_level.txt
```

### Comparing `quick-pypi-0.0.3a1/LICENSE` & `quick-pypi-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/PKG-INFO` & `quick-pypi-0.0.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi
-Version: 0.0.3a1
+Version: 0.0.3a3
 Summary: The simplest and quickest way to build and publish a PyPI package
 Home-page: https://github.com/dhchenx/quick-pypi
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-pypi/issues
 Project-URL: Source, https://github.com/dhchenx/quick-pypi
```

### Comparing `quick-pypi-0.0.3a1/README.md` & `quick-pypi-0.0.3a3/README.md`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/setup.py` & `quick-pypi-0.0.3a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3a1',  # Required
+    version='0.0.3a3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='The simplest and quickest way to build and publish a PyPI package',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/__pycache__/deploy.cpython-36.pyc` & `quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/deploy.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/deploy.py` & `quick-pypi-0.0.3a3/src/quick_pypi/deploy.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/deploy_toml.py` & `quick-pypi-0.0.3a3/src/quick_pypi/deploy_toml.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/LICENSE` & `quick-pypi-0.0.3a3/src/quick_pypi/template/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/pyproject.toml` & `quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -142,13 +142,23 @@
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 # package-data = {"sample" = ["*.dat"]}
+# ...
+# By default, include-package-data is true in pyproject.toml, so you do
+# NOT have to specify this line.
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["*.ipynb"]
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/pyproject_no_urls.toml` & `quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_no_urls.toml`

 * *Files 6% similar despite different names*

```diff
@@ -142,13 +142,24 @@
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 # package-data = {"sample" = ["*.dat"]}
+# ...
+# By default, include-package-data is true in pyproject.toml, so you do
+# NOT have to specify this line.
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["*.ipynb"]
+
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/pyproject_only_project_url.toml` & `quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_only_project_url.toml`

 * *Files 6% similar despite different names*

```diff
@@ -142,13 +142,24 @@
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 # package-data = {"sample" = ["*.dat"]}
+# ...
+# By default, include-package-data is true in pyproject.toml, so you do
+# NOT have to specify this line.
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["*.ipynb"]
+
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/setup.py` & `quick-pypi-0.0.3a3/src/quick_pypi/template/setup.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/setup_no_urls.py` & `quick-pypi-0.0.3a3/src/quick_pypi/template/setup_no_urls.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi/template/setup_with_only_project_url.py` & `quick-pypi-0.0.3a3/src/quick_pypi/template/setup_with_only_project_url.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi.egg-info/PKG-INFO` & `quick-pypi-0.0.3a3/src/quick_pypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi
-Version: 0.0.3a1
+Version: 0.0.3a3
 Summary: The simplest and quickest way to build and publish a PyPI package
 Home-page: https://github.com/dhchenx/quick-pypi
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-pypi/issues
 Project-URL: Source, https://github.com/dhchenx/quick-pypi
```

### Comparing `quick-pypi-0.0.3a1/src/quick_pypi.egg-info/SOURCES.txt` & `quick-pypi-0.0.3a3/src/quick_pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

