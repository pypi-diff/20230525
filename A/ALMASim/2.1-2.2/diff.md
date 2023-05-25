# Comparing `tmp/ALMASim-2.1.tar.gz` & `tmp/ALMASim-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALMASim-2.1.tar", last modified: Thu May 25 13:50:50 2023, max compression
+gzip compressed data, was "ALMASim-2.2.tar", last modified: Thu May 25 14:02:00 2023, max compression
```

## Comparing `ALMASim-2.1.tar` & `ALMASim-2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.858318 ALMASim-2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.854318 ALMASim-2.1/ALMASim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 13:50:50.000000 ALMASim-2.1/ALMASim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-25 13:50:50.000000 ALMASim-2.1/ALMASim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:50:50.000000 ALMASim-2.1/ALMASim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 13:50:50.000000 ALMASim-2.1/ALMASim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 13:50:50.000000 ALMASim-2.1/ALMASim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 13:49:35.000000 ALMASim-2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 13:49:35.000000 ALMASim-2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 13:50:50.858318 ALMASim-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-25 13:49:35.000000 ALMASim-2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.850318 ALMASim-2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.854318 ALMASim-2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 13:49:35.000000 ALMASim-2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-25 13:49:35.000000 ALMASim-2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:50:50.858318 ALMASim-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 13:49:35.000000 ALMASim-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.854318 ALMASim-2.1/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.850318 ALMASim-2.1/submodules/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.854318 ALMASim-2.1/submodules/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.854318 ALMASim-2.1/submodules/build/lib/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/build/lib/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/build/lib/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/build/lib/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/build/lib/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/build/lib/illustris_python/sublink.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/build/lib/illustris_python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.858318 ALMASim-2.1/submodules/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/sublink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.858318 ALMASim-2.1/submodules/illustris_python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/tests/groupcat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/tests/sublink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/illustris_python/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 13:49:48.000000 ALMASim-2.1/submodules/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:50:50.858318 ALMASim-2.1/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 13:49:35.000000 ALMASim-2.1/utility/generate_gaussian_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 13:49:35.000000 ALMASim-2.1/utility/split_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 13:49:35.000000 ALMASim-2.1/utility/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.119631 ALMASim-2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/ALMASim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 14:02:00.000000 ALMASim-2.2/ALMASim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-25 14:02:00.000000 ALMASim-2.2/ALMASim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:02:00.000000 ALMASim-2.2/ALMASim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 14:02:00.000000 ALMASim-2.2/ALMASim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 14:02:00.000000 ALMASim-2.2/ALMASim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 14:00:42.000000 ALMASim-2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 14:00:42.000000 ALMASim-2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 14:02:00.119631 ALMASim-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-25 14:00:42.000000 ALMASim-2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 14:00:42.000000 ALMASim-2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-25 14:00:42.000000 ALMASim-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:02:00.119631 ALMASim-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 14:00:42.000000 ALMASim-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/submodules/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/submodules/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.115631 ALMASim-2.2/submodules/build/lib/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/build/lib/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/build/lib/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/build/lib/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/build/lib/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/build/lib/illustris_python/sublink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/build/lib/illustris_python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.119631 ALMASim-2.2/submodules/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/sublink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.119631 ALMASim-2.2/submodules/illustris_python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/tests/groupcat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/tests/sublink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/illustris_python/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 14:00:55.000000 ALMASim-2.2/submodules/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:02:00.119631 ALMASim-2.2/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 14:00:42.000000 ALMASim-2.2/utility/generate_gaussian_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 14:00:42.000000 ALMASim-2.2/utility/split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 14:00:42.000000 ALMASim-2.2/utility/test.py
```

### Comparing `ALMASim-2.1/ALMASim.egg-info/PKG-INFO` & `ALMASim-2.2/ALMASim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALMASim
-Version: 2.1
+Version: 2.2
 Summary: Simulation code for ALMA observations of both high redshift and local galaxies.
 Author-email: "M. Delli Veneri" <micheledelliveneri@gmail.com>, "L. Tychoniec" <lukasz.tychoniec@eso.org>, "F. Guglielmetti" <fgugliel@eso.org>, "I. Baronchelli" <ivano.baronchelli@inaf.it>, "E. Villard" <evillard@eso.org>, "G. Longo" <giuseppe.longo@unina.it>
 Project-URL: Homepage, https://github.com/MicheleDelliVeneri/ALMASim
 Project-URL: Documentation, https://almasim.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MicheleDelliVeneri/ALMASim/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ALMASim-2.1/ALMASim.egg-info/SOURCES.txt` & `ALMASim-2.2/ALMASim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/LICENSE.md` & `ALMASim-2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/PKG-INFO` & `ALMASim-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALMASim
-Version: 2.1
+Version: 2.2
 Summary: Simulation code for ALMA observations of both high redshift and local galaxies.
 Author-email: "M. Delli Veneri" <micheledelliveneri@gmail.com>, "L. Tychoniec" <lukasz.tychoniec@eso.org>, "F. Guglielmetti" <fgugliel@eso.org>, "I. Baronchelli" <ivano.baronchelli@inaf.it>, "E. Villard" <evillard@eso.org>, "G. Longo" <giuseppe.longo@unina.it>
 Project-URL: Homepage, https://github.com/MicheleDelliVeneri/ALMASim
 Project-URL: Documentation, https://almasim.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MicheleDelliVeneri/ALMASim/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ALMASim-2.1/README.rst` & `ALMASim-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/docs/source/conf.py` & `ALMASim-2.2/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ALMASim"
 copyright = "2023, Michele Delli Veneri"
 author = "Michele Delli Veneri"
 
 # The full version, including alpha/beta/rc tags
-release = "2.1"
+release = "2.2"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `ALMASim-2.1/pyproject.toml` & `ALMASim-2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ALMASim"
-version = "2.1"
+version = "2.2"
 authors = [
     {name="M. Delli Veneri", email="micheledelliveneri@gmail.com"},
     {name="L. Tychoniec", email="lukasz.tychoniec@eso.org"},
     {name="F. Guglielmetti", email="fgugliel@eso.org"},
     {name="I. Baronchelli", email="ivano.baronchelli@inaf.it"},
     {name="E. Villard", email="evillard@eso.org"},
     {name="G. Longo", email="giuseppe.longo@unina.it"}
```

### Comparing `ALMASim-2.1/setup.py` & `ALMASim-2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='ALMASim',
-    version='2.1',
+    version='2.2',
     description='ALMA Simulator for synthetic observations of galaxies. To know more about the code, please visit https://github.com/MicheleDelliVeneri/ALMASim',
     long_description="fobar",
     packages=find_namespace_packages(),
     install_requires=["numpy", "h5py", "six", 
                       "astropy==5.1.1", "scipy", "matplotlib", "pandas", "tqdm",
                       "h5py", "hdecompose", "spectral-cube", "astromartini", 
                       "dask", "dask[distributed]", "natsort", "distributed", "casatools==6.5.5.21",
```

### Comparing `ALMASim-2.1/submodules/build/lib/illustris_python/groupcat.py` & `ALMASim-2.2/submodules/build/lib/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/build/lib/illustris_python/lhalotree.py` & `ALMASim-2.2/submodules/build/lib/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/build/lib/illustris_python/snapshot.py` & `ALMASim-2.2/submodules/build/lib/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/build/lib/illustris_python/sublink.py` & `ALMASim-2.2/submodules/build/lib/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/build/lib/illustris_python/util.py` & `ALMASim-2.2/submodules/build/lib/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/groupcat.py` & `ALMASim-2.2/submodules/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/lhalotree.py` & `ALMASim-2.2/submodules/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/snapshot.py` & `ALMASim-2.2/submodules/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/sublink.py` & `ALMASim-2.2/submodules/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/tests/groupcat_test.py` & `ALMASim-2.2/submodules/illustris_python/tests/groupcat_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/tests/snapshot_test.py` & `ALMASim-2.2/submodules/illustris_python/tests/snapshot_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/tests/sublink_test.py` & `ALMASim-2.2/submodules/illustris_python/tests/sublink_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/submodules/illustris_python/util.py` & `ALMASim-2.2/submodules/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/utility/generate_gaussian_params.py` & `ALMASim-2.2/utility/generate_gaussian_params.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.1/utility/split_data.py` & `ALMASim-2.2/utility/split_data.py`

 * *Files identical despite different names*

