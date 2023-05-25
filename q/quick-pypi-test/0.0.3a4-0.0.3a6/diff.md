# Comparing `tmp/quick-pypi-test-0.0.3a4.tar.gz` & `tmp/quick-pypi-test-0.0.3a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-test-0.0.3a4.tar", last modified: Wed May 24 14:54:20 2023, max compression
+gzip compressed data, was "quick-pypi-test-0.0.3a6.tar", last modified: Thu May 25 01:31:03 2023, max compression
```

## Comparing `quick-pypi-test-0.0.3a4.tar` & `quick-pypi-test-0.0.3a6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:54:20.267087 quick-pypi-test-0.0.3a4/
--rw-rw-rw-   0        0        0     1106 2023-05-24 14:54:09.000000 quick-pypi-test-0.0.3a4/LICENSE
--rw-rw-rw-   0        0        0     2582 2023-05-24 14:54:20.267087 quick-pypi-test-0.0.3a4/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-24 14:54:09.000000 quick-pypi-test-0.0.3a4/README.md
--rw-rw-rw-   0        0        0     6384 2023-05-24 14:54:09.000000 quick-pypi-test-0.0.3a4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 14:54:20.268090 quick-pypi-test-0.0.3a4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 14:54:20.248085 quick-pypi-test-0.0.3a4/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:54:20.252085 quick-pypi-test-0.0.3a4/src/quick_pypi_test/
--rw-rw-rw-   0        0        0       15 2023-05-24 14:54:02.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:54:20.266085 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/
--rw-rw-rw-   0        0        0     2582 2023-05-24 14:54:20.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-24 14:54:20.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:54:20.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-24 14:54:20.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-05-24 14:54:20.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 14:54:20.000000 quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 01:31:03.675107 quick-pypi-test-0.0.3a6/
+-rw-rw-rw-   0        0        0     1106 2023-05-25 01:27:53.000000 quick-pypi-test-0.0.3a6/LICENSE
+-rw-rw-rw-   0        0        0     2582 2023-05-25 01:31:03.675107 quick-pypi-test-0.0.3a6/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-25 01:27:53.000000 quick-pypi-test-0.0.3a6/README.md
+-rw-rw-rw-   0        0        0     6632 2023-05-25 01:30:04.000000 quick-pypi-test-0.0.3a6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 01:31:03.676106 quick-pypi-test-0.0.3a6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 01:31:03.662107 quick-pypi-test-0.0.3a6/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 01:31:03.665105 quick-pypi-test-0.0.3a6/src/quick_pypi_test/
+-rw-rw-rw-   0        0        0       15 2023-05-24 14:54:02.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test/__init__.py
+-rw-rw-rw-   0        0        0      307 2023-05-24 14:54:02.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test/lib.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-25 01:31:03.674111 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0     2582 2023-05-25 01:31:03.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-05-25 01:31:03.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:31:03.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-25 01:31:03.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-05-25 01:31:03.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-25 01:31:03.000000 quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/top_level.txt
```

### Comparing `quick-pypi-test-0.0.3a4/LICENSE` & `quick-pypi-test-0.0.3a6/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-test-0.0.3a4/PKG-INFO` & `quick-pypi-test-0.0.3a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.3a4
+Version: 0.0.3a6
 Summary: This is a quick-pypi-test package!
 Author-email: Donghua Chen <douglaschan@126.com>
 License: MIT License
         
         Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,12 +47,12 @@
 
 # A quick-pypi-test package!
 
 This is a quick-pypi-test package!
 
 ## Installation
 ```pip
-pip install quick-pypi-test==0.0.3a4
+pip install quick-pypi-test==0.0.3a6
 ```
 
 ## License
 This project follows the MIT license.
```

### Comparing `quick-pypi-test-0.0.3a4/pyproject.toml` & `quick-pypi-test-0.0.3a6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "quick-pypi-test"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3a4"  # Required
+version = "0.0.3a6"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "This is a quick-pypi-test package!"  # Optional
 
 # This is an optional longer description of your project that represents
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

### Comparing `quick-pypi-test-0.0.3a4/src/quick_pypi_test.egg-info/PKG-INFO` & `quick-pypi-test-0.0.3a6/src/quick_pypi_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.3a4
+Version: 0.0.3a6
 Summary: This is a quick-pypi-test package!
 Author-email: Donghua Chen <douglaschan@126.com>
 License: MIT License
         
         Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,12 +47,12 @@
 
 # A quick-pypi-test package!
 
 This is a quick-pypi-test package!
 
 ## Installation
 ```pip
-pip install quick-pypi-test==0.0.3a4
+pip install quick-pypi-test==0.0.3a6
 ```
 
 ## License
 This project follows the MIT license.
```

