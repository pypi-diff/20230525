# Comparing `tmp/circuitpython-bma220-0.4.0.tar.gz` & `tmp/circuitpython-bma220-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bma220-0.4.0.tar", last modified: Sat May 20 17:19:25 2023, max compression
+gzip compressed data, was "circuitpython-bma220-0.5.0.tar", last modified: Thu May 25 02:18:27 2023, max compression
```

## Comparing `circuitpython-bma220-0.4.0.tar` & `circuitpython-bma220-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.942941 circuitpython-bma220-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.946941 circuitpython-bma220-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.946941 circuitpython-bma220-0.4.0/bma220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_slope.py
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_tap_sensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_double_tap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_filter_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_latched_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_sleep_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_slope_slope_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_slope_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.023637 circuitpython-bma220-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.015637 circuitpython-bma220-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.019637 circuitpython-bma220-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-25 02:18:27.023637 circuitpython-bma220-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.019637 circuitpython-bma220-0.5.0/bma220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/bma220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/bma220_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/bma220_lowg_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/bma220_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/bma220/bma220_tap_sensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.019637 circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-25 02:18:26.000000 circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-25 02:18:27.000000 circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:18:26.000000 circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 02:18:26.000000 circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 02:18:26.000000 circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.019637 circuitpython-bma220-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.019637 circuitpython-bma220-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:18:27.023637 circuitpython-bma220-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_double_tap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_latched_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_lowg_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_sleep_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_slope_slope_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/examples/bma220_slope_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-25 02:18:19.000000 circuitpython-bma220-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-25 02:18:08.000000 circuitpython-bma220-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 02:18:27.023637 circuitpython-bma220-0.5.0/setup.cfg
```

### Comparing `circuitpython-bma220-0.4.0/.github/workflows/build.yml` & `circuitpython-bma220-0.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/.github/workflows/release_gh.yml` & `circuitpython-bma220-0.5.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/.gitignore` & `circuitpython-bma220-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/.pre-commit-config.yaml` & `circuitpython-bma220-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/.pylintrc` & `circuitpython-bma220-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/LICENSE` & `circuitpython-bma220-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/PKG-INFO` & `circuitpython-bma220-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.4.0
+Version: 0.5.0
 Summary: BMA220 Bosch Circuitpython Driver library
-Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
+Author-email: JDM <jdm@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
```

### Comparing `circuitpython-bma220-0.4.0/README.rst` & `circuitpython-bma220-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/bma220/bma220.py` & `circuitpython-bma220-0.5.0/bma220/bma220.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     from busio import I2C
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 
 _REG_WHOAMI = const(0x00)
 _FILTER_CONF = const(0x20)
 _ACC_RANGE = const(0x22)
 _SLEEP_CONF = const(0x0F)
