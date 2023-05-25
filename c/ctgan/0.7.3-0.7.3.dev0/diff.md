# Comparing `tmp/ctgan-0.7.3.tar.gz` & `tmp/ctgan-0.7.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctgan-0.7.3.tar", last modified: Thu May 25 18:58:34 2023, max compression
+gzip compressed data, was "ctgan-0.7.3.dev0.tar", last modified: Thu May 25 00:07:21 2023, max compression
```

## Comparing `ctgan-0.7.3.tar` & `ctgan-0.7.3.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.543942 ctgan-0.7.3/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-01-20 22:22:05.000000 ctgan-0.7.3/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8300 2022-08-17 21:26:32.000000 ctgan-0.7.3/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9569 2023-05-25 18:58:31.000000 ctgan-0.7.3/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2023-01-20 22:22:05.000000 ctgan-0.7.3/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      265 2022-08-17 21:26:32.000000 ctgan-0.7.3/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17776 2023-05-25 18:58:34.544047 ctgan-0.7.3/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7298 2023-01-20 22:22:05.000000 ctgan-0.7.3/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.540634 ctgan-0.7.3/ctgan/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      314 2023-05-25 18:58:32.000000 ctgan-0.7.3/ctgan/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4415 2022-10-07 17:29:33.000000 ctgan-0.7.3/ctgan/__main__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2457 2022-08-17 21:26:32.000000 ctgan-0.7.3/ctgan/data.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6203 2022-08-17 21:26:32.000000 ctgan-0.7.3/ctgan/data_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10417 2023-01-20 22:22:05.000000 ctgan-0.7.3/ctgan/data_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2023-05-09 17:51:59.000000 ctgan-0.7.3/ctgan/demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.542270 ctgan-0.7.3/ctgan/synthesizers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      258 2022-10-07 17:29:33.000000 ctgan-0.7.3/ctgan/synthesizers/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5287 2023-02-25 01:28:14.000000 ctgan-0.7.3/ctgan/synthesizers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18827 2023-05-25 18:58:31.000000 ctgan-0.7.3/ctgan/synthesizers/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6953 2022-10-07 17:29:33.000000 ctgan-0.7.3/ctgan/synthesizers/tvae.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.541722 ctgan-0.7.3/ctgan.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17776 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      922 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/entry_points.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1098 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-05-25 18:58:34.000000 ctgan-0.7.3/ctgan.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1297 2023-05-25 18:58:34.544488 ctgan-0.7.3/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3415 2023-05-25 18:58:32.000000 ctgan-0.7.3/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.538243 ctgan-0.7.3/tests/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.542557 ctgan-0.7.3/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2023-05-10 22:06:03.000000 ctgan-0.7.3/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.542981 ctgan-0.7.3/tests/integration/synthesizer/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-05-10 22:06:03.000000 ctgan-0.7.3/tests/integration/synthesizer/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9212 2023-05-09 17:51:59.000000 ctgan-0.7.3/tests/integration/synthesizer/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4316 2023-05-09 17:51:59.000000 ctgan-0.7.3/tests/integration/synthesizer/test_tvae.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1296 2022-08-17 21:26:32.000000 ctgan-0.7.3/tests/integration/test_data_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.543243 ctgan-0.7.3/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       27 2023-05-09 00:17:46.000000 ctgan-0.7.3/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 18:58:34.543821 ctgan-0.7.3/tests/unit/synthesizer/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2022-10-07 17:29:33.000000 ctgan-0.7.3/tests/unit/synthesizer/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3593 2022-08-17 21:26:32.000000 ctgan-0.7.3/tests/unit/synthesizer/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11121 2022-10-07 17:29:33.000000 ctgan-0.7.3/tests/unit/synthesizer/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3367 2022-10-07 17:29:33.000000 ctgan-0.7.3/tests/unit/synthesizer/test_tvae.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20075 2022-08-17 21:26:32.000000 ctgan-0.7.3/tests/unit/test_data_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.015591 ctgan-0.7.3.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8300 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9261 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      265 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17473 2023-05-25 00:07:21.015692 ctgan-0.7.3.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7298 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.010539 ctgan-0.7.3.dev0/ctgan/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      319 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/ctgan/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4415 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/ctgan/__main__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2457 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/ctgan/data.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6203 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/ctgan/data_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10417 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/ctgan/data_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2023-05-09 17:51:59.000000 ctgan-0.7.3.dev0/ctgan/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.012491 ctgan-0.7.3.dev0/ctgan/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      258 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5287 2023-02-25 01:28:14.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18827 2023-05-24 23:35:47.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6953 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/tvae.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.011685 ctgan-0.7.3.dev0/ctgan.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17473 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      922 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/entry_points.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1098 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1302 2023-05-25 00:07:21.016137 ctgan-0.7.3.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3420 2023-05-24 23:35:47.000000 ctgan-0.7.3.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.007591 ctgan-0.7.3.dev0/tests/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.012985 ctgan-0.7.3.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.013720 ctgan-0.7.3.dev0/tests/integration/synthesizer/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/tests/integration/synthesizer/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9212 2023-05-09 17:51:59.000000 ctgan-0.7.3.dev0/tests/integration/synthesizer/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4316 2023-05-09 17:51:59.000000 ctgan-0.7.3.dev0/tests/integration/synthesizer/test_tvae.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1296 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/tests/integration/test_data_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.014228 ctgan-0.7.3.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       27 2023-05-09 00:17:46.000000 ctgan-0.7.3.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.015403 ctgan-0.7.3.dev0/tests/unit/synthesizer/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3593 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11121 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3367 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/test_tvae.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20075 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/tests/unit/test_data_transformer.py
```

### Comparing `ctgan-0.7.3/CONTRIBUTING.rst` & `ctgan-0.7.3.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/HISTORY.md` & `ctgan-0.7.3.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 # History
 
