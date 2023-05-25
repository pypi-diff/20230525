# Comparing `tmp/strongtyping-pyoverload-0.3.0.tar.gz` & `tmp/strongtyping-pyoverload-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strongtyping-pyoverload-0.3.0.tar", last modified: Sat Feb 12 10:16:48 2022, max compression
+gzip compressed data, was "strongtyping-pyoverload-0.3.1.tar", last modified: Thu May 25 19:15:01 2023, max compression
```

## Comparing `strongtyping-pyoverload-0.3.0.tar` & `strongtyping-pyoverload-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 10:16:48.035303 strongtyping-pyoverload-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-02-12 10:16:48.031304 strongtyping-pyoverload-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-12 10:16:48.035303 strongtyping-pyoverload-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 10:16:48.031304 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9457 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload/class_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 10:16:48.031304 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-02-12 10:16:47.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-02-12 10:16:47.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 10:16:47.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-12 10:16:47.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-02-12 10:16:47.000000 strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 10:16:48.031304 strongtyping-pyoverload-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/tests/module_based_test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5537 2022-02-12 10:16:38.000000 strongtyping-pyoverload-0.3.0/tests/test_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:15:01.809256 strongtyping-pyoverload-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-25 19:15:01.809256 strongtyping-pyoverload-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:15:01.809256 strongtyping-pyoverload-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:15:01.809256 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload/class_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:15:01.809256 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-25 19:15:01.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-25 19:15:01.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:15:01.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 19:15:01.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 19:15:01.000000 strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:15:01.809256 strongtyping-pyoverload-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/tests/module_based_test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-25 19:14:51.000000 strongtyping-pyoverload-0.3.1/tests/test_override.py
```

### Comparing `strongtyping-pyoverload-0.3.0/PKG-INFO` & `strongtyping-pyoverload-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: strongtyping-pyoverload
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Runtime method overload decorator.
 Home-page: https://strongtyping-pyoverload.readthedocs.io/en/latest/
 Author: FelixTheC
 Author-email: fberndt87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # strongtyping-pyoverload
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Python application](https://github.com/FelixTheC/py-overload/workflows/Python%20application/badge.svg)
 ![Python tox](https://github.com/FelixTheC/py-overload/workflows/Python%20tox/badge.svg)
 ![image](https://codecov.io/gh/FelixTheC/py-overload/graph/badge.svg)
+![](https://img.shields.io/pypi/dm/pyoverload)
 
 ## A Runtime method overload decorator which add overloading capacity similar to C++
 - there is a `override` decorator from `typing` which works only for static type checking
 - this decorator works on `runtime`
 
 
 ## Documentation can be found here
```

### Comparing `strongtyping-pyoverload-0.3.0/README.md` & `strongtyping-pyoverload-0.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # strongtyping-pyoverload
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Python application](https://github.com/FelixTheC/py-overload/workflows/Python%20application/badge.svg)
 ![Python tox](https://github.com/FelixTheC/py-overload/workflows/Python%20tox/badge.svg)
 ![image](https://codecov.io/gh/FelixTheC/py-overload/graph/badge.svg)
+![](https://img.shields.io/pypi/dm/pyoverload)
 
 ## A Runtime method overload decorator which add overloading capacity similar to C++
 - there is a `override` decorator from `typing` which works only for static type checking
 - this decorator works on `runtime`
 
 
 ## Documentation can be found here
```

### Comparing `strongtyping-pyoverload-0.3.0/setup.py` & `strongtyping-pyoverload-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 packages = find_packages(exclude=["test_*", "*.tests"])
 
 setup(
     name="strongtyping-pyoverload",
-    version="0.3.0",
+    version="0.3.1",
     description="A Runtime method overload decorator.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://strongtyping-pyoverload.readthedocs.io/en/latest/",
     author="FelixTheC",
     author_email="fberndt87@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    install_requires=["strongtyping"],
+    install_requires=["strongtyping>=3.9,>=3.10,<=3.11"],
     dependencies="",
     packages=packages,
     python_requires=">=3.9",
     include_package_data=True,
 )
```

### Comparing `strongtyping-pyoverload-0.3.0/strongtyping_pyoverload/class_tools.py` & `strongtyping-pyoverload-0.3.1/strongtyping_pyoverload/class_tools.py`

 * *Files identical despite different names*

### Comparing `strongtyping-pyoverload-0.3.0/strongtyping_pyoverload.egg-info/PKG-INFO` & `strongtyping-pyoverload-0.3.1/strongtyping_pyoverload.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: strongtyping-pyoverload
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Runtime method overload decorator.
 Home-page: https://strongtyping-pyoverload.readthedocs.io/en/latest/
 Author: FelixTheC
 Author-email: fberndt87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # strongtyping-pyoverload
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Python application](https://github.com/FelixTheC/py-overload/workflows/Python%20application/badge.svg)
 ![Python tox](https://github.com/FelixTheC/py-overload/workflows/Python%20tox/badge.svg)
 ![image](https://codecov.io/gh/FelixTheC/py-overload/graph/badge.svg)
+![](https://img.shields.io/pypi/dm/pyoverload)
 
 ## A Runtime method overload decorator which add overloading capacity similar to C++
 - there is a `override` decorator from `typing` which works only for static type checking
 - this decorator works on `runtime`
 
 
 ## Documentation can be found here
```

### Comparing `strongtyping-pyoverload-0.3.0/tests/test_override.py` & `strongtyping-pyoverload-0.3.1/tests/test_override.py`

 * *Files identical despite different names*