```

### Comparing `circuitpython-bma220-0.4.0/bma220/bma220_const.py` & `circuitpython-bma220-0.5.0/bma220/bma220_const.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Author(s): Jose D. Montoya
 
 
 """
 
 from micropython import const
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 # pylint: disable=duplicate-code
 # Acceleration range
 ACC_RANGE_2 = const(0b00)
 ACC_RANGE_4 = const(0b01)
 ACC_RANGE_8 = const(0b10)
```

### Comparing `circuitpython-bma220-0.4.0/bma220/bma220_orientation.py` & `circuitpython-bma220-0.5.0/bma220/bma220_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 from micropython import const
 from adafruit_register.i2c_bit import RWBit, ROBit
 from bma220.bma220 import BMA220
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 _CONF = const(0x1A)
 _ORIENT_EX = const(0x12)
 _INTERRUPTS = const(0x16)
 
 # Orientation Enabled
```

### Comparing `circuitpython-bma220-0.4.0/bma220/bma220_slope.py` & `circuitpython-bma220-0.5.0/bma220/bma220_slope.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 _CONF = const(0x1A)
 _SLOPE_INFO = const(0x12)
 _SLOPE_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `circuitpython-bma220-0.4.0/bma220/bma220_tap_sensing.py` & `circuitpython-bma220-0.5.0/bma220/bma220_tap_sensing.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 _CONF = const(0x1A)
 _TT_INFO = const(0x10)
 _TT_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/PKG-INFO` & `circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.4.0
+Version: 0.5.0
 Summary: BMA220 Bosch Circuitpython Driver library
-Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
+Author-email: JDM <jdm@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
```

### Comparing `circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/SOURCES.txt` & `circuitpython-bma220-0.5.0/circuitpython_bma220.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
 bma220/__init__.py
 bma220/bma220.py
 bma220/bma220_const.py
+bma220/bma220_lowg_detection.py
 bma220/bma220_orientation.py
 bma220/bma220_slope.py
 bma220/bma220_tap_sensing.py
 circuitpython_bma220.egg-info/PKG-INFO
 circuitpython_bma220.egg-info/SOURCES.txt
 circuitpython_bma220.egg-info/dependency_links.txt
 circuitpython_bma220.egg-info/requires.txt
@@ -32,12 +33,13 @@
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/bma220_acc_range.py
 examples/bma220_double_tap_test.py
 examples/bma220_filter_bandwidth.py
 examples/bma220_latched_mode.py
+examples/bma220_lowg_test.py
 examples/bma220_orientation.py
 examples/bma220_simpletest.py
 examples/bma220_sleep_duration.py
 examples/bma220_slope_slope_sign.py
 examples/bma220_slope_test.py
```

### Comparing `circuitpython-bma220-0.4.0/docs/_static/Logo.png` & `circuitpython-bma220-0.5.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/docs/_static/favicon.ico` & `circuitpython-bma220-0.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/docs/conf.py` & `circuitpython-bma220-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/docs/examples.rst` & `circuitpython-bma220-0.5.0/docs/examples.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,89 @@
 Simple test
 ------------
 
 Ensure your device works with this simple test.
 
 .. literalinclude:: ../examples/bma220_simpletest.py
     :caption: examples/bma220_simpletest.py
-    :linenos:
+    :lines: 5-
 
 Acc range settings
 -------------------
 
 Example showing the Acc range setting
 
 .. literalinclude:: ../examples/bma220_acc_range.py
     :caption: examples/bma220_acc_range.py
-    :linenos:
+    :lines: 5-
 
 Sleep duration settings
 ------------------------
 
 Example showing the Sleep duration setting
 
 .. literalinclude:: ../examples/bma220_sleep_duration.py
     :caption: examples/bma220_sleep_duration.py
-    :linenos:
+    :lines: 5-
 
 Filter bandwidth settings
 --------------------------
 
 Example showing the Filter bandwidth setting
 
 .. literalinclude:: ../examples/bma220_filter_bandwidth.py
     :caption: examples/bma220_filter_bandwidth.py
-    :linenos:
+    :lines: 5-
 
 Latched mode settings
 ----------------------
 
 Example showing the Latched mode setting
 
 .. literalinclude:: ../examples/bma220_latched_mode.py
     :caption: examples/bma220_latched_mode.py
-    :linenos:
+    :lines: 5-
 
 Slope Test
 ----------------------
 
 Example for the Slope mode
 
 .. literalinclude:: ../examples/bma220_slope_test.py
     :caption: examples/bma220_slope_test.py
-    :linenos:
+    :lines: 5-
 
 Slope sign settings
 --------------------
 
 Example showing the Slope sign setting
 
 .. literalinclude:: ../examples/bma220_slope_slope_sign.py
     :caption: examples/bma220_slope_slope_sign.py
-    :linenos:
+    :lines: 5-
 
 Double Tap Example
 --------------------
 
 Example showing the Double Tap Mode
 
 .. literalinclude:: ../examples/bma220_double_tap_test.py
     :caption: examples/bma220_double_tap_test.py
-    :linenos:
+    :lines: 5-
 
 Orientation Mode Example
 -------------------------
 
 Example showing the Orientation Mode
 
 .. literalinclude:: ../examples/bma220_orientation.py
     :caption: examples/bma220_orientation.py
-    :linenos:
+    :lines: 5-
+
+Low G Mode Example
+-------------------------
+
+Example showing the Log g Mode
+
+.. literalinclude:: ../examples/bma220_lowg_test.py
+    :caption: examples/bma220_lowg_test.py
+    :lines: 5-
```

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_acc_range.py` & `circuitpython-bma220-0.5.0/examples/bma220_acc_range.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_double_tap_test.py` & `circuitpython-bma220-0.5.0/examples/bma220_double_tap_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_filter_bandwidth.py` & `circuitpython-bma220-0.5.0/examples/bma220_filter_bandwidth.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_latched_mode.py` & `circuitpython-bma220-0.5.0/examples/bma220_latched_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_orientation.py` & `circuitpython-bma220-0.5.0/examples/bma220_orientation.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_sleep_duration.py` & `circuitpython-bma220-0.5.0/examples/bma220_sleep_duration.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/examples/bma220_slope_slope_sign.py` & `circuitpython-bma220-0.5.0/examples/bma220_slope_slope_sign.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.4.0/pyproject.toml` & `circuitpython-bma220-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bma220"
 description = "BMA220 Bosch Circuitpython Driver library"
-version = "0.4.0"
+version = "0.5.0"
 readme = "README.rst"
 authors = [
-    {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
+    {name = "JDM", email = "jdm@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMA220"}
 keywords = [
     "sensor",
     "blinka",
     "circuitpython",
     "micropython",
```