-## v0.7.3 - 2023-05-25
-
-This release adds support for Torch 2.0!
-
-### Bugs Fixed
-
-* Torch 2.0 fails with cuda=False - Issue [#288](https://github.com/sdv-dev/CTGAN/issues/288) by @amontanez24
-
-### Maintenance
-
-* Upgrade to torch 2.0 - Issue [#280](https://github.com/sdv-dev/CTGAN/issues/280) by @frances-h
-
 ## v0.7.2 - 2023-05-09
 
 This release adds support for Pandas 2.0! It also fixes a bug in the `load_demo` function.
 
 ### Bugs Fixed
 
 * load_demo raises urllib.error.HTTPError: HTTP Error 403: Forbidden - Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by @amontanez24
```

### Comparing `ctgan-0.7.3/LICENSE` & `ctgan-0.7.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/PKG-INFO` & `ctgan-0.7.3.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctgan
-Version: 0.7.3
+Version: 0.7.3.dev0
 Summary: Create tabular synthetic data using a conditional GAN
 Home-page: https://github.com/sdv-dev/CTGAN
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: ctgan CTGAN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -188,26 +188,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.7.3 - 2023-05-25
-
-This release adds support for Torch 2.0!
-
-### Bugs Fixed
-
-* Torch 2.0 fails with cuda=False - Issue [#288](https://github.com/sdv-dev/CTGAN/issues/288) by @amontanez24
-
-### Maintenance
-
-* Upgrade to torch 2.0 - Issue [#280](https://github.com/sdv-dev/CTGAN/issues/280) by @frances-h
-
 ## v0.7.2 - 2023-05-09
 
 This release adds support for Pandas 2.0! It also fixes a bug in the `load_demo` function.
 
 ### Bugs Fixed
 
 * load_demo raises urllib.error.HTTPError: HTTP Error 403: Forbidden - Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by @amontanez24
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctgan Version: 0.7.3 Summary: Create tabular
+Metadata-Version: 2.1 Name: ctgan Version: 0.7.3.dev0 Summary: Create tabular
 synthetic data using a conditional GAN Home-page: https://github.com/sdv-dev/
 CTGAN Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: ctgan CTGAN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: Free for
 non-commercial use Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -99,132 +99,128 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.7.3 - 2023-05-25 This release
-adds support for Torch 2.0! ### Bugs Fixed * Torch 2.0 fails with cuda=False -
-Issue [#288](https://github.com/sdv-dev/CTGAN/issues/288) by @amontanez24 ###
-Maintenance * Upgrade to torch 2.0 - Issue [#280](https://github.com/sdv-dev/
-CTGAN/issues/280) by @frances-h ## v0.7.2 - 2023-05-09 This release adds
-support for Pandas 2.0! It also fixes a bug in the `load_demo` function. ###
-Bugs Fixed * load_demo raises urllib.error.HTTPError: HTTP Error 403: Forbidden
-- Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by @amontanez24 ###
-Maintenance * Remove upper bound for pandas - Issue [#282](https://github.com/
-sdv-dev/CTGAN/issues/282) by @frances-h ## v0.7.1 - 2023-02-23 This release
-fixes a bug that prevented the `CTGAN` model from being saved after sampling.
-### Bugs Fixed * Cannot save CTGANSynthesizer after sampling (TypeError) -
-Issue [#270](https://github.com/sdv-dev/CTGAN/issues/270) by @pvk-developer ##
-v0.7.0 - 2023-01-20 This release adds support for python 3.10 and drops support
-for python 3.6. It also fixes a couple of the most common warnings that were
-surfacing. ### New Features * Support Python 3.10 and 3.11 - Issue [#259]
-(https://github.com/sdv-dev/CTGAN/issues/259) by @pvk-developer ### Bugs Fixed
-* Fix SettingWithCopyWarning (may be leading to a numerical calculation bug) -
-Issue [#215](https://github.com/sdv-dev/CTGAN/issues/215) by @amontanez24 *
-FutureWarning in data_transformer with pandas 1.5.0 - Issue [#246](https://
-github.com/sdv-dev/CTGAN/issues/246) by @amontanez24 ### Maintenance * CTGAN
-Package Maintenance Updates - Issue [#257](https://github.com/sdv-dev/CTGAN/
-issues/257) by @amontanez24 ## v0.6.0 - 2022-10-07 This release renames the
-models in CTGAN. `CTGANSynthesizer` is now called `CTGAN` and `TVAESynthesizer`
-is now called `TVAE`. ### New Features * Rename synthesizers - Issue [#243]
-(https://github.com/sdv-dev/CTGAN/issues/243) by @amontanez24 ## v0.5.2 - 2022-
-08-18 This release updates CTGAN to use the latest version of RDT. It also
-includes performance and robustness updates to the data transformer. ### Issues
-closed * Bump rdt version - Issue [#242](https://github.com/sdv-dev/CTGAN/
-issues/242) by @katxiao * Single thread data transform is slow for huge table -
-Issue [#151](https://github.com/sdv-dev/CTGAN/issues/151) by @mfhbree * Fix RDT
-api - Issue [#232](https://github.com/sdv-dev/CTGAN/issues/232) by @pvk-
-developer * Update macos to use latest version. - Issue [#237](https://
-github.com/sdv-dev/CTGAN/issues/237) by @pvk-developer * Update the RDT version
-to 1.0 - Issue [#224](https://github.com/sdv-dev/CTGAN/issues/224) by @pvk-
-developer * Update slack invite link. - Issue [#222](https://github.com/sdv-
-dev/CTGAN/issues/222) by @pvk-developer * robustness fix, when data have less
-rows than the default number of clâ¦ - Issue [#211](https://github.com/sdv-
-dev/CTGAN/issues/211) by @Deathn0t ## v0.5.1 - 2022-02-25 This release fixes a
-bug with the decoder instantiation, and also allows users to set a random state
-for the model fitting and sampling. ### Issues closed * Update self.decoder
-with correct variable name - Issue [#203](https://github.com/sdv-dev/CTGAN/
-issues/203) by @tejuafonja * Add random state - Issue [#204](https://
-github.com/sdv-dev/CTGAN/issues/204) by @katxiao ## v0.5.0 - 2021-11-18 This
-release adds support for Python 3.9 and updates dependencies to ensure
-compatibility with the rest of the SDV ecosystem, and upgrades to the latests
-[RDT](https://github.com/sdv-dev/RDT/releases/tag/v0.6.1) release. ### Issues
-closed * Add support for Python 3.9 - Issue [#177](https://github.com/sdv-dev/
-CTGAN/issues/177) by @pvk-developer * Add pip check to CI workflows - Issue
-[#174](https://github.com/sdv-dev/CTGAN/issues/174) by @pvk-developer * Typo in
-`CTGAN` code - Issue [#158](https://github.com/sdv-dev/CTGAN/issues/158) by
-@ori-katz100 and @fealho ## v0.4.3 - 2021-07-12 Dependency upgrades to ensure
-compatibility with the rest of the SDV ecosystem. ## v0.4.2 - 2021-04-27 In
-this release, the way in which the loss function of the TVAE model was computed
-has been fixed. In addition, the default value of the `discriminator_decay` has
-been changed to a more optimal value. Also some improvements to the tests were
-added. ### Issues closed * `TVAE`: loss function - Issue [#143](https://
-github.com/sdv-dev/CTGAN/issues/143) by @fealho and @DingfanChen * Set
-`discriminator_decay` to `1e-6` - Pull request [#145](https://github.com/sdv-
-dev/CTGAN/pull/145/) by @fealho * Adds unit tests - Pull requests [#140](https:
-//github.com/sdv-dev/CTGAN/pull/140) by @fealho ## v0.4.1 - 2021-03-30 This
-release exposes all the hyperparameters which the user may find useful for both
-`CTGAN` and `TVAE`. Also `TVAE` can now be fitted on datasets that are shorter
-than the batch size and drops the last batch only if the data size is not
-divisible by the batch size. ### Issues closed * `TVAE`: Adapt `batch_size` to
-data size - Issue [#135](https://github.com/sdv-dev/CTGAN/issues/135) by
-@fealho and @csala * `ValueError` from `validate_discre_columns` with
-`uniqueCombinationConstraint` - Issue [133](https://github.com/sdv-dev/CTGAN/
-issues/133) by @fealho and @MLjungg ## v0.4.0 - 2021-02-24 Maintenance relese
-to upgrade dependencies to ensure compatibility with the rest of the SDV
-libraries. Also add a validation on the CTGAN `condition_column` and
-`condition_value` inputs. ### Improvements * Validate condition_column and
-condition_value - Issue [#124](https://github.com/sdv-dev/CTGAN/issues/124) by
-@fealho ## v0.3.1 - 2021-01-27 ### Improvements * Check discrete_columns valid
-before fitting - [Issue #35](https://github.com/sdv-dev/CTGAN/issues/35) by
-@fealho ## Bugs fixed * ValueError: max() arg is an empty sequence - [Issue
-#115](https://github.com/sdv-dev/CTGAN/issues/115) by @fealho ## v0.3.0 - 2020-
-12-18 In this release we add a new TVAE model which was presented in the
-original CTGAN paper. It also exposes more hyperparameters and moves epochs and
-log_frequency from fit to the constructor. A new verbose argument has been
-added to optionally disable unnecessary printing, and a new hyperparameter
-called `discriminator_steps` has been added to CTGAN to control the number of
-optimization steps performed in the discriminator for each generator epoch. The
-code has also been reorganized and cleaned up for better readability and
-interpretability. Special thanks to @Baukebrenninkmeijer @fealho @leix28 @csala
-for the contributions! ### Improvements * Add TVAE - [Issue #111](https://
-github.com/sdv-dev/CTGAN/issues/111) by @fealho * Move `log_frequency` to
-`__init__` - [Issue #102](https://github.com/sdv-dev/CTGAN/issues/102) by
-@fealho * Add discriminator steps hyperparameter - [Issue #101](https://
-github.com/sdv-dev/CTGAN/issues/101) by @Baukebrenninkmeijer * Code cleanup /
-Expose hyperparameters - [Issue #59](https://github.com/sdv-dev/CTGAN/issues/
-59) by @fealho and @leix28 * Publish to conda repo - [Issue #54](https://
-github.com/sdv-dev/CTGAN/issues/54) by @fealho ### Bugs fixed * Fixed NaN !=
-NaN counting bug. - [Issue #100](https://github.com/sdv-dev/CTGAN/issues/100)
-by @fealho * Update dependencies and testing - [Issue #90](https://github.com/
-sdv-dev/CTGAN/issues/90) by @csala ## v0.2.2 - 2020-11-13 In this release we
-introduce several minor improvements to make CTGAN more versatile and propertly
-support new types of data, such as categorical NaN values, as well as
-conditional sampling and features to save and load models. Additionally, the
-dependency ranges and python versions have been updated to support up to date
-runtimes. Many thanks @fealho @leix28 @csala @oregonpillow and @lurosenb for
-working on making this release possible! ### Improvements * Drop Python 3.5
-support - [Issue #79](https://github.com/sdv-dev/CTGAN/issues/79) by @fealho *
-Support NaN values in categorical variables - [Issue #78](https://github.com/
-sdv-dev/CTGAN/issues/78) by @fealho * Sample synthetic data conditioning on a
-discrete column - [Issue #69](https://github.com/sdv-dev/CTGAN/issues/69) by
-@leix28 * Support recent versions of pandas - [Issue #57](https://github.com/
-sdv-dev/CTGAN/issues/57) by @csala * Easy solution for restoring original
-dtypes - [Issue #26](https://github.com/sdv-dev/CTGAN/issues/26) by
-@oregonpillow ### Bugs fixed * Loss to nan - [Issue #73](https://github.com/
-sdv-dev/CTGAN/issues/73) by @fealho * Swapped the sklearn utils testing import
-statement - [Issue #53](https://github.com/sdv-dev/CTGAN/issues/53) by
-@lurosenb ## v0.2.1 - 2020-01-27 Minor version including changes to ensure the
-logs are properly printed and the option to disable the log transformation to
-the discrete column frequencies. Special thanks to @kevinykuo for the
-contributions! ### Issues Resolved: * Option to sample from true data frequency
-instead of logged frequency - [Issue #16](https://github.com/sdv-dev/CTGAN/
-issues/16) by @kevinykuo * Flush stdout buffer for epoch updates - [Issue #14]
-(https://github.com/sdv-dev/CTGAN/issues/14) by @kevinykuo ## v0.2.0 - 2019-12-
-18 Reorganization of the project structure with a new Python API, new Command
-Line Interface and increased data format support. ### Issues Resolved: *
-Reorganize the project structure - [Issue #10](https://github.com/sdv-dev/
+libraries for specific needs. # History ## v0.7.2 - 2023-05-09 This release
+adds support for Pandas 2.0! It also fixes a bug in the `load_demo` function.
+### Bugs Fixed * load_demo raises urllib.error.HTTPError: HTTP Error 403:
+Forbidden - Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by
+@amontanez24 ### Maintenance * Remove upper bound for pandas - Issue [#282]
+(https://github.com/sdv-dev/CTGAN/issues/282) by @frances-h ## v0.7.1 - 2023-
+02-23 This release fixes a bug that prevented the `CTGAN` model from being
+saved after sampling. ### Bugs Fixed * Cannot save CTGANSynthesizer after
+sampling (TypeError) - Issue [#270](https://github.com/sdv-dev/CTGAN/issues/
+270) by @pvk-developer ## v0.7.0 - 2023-01-20 This release adds support for
+python 3.10 and drops support for python 3.6. It also fixes a couple of the
+most common warnings that were surfacing. ### New Features * Support Python
+3.10 and 3.11 - Issue [#259](https://github.com/sdv-dev/CTGAN/issues/259) by
+@pvk-developer ### Bugs Fixed * Fix SettingWithCopyWarning (may be leading to a
+numerical calculation bug) - Issue [#215](https://github.com/sdv-dev/CTGAN/
+issues/215) by @amontanez24 * FutureWarning in data_transformer with pandas
+1.5.0 - Issue [#246](https://github.com/sdv-dev/CTGAN/issues/246) by
+@amontanez24 ### Maintenance * CTGAN Package Maintenance Updates - Issue [#257]
+(https://github.com/sdv-dev/CTGAN/issues/257) by @amontanez24 ## v0.6.0 - 2022-
+10-07 This release renames the models in CTGAN. `CTGANSynthesizer` is now
+called `CTGAN` and `TVAESynthesizer` is now called `TVAE`. ### New Features *
+Rename synthesizers - Issue [#243](https://github.com/sdv-dev/CTGAN/issues/243)
+by @amontanez24 ## v0.5.2 - 2022-08-18 This release updates CTGAN to use the
+latest version of RDT. It also includes performance and robustness updates to
+the data transformer. ### Issues closed * Bump rdt version - Issue [#242]
+(https://github.com/sdv-dev/CTGAN/issues/242) by @katxiao * Single thread data
+transform is slow for huge table - Issue [#151](https://github.com/sdv-dev/
+CTGAN/issues/151) by @mfhbree * Fix RDT api - Issue [#232](https://github.com/
+sdv-dev/CTGAN/issues/232) by @pvk-developer * Update macos to use latest
+version. - Issue [#237](https://github.com/sdv-dev/CTGAN/issues/237) by @pvk-
+developer * Update the RDT version to 1.0 - Issue [#224](https://github.com/
+sdv-dev/CTGAN/issues/224) by @pvk-developer * Update slack invite link. - Issue
+[#222](https://github.com/sdv-dev/CTGAN/issues/222) by @pvk-developer *
+robustness fix, when data have less rows than the default number of clâ¦ -
+Issue [#211](https://github.com/sdv-dev/CTGAN/issues/211) by @Deathn0t ##
+v0.5.1 - 2022-02-25 This release fixes a bug with the decoder instantiation,
+and also allows users to set a random state for the model fitting and sampling.
+### Issues closed * Update self.decoder with correct variable name - Issue
+[#203](https://github.com/sdv-dev/CTGAN/issues/203) by @tejuafonja * Add random
+state - Issue [#204](https://github.com/sdv-dev/CTGAN/issues/204) by @katxiao
+## v0.5.0 - 2021-11-18 This release adds support for Python 3.9 and updates
+dependencies to ensure compatibility with the rest of the SDV ecosystem, and
+upgrades to the latests [RDT](https://github.com/sdv-dev/RDT/releases/tag/
+v0.6.1) release. ### Issues closed * Add support for Python 3.9 - Issue [#177]
+(https://github.com/sdv-dev/CTGAN/issues/177) by @pvk-developer * Add pip check
+to CI workflows - Issue [#174](https://github.com/sdv-dev/CTGAN/issues/174) by
+@pvk-developer * Typo in `CTGAN` code - Issue [#158](https://github.com/sdv-
+dev/CTGAN/issues/158) by @ori-katz100 and @fealho ## v0.4.3 - 2021-07-12
+Dependency upgrades to ensure compatibility with the rest of the SDV ecosystem.
+## v0.4.2 - 2021-04-27 In this release, the way in which the loss function of
+the TVAE model was computed has been fixed. In addition, the default value of
+the `discriminator_decay` has been changed to a more optimal value. Also some
+improvements to the tests were added. ### Issues closed * `TVAE`: loss function
+- Issue [#143](https://github.com/sdv-dev/CTGAN/issues/143) by @fealho and
+@DingfanChen * Set `discriminator_decay` to `1e-6` - Pull request [#145](https:
+//github.com/sdv-dev/CTGAN/pull/145/) by @fealho * Adds unit tests - Pull
+requests [#140](https://github.com/sdv-dev/CTGAN/pull/140) by @fealho ## v0.4.1
+- 2021-03-30 This release exposes all the hyperparameters which the user may
+find useful for both `CTGAN` and `TVAE`. Also `TVAE` can now be fitted on
+datasets that are shorter than the batch size and drops the last batch only if
+the data size is not divisible by the batch size. ### Issues closed * `TVAE`:
+Adapt `batch_size` to data size - Issue [#135](https://github.com/sdv-dev/
+CTGAN/issues/135) by @fealho and @csala * `ValueError` from
+`validate_discre_columns` with `uniqueCombinationConstraint` - Issue [133]
+(https://github.com/sdv-dev/CTGAN/issues/133) by @fealho and @MLjungg ## v0.4.0
+- 2021-02-24 Maintenance relese to upgrade dependencies to ensure compatibility
+with the rest of the SDV libraries. Also add a validation on the CTGAN
+`condition_column` and `condition_value` inputs. ### Improvements * Validate
+condition_column and condition_value - Issue [#124](https://github.com/sdv-dev/
+CTGAN/issues/124) by @fealho ## v0.3.1 - 2021-01-27 ### Improvements * Check
+discrete_columns valid before fitting - [Issue #35](https://github.com/sdv-dev/
+CTGAN/issues/35) by @fealho ## Bugs fixed * ValueError: max() arg is an empty
+sequence - [Issue #115](https://github.com/sdv-dev/CTGAN/issues/115) by @fealho
+## v0.3.0 - 2020-12-18 In this release we add a new TVAE model which was
+presented in the original CTGAN paper. It also exposes more hyperparameters and
+moves epochs and log_frequency from fit to the constructor. A new verbose
+argument has been added to optionally disable unnecessary printing, and a new
+hyperparameter called `discriminator_steps` has been added to CTGAN to control
+the number of optimization steps performed in the discriminator for each
+generator epoch. The code has also been reorganized and cleaned up for better
+readability and interpretability. Special thanks to @Baukebrenninkmeijer
+@fealho @leix28 @csala for the contributions! ### Improvements * Add TVAE -
+[Issue #111](https://github.com/sdv-dev/CTGAN/issues/111) by @fealho * Move
+`log_frequency` to `__init__` - [Issue #102](https://github.com/sdv-dev/CTGAN/
+issues/102) by @fealho * Add discriminator steps hyperparameter - [Issue #101]
+(https://github.com/sdv-dev/CTGAN/issues/101) by @Baukebrenninkmeijer * Code
+cleanup / Expose hyperparameters - [Issue #59](https://github.com/sdv-dev/
+CTGAN/issues/59) by @fealho and @leix28 * Publish to conda repo - [Issue #54]
+(https://github.com/sdv-dev/CTGAN/issues/54) by @fealho ### Bugs fixed * Fixed
+NaN != NaN counting bug. - [Issue #100](https://github.com/sdv-dev/CTGAN/
+issues/100) by @fealho * Update dependencies and testing - [Issue #90](https://
+github.com/sdv-dev/CTGAN/issues/90) by @csala ## v0.2.2 - 2020-11-13 In this
+release we introduce several minor improvements to make CTGAN more versatile
+and propertly support new types of data, such as categorical NaN values, as
+well as conditional sampling and features to save and load models.
+Additionally, the dependency ranges and python versions have been updated to
+support up to date runtimes. Many thanks @fealho @leix28 @csala @oregonpillow
+and @lurosenb for working on making this release possible! ### Improvements *
+Drop Python 3.5 support - [Issue #79](https://github.com/sdv-dev/CTGAN/issues/
+79) by @fealho * Support NaN values in categorical variables - [Issue #78]
+(https://github.com/sdv-dev/CTGAN/issues/78) by @fealho * Sample synthetic data
+conditioning on a discrete column - [Issue #69](https://github.com/sdv-dev/
+CTGAN/issues/69) by @leix28 * Support recent versions of pandas - [Issue #57]
+(https://github.com/sdv-dev/CTGAN/issues/57) by @csala * Easy solution for
+restoring original dtypes - [Issue #26](https://github.com/sdv-dev/CTGAN/
+issues/26) by @oregonpillow ### Bugs fixed * Loss to nan - [Issue #73](https://
+github.com/sdv-dev/CTGAN/issues/73) by @fealho * Swapped the sklearn utils
+testing import statement - [Issue #53](https://github.com/sdv-dev/CTGAN/issues/
+53) by @lurosenb ## v0.2.1 - 2020-01-27 Minor version including changes to
+ensure the logs are properly printed and the option to disable the log
+transformation to the discrete column frequencies. Special thanks to @kevinykuo
+for the contributions! ### Issues Resolved: * Option to sample from true data
+frequency instead of logged frequency - [Issue #16](https://github.com/sdv-dev/
+CTGAN/issues/16) by @kevinykuo * Flush stdout buffer for epoch updates - [Issue
+#14](https://github.com/sdv-dev/CTGAN/issues/14) by @kevinykuo ## v0.2.0 -
+2019-12-18 Reorganization of the project structure with a new Python API, new
+Command Line Interface and increased data format support. ### Issues Resolved:
+* Reorganize the project structure - [Issue #10](https://github.com/sdv-dev/
 CTGAN/issues/10) by @csala * Move epochs to the fit method - [Issue #5](https:/
 /github.com/sdv-dev/CTGAN/issues/5) by @csala ## v0.1.0 - 2019-11-07 First
 Release - NeurIPS 2019 Version.
```

### Comparing `ctgan-0.7.3/README.md` & `ctgan-0.7.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/__main__.py` & `ctgan-0.7.3.dev0/ctgan/__main__.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/data.py` & `ctgan-0.7.3.dev0/ctgan/data.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/data_sampler.py` & `ctgan-0.7.3.dev0/ctgan/data_sampler.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/data_transformer.py` & `ctgan-0.7.3.dev0/ctgan/data_transformer.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/synthesizers/base.py` & `ctgan-0.7.3.dev0/ctgan/synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/synthesizers/ctgan.py` & `ctgan-0.7.3.dev0/ctgan/synthesizers/ctgan.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan/synthesizers/tvae.py` & `ctgan-0.7.3.dev0/ctgan/synthesizers/tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan.egg-info/PKG-INFO` & `ctgan-0.7.3.dev0/ctgan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctgan
-Version: 0.7.3
+Version: 0.7.3.dev0
 Summary: Create tabular synthetic data using a conditional GAN
 Home-page: https://github.com/sdv-dev/CTGAN
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: ctgan CTGAN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -188,26 +188,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.7.3 - 2023-05-25
-
-This release adds support for Torch 2.0!
-
-### Bugs Fixed
-
-* Torch 2.0 fails with cuda=False - Issue [#288](https://github.com/sdv-dev/CTGAN/issues/288) by @amontanez24
-
-### Maintenance
-
-* Upgrade to torch 2.0 - Issue [#280](https://github.com/sdv-dev/CTGAN/issues/280) by @frances-h
-
 ## v0.7.2 - 2023-05-09
 
 This release adds support for Pandas 2.0! It also fixes a bug in the `load_demo` function.
 
 ### Bugs Fixed
 
 * load_demo raises urllib.error.HTTPError: HTTP Error 403: Forbidden - Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by @amontanez24
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctgan Version: 0.7.3 Summary: Create tabular
+Metadata-Version: 2.1 Name: ctgan Version: 0.7.3.dev0 Summary: Create tabular
 synthetic data using a conditional GAN Home-page: https://github.com/sdv-dev/
 CTGAN Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: ctgan CTGAN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: Free for
 non-commercial use Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -99,132 +99,128 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.7.3 - 2023-05-25 This release
-adds support for Torch 2.0! ### Bugs Fixed * Torch 2.0 fails with cuda=False -
-Issue [#288](https://github.com/sdv-dev/CTGAN/issues/288) by @amontanez24 ###
-Maintenance * Upgrade to torch 2.0 - Issue [#280](https://github.com/sdv-dev/
-CTGAN/issues/280) by @frances-h ## v0.7.2 - 2023-05-09 This release adds
-support for Pandas 2.0! It also fixes a bug in the `load_demo` function. ###
-Bugs Fixed * load_demo raises urllib.error.HTTPError: HTTP Error 403: Forbidden
-- Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by @amontanez24 ###
-Maintenance * Remove upper bound for pandas - Issue [#282](https://github.com/
-sdv-dev/CTGAN/issues/282) by @frances-h ## v0.7.1 - 2023-02-23 This release
-fixes a bug that prevented the `CTGAN` model from being saved after sampling.
-### Bugs Fixed * Cannot save CTGANSynthesizer after sampling (TypeError) -
-Issue [#270](https://github.com/sdv-dev/CTGAN/issues/270) by @pvk-developer ##
-v0.7.0 - 2023-01-20 This release adds support for python 3.10 and drops support
-for python 3.6. It also fixes a couple of the most common warnings that were
-surfacing. ### New Features * Support Python 3.10 and 3.11 - Issue [#259]
-(https://github.com/sdv-dev/CTGAN/issues/259) by @pvk-developer ### Bugs Fixed
-* Fix SettingWithCopyWarning (may be leading to a numerical calculation bug) -
-Issue [#215](https://github.com/sdv-dev/CTGAN/issues/215) by @amontanez24 *
-FutureWarning in data_transformer with pandas 1.5.0 - Issue [#246](https://
-github.com/sdv-dev/CTGAN/issues/246) by @amontanez24 ### Maintenance * CTGAN
-Package Maintenance Updates - Issue [#257](https://github.com/sdv-dev/CTGAN/
-issues/257) by @amontanez24 ## v0.6.0 - 2022-10-07 This release renames the
-models in CTGAN. `CTGANSynthesizer` is now called `CTGAN` and `TVAESynthesizer`
-is now called `TVAE`. ### New Features * Rename synthesizers - Issue [#243]
-(https://github.com/sdv-dev/CTGAN/issues/243) by @amontanez24 ## v0.5.2 - 2022-
-08-18 This release updates CTGAN to use the latest version of RDT. It also
-includes performance and robustness updates to the data transformer. ### Issues
-closed * Bump rdt version - Issue [#242](https://github.com/sdv-dev/CTGAN/
-issues/242) by @katxiao * Single thread data transform is slow for huge table -
-Issue [#151](https://github.com/sdv-dev/CTGAN/issues/151) by @mfhbree * Fix RDT
-api - Issue [#232](https://github.com/sdv-dev/CTGAN/issues/232) by @pvk-
-developer * Update macos to use latest version. - Issue [#237](https://
-github.com/sdv-dev/CTGAN/issues/237) by @pvk-developer * Update the RDT version
-to 1.0 - Issue [#224](https://github.com/sdv-dev/CTGAN/issues/224) by @pvk-
-developer * Update slack invite link. - Issue [#222](https://github.com/sdv-
-dev/CTGAN/issues/222) by @pvk-developer * robustness fix, when data have less
-rows than the default number of clâ¦ - Issue [#211](https://github.com/sdv-
-dev/CTGAN/issues/211) by @Deathn0t ## v0.5.1 - 2022-02-25 This release fixes a
-bug with the decoder instantiation, and also allows users to set a random state
-for the model fitting and sampling. ### Issues closed * Update self.decoder
-with correct variable name - Issue [#203](https://github.com/sdv-dev/CTGAN/
-issues/203) by @tejuafonja * Add random state - Issue [#204](https://
-github.com/sdv-dev/CTGAN/issues/204) by @katxiao ## v0.5.0 - 2021-11-18 This
-release adds support for Python 3.9 and updates dependencies to ensure
-compatibility with the rest of the SDV ecosystem, and upgrades to the latests
-[RDT](https://github.com/sdv-dev/RDT/releases/tag/v0.6.1) release. ### Issues
-closed * Add support for Python 3.9 - Issue [#177](https://github.com/sdv-dev/
-CTGAN/issues/177) by @pvk-developer * Add pip check to CI workflows - Issue
-[#174](https://github.com/sdv-dev/CTGAN/issues/174) by @pvk-developer * Typo in
-`CTGAN` code - Issue [#158](https://github.com/sdv-dev/CTGAN/issues/158) by
-@ori-katz100 and @fealho ## v0.4.3 - 2021-07-12 Dependency upgrades to ensure
-compatibility with the rest of the SDV ecosystem. ## v0.4.2 - 2021-04-27 In
-this release, the way in which the loss function of the TVAE model was computed
-has been fixed. In addition, the default value of the `discriminator_decay` has
-been changed to a more optimal value. Also some improvements to the tests were
-added. ### Issues closed * `TVAE`: loss function - Issue [#143](https://
-github.com/sdv-dev/CTGAN/issues/143) by @fealho and @DingfanChen * Set
-`discriminator_decay` to `1e-6` - Pull request [#145](https://github.com/sdv-
-dev/CTGAN/pull/145/) by @fealho * Adds unit tests - Pull requests [#140](https:
-//github.com/sdv-dev/CTGAN/pull/140) by @fealho ## v0.4.1 - 2021-03-30 This
-release exposes all the hyperparameters which the user may find useful for both
-`CTGAN` and `TVAE`. Also `TVAE` can now be fitted on datasets that are shorter
-than the batch size and drops the last batch only if the data size is not
-divisible by the batch size. ### Issues closed * `TVAE`: Adapt `batch_size` to
-data size - Issue [#135](https://github.com/sdv-dev/CTGAN/issues/135) by
-@fealho and @csala * `ValueError` from `validate_discre_columns` with
-`uniqueCombinationConstraint` - Issue [133](https://github.com/sdv-dev/CTGAN/
-issues/133) by @fealho and @MLjungg ## v0.4.0 - 2021-02-24 Maintenance relese
-to upgrade dependencies to ensure compatibility with the rest of the SDV
-libraries. Also add a validation on the CTGAN `condition_column` and
-`condition_value` inputs. ### Improvements * Validate condition_column and
-condition_value - Issue [#124](https://github.com/sdv-dev/CTGAN/issues/124) by
-@fealho ## v0.3.1 - 2021-01-27 ### Improvements * Check discrete_columns valid
-before fitting - [Issue #35](https://github.com/sdv-dev/CTGAN/issues/35) by
-@fealho ## Bugs fixed * ValueError: max() arg is an empty sequence - [Issue
-#115](https://github.com/sdv-dev/CTGAN/issues/115) by @fealho ## v0.3.0 - 2020-
-12-18 In this release we add a new TVAE model which was presented in the
-original CTGAN paper. It also exposes more hyperparameters and moves epochs and
-log_frequency from fit to the constructor. A new verbose argument has been
-added to optionally disable unnecessary printing, and a new hyperparameter
-called `discriminator_steps` has been added to CTGAN to control the number of
-optimization steps performed in the discriminator for each generator epoch. The
-code has also been reorganized and cleaned up for better readability and
-interpretability. Special thanks to @Baukebrenninkmeijer @fealho @leix28 @csala
-for the contributions! ### Improvements * Add TVAE - [Issue #111](https://
-github.com/sdv-dev/CTGAN/issues/111) by @fealho * Move `log_frequency` to
-`__init__` - [Issue #102](https://github.com/sdv-dev/CTGAN/issues/102) by
-@fealho * Add discriminator steps hyperparameter - [Issue #101](https://
-github.com/sdv-dev/CTGAN/issues/101) by @Baukebrenninkmeijer * Code cleanup /
-Expose hyperparameters - [Issue #59](https://github.com/sdv-dev/CTGAN/issues/
-59) by @fealho and @leix28 * Publish to conda repo - [Issue #54](https://
-github.com/sdv-dev/CTGAN/issues/54) by @fealho ### Bugs fixed * Fixed NaN !=
-NaN counting bug. - [Issue #100](https://github.com/sdv-dev/CTGAN/issues/100)
-by @fealho * Update dependencies and testing - [Issue #90](https://github.com/
-sdv-dev/CTGAN/issues/90) by @csala ## v0.2.2 - 2020-11-13 In this release we
-introduce several minor improvements to make CTGAN more versatile and propertly
-support new types of data, such as categorical NaN values, as well as
-conditional sampling and features to save and load models. Additionally, the
-dependency ranges and python versions have been updated to support up to date
-runtimes. Many thanks @fealho @leix28 @csala @oregonpillow and @lurosenb for
-working on making this release possible! ### Improvements * Drop Python 3.5
-support - [Issue #79](https://github.com/sdv-dev/CTGAN/issues/79) by @fealho *
-Support NaN values in categorical variables - [Issue #78](https://github.com/
-sdv-dev/CTGAN/issues/78) by @fealho * Sample synthetic data conditioning on a
-discrete column - [Issue #69](https://github.com/sdv-dev/CTGAN/issues/69) by
-@leix28 * Support recent versions of pandas - [Issue #57](https://github.com/
-sdv-dev/CTGAN/issues/57) by @csala * Easy solution for restoring original
-dtypes - [Issue #26](https://github.com/sdv-dev/CTGAN/issues/26) by
-@oregonpillow ### Bugs fixed * Loss to nan - [Issue #73](https://github.com/
-sdv-dev/CTGAN/issues/73) by @fealho * Swapped the sklearn utils testing import
-statement - [Issue #53](https://github.com/sdv-dev/CTGAN/issues/53) by
-@lurosenb ## v0.2.1 - 2020-01-27 Minor version including changes to ensure the
-logs are properly printed and the option to disable the log transformation to
-the discrete column frequencies. Special thanks to @kevinykuo for the
-contributions! ### Issues Resolved: * Option to sample from true data frequency
-instead of logged frequency - [Issue #16](https://github.com/sdv-dev/CTGAN/
-issues/16) by @kevinykuo * Flush stdout buffer for epoch updates - [Issue #14]
-(https://github.com/sdv-dev/CTGAN/issues/14) by @kevinykuo ## v0.2.0 - 2019-12-
-18 Reorganization of the project structure with a new Python API, new Command
-Line Interface and increased data format support. ### Issues Resolved: *
-Reorganize the project structure - [Issue #10](https://github.com/sdv-dev/
+libraries for specific needs. # History ## v0.7.2 - 2023-05-09 This release
+adds support for Pandas 2.0! It also fixes a bug in the `load_demo` function.
+### Bugs Fixed * load_demo raises urllib.error.HTTPError: HTTP Error 403:
+Forbidden - Issue [#284](https://github.com/sdv-dev/CTGAN/issues/284) by
+@amontanez24 ### Maintenance * Remove upper bound for pandas - Issue [#282]
+(https://github.com/sdv-dev/CTGAN/issues/282) by @frances-h ## v0.7.1 - 2023-
+02-23 This release fixes a bug that prevented the `CTGAN` model from being
+saved after sampling. ### Bugs Fixed * Cannot save CTGANSynthesizer after
+sampling (TypeError) - Issue [#270](https://github.com/sdv-dev/CTGAN/issues/
+270) by @pvk-developer ## v0.7.0 - 2023-01-20 This release adds support for
+python 3.10 and drops support for python 3.6. It also fixes a couple of the
+most common warnings that were surfacing. ### New Features * Support Python
+3.10 and 3.11 - Issue [#259](https://github.com/sdv-dev/CTGAN/issues/259) by
+@pvk-developer ### Bugs Fixed * Fix SettingWithCopyWarning (may be leading to a
+numerical calculation bug) - Issue [#215](https://github.com/sdv-dev/CTGAN/
+issues/215) by @amontanez24 * FutureWarning in data_transformer with pandas
+1.5.0 - Issue [#246](https://github.com/sdv-dev/CTGAN/issues/246) by
+@amontanez24 ### Maintenance * CTGAN Package Maintenance Updates - Issue [#257]
+(https://github.com/sdv-dev/CTGAN/issues/257) by @amontanez24 ## v0.6.0 - 2022-
+10-07 This release renames the models in CTGAN. `CTGANSynthesizer` is now
+called `CTGAN` and `TVAESynthesizer` is now called `TVAE`. ### New Features *
+Rename synthesizers - Issue [#243](https://github.com/sdv-dev/CTGAN/issues/243)
+by @amontanez24 ## v0.5.2 - 2022-08-18 This release updates CTGAN to use the
+latest version of RDT. It also includes performance and robustness updates to
+the data transformer. ### Issues closed * Bump rdt version - Issue [#242]
+(https://github.com/sdv-dev/CTGAN/issues/242) by @katxiao * Single thread data
+transform is slow for huge table - Issue [#151](https://github.com/sdv-dev/
+CTGAN/issues/151) by @mfhbree * Fix RDT api - Issue [#232](https://github.com/
+sdv-dev/CTGAN/issues/232) by @pvk-developer * Update macos to use latest
+version. - Issue [#237](https://github.com/sdv-dev/CTGAN/issues/237) by @pvk-
+developer * Update the RDT version to 1.0 - Issue [#224](https://github.com/
+sdv-dev/CTGAN/issues/224) by @pvk-developer * Update slack invite link. - Issue
+[#222](https://github.com/sdv-dev/CTGAN/issues/222) by @pvk-developer *
+robustness fix, when data have less rows than the default number of clâ¦ -
+Issue [#211](https://github.com/sdv-dev/CTGAN/issues/211) by @Deathn0t ##
+v0.5.1 - 2022-02-25 This release fixes a bug with the decoder instantiation,
+and also allows users to set a random state for the model fitting and sampling.
+### Issues closed * Update self.decoder with correct variable name - Issue
+[#203](https://github.com/sdv-dev/CTGAN/issues/203) by @tejuafonja * Add random
+state - Issue [#204](https://github.com/sdv-dev/CTGAN/issues/204) by @katxiao
+## v0.5.0 - 2021-11-18 This release adds support for Python 3.9 and updates
+dependencies to ensure compatibility with the rest of the SDV ecosystem, and
+upgrades to the latests [RDT](https://github.com/sdv-dev/RDT/releases/tag/
+v0.6.1) release. ### Issues closed * Add support for Python 3.9 - Issue [#177]
+(https://github.com/sdv-dev/CTGAN/issues/177) by @pvk-developer * Add pip check
+to CI workflows - Issue [#174](https://github.com/sdv-dev/CTGAN/issues/174) by
+@pvk-developer * Typo in `CTGAN` code - Issue [#158](https://github.com/sdv-
+dev/CTGAN/issues/158) by @ori-katz100 and @fealho ## v0.4.3 - 2021-07-12
+Dependency upgrades to ensure compatibility with the rest of the SDV ecosystem.
+## v0.4.2 - 2021-04-27 In this release, the way in which the loss function of
+the TVAE model was computed has been fixed. In addition, the default value of
+the `discriminator_decay` has been changed to a more optimal value. Also some
+improvements to the tests were added. ### Issues closed * `TVAE`: loss function
+- Issue [#143](https://github.com/sdv-dev/CTGAN/issues/143) by @fealho and
+@DingfanChen * Set `discriminator_decay` to `1e-6` - Pull request [#145](https:
+//github.com/sdv-dev/CTGAN/pull/145/) by @fealho * Adds unit tests - Pull
+requests [#140](https://github.com/sdv-dev/CTGAN/pull/140) by @fealho ## v0.4.1
+- 2021-03-30 This release exposes all the hyperparameters which the user may
+find useful for both `CTGAN` and `TVAE`. Also `TVAE` can now be fitted on
+datasets that are shorter than the batch size and drops the last batch only if
+the data size is not divisible by the batch size. ### Issues closed * `TVAE`:
+Adapt `batch_size` to data size - Issue [#135](https://github.com/sdv-dev/
+CTGAN/issues/135) by @fealho and @csala * `ValueError` from
+`validate_discre_columns` with `uniqueCombinationConstraint` - Issue [133]
+(https://github.com/sdv-dev/CTGAN/issues/133) by @fealho and @MLjungg ## v0.4.0
+- 2021-02-24 Maintenance relese to upgrade dependencies to ensure compatibility
+with the rest of the SDV libraries. Also add a validation on the CTGAN
+`condition_column` and `condition_value` inputs. ### Improvements * Validate
+condition_column and condition_value - Issue [#124](https://github.com/sdv-dev/
+CTGAN/issues/124) by @fealho ## v0.3.1 - 2021-01-27 ### Improvements * Check
+discrete_columns valid before fitting - [Issue #35](https://github.com/sdv-dev/
+CTGAN/issues/35) by @fealho ## Bugs fixed * ValueError: max() arg is an empty
+sequence - [Issue #115](https://github.com/sdv-dev/CTGAN/issues/115) by @fealho
+## v0.3.0 - 2020-12-18 In this release we add a new TVAE model which was
+presented in the original CTGAN paper. It also exposes more hyperparameters and
+moves epochs and log_frequency from fit to the constructor. A new verbose
+argument has been added to optionally disable unnecessary printing, and a new
+hyperparameter called `discriminator_steps` has been added to CTGAN to control
+the number of optimization steps performed in the discriminator for each
+generator epoch. The code has also been reorganized and cleaned up for better
+readability and interpretability. Special thanks to @Baukebrenninkmeijer
+@fealho @leix28 @csala for the contributions! ### Improvements * Add TVAE -
+[Issue #111](https://github.com/sdv-dev/CTGAN/issues/111) by @fealho * Move
+`log_frequency` to `__init__` - [Issue #102](https://github.com/sdv-dev/CTGAN/
+issues/102) by @fealho * Add discriminator steps hyperparameter - [Issue #101]
+(https://github.com/sdv-dev/CTGAN/issues/101) by @Baukebrenninkmeijer * Code
+cleanup / Expose hyperparameters - [Issue #59](https://github.com/sdv-dev/
+CTGAN/issues/59) by @fealho and @leix28 * Publish to conda repo - [Issue #54]
+(https://github.com/sdv-dev/CTGAN/issues/54) by @fealho ### Bugs fixed * Fixed
+NaN != NaN counting bug. - [Issue #100](https://github.com/sdv-dev/CTGAN/
+issues/100) by @fealho * Update dependencies and testing - [Issue #90](https://
+github.com/sdv-dev/CTGAN/issues/90) by @csala ## v0.2.2 - 2020-11-13 In this
+release we introduce several minor improvements to make CTGAN more versatile
+and propertly support new types of data, such as categorical NaN values, as
+well as conditional sampling and features to save and load models.
+Additionally, the dependency ranges and python versions have been updated to
+support up to date runtimes. Many thanks @fealho @leix28 @csala @oregonpillow
+and @lurosenb for working on making this release possible! ### Improvements *
+Drop Python 3.5 support - [Issue #79](https://github.com/sdv-dev/CTGAN/issues/
+79) by @fealho * Support NaN values in categorical variables - [Issue #78]
+(https://github.com/sdv-dev/CTGAN/issues/78) by @fealho * Sample synthetic data
+conditioning on a discrete column - [Issue #69](https://github.com/sdv-dev/
+CTGAN/issues/69) by @leix28 * Support recent versions of pandas - [Issue #57]
+(https://github.com/sdv-dev/CTGAN/issues/57) by @csala * Easy solution for
+restoring original dtypes - [Issue #26](https://github.com/sdv-dev/CTGAN/
+issues/26) by @oregonpillow ### Bugs fixed * Loss to nan - [Issue #73](https://
+github.com/sdv-dev/CTGAN/issues/73) by @fealho * Swapped the sklearn utils
+testing import statement - [Issue #53](https://github.com/sdv-dev/CTGAN/issues/
+53) by @lurosenb ## v0.2.1 - 2020-01-27 Minor version including changes to
+ensure the logs are properly printed and the option to disable the log
+transformation to the discrete column frequencies. Special thanks to @kevinykuo
+for the contributions! ### Issues Resolved: * Option to sample from true data
+frequency instead of logged frequency - [Issue #16](https://github.com/sdv-dev/
+CTGAN/issues/16) by @kevinykuo * Flush stdout buffer for epoch updates - [Issue
+#14](https://github.com/sdv-dev/CTGAN/issues/14) by @kevinykuo ## v0.2.0 -
+2019-12-18 Reorganization of the project structure with a new Python API, new
+Command Line Interface and increased data format support. ### Issues Resolved:
+* Reorganize the project structure - [Issue #10](https://github.com/sdv-dev/
 CTGAN/issues/10) by @csala * Move epochs to the fit method - [Issue #5](https:/
 /github.com/sdv-dev/CTGAN/issues/5) by @csala ## v0.1.0 - 2019-11-07 First
 Release - NeurIPS 2019 Version.
```

### Comparing `ctgan-0.7.3/ctgan.egg-info/SOURCES.txt` & `ctgan-0.7.3.dev0/ctgan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/ctgan.egg-info/requires.txt` & `ctgan-0.7.3.dev0/ctgan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/setup.cfg` & `ctgan-0.7.3.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.3
+current_version = 0.7.3.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `ctgan-0.7.3/setup.py` & `ctgan-0.7.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,10 +113,10 @@
     name='ctgan',
     packages=find_packages(include=['ctgan', 'ctgan.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/CTGAN',
-    version='0.7.3',
+    version='0.7.3.dev0',
     zip_safe=False,
 )
```

### Comparing `ctgan-0.7.3/tests/integration/synthesizer/test_ctgan.py` & `ctgan-0.7.3.dev0/tests/integration/synthesizer/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/tests/integration/synthesizer/test_tvae.py` & `ctgan-0.7.3.dev0/tests/integration/synthesizer/test_tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/tests/integration/test_data_transformer.py` & `ctgan-0.7.3.dev0/tests/integration/test_data_transformer.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/tests/unit/synthesizer/test_base.py` & `ctgan-0.7.3.dev0/tests/unit/synthesizer/test_base.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/tests/unit/synthesizer/test_ctgan.py` & `ctgan-0.7.3.dev0/tests/unit/synthesizer/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/tests/unit/synthesizer/test_tvae.py` & `ctgan-0.7.3.dev0/tests/unit/synthesizer/test_tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.3/tests/unit/test_data_transformer.py` & `ctgan-0.7.3.dev0/tests/unit/test_data_transformer.py`

 * *Files identical despite different names*

