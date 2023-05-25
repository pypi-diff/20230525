# Comparing `tmp/quick-pypi-0.0.3a3.tar.gz` & `tmp/quick-pypi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-0.0.3a3.tar", last modified: Thu May 25 01:43:20 2023, max compression
+gzip compressed data, was "quick-pypi-0.0.4.tar", last modified: Thu May 25 01:54:35 2023, max compression
```

## Comparing `quick-pypi-0.0.3a3.tar` & `quick-pypi-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.3a3/LICENSE
--rw-rw-rw-   0        0        0      252 2022-01-17 11:10:09.000000 quick-pypi-0.0.3a3/MANIFEST.in
--rw-rw-rw-   0        0        0     4916 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/PKG-INFO
--rw-rw-rw-   0        0        0     3709 2023-05-24 10:36:19.000000 quick-pypi-0.0.3a3/README.md
--rw-rw-rw-   0        0        0       81 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/setup.cfg
--rw-rw-rw-   0        0        0     8548 2023-05-25 01:42:59.000000 quick-pypi-0.0.3a3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.777375 quick-pypi-0.0.3a3/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.823202 quick-pypi-0.0.3a3/src/quick_pypi/
--rw-rw-rw-   0        0        0       21 2022-01-28 20:43:51.000000 quick-pypi-0.0.3a3/src/quick_pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.867552 quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/
--rw-rw-rw-   0        0        0      208 2022-01-28 18:44:01.000000 quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0     6124 2022-01-28 19:04:43.000000 quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/deploy.cpython-36.pyc
--rw-rw-rw-   0        0        0     9920 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/deploy.py
--rw-rw-rw-   0        0        0    10376 2023-05-24 14:06:10.000000 quick-pypi-0.0.3a3/src/quick_pypi/deploy_toml.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.967944 quick-pypi-0.0.3a3/src/quick_pypi/template/
--rw-rw-rw-   0        0        0     1106 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/LICENSE
--rw-rw-rw-   0        0        0      292 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2022-01-28 19:03:49.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/README.md
--rw-rw-rw-   0        0        0     6548 2023-05-25 01:40:08.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject.toml
--rw-rw-rw-   0        0        0     6558 2023-05-25 01:40:08.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_no_urls.toml
--rw-rw-rw-   0        0        0     6568 2023-05-25 01:40:08.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_only_project_url.toml
--rw-rw-rw-   0        0        0      205 2022-01-28 16:39:43.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup.cfg
--rw-rw-rw-   0        0        0     8606 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup.py
--rw-rw-rw-   0        0        0     8591 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup_no_urls.py
--rw-rw-rw-   0        0        0     8590 2023-05-24 10:26:00.000000 quick-pypi-0.0.3a3/src/quick_pypi/template/setup_with_only_project_url.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:43:20.866546 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/
--rw-rw-rw-   0        0        0     4916 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-25 01:43:20.000000 quick-pypi-0.0.3a3/src/quick_pypi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 01:54:35.167341 quick-pypi-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      252 2022-01-17 11:10:09.000000 quick-pypi-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5008 2023-05-25 01:54:35.167341 quick-pypi-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3800 2023-05-25 01:54:17.000000 quick-pypi-0.0.4/README.md
+-rw-rw-rw-   0        0        0       81 2023-05-25 01:54:35.172341 quick-pypi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     8546 2023-05-25 01:54:17.000000 quick-pypi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:54:35.083370 quick-pypi-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 01:54:35.107548 quick-pypi-0.0.4/src/quick_pypi/
+-rw-rw-rw-   0        0        0       21 2022-01-28 20:43:51.000000 quick-pypi-0.0.4/src/quick_pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:54:35.145961 quick-pypi-0.0.4/src/quick_pypi/__pycache__/
+-rw-rw-rw-   0        0        0      208 2022-01-28 18:44:01.000000 quick-pypi-0.0.4/src/quick_pypi/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0     6124 2022-01-28 19:04:43.000000 quick-pypi-0.0.4/src/quick_pypi/__pycache__/deploy.cpython-36.pyc
+-rw-rw-rw-   0        0        0     9920 2023-05-24 10:26:00.000000 quick-pypi-0.0.4/src/quick_pypi/deploy.py
+-rw-rw-rw-   0        0        0    10376 2023-05-24 14:06:10.000000 quick-pypi-0.0.4/src/quick_pypi/deploy_toml.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:54:35.165343 quick-pypi-0.0.4/src/quick_pypi/template/
+-rw-rw-rw-   0        0        0     1106 2023-05-24 10:26:00.000000 quick-pypi-0.0.4/src/quick_pypi/template/LICENSE
+-rw-rw-rw-   0        0        0      292 2023-05-24 10:26:00.000000 quick-pypi-0.0.4/src/quick_pypi/template/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2022-01-28 19:03:49.000000 quick-pypi-0.0.4/src/quick_pypi/template/README.md
+-rw-rw-rw-   0        0        0     6548 2023-05-25 01:40:08.000000 quick-pypi-0.0.4/src/quick_pypi/template/pyproject.toml
+-rw-rw-rw-   0        0        0     6558 2023-05-25 01:40:08.000000 quick-pypi-0.0.4/src/quick_pypi/template/pyproject_no_urls.toml
+-rw-rw-rw-   0        0        0     6568 2023-05-25 01:40:08.000000 quick-pypi-0.0.4/src/quick_pypi/template/pyproject_only_project_url.toml
+-rw-rw-rw-   0        0        0      205 2022-01-28 16:39:43.000000 quick-pypi-0.0.4/src/quick_pypi/template/setup.cfg
+-rw-rw-rw-   0        0        0     8606 2023-05-24 10:26:00.000000 quick-pypi-0.0.4/src/quick_pypi/template/setup.py
+-rw-rw-rw-   0        0        0     8591 2023-05-24 10:26:00.000000 quick-pypi-0.0.4/src/quick_pypi/template/setup_no_urls.py
+-rw-rw-rw-   0        0        0     8590 2023-05-24 10:26:00.000000 quick-pypi-0.0.4/src/quick_pypi/template/setup_with_only_project_url.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:54:35.141997 quick-pypi-0.0.4/src/quick_pypi.egg-info/
+-rw-rw-rw-   0        0        0     5008 2023-05-25 01:54:35.000000 quick-pypi-0.0.4/src/quick_pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-05-25 01:54:35.000000 quick-pypi-0.0.4/src/quick_pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:54:35.000000 quick-pypi-0.0.4/src/quick_pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-25 01:54:35.000000 quick-pypi-0.0.4/src/quick_pypi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 01:54:35.000000 quick-pypi-0.0.4/src/quick_pypi.egg-info/top_level.txt
```

### Comparing `quick-pypi-0.0.3a3/LICENSE` & `quick-pypi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/PKG-INFO` & `quick-pypi-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi
-Version: 0.0.3a3
+Version: 0.0.4
 Summary: The simplest and quickest way to build and publish a PyPI package
 Home-page: https://github.com/dhchenx/quick-pypi
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-pypi/issues
 Project-URL: Source, https://github.com/dhchenx/quick-pypi
@@ -35,15 +35,15 @@
 ```
 
 ## Minimum Example
 
 Before you start, you need to have several things:
 - Determine a unique PyPI package name, easy to remember, like 'quick-pypi-test';
 - Have a PyPI account, then export your upload token to a txt file in your computer;
-- Use PyCharm IDE to develop your own package. We support Jupyter Notebook now!
+- Use PyCharm IDE or VSCode to develop your own package. We support Jupyter Notebook now!
 
 Step 1: Prepare your project tree like:
 ```
 Project Root
  -- src
    -- your_package_name
      -- __init__.py
@@ -75,14 +75,15 @@
 
 ## Complicated Example settings for advanced users
 
 A real example is here:
 
 ```python
 from quick_pypi.deploy import *
+# or you can use: `from quick_pypi.deploy_toml import *`
 
 auto_deploy(
     cwd=os.path.dirname(os.path.realpath(__file__)),
     name="pyrefworks",
     long_name="A Python Toolkit for RefWorks Data Analysis",
     description="Converting RefWorks files into a CSV table file",
     long_description="This is a project to convert RefWork files to a CSV file",
@@ -96,15 +97,16 @@
     author_email="xxx@xxx.com",
     requires="quick-csv",
     license='MIT',
     license_filename='LICENSE',
     keywords="refworks, csv file",
     github_username="dhchenx",
     max_number_micro=20, # major.minor.micro
-    max_number_minor=20 # version maximum numbers in each part, e.g. 0.0.20 --> 0.1.0; 0.20.20 --> 1.0.0
+    max_number_minor=20, # version maximum numbers in each part, e.g. 0.0.20 --> 0.1.0; 0.20.20 --> 1.0.0
+    # only_build=True
 )
 ```
 Here you can provide more information about your package, like setting your author's name, email, license, short or long names and descriptions, etc. 
 
 ### Deploy to local computer without upload
 
 ```python
@@ -118,14 +120,15 @@
     version="0.0.1a0", # fixed version number, wont change
    # project_url="http://github.com/dhchenx/quick-pypi-test",
    #  author_name="Donghua Chen",
     # author_email="douglaschan@126.com",
     # requires="jieba;quick-crawler",
     # license='MIT',
     # license_filename='LICENSE'
+
 )
 ```
 This will generate a series of actual package files (e.g. README.md, LICENSE,setup.py, etc. ).
 
 Then, you can manually build the package through twine in the directory of `dist1`. 
 
 An example using our toolkit to deploy in the PyPI platform is demonstrated [here](https://pypi.org/project/pyrefworks/).
```

### Comparing `quick-pypi-0.0.3a3/README.md` & `quick-pypi-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ```
 
 ## Minimum Example
 
 Before you start, you need to have several things:
 - Determine a unique PyPI package name, easy to remember, like 'quick-pypi-test';
 - Have a PyPI account, then export your upload token to a txt file in your computer;
-- Use PyCharm IDE to develop your own package. We support Jupyter Notebook now!
+- Use PyCharm IDE or VSCode to develop your own package. We support Jupyter Notebook now!
 
 Step 1: Prepare your project tree like:
 ```
 Project Root
  -- src
    -- your_package_name
      -- __init__.py
@@ -48,14 +48,15 @@
 
 ## Complicated Example settings for advanced users
 
 A real example is here:
 
 ```python
 from quick_pypi.deploy import *
+# or you can use: `from quick_pypi.deploy_toml import *`
 
 auto_deploy(
     cwd=os.path.dirname(os.path.realpath(__file__)),
     name="pyrefworks",
     long_name="A Python Toolkit for RefWorks Data Analysis",
     description="Converting RefWorks files into a CSV table file",
     long_description="This is a project to convert RefWork files to a CSV file",
@@ -69,15 +70,16 @@
     author_email="xxx@xxx.com",
     requires="quick-csv",
     license='MIT',
     license_filename='LICENSE',
     keywords="refworks, csv file",
     github_username="dhchenx",
     max_number_micro=20, # major.minor.micro
-    max_number_minor=20 # version maximum numbers in each part, e.g. 0.0.20 --> 0.1.0; 0.20.20 --> 1.0.0
+    max_number_minor=20, # version maximum numbers in each part, e.g. 0.0.20 --> 0.1.0; 0.20.20 --> 1.0.0
+    # only_build=True
 )
 ```
 Here you can provide more information about your package, like setting your author's name, email, license, short or long names and descriptions, etc. 
 
 ### Deploy to local computer without upload
 
 ```python
@@ -91,14 +93,15 @@
     version="0.0.1a0", # fixed version number, wont change
    # project_url="http://github.com/dhchenx/quick-pypi-test",
    #  author_name="Donghua Chen",
     # author_email="douglaschan@126.com",
     # requires="jieba;quick-crawler",
     # license='MIT',
     # license_filename='LICENSE'
+
 )
 ```
 This will generate a series of actual package files (e.g. README.md, LICENSE,setup.py, etc. ).
 
 Then, you can manually build the package through twine in the directory of `dist1`. 
 
 An example using our toolkit to deploy in the PyPI platform is demonstrated [here](https://pypi.org/project/pyrefworks/).
```

### Comparing `quick-pypi-0.0.3a3/setup.py` & `quick-pypi-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3a3',  # Required
+    version='0.0.4',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='The simplest and quickest way to build and publish a PyPI package',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/__pycache__/deploy.cpython-36.pyc` & `quick-pypi-0.0.4/src/quick_pypi/__pycache__/deploy.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/deploy.py` & `quick-pypi-0.0.4/src/quick_pypi/deploy.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/deploy_toml.py` & `quick-pypi-0.0.4/src/quick_pypi/deploy_toml.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/LICENSE` & `quick-pypi-0.0.4/src/quick_pypi/template/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject.toml` & `quick-pypi-0.0.4/src/quick_pypi/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_no_urls.toml` & `quick-pypi-0.0.4/src/quick_pypi/template/pyproject_no_urls.toml`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/pyproject_only_project_url.toml` & `quick-pypi-0.0.4/src/quick_pypi/template/pyproject_only_project_url.toml`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/setup.py` & `quick-pypi-0.0.4/src/quick_pypi/template/setup.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/setup_no_urls.py` & `quick-pypi-0.0.4/src/quick_pypi/template/setup_no_urls.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi/template/setup_with_only_project_url.py` & `quick-pypi-0.0.4/src/quick_pypi/template/setup_with_only_project_url.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi.egg-info/PKG-INFO` & `quick-pypi-0.0.4/src/quick_pypi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi
-Version: 0.0.3a3
+Version: 0.0.4
 Summary: The simplest and quickest way to build and publish a PyPI package
 Home-page: https://github.com/dhchenx/quick-pypi
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-pypi/issues
 Project-URL: Source, https://github.com/dhchenx/quick-pypi
@@ -35,15 +35,15 @@
 ```
 
 ## Minimum Example
 
 Before you start, you need to have several things:
 - Determine a unique PyPI package name, easy to remember, like 'quick-pypi-test';
 - Have a PyPI account, then export your upload token to a txt file in your computer;
-- Use PyCharm IDE to develop your own package. We support Jupyter Notebook now!
+- Use PyCharm IDE or VSCode to develop your own package. We support Jupyter Notebook now!
 
 Step 1: Prepare your project tree like:
 ```
 Project Root
  -- src
    -- your_package_name
      -- __init__.py
@@ -75,14 +75,15 @@
 
 ## Complicated Example settings for advanced users
 
 A real example is here:
 
 ```python
 from quick_pypi.deploy import *
+# or you can use: `from quick_pypi.deploy_toml import *`
 
 auto_deploy(
     cwd=os.path.dirname(os.path.realpath(__file__)),
     name="pyrefworks",
     long_name="A Python Toolkit for RefWorks Data Analysis",
     description="Converting RefWorks files into a CSV table file",
     long_description="This is a project to convert RefWork files to a CSV file",
@@ -96,15 +97,16 @@
     author_email="xxx@xxx.com",
     requires="quick-csv",
     license='MIT',
     license_filename='LICENSE',
     keywords="refworks, csv file",
     github_username="dhchenx",
     max_number_micro=20, # major.minor.micro
-    max_number_minor=20 # version maximum numbers in each part, e.g. 0.0.20 --> 0.1.0; 0.20.20 --> 1.0.0
+    max_number_minor=20, # version maximum numbers in each part, e.g. 0.0.20 --> 0.1.0; 0.20.20 --> 1.0.0
+    # only_build=True
 )
 ```
 Here you can provide more information about your package, like setting your author's name, email, license, short or long names and descriptions, etc. 
 
 ### Deploy to local computer without upload
 
 ```python
@@ -118,14 +120,15 @@
     version="0.0.1a0", # fixed version number, wont change
    # project_url="http://github.com/dhchenx/quick-pypi-test",
    #  author_name="Donghua Chen",
     # author_email="douglaschan@126.com",
     # requires="jieba;quick-crawler",
     # license='MIT',
     # license_filename='LICENSE'
+
 )
 ```
 This will generate a series of actual package files (e.g. README.md, LICENSE,setup.py, etc. ).
 
 Then, you can manually build the package through twine in the directory of `dist1`. 
 
 An example using our toolkit to deploy in the PyPI platform is demonstrated [here](https://pypi.org/project/pyrefworks/).
```

### Comparing `quick-pypi-0.0.3a3/src/quick_pypi.egg-info/SOURCES.txt` & `quick-pypi-0.0.4/src/quick_pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

