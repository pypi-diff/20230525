# Comparing `tmp/Pint-0.8.1.tar.gz` & `tmp/Pint-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Pint-0.8.1.tar", last modified: Tue Jun  6 00:46:23 2017, max compression
+gzip compressed data, was "dist/Pint-0.9.tar", last modified: Sat Jan 12 23:30:31 2019, max compression
```

## Comparing `Pint-0.8.1.tar` & `Pint-0.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/
--rw-r--r--   0 hernan     (501) staff       (20)     1469 2017-06-06 00:46:21.000000 Pint-0.8.1/AUTHORS
--rw-r--r--   0 hernan     (501) staff       (20)      906 2017-06-06 00:46:21.000000 Pint-0.8.1/BADGES.rst
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/bench/
--rw-r--r--   0 hernan     (501) staff       (20)     3039 2017-06-06 00:46:21.000000 Pint-0.8.1/bench/bench.py
--rw-r--r--   0 hernan     (501) staff       (20)      883 2017-06-06 00:46:21.000000 Pint-0.8.1/bench/bench_base.yaml
--rw-r--r--   0 hernan     (501) staff       (20)      536 2017-06-06 00:46:21.000000 Pint-0.8.1/bench/bench_numpy.yaml
--rw-r--r--   0 hernan     (501) staff       (20)    13791 2017-06-06 00:46:21.000000 Pint-0.8.1/CHANGES
--rw-r--r--   0 hernan     (501) staff       (20)       37 2017-06-06 00:46:21.000000 Pint-0.8.1/CHANGES_DEV
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/docs/
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/docs/_static/
--rw-r--r--   0 hernan     (501) staff       (20)    11783 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_static/logo-full.jpg
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/docs/_templates/
--rw-r--r--   0 hernan     (501) staff       (20)      734 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_templates/sidebarintro.html
--rw-r--r--   0 hernan     (501) staff       (20)      877 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_templates/sidebarlogo.html
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/docs/_themes/
--rw-r--r--   0 hernan     (501) staff       (20)       22 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/.gitignore
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/docs/_themes/flask/
--rw-r--r--   0 hernan     (501) staff       (20)     1023 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/flask/layout.html
--rw-r--r--   0 hernan     (501) staff       (20)      505 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/flask/relations.html
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/docs/_themes/flask/static/
--rw-r--r--   0 hernan     (501) staff       (20)     6436 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 hernan     (501) staff       (20)      976 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/flask/static/small_flask.css
--rw-r--r--   0 hernan     (501) staff       (20)      191 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/flask/theme.conf
--rw-r--r--   0 hernan     (501) staff       (20)     4875 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/flask_theme_support.py
--rw-r--r--   0 hernan     (501) staff       (20)     1789 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/LICENSE
--rw-r--r--   0 hernan     (501) staff       (20)     1093 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/_themes/README
--rw-r--r--   0 hernan     (501) staff       (20)     9848 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/conf.py
--rw-r--r--   0 hernan     (501) staff       (20)     6238 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/contexts.rst
--rw-r--r--   0 hernan     (501) staff       (20)     1090 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/contributing.rst
--rw-r--r--   0 hernan     (501) staff       (20)     3688 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/defining.rst
--rw-r--r--   0 hernan     (501) staff       (20)     1039 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/faq.rst
--rw-r--r--   0 hernan     (501) staff       (20)     2177 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/getting.rst
--rw-r--r--   0 hernan     (501) staff       (20)     5409 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/index.rst
--rw-r--r--   0 hernan     (501) staff       (20)     5092 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/make.bat
--rw-r--r--   0 hernan     (501) staff       (20)     5634 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/Makefile
--rw-r--r--   0 hernan     (501) staff       (20)     1747 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/measurement.rst
--rw-r--r--   0 hernan     (501) staff       (20)     6037 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/nonmult.rst
--rw-r--r--   0 hernan     (501) staff       (20)     5502 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/numpy.rst
--rw-r--r--   0 hernan     (501) staff       (20)     3116 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/performance.rst
--rw-r--r--   0 hernan     (501) staff       (20)     3657 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/pitheorem.rst
--rw-r--r--   0 hernan     (501) staff       (20)     3630 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/serialization.rst
--rw-r--r--   0 hernan     (501) staff       (20)     2564 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/systems.rst
--rw-r--r--   0 hernan     (501) staff       (20)     9106 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/tutorial.rst
--rw-r--r--   0 hernan     (501) staff       (20)     6089 2017-06-06 00:46:21.000000 Pint-0.8.1/docs/wrapping.rst
--rw-r--r--   0 hernan     (501) staff       (20)     1584 2017-06-06 00:46:21.000000 Pint-0.8.1/LICENSE
--rw-r--r--   0 hernan     (501) staff       (20)      265 2017-06-06 00:46:21.000000 Pint-0.8.1/MANIFEST.in
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/pint/
--rw-r--r--   0 hernan     (501) staff       (20)     2736 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/__init__.py
--rw-r--r--   0 hernan     (501) staff       (20)     4258 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/babel_names.py
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/pint/compat/
--rw-r--r--   0 hernan     (501) staff       (20)     3224 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/compat/__init__.py
--rw-r--r--   0 hernan     (501) staff       (20)     4871 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/compat/chainmap.py
--rw-r--r--   0 hernan     (501) staff       (20)     7047 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/compat/lrucache.py
--rw-r--r--   0 hernan     (501) staff       (20)      684 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/compat/meta.py
--rw-r--r--   0 hernan     (501) staff       (20)      860 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/compat/nullhandler.py
--rw-r--r--   0 hernan     (501) staff       (20)    22787 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/compat/tokenize.py
--rw-r--r--   0 hernan     (501) staff       (20)     1494 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/constants_en.txt
--rw-r--r--   0 hernan     (501) staff       (20)     8549 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/context.py
--rw-r--r--   0 hernan     (501) staff       (20)     1827 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/converters.py
--rw-r--r--   0 hernan     (501) staff       (20)    14299 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/default_en.txt
--rw-r--r--   0 hernan     (501) staff       (20)    11767 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/default_en_0.6.txt
--rw-r--r--   0 hernan     (501) staff       (20)     5321 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/definitions.py
--rw-r--r--   0 hernan     (501) staff       (20)     3650 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/errors.py
--rw-r--r--   0 hernan     (501) staff       (20)     9950 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/formatting.py
--rw-r--r--   0 hernan     (501) staff       (20)     4739 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/measurement.py
--rw-r--r--   0 hernan     (501) staff       (20)     7280 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/pint_eval.py
--rw-r--r--   0 hernan     (501) staff       (20)    61409 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/quantity.py
--rw-r--r--   0 hernan     (501) staff       (20)    55585 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/registry.py
--rw-r--r--   0 hernan     (501) staff       (20)     8099 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/registry_helpers.py
--rw-r--r--   0 hernan     (501) staff       (20)    13691 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/systems.py
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/pint/testsuite/
--rw-r--r--   0 hernan     (501) staff       (20)     5958 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/__init__.py
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/pint/testsuite/compat/
--rw-r--r--   0 hernan     (501) staff       (20)      228 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/compat/__init__.py
--rw-r--r--   0 hernan     (501) staff       (20)     3272 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/helpers.py
--rw-r--r--   0 hernan     (501) staff       (20)     5058 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/parameterized.py
--rw-r--r--   0 hernan     (501) staff       (20)     1217 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_babel.py
--rw-r--r--   0 hernan     (501) staff       (20)    21213 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_contexts.py
--rw-r--r--   0 hernan     (501) staff       (20)     1580 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_converters.py
--rw-r--r--   0 hernan     (501) staff       (20)     3552 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_definitions.py
--rw-r--r--   0 hernan     (501) staff       (20)      701 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_errors.py
--rw-r--r--   0 hernan     (501) staff       (20)     1941 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_formatter.py
--rw-r--r--   0 hernan     (501) staff       (20)     1211 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_infer_base_unit.py
--rw-r--r--   0 hernan     (501) staff       (20)    19906 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_issues.py
--rw-r--r--   0 hernan     (501) staff       (20)     7837 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_measurement.py
--rw-r--r--   0 hernan     (501) staff       (20)    15985 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_numpy.py
--rw-r--r--   0 hernan     (501) staff       (20)     3117 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_pint_eval.py
--rw-r--r--   0 hernan     (501) staff       (20)     1281 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_pitheorem.py
--rw-r--r--   0 hernan     (501) staff       (20)    58052 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_quantity.py
--rw-r--r--   0 hernan     (501) staff       (20)    11188 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_systems.py
--rw-r--r--   0 hernan     (501) staff       (20)    26904 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_umath.py
--rw-r--r--   0 hernan     (501) staff       (20)    25614 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_unit.py
--rw-r--r--   0 hernan     (501) staff       (20)    12462 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/testsuite/test_util.py
--rw-r--r--   0 hernan     (501) staff       (20)     8218 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/unit.py
--rw-r--r--   0 hernan     (501) staff       (20)    22929 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/util.py
--rw-r--r--   0 hernan     (501) staff       (20)      854 2017-06-06 00:46:21.000000 Pint-0.8.1/pint/xtranslated.txt
-drwxr-xr-x   0 hernan     (501) staff       (20)        0 2017-06-06 00:46:23.000000 Pint-0.8.1/Pint.egg-info/
--rw-r--r--   0 hernan     (501) staff       (20)        1 2017-06-06 00:46:23.000000 Pint-0.8.1/Pint.egg-info/dependency_links.txt
--rw-r--r--   0 hernan     (501) staff       (20)    23674 2017-06-06 00:46:23.000000 Pint-0.8.1/Pint.egg-info/PKG-INFO
--rw-r--r--   0 hernan     (501) staff       (20)     2128 2017-06-06 00:46:23.000000 Pint-0.8.1/Pint.egg-info/SOURCES.txt
--rw-r--r--   0 hernan     (501) staff       (20)        5 2017-06-06 00:46:23.000000 Pint-0.8.1/Pint.egg-info/top_level.txt
--rw-r--r--   0 hernan     (501) staff       (20)        1 2017-06-06 00:46:23.000000 Pint-0.8.1/Pint.egg-info/zip-safe
--rw-r--r--   0 hernan     (501) staff       (20)    23674 2017-06-06 00:46:23.000000 Pint-0.8.1/PKG-INFO
--rw-r--r--   0 hernan     (501) staff       (20)     2747 2017-06-06 00:46:21.000000 Pint-0.8.1/README
--rw-r--r--   0 hernan     (501) staff       (20)     3652 2017-06-06 00:46:21.000000 Pint-0.8.1/README.rst
--rw-r--r--   0 hernan     (501) staff       (20)      138 2017-06-06 00:46:23.000000 Pint-0.8.1/setup.cfg
--rw-r--r--   0 hernan     (501) staff       (20)     2082 2017-06-06 00:46:21.000000 Pint-0.8.1/setup.py
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/pint/
+-rw-r--r--   0 grecco   (11832)    32000     1494 2019-01-12 23:30:30.000000 Pint-0.9/pint/constants_en.txt
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/pint/compat/
+-rw-r--r--   0 grecco   (11832)    32000     3436 2019-01-12 23:30:30.000000 Pint-0.9/pint/compat/__init__.py
+-rw-r--r--   0 grecco   (11832)    32000     4893 2019-01-12 23:30:30.000000 Pint-0.9/pint/compat/chainmap.py
+-rw-r--r--   0 grecco   (11832)    32000     7047 2019-01-12 23:30:30.000000 Pint-0.9/pint/compat/lrucache.py
+-rw-r--r--   0 grecco   (11832)    32000    22787 2019-01-12 23:30:30.000000 Pint-0.9/pint/compat/tokenize.py
+-rw-r--r--   0 grecco   (11832)    32000      684 2019-01-12 23:30:30.000000 Pint-0.9/pint/compat/meta.py
+-rw-r--r--   0 grecco   (11832)    32000    13681 2019-01-12 23:30:30.000000 Pint-0.9/pint/systems.py
+-rw-r--r--   0 grecco   (11832)    32000     5321 2019-01-12 23:30:30.000000 Pint-0.9/pint/definitions.py
+-rw-r--r--   0 grecco   (11832)    32000    14788 2019-01-12 23:30:30.000000 Pint-0.9/pint/default_en.txt
+-rw-r--r--   0 grecco   (11832)    32000     2386 2019-01-12 23:30:30.000000 Pint-0.9/pint/matplotlib.py
+-rw-r--r--   0 grecco   (11832)    32000    56734 2019-01-12 23:30:30.000000 Pint-0.9/pint/registry.py
+-rw-r--r--   0 grecco   (11832)    32000    23567 2019-01-12 23:30:30.000000 Pint-0.9/pint/util.py
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/pint/testsuite/
+-rw-r--r--   0 grecco   (11832)    32000     3090 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_pint_eval.py
+-rw-r--r--   0 grecco   (11832)    32000    11104 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_systems.py
+-rw-r--r--   0 grecco   (11832)    32000     1217 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_babel.py
+-rw-r--r--   0 grecco   (11832)    32000     1580 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_converters.py
+-rw-r--r--   0 grecco   (11832)    32000     7837 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_measurement.py
+-rw-r--r--   0 grecco   (11832)    32000      701 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_errors.py
+-rw-r--r--   0 grecco   (11832)    32000     5931 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/__init__.py
+-rw-r--r--   0 grecco   (11832)    32000     3552 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_definitions.py
+-rw-r--r--   0 grecco   (11832)    32000    12462 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_util.py
+-rw-r--r--   0 grecco   (11832)    32000    22738 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_contexts.py
+-rw-r--r--   0 grecco   (11832)    32000    65787 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_quantity.py
+-rw-r--r--   0 grecco   (11832)    32000    26887 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_umath.py
+-rw-r--r--   0 grecco   (11832)    32000    23766 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_issues.py
+-rw-r--r--   0 grecco   (11832)    32000    26779 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_unit.py
+-rw-r--r--   0 grecco   (11832)    32000     1941 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_formatter.py
+-rw-r--r--   0 grecco   (11832)    32000     3245 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/helpers.py
+-rw-r--r--   0 grecco   (11832)    32000    16213 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_numpy.py
+-rw-r--r--   0 grecco   (11832)    32000     5029 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/parameterized.py
+-rw-r--r--   0 grecco   (11832)    32000     1281 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_pitheorem.py
+-rw-r--r--   0 grecco   (11832)    32000     1211 2019-01-12 23:30:30.000000 Pint-0.9/pint/testsuite/test_infer_base_unit.py
+-rw-r--r--   0 grecco   (11832)    32000     4739 2019-01-12 23:30:30.000000 Pint-0.9/pint/measurement.py
+-rw-r--r--   0 grecco   (11832)    32000     2938 2019-01-12 23:30:30.000000 Pint-0.9/pint/__init__.py
+-rw-r--r--   0 grecco   (11832)    32000    11767 2019-01-12 23:30:30.000000 Pint-0.9/pint/default_en_0.6.txt
+-rw-r--r--   0 grecco   (11832)    32000    10098 2019-01-12 23:30:30.000000 Pint-0.9/pint/formatting.py
+-rw-r--r--   0 grecco   (11832)    32000     9293 2019-01-12 23:30:30.000000 Pint-0.9/pint/registry_helpers.py
+-rw-r--r--   0 grecco   (11832)    32000      854 2019-01-12 23:30:30.000000 Pint-0.9/pint/xtranslated.txt
+-rw-r--r--   0 grecco   (11832)    32000     8548 2019-01-12 23:30:30.000000 Pint-0.9/pint/context.py
+-rw-r--r--   0 grecco   (11832)    32000     9552 2019-01-12 23:30:30.000000 Pint-0.9/pint/unit.py
+-rw-r--r--   0 grecco   (11832)    32000     7387 2019-01-12 23:30:30.000000 Pint-0.9/pint/pint_eval.py
+-rw-r--r--   0 grecco   (11832)    32000     4258 2019-01-12 23:30:30.000000 Pint-0.9/pint/babel_names.py
+-rw-r--r--   0 grecco   (11832)    32000     1827 2019-01-12 23:30:30.000000 Pint-0.9/pint/converters.py
+-rw-r--r--   0 grecco   (11832)    32000     3687 2019-01-12 23:30:30.000000 Pint-0.9/pint/errors.py
+-rw-r--r--   0 grecco   (11832)    32000    66754 2019-01-12 23:30:30.000000 Pint-0.9/pint/quantity.py
+-rw-r--r--   0 grecco   (11832)    32000    25157 2019-01-12 23:30:31.000000 Pint-0.9/PKG-INFO
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/bench/
+-rw-r--r--   0 grecco   (11832)    32000      883 2019-01-12 23:30:30.000000 Pint-0.9/bench/bench_base.yaml
+-rw-r--r--   0 grecco   (11832)    32000      536 2019-01-12 23:30:30.000000 Pint-0.9/bench/bench_numpy.yaml
+-rw-r--r--   0 grecco   (11832)    32000     3039 2019-01-12 23:30:30.000000 Pint-0.9/bench/bench.py
+-rw-r--r--   0 grecco   (11832)    32000     1584 2019-01-12 23:30:30.000000 Pint-0.9/LICENSE
+-rw-r--r--   0 grecco   (11832)    32000     1630 2019-01-12 23:30:30.000000 Pint-0.9/AUTHORS
+-rw-r--r--   0 grecco   (11832)    32000    15011 2019-01-12 23:30:30.000000 Pint-0.9/CHANGES
+-rw-r--r--   0 grecco   (11832)    32000      265 2019-01-12 23:30:30.000000 Pint-0.9/MANIFEST.in
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/docs/
+-rw-r--r--   0 grecco   (11832)    32000     6102 2019-01-12 23:30:30.000000 Pint-0.9/docs/index.rst
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/docs/_themes/
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/docs/_themes/flask/
+-rw-r--r--   0 grecco   (11832)    32000     1023 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/flask/layout.html
+-rw-r--r--   0 grecco   (11832)    32000      191 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/docs/_themes/flask/static/
+-rw-r--r--   0 grecco   (11832)    32000     6436 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 grecco   (11832)    32000      976 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/flask/static/small_flask.css
+-rw-r--r--   0 grecco   (11832)    32000      505 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/flask/relations.html
+-rw-r--r--   0 grecco   (11832)    32000     1789 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/LICENSE
+-rw-r--r--   0 grecco   (11832)    32000     4875 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 grecco   (11832)    32000     1093 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/README
+-rw-r--r--   0 grecco   (11832)    32000       22 2019-01-12 23:30:30.000000 Pint-0.9/docs/_themes/.gitignore
+-rw-r--r--   0 grecco   (11832)    32000     1090 2019-01-12 23:30:30.000000 Pint-0.9/docs/contributing.rst
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/docs/_templates/
+-rw-r--r--   0 grecco   (11832)    32000      734 2019-01-12 23:30:30.000000 Pint-0.9/docs/_templates/sidebarintro.html
+-rw-r--r--   0 grecco   (11832)    32000      877 2019-01-12 23:30:30.000000 Pint-0.9/docs/_templates/sidebarlogo.html
+-rw-r--r--   0 grecco   (11832)    32000     5634 2019-01-12 23:30:30.000000 Pint-0.9/docs/Makefile
+-rw-r--r--   0 grecco   (11832)    32000     9887 2019-01-12 23:30:30.000000 Pint-0.9/docs/conf.py
+-rw-r--r--   0 grecco   (11832)    32000    10569 2019-01-12 23:30:30.000000 Pint-0.9/docs/tutorial.rst
+-rw-r--r--   0 grecco   (11832)    32000     3630 2019-01-12 23:30:30.000000 Pint-0.9/docs/serialization.rst
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/docs/_static/
+-rw-r--r--   0 grecco   (11832)    32000    11783 2019-01-12 23:30:30.000000 Pint-0.9/docs/_static/logo-full.jpg
+-rw-r--r--   0 grecco   (11832)    32000     2177 2019-01-12 23:30:30.000000 Pint-0.9/docs/getting.rst
+-rw-r--r--   0 grecco   (11832)    32000     6037 2019-01-12 23:30:30.000000 Pint-0.9/docs/nonmult.rst
+-rw-r--r--   0 grecco   (11832)    32000     1747 2019-01-12 23:30:30.000000 Pint-0.9/docs/measurement.rst
+-rw-r--r--   0 grecco   (11832)    32000     1799 2019-01-12 23:30:30.000000 Pint-0.9/docs/plotting.rst
+-rw-r--r--   0 grecco   (11832)    32000     6238 2019-01-12 23:30:30.000000 Pint-0.9/docs/contexts.rst
+-rw-r--r--   0 grecco   (11832)    32000     5092 2019-01-12 23:30:30.000000 Pint-0.9/docs/make.bat
+-rw-r--r--   0 grecco   (11832)    32000     5502 2019-01-12 23:30:30.000000 Pint-0.9/docs/numpy.rst
+-rw-r--r--   0 grecco   (11832)    32000     7716 2019-01-12 23:30:30.000000 Pint-0.9/docs/wrapping.rst
+-rw-r--r--   0 grecco   (11832)    32000     2564 2019-01-12 23:30:30.000000 Pint-0.9/docs/systems.rst
+-rw-r--r--   0 grecco   (11832)    32000     1137 2019-01-12 23:30:30.000000 Pint-0.9/docs/faq.rst
+-rw-r--r--   0 grecco   (11832)    32000     3116 2019-01-12 23:30:30.000000 Pint-0.9/docs/performance.rst
+-rw-r--r--   0 grecco   (11832)    32000     3657 2019-01-12 23:30:30.000000 Pint-0.9/docs/pitheorem.rst
+-rw-r--r--   0 grecco   (11832)    32000     3688 2019-01-12 23:30:30.000000 Pint-0.9/docs/defining.rst
+-rw-r--r--   0 grecco   (11832)    32000     2747 2019-01-12 23:30:30.000000 Pint-0.9/README
+-rw-r--r--   0 grecco   (11832)    32000     1871 2019-01-12 23:30:30.000000 Pint-0.9/setup.py
+-rw-r--r--   0 grecco   (11832)    32000      117 2019-01-12 23:30:31.000000 Pint-0.9/setup.cfg
+-rw-r--r--   0 grecco   (11832)    32000     3652 2019-01-12 23:30:30.000000 Pint-0.9/README.rst
+-rw-r--r--   0 grecco   (11832)    32000      906 2019-01-12 23:30:30.000000 Pint-0.9/BADGES.rst
+drwxr-xr-x   0 grecco   (11832)    32000        0 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/
+-rw-r--r--   0 grecco   (11832)    32000    25157 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/PKG-INFO
+-rw-r--r--   0 grecco   (11832)    32000        1 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/zip-safe
+-rw-r--r--   0 grecco   (11832)    32000     2131 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/SOURCES.txt
+-rw-r--r--   0 grecco   (11832)    32000       37 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/requires.txt
+-rw-r--r--   0 grecco   (11832)    32000        5 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/top_level.txt
+-rw-r--r--   0 grecco   (11832)    32000        1 2019-01-12 23:30:31.000000 Pint-0.9/Pint.egg-info/dependency_links.txt
+-rw-r--r--   0 grecco   (11832)    32000       37 2019-01-12 23:30:30.000000 Pint-0.9/CHANGES_DEV
```

### Comparing `Pint-0.8.1/AUTHORS` & `Pint-0.9/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Other contributors, listed alphabetically, are:
 
 * Aaron Coleman
 * Alexander Böhn <fish2000@gmail.com>
 * Ana Krivokapic <akrivokapic1@gmail.com>
 * Andrea Zonca <code@andreazonca.com>
+* Andrew Savage <andrewgsavage@gmail.com>
 * Brend Wanders <b.wanders@utwente.nl>
 * choloepus
 * coutinho <coutinho@esrf.fr>
 * Daniel Sokolowski <daniel.sokolowski@danols.com>
 * Dave Brooks <dave@bcs.co.nz>
 * David Linke
 * Ed Schofield <ed@pythoncharmers.com>
@@ -28,14 +29,17 @@
 * Luke Campbell <luke.s.campbell@gmail.com>
 * Matthieu Dartiailh <marul@laposte.net>
 * Nate Bogdanowicz <natezb@gmail.com>
 * Peter Grayson <jpgrayson@gmail.com>
 * Richard Barnes <rbarnes@umn.edu>
 * Ryan Dwyer <ryanpdwyer@gmail.com>
 * Ryan Kingsbury <RyanSKingsbury@alumni.unc.edu>
+* Ryan May
+* Sigvald Marholm <sigvald@marebakken.com>
 * Sundar Raman <cybertoast@gmail.com>
 * Tiago Coutinho <coutinho@esrf.fr>
 * Thomas Kluyver <takowl@gmail.com>
 * Tom Ritchford <tom@swirly.com>
 * Virgil Dupras <virgil.dupras@savoirfairelinux.com>
+* Zebedee Nicholls <zebedee.nicholls@climate-energy-college.org>
 
 (If you think that your name belongs here, please let the maintainer know)
```

### Comparing `Pint-0.8.1/BADGES.rst` & `Pint-0.9/BADGES.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/bench/bench.py` & `Pint-0.9/bench/bench.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/bench/bench_base.yaml` & `Pint-0.9/bench/bench_base.yaml`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/bench/bench_numpy.yaml` & `Pint-0.9/bench/bench_numpy.yaml`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/CHANGES` & `Pint-0.9/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,44 @@
 Pint Changelog
 ==============
 
+0.9 (2019-01-12)
+----------------
+
+- Add support for registering with matplotlib's unit handling
+  (Issue #317, thanks dopplershift)
+- Add converters for matplotlib's unit support.
+  (Issue #317, thanks Ryan May)
+- Fix unwanted side effects in auto dimensionality reduction.
+  (Issue #516, thanks Ben Loer)
+- Allow dimensionality check for non Quantity arguments.
+- Make Quantity and UnitContainer objects hashable.
+  (Issue #286, thanks Nevada Sanchez)
+- Fix unit tests errors with numpy >=1.13.
+  (Issue #577, thanks cpascual)
+- Avoid error in in-place exponentiation with numpy > 1.11.
+  (Issue #577, thanks cpascual)
+- fix compatible units in context.
+  (thanks enrico)
+- Added warning for unsupported ufunc.
+  (Issue #626, thanks kanhua)
+- Improve IPython pretty printers.
+  (Issue #590, thanks tecki)
+- Drop Support for Python 2.6, 3.0, 3.1 and 3.2.
+  (Issue #567)
+- Prepare for deprecation announced in Python 3.7
+  (Issue #747, thanks Simon Willison)
+- Added several new units and Systems
+  (Issues #749, #737, )
+- Started experimental pandas support
+  (Issue #746 and others. Thanks andrewgsavage, znicholls and others)  
+- wraps and checks now supports kwargs and defaults.
+  (Issue #660, thanks jondoesntgit)
+
+
 0.8.1 (2017-06-05)
 ------------------
 
 - Add support for datetime math.
   (Issue #510, thanks robertd)
 - Fixed _repr_html_ in Python 2.7.
   (Issue #512)
@@ -24,15 +58,15 @@
   (Issue #483)
 - Wraps now gets the canonical name of the unit when passed as string.
   (Issue #468)
 - NumPy exp and log keeps the type
   (Issue #95)
 - Implemented a function decorator to ensure that a context is active (with_context)
   (Issue #465)
-- Add warning when a System contains an unknown Group. 
+- Add warning when a System contains an unknown Group.
   (Issue #472)
 - Add conda-forge installation snippet.
   (Issue #485, thanks stadelmanma)
 - Properly support floor division and modulo.
   (Issue #474, thanks tecki)
 - Measurement Correlated variable fix.
   (Issue #463, thanks tadhgmister)
@@ -47,15 +81,15 @@
   (Issue #425, thanks GloriaVictis)
 - Fixed issue with negative values in to_compact() method.
   (Issue #443, thanks nowox)
 - Improved defintions.
   (Issues #448, thanks gdonval)
 - Improved Parser to support capital "E" on scientific notation.
   (Issue #390, thanks javenoneal)
-- Make sure that prefixed units are defined on the registry when unplicking.
+- Make sure that prefixed units are defined on the registry when unpickling.
   (Issue #405)
 - Automatic unit names translation through babel.
   (Issue #338, thanks alexbodn)
 - Support pickling Unit objects.
   (Issue #349)
 - Add support for wavenumber/kayser in spectroscopy context.
   (Issue #321, thanks gerritholl)
@@ -224,15 +258,15 @@
   (Issue #111, thanks rec)
 - Default registry to lazy load, raise error on redefinition
   (Issue #108, thanks rec, aepsil0n)
 - Added condensed format.
   (Issue #107, thanks rec)
 - Added UnitRegistry () operator to parse expression replacing [].
   (Issue #106, thanks rec)
-- Optional case insensitive unit parsing. 
+- Optional case insensitive unit parsing.
   (Issue #105, thanks rec, jeremyfreeman, dbrnz)
 - Change the Quantity mutability depending on magnitude type.
   (Issue #104, thanks rec)
 - Implemented API to list compatible units.
   (Issue #89)
 - Implemented cache of key UnitRegistry methods.
 - Rewrote the Measurement class to use uncertainties.
```

### Comparing `Pint-0.8.1/docs/_static/logo-full.jpg` & `Pint-0.9/docs/_static/logo-full.jpg`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_templates/sidebarintro.html` & `Pint-0.9/docs/_templates/sidebarintro.html`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_templates/sidebarlogo.html` & `Pint-0.9/docs/_templates/sidebarlogo.html`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_themes/flask/layout.html` & `Pint-0.9/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_themes/flask/static/flasky.css_t` & `Pint-0.9/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_themes/flask/static/small_flask.css` & `Pint-0.9/docs/_themes/flask/static/small_flask.css`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_themes/flask_theme_support.py` & `Pint-0.9/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_themes/LICENSE` & `Pint-0.9/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/_themes/README` & `Pint-0.9/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/conf.py` & `Pint-0.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest', 'sphinx.ext.intersphinx', 'sphinx.ext.coverage', 'sphinx.ext.viewcode', 'sphinx.ext.mathjax']
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest', 'sphinx.ext.intersphinx', 'sphinx.ext.coverage', 'sphinx.ext.viewcode', 'sphinx.ext.mathjax', 'matplotlib.sphinxext.plot_directive']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
```

### Comparing `Pint-0.8.1/docs/contexts.rst` & `Pint-0.9/docs/contexts.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/contributing.rst` & `Pint-0.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/defining.rst` & `Pint-0.9/docs/defining.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/faq.rst` & `Pint-0.9/docs/faq.rst`

 * *Files 11% similar despite different names*

```diff
@@ -31,8 +31,13 @@
 
 `SymPy <http://docs.sympy.org/dev/modules/physics/units.html>`_
 
 `Units <https://bitbucket.org/adonohue/units/>`_
 
 `cf units <https://github.com/SciTools/cf_units>`_
 
+`astropy units <https://github.com/astropy/astropy>`_
+
+`yt <https://github.com/yt-project/yt>`_
+
+
 If your are aware of another one, please contribute a patch to the docs.
```

### Comparing `Pint-0.8.1/docs/getting.rst` & `Pint-0.9/docs/getting.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _getting:
 
 Installation
 ============
 
-Pint has no dependencies except Python_ itself. In runs on Python 2.6 and 3.0+.
+Pint has no dependencies except Python_ itself. In runs on Python 2.7 and 3.3+.
 
 You can install it (or upgrade to the latest version) using pip_::
 
     $ pip install -U pint
 
 That's all! You can check that Pint is correctly installed by starting up python, and importing pint:
```

### Comparing `Pint-0.8.1/docs/index.rst` & `Pint-0.9/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 arithmetic operations between them and conversions from and to different units.
 
 It is distributed with a `comprehensive list of physical units, prefixes and constants`_.
 Due to its modular design, you can extend (or even rewrite!) the complete list
 without changing the source code. It supports a lot of numpy mathematical
 operations **without monkey patching or wrapping numpy**.
 
-It has a complete test coverage. It runs in Python 2.6+ and 3.2+ with no other
+It has a complete test coverage. It runs in Python 2.7 and 3.3+ with no other
 dependency. It is licensed under BSD.
 
 
 It is extremely easy and natural to use:
 
 .. code-block:: python
 
@@ -96,29 +96,37 @@
 points, like positions on a map or absolute temperature scales.
 
 **Small codebase**: easy to maintain codebase with a flat hierarchy.
 
 **Dependency free**: it depends only on Python and its standard library.
 
 **Python 2 and 3**: a single codebase that runs unchanged in Python 2.7+ and
-Python 3.0+.
+Python 3.3+.
 
+**Pandas integration**: Thanks to `Pandas Extension Types`_ it is now possible to use Pint with Pandas. Operations on DataFrames and between columns are units aware, providing even more convenience for users of Pandas DataFrames. For full details, see the `Pandas Support Documentation`_.
+
+
+When you choose to use a NumPy_ ndarray, its methods and
+ufuncs are supported including automatic conversion of units. For example
+`numpy.arccos(q)` will require a dimensionless `q` and the units of the output
+quantity will be radian.
 
 
 User Guide
 ----------
 
 .. toctree::
     :maxdepth: 1
 
     getting
     tutorial
     numpy
     nonmult
     wrapping
+    plotting
     serialization
     pitheorem
     contexts
     measurement
     defining
     performance
     systems
@@ -147,7 +155,9 @@
 
 
 .. _`comprehensive list of physical units, prefixes and constants`: https://github.com/hgrecco/pint/blob/master/pint/default_en.txt
 .. _`uncertainties package`: https://pythonhosted.org/uncertainties/
 .. _`NumPy`: http://www.numpy.org/
 .. _`PEP 3101`: https://www.python.org/dev/peps/pep-3101/
 .. _`Babel`: http://babel.pocoo.org/
+.. _`Pandas Extension Types`: https://pandas.pydata.org/pandas-docs/stable/extending.html#extension-types
+.. _`Pandas Support Documentation`: ./pandas.rst
```

### Comparing `Pint-0.8.1/docs/make.bat` & `Pint-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/Makefile` & `Pint-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/measurement.rst` & `Pint-0.9/docs/measurement.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/nonmult.rst` & `Pint-0.9/docs/nonmult.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/numpy.rst` & `Pint-0.9/docs/numpy.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/performance.rst` & `Pint-0.9/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/pitheorem.rst` & `Pint-0.9/docs/pitheorem.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/serialization.rst` & `Pint-0.9/docs/serialization.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/systems.rst` & `Pint-0.9/docs/systems.rst`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/docs/tutorial.rst` & `Pint-0.9/docs/tutorial.rst`

 * *Files 10% similar despite different names*

```diff
@@ -87,14 +87,26 @@
 .. doctest::
 
    >>> speed.to(ureg.joule)
    Traceback (most recent call last):
    ...
    pint.errors.DimensionalityError: Cannot convert from 'inch / minute' ([length] / [time]) to 'joule' ([length] ** 2 * [mass] / [time] ** 2)
 
+Sometimes, the magnitude of the quantity will be very large or very small.
+The method 'to_compact' can adjust the units to make the quantity more
+human-readable.
+
+.. doctest::
+
+   >>> wavelength = 1550 * ureg.nm
+   >>> frequency = (ureg.speed_of_light / wavelength).to('Hz')
+   >>> print(frequency)
+   193414489032258.03 hertz
+   >>> print(frequency.to_compact())
+   193.41448903225802 terahertz
 
 There are also methods 'to_base_units' and 'ito_base_units' which automatically
 convert to the reference units with the correct dimensionality:
 
 .. doctest::
 
    >>> height = 5.0 * ureg.foot + 9.0 * ureg.inch
@@ -104,14 +116,36 @@
    1.7526 meter
    >>> print(height)
    5.75 foot
    >>> height.ito_base_units()
    >>> print(height)
    1.7526 meter
 
+There are also methods 'to_reduced_units' and 'ito_reduced_units' which perform
+a simplified dimensional reduction, combining units with the same dimensionality
+but otherwise keeping your unit definitions intact.
+
+.. doctest::
+
+   >>> density = 1.4 * ureg.gram / ureg.cm**3
+   >>> volume = 10*ureg.cc
+   >>> mass = density*volume
+   >>> print(mass)
+   14.0 cc * gram / centimeter ** 3
+   >>> print(mass.to_reduced_units())
+   14.0 gram
+   >>> print(mass)
+   14.0 cc * gram / centimeter ** 3
+   >>> mass.ito_reduced_units()
+   >>> print(mass)
+   14.0 gram
+
+If you want pint to automatically perform dimensional reduction when producing
+new quantities, the UnitRegistry accepts a parameter `auto_reduce_dimensions`.
+Dimensional reduction can be slow, so auto-reducing is disabled by default.
 
 In some cases it is useful to define physical quantities objects using the
 class constructor:
 
 .. doctest::
 
    >>> Q_ = ureg.Quantity
@@ -202,23 +236,41 @@
 .. doctest::
 
    >>> ureg('2.54')
    2.54
    >>> type(ureg('2.54'))
    <class 'float'>
 
-or 
+or
 
 .. doctest::
 
    >>> Q_('2.54')
    <Quantity(2.54, 'dimensionless')>
    >>> type(Q_('2.54'))
    <class 'pint.quantity.build_quantity_class.<locals>.Quantity'>
 
+.. note:: Pint´s rule for parsing strings with a mixture of numbers and
+   units is that **units are treated with the same precedence as numbers**.
+   
+For example, the unit of
+
+.. doctest::
+
+   >>> Q_('3 l / 100 km')
+   <Quantity(0.03, 'kilometer * liter')>
+   
+may be unexpected first but is a consequence of applying this rule. Use
+brackets to get the expected result:
+
+.. doctest::
+
+   >>> Q_('3 l / (100 km)')
+   <Quantity(0.03, 'liter / kilometer')>
+
 .. note:: Since version 0.7, Pint **does not** use eval_ under the hood.
    This change removes the `serious security problems`_ that the system is
    exposed to when parsing information from untrusted sources.
 
 
 .. _sec-string-formatting:
 
@@ -237,19 +289,14 @@
    >>> print('The repr is {!r}'.format(accel))
    The repr is <Quantity(1.3, 'meter / second ** 2')>
    >>> # Accessing useful attributes
    >>> print('The magnitude is {0.magnitude} with units {0.units}'.format(accel))
    The magnitude is 1.3 with units meter / second ** 2
 
 
-.. note::
-   In Python 2.6, unnumbered placeholders are invalid. Therefore you need to write `{0}` instead
-   of `{}`, `{0!s}` instead of `{!s}` in string formatting operations.
-
-
 But Pint also extends the standard formatting capabilities for unicode and
 LaTeX representations:
 
 .. doctest::
 
    >>> accel = 1.3 * ureg['meter/second**2']
    >>> # Pretty print
```

### Comparing `Pint-0.8.1/docs/wrapping.rst` & `Pint-0.9/docs/wrapping.rst`

 * *Files 14% similar despite different names*

```diff
@@ -140,18 +140,49 @@
     ...
 
 If there are more return values than specified units, ``None`` is assumed for
 the extra outputs. For example, given the NREL SOLPOS calculator that outputs
 solar zenith, azimuth and air mass, the following wrapper assumes no units for
 airmass::
 
-    @UREG.wraps(('deg', 'deg'), ('deg', 'deg', 'millibar', 'degC')
+    @UREG.wraps(('deg', 'deg'), ('deg', 'deg', 'millibar', 'degC'))
     def solar_position(lat, lon, press, tamb, timestamp):
         return zenith, azimuth, airmass
 
+Optional arguments
+------------------
+
+For a function with named keywords with optional values, use a tuple for all
+arguments:
+
+.. doctest::
+
+    >>> @ureg.wraps(ureg.second, (ureg.meters, ureg.meters/ureg.second**2))
+    ... def calculate_time_to_fall(height, gravity=Q_(9.8, 'm/s^2'), verbose=False):
+    ...     """Calculate time to fall from a height h.
+    ...
+    ...     By default, the gravity is assumed to be earth gravity,
+    ...     but it can be modified.
+    ...
+    ...     d = .5 * g * t**2
+    ...     t = sqrt(2 * d / g)
+    ...     """
+    ...     t = sqrt(2 * height / gravity)
+    ...     if verbose: print(str(t) + " seconds to fall")
+    ...     return t
+    ...
+    >>> lunar_module_height = Q_(22, 'feet') + Q_(11, 'inches')
+    >>> calculate_time_to_fall(lunar_module_height, verbose=True)
+    1.1939473204801092 seconds to fall
+    <Quantity(1.1939473204801092, 'second')>
+    >>>
+    >>> moon_gravity = Q_(1.625, 'm/s^2')
+    >>> tcalculate_time_to_fall(lunar_module_height, moon_gravity)
+    <Quantity(2.932051001760214, 'second')>
+
 
 Specifying relations between arguments
 --------------------------------------
 
 In certain cases the actual units but just their relation. This is done using string
 starting with the equal sign `=`:
 
@@ -167,14 +198,27 @@
 
 You can use more than one label:
 
     >>> @ureg.wraps('=A**2*B', ('=A', '=A*B', '=B'))
     ... def some_function(x, y, z):
     ...     pass
 
+With optional arguments
+
+.. doctest::
+
+    >>> @ureg.wraps('=A*B', ('=A', '=B'))
+    ... def get_displacement(time, rate=Q_(1, 'm/s')):
+    ...     return time * rate
+    ...
+    >>> get_displacement(Q_(2, 's'))
+    <Quantity(2, 'meter')>
+    >>> get_displacement(Q_(2, 's'), Q_(1, 'deg/s'))
+    <Quantity(2, 'degree')>
+
 
 Ignoring an argument or return value
 ------------------------------------
 
 To avoid the conversion of an argument or return value, use None
 
 .. doctest::
@@ -198,7 +242,16 @@
 
 .. doctest::
 
     >>> @ureg.check('[length]')
     ... def pendulum_period(length):
     ...     return 2*math.pi*math.sqrt(length/G)
 
+If you just want to check the dimensionality of a quantity, you can do so with the built-in 'check' function.
+
+.. doctest::
+
+    >>> distance = 1 * ureg.m
+    >>> distance.check('[length]')
+    True
+    >>> distance.check('[time]')
+    False
```

### Comparing `Pint-0.8.1/LICENSE` & `Pint-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/__init__.py` & `Pint-0.9/pint/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,26 @@
 from __future__ import with_statement
 
 
 import pkg_resources
 from .formatting import formatter
 from .registry import (UnitRegistry, LazyRegistry)
 from .errors import (DimensionalityError, OffsetUnitCalculusError,
-                   UndefinedUnitError)
+                   UndefinedUnitError, UnitStrippedWarning)
 from .util import pi_theorem, logger
 
 from .context import Context
 
+import sys
+try:
+    from pintpandas import PintType, PintArray
+    _HAS_PINTPANDAS = True
+except Exception:
+    _HAS_PINTPANDAS = False
+    _, _pintpandas_error, _ = sys.exc_info()
 
 try:                # pragma: no cover
     __version__ = pkg_resources.get_distribution('pint').version
 except:             # pragma: no cover
     # we seem to have a local copy not installed without setuptools
     # so the reported version will be unknown
     __version__ = "unknown"
```

### Comparing `Pint-0.8.1/pint/babel_names.py` & `Pint-0.9/pint/babel_names.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/compat/__init__.py` & `Pint-0.9/pint/compat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,19 +58,14 @@
 
 try:
     from functools import lru_cache
 except ImportError:
     from .lrucache import lru_cache
 
 try:
-    from logging import NullHandler
-except ImportError:
-    from .nullhandler import NullHandler
-
-try:
     from itertools import zip_longest
 except ImportError:
     from itertools import izip_longest as zip_longest
 
 try:
     import numpy as np
     from numpy import ndarray
@@ -124,7 +119,21 @@
     HAS_BABEL = True
     HAS_PROPER_BABEL = hasattr(babel_units, 'format_unit')
 except ImportError:
     HAS_PROPER_BABEL = HAS_BABEL = False
 
 if not HAS_PROPER_BABEL:
     Loc = babel_units = None
+
+try:
+    import pandas as pd
+    HAS_PANDAS = True
+    # pin Pandas version for now
+    HAS_PROPER_PANDAS = pd.__version__.startswith("0.24.0.dev0+625.gbdb7a16")
+except ImportError:
+    HAS_PROPER_PANDAS = HAS_PANDAS = False
+
+try:
+    import pytest
+    HAS_PYTEST = True
+except ImportError:
+    HAS_PYTEST = False
```

### Comparing `Pint-0.8.1/pint/compat/chainmap.py` & `Pint-0.9/pint/compat/chainmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,21 @@
     :license: PSF License
 """
 
 from __future__ import division, unicode_literals, print_function, absolute_import
 
 import sys
 
-from collections import MutableMapping
+if sys.version_info < (3, 3):
+    from collections import MutableMapping
+else:
+    from collections.abc import MutableMapping
+
 if sys.version_info < (3, 0):
     from thread import get_ident
-elif sys.version_info < (3, 3):
-    from _thread import get_ident
 else:
     from threading import get_ident
 
 
 def _recursive_repr(fillvalue='...'):
     'Decorator to make a repr function return fillvalue for a recursive call'
```

### Comparing `Pint-0.8.1/pint/compat/lrucache.py` & `Pint-0.9/pint/compat/lrucache.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/compat/meta.py` & `Pint-0.9/pint/compat/meta.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/compat/tokenize.py` & `Pint-0.9/pint/compat/tokenize.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/constants_en.txt` & `Pint-0.9/pint/constants_en.txt`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/context.py` & `Pint-0.9/pint/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             except:
                 raise DefinitionSyntaxError("Could not parse Context %s relation '%s'" % (name, line),
                                             lineno=lineno)
 
         if defaults:
             missing_pars = set(defaults.keys()).difference(set(names))
             if missing_pars:
-                raise DefinitionSyntaxError('Context parameters {0} not found in any equation.'.format(missing_pars))
+                raise DefinitionSyntaxError('Context parameters {} not found in any equation.'.format(missing_pars))
 
         return ctx
 
     def add_transformation(self, src, dst, func):
         """Add a transformation function to the context.
         """
         _key = self.__keytransform__(src, dst)
```

### Comparing `Pint-0.8.1/pint/converters.py` & `Pint-0.9/pint/converters.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/default_en.txt` & `Pint-0.9/pint/default_en.txt`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 [area] = [length] ** 2
 are = 100 * m**2
 barn = 1e-28 * m ** 2 = b
 cmil = 5.067075e-10 * m ** 2 = circular_mils
 darcy = 9.869233e-13 * m ** 2
 hectare = 100 * are = ha
 
+# Concentration
+[concentration] = [substance] / [volume]
+molar = mol / (1e-3 * m ** 3) = M
+
+# Activity
+[activity] = [substance] / [time]
+katal = mole / second = kat
+
 # EM
 esu = 1 * erg**0.5 * centimeter**0.5 = statcoulombs = statC = franklin = Fr
 esu_per_second = 1 * esu / second = statampere
 ampere_turn = 1 * A
 gilbert = 10 / (4 * pi ) * ampere_turn
 coulomb = ampere * second = C
 volt = joule / coulomb = V
@@ -109,15 +117,15 @@
 quadrillion_btu = 10**15 * btu = quad
 thm = 100000 * BTU = therm = EC_therm
 calorie = 4.184 * joule = cal = thermochemical_calorie
 international_steam_table_calorie = 4.1868 * joule
 ton_TNT = 4.184e9 * joule = tTNT
 US_therm = 1.054804e8 * joule
 watt_hour = watt * hour = Wh = watthour
-hartree = 4.35974394e-18 * joule = E_h = hartree_energy
+hartree = 4.35974394e-18 * joule = = Eh = E_h = hartree_energy
 toe = 41.868e9 * joule = tonne_of_oil_equivalent
 
 # Force
 [force] = [mass] * [acceleration]
 newton = kilogram * meter / second ** 2 = N
 dyne = gram * centimeter / second ** 2 = dyn
 force_kilogram = g_0 * kilogram = kgf = kilogram_force = pond
@@ -160,14 +168,25 @@
 bag = 94 * lb
 
 # Textile
 denier =  gram / (9000 * meter)
 tex = gram / (1000 * meter)
 dtex = decitex
 
+# These are Indirect yarn numbering systems (length/unit mass)
+jute = lb / (14400 * yd) = Tj
+Ne = 1/590.5 / tex
+Nm = 1/1000 / tex
+
+@context textile
+    # Allow switching between Direct count system (i.e. tex) and
+    # Indirect count system (i.e. Ne, Nm)
+    [mass] / [length] <-> [length] / [mass]: 1 / value
+@end
+
 # Photometry
 lumen = candela * steradian = lm
 lux = lumen / meter ** 2 = lx
 
 # Power
 [power] = [energy] / [time]
 watt = joule / second = W = volt_ampere = VA
```

### Comparing `Pint-0.8.1/pint/default_en_0.6.txt` & `Pint-0.9/pint/default_en_0.6.txt`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/definitions.py` & `Pint-0.9/pint/definitions.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/errors.py` & `Pint-0.9/pint/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, msg, filename=None, lineno=None):
         super(DefinitionSyntaxError, self).__init__()
         self.msg = msg
         self.filename = None
         self.lineno = None
 
     def __str__(self):
-        mess = "While opening {0}, in line {1}: "
+        mess = "While opening {}, in line {}: "
         return mess.format(self.filename, self.lineno) + self.msg
 
 
 class RedefinitionError(ValueError):
     """Raised when a unit or prefix is redefined.
     """
 
@@ -37,33 +37,33 @@
         super(RedefinitionError, self).__init__()
         self.name = name
         self.definition_type = definition_type
         self.filename = None
         self.lineno = None
 
     def __str__(self):
-        msg = "cannot redefine '{0}' ({1})".format(self.name,
+        msg = "cannot redefine '{}' ({})".format(self.name,
                                                    self.definition_type)
         if self.filename:
-            mess = "While opening {0}, in line {1}: "
+            mess = "While opening {}, in line {}: "
             return mess.format(self.filename, self.lineno) + msg
         return msg
 
 
 class UndefinedUnitError(AttributeError):
     """Raised when the units are not defined in the unit registry.
     """
 
     def __init__(self, unit_names):
         super(UndefinedUnitError, self).__init__()
         self.unit_names = unit_names
 
     def __str__(self):
-        mess = "'{0}' is not defined in the unit registry"
-        mess_plural = "'{0}' are not defined in the unit registry"
+        mess = "'{}' is not defined in the unit registry"
+        mess_plural = "'{}' are not defined in the unit registry"
         if isinstance(self.unit_names, string_types):
             return mess.format(self.unit_names)
         elif isinstance(self.unit_names, (list, tuple))\
                 and len(self.unit_names) == 1:
             return mess.format(self.unit_names[0])
         elif isinstance(self.unit_names, set) and len(self.unit_names) == 1:
             uname = list(self.unit_names)[0]
@@ -82,21 +82,21 @@
         self.units2 = units2
         self.dim1 = dim1
         self.dim2 = dim2
         self.extra_msg = extra_msg
 
     def __str__(self):
         if self.dim1 or self.dim2:
-            dim1 = ' ({0})'.format(self.dim1)
-            dim2 = ' ({0})'.format(self.dim2)
+            dim1 = ' ({})'.format(self.dim1)
+            dim2 = ' ({})'.format(self.dim2)
         else:
             dim1 = ''
             dim2 = ''
 
-        msg = "Cannot convert from '{0}'{1} to '{2}'{3}" + self.extra_msg
+        msg = "Cannot convert from '{}'{} to '{}'{}" + self.extra_msg
 
         return msg.format(self.units1, dim1, self.units2, dim2)
 
 
 class OffsetUnitCalculusError(ValueError):
     """Raised on ambiguous operations with offset units.
     """
@@ -107,7 +107,11 @@
         self.extra_msg = extra_msg
 
     def __str__(self):
         msg = ("Ambiguous operation with offset unit (%s)." %
                ', '.join(['%s' % u for u in [self.units1, self.units2] if u])
                + self.extra_msg)
         return msg.format(self.units1, self.units2)
+
+
+class UnitStrippedWarning(UserWarning):
+    pass
```

### Comparing `Pint-0.8.1/pint/formatting.py` & `Pint-0.9/pint/formatting.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 __JOIN_REG_EXP = re.compile("\{\d*\}")
 
 
 def _join(fmt, iterable):
     """Join an iterable with the format specified in fmt.
 
     The format can be specified in two ways:
-    - PEP3101 format with two replacement fields (eg. '{0} * {1}')
+    - PEP3101 format with two replacement fields (eg. '{} * {}')
     - The concatenating string (eg. ' * ')
     """
     if not iterable:
         return ''
     if not __JOIN_REG_EXP.search(fmt):
         return fmt.join(iterable)
     miter = iter(iterable)
@@ -54,59 +54,59 @@
 #: formatter().
 _FORMATS = {
     'P': {   # Pretty format.
         'as_ratio': True,
         'single_denominator': False,
         'product_fmt': '·',
         'division_fmt': '/',
-        'power_fmt': '{0}{1}',
-        'parentheses_fmt': '({0})',
+        'power_fmt': '{}{}',
+        'parentheses_fmt': '({})',
         'exp_call': _pretty_fmt_exponent,
         },
 
     'L': {   # Latex format.
         'as_ratio': True,
         'single_denominator': True,
         'product_fmt': r' \cdot ',
-        'division_fmt': r'\frac[{0}][{1}]',
-        'power_fmt': '{0}^[{1}]',
-        'parentheses_fmt': r'\left({0}\right)',
+        'division_fmt': r'\frac[{}][{}]',
+        'power_fmt': '{}^[{}]',
+        'parentheses_fmt': r'\left({}\right)',
         },
 
     'H': {   # HTML format.
         'as_ratio': True,
         'single_denominator': True,
         'product_fmt': r' ',
-        'division_fmt': r'{0}/{1}',
-        'power_fmt': '{0}<sup>{1}</sup>',
-        'parentheses_fmt': r'({0})',
+        'division_fmt': r'{}/{}',
+        'power_fmt': '{}<sup>{}</sup>',
+        'parentheses_fmt': r'({})',
         },
 
     '': {   # Default format.
         'as_ratio': True,
         'single_denominator': False,
         'product_fmt': ' * ',
         'division_fmt': ' / ',
-        'power_fmt': '{0} ** {1}',
-        'parentheses_fmt': r'({0})',
+        'power_fmt': '{} ** {}',
+        'parentheses_fmt': r'({})',
         },
 
     'C': {  # Compact format.
         'as_ratio': True,
         'single_denominator': False,
         'product_fmt': '*',  # TODO: Should this just be ''?
         'division_fmt': '/',
-        'power_fmt': '{0}**{1}',
-        'parentheses_fmt': r'({0})',
+        'power_fmt': '{}**{}',
+        'parentheses_fmt': r'({})',
         },
     }
 
 
 def formatter(items, as_ratio=True, single_denominator=False,
-              product_fmt=' * ', division_fmt=' / ', power_fmt='{0} ** {1}',
+              product_fmt=' * ', division_fmt=' / ', power_fmt='{} ** {}',
               parentheses_fmt='({0})', exp_call=lambda x: '{0:n}'.format(x),
               locale=None, babel_length='long', babel_plural_form='one'):
     """Format a list of (name, exponent) pairs.
 
     :param items: a list of (name, exponent) pairs.
     :param as_ratio: True to display as ratio, False as negative powers.
     :param single_denominator: all with terms with negative exponents are
@@ -145,18 +145,18 @@
                     if babel_length != _babel_length
                 ]
             else:
                 other_lengths = []
             for _babel_length in [babel_length] + other_lengths:
                 pat = unit_patterns.get(_key, {}).get(_babel_length, {}).get(plural)
                 if pat is not None:
-                    key = pat.replace('{0}', '').strip()
+                    key = pat.replace('{}', '').strip()
                     break
             division_fmt = compound_unit_patterns.get("per", {}).get(babel_length, division_fmt)
-            power_fmt = '{0}{1}'
+            power_fmt = '{}{}'
             exp_call = _pretty_fmt_exponent
         if value == 1:
             pos_terms.append(key)
         elif value > 0:
             pos_terms.append(power_fmt.format(key, fun(value)))
         elif value == -1 and as_ratio:
             neg_terms.append(key)
@@ -203,22 +203,25 @@
         else:
              break
     return result
 
 
 def format_unit(unit, spec, **kwspec):
     if not unit:
-        return 'dimensionless'
+        if spec.endswith('%'):
+            return ''
+        else:
+            return 'dimensionless'
 
     spec = _parse_spec(spec)
     fmt = dict(_FORMATS[spec])
     fmt.update(kwspec)
 
     if spec == 'L':
-        rm = [(r'\mathrm{{{0}}}'.format(u), p) for u, p in unit.items()]
+        rm = [(r'\mathrm{{{}}}'.format(u), p) for u, p in unit.items()]
         result = formatter(rm, **fmt)
     else:
         result = formatter(unit.items(), **fmt)
     if spec == 'L':
         result = result.replace('[', '{').replace(']', '}')
     return result
 
@@ -256,17 +259,17 @@
             if len(p) > 0 and unit.find(p) == 0:
                 prefix = p
                 unit = unit.replace(prefix, '', 1)
 
         if power < 0:
             l.append(r'\per')
         if prefix is not None:
-            l.append(r'\{0}'.format(prefix))
-        l.append(r'\{0}'.format(unit))
-        l.append(r'{0}'.format(_tothe(abs(power))))
+            l.append(r'\{}'.format(prefix))
+        l.append(r'\{}'.format(unit))
+        l.append(r'{}'.format(_tothe(abs(power))))
 
     return ''.join(lpos) + ''.join(lneg)
 
 
 def remove_custom_flags(spec):
     for flag in _KNOWN_TYPES:
          if flag:
@@ -288,14 +291,17 @@
 
 
 def ndarray_to_latex_parts(ndarr, fmtfun=lambda x: format(x, '.2f'), dim=()):
     if isinstance(fmtfun, string_types):
         fmt = fmtfun
         fmtfun = lambda x: format(x, fmt)
 
+    if ndarr.ndim == 0:
+        _ndarr = ndarr.reshape(1)
+        return [vector_to_latex(_ndarr, fmtfun)]
     if ndarr.ndim == 1:
         return [vector_to_latex(ndarr, fmtfun)]
     if ndarr.ndim == 2:
         return [matrix_to_latex(ndarr, fmtfun)]
     else:
         ret = []
         if ndarr.ndim == 3:
```

### Comparing `Pint-0.8.1/pint/measurement.py` & `Pint-0.9/pint/measurement.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/pint_eval.py` & `Pint-0.9/pint/pint_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from decimal import Decimal
 import math
 import operator
 
 import token as tokenlib
 
+from .errors import DefinitionSyntaxError
+
 # For controlling order of operations
 _OP_PRIORITY = {
     '**': 3,
     '^': 3,
     'unary': 2,
     '*': 1,
     '': 1, # operator for implicit ops
@@ -74,22 +76,22 @@
         bin_op and un_op provide functions for performing binary and unary operations
         """
         
         if self.right:
             # binary or implicit operator
             op_text = self.operator[1] if self.operator else ''
             if op_text not in bin_op:
-                raise Exception('missing binary operator "%s"' % op_text)
+                raise DefinitionSyntaxError('missing binary operator "%s"' % op_text)
             left = self.left.evaluate(define_op, bin_op, un_op)
             return bin_op[op_text](left, self.right.evaluate(define_op, bin_op, un_op))
         elif self.operator:
             # unary operator
             op_text = self.operator[1]
             if op_text not in un_op:
-                raise Exception('missing unary operator "%s"' % op_text)
+                raise DefinitionSyntaxError('missing unary operator "%s"' % op_text)
             return un_op[op_text](self.left.evaluate(define_op, bin_op, un_op))
         else:
             # single value
             return define_op(self.left)
         
 
 def build_eval_tree(tokens, op_priority=_OP_PRIORITY, index=0, depth=0, prev_op=None, ):
@@ -121,26 +123,26 @@
         current_token = tokens[index]
         token_type = current_token[0]
         token_text = current_token[1]
         
         if token_type == tokenlib.OP:
             if token_text == ')':
                 if prev_op is None:
-                    raise Exception('unopened parentheses in tokens: %s' % current_token)
+                    raise DefinitionSyntaxError('unopened parentheses in tokens: %s' % current_token)
                 elif prev_op == '(':
                     # close parenthetical group
                     return result, index
                 else:
                     # parenthetical group ending, but we need to close sub-operations within group
                     return result, index - 1
             elif token_text == '(':
                 # gather parenthetical group
                 right, index = build_eval_tree(tokens, op_priority, index+1, 0, token_text)
                 if not tokens[index][1] == ')':
-                    raise Exception('weird exit from parentheses')
+                    raise DefinitionSyntaxError('weird exit from parentheses')
                 if result:
                     # implicit op with a parenthetical group, i.e. "3 (kg ** 2)"
                     result = EvalTreeNode(left=result, right=right)
                 else:
                     # get first token
                     result = right
             elif token_text in op_priority:
@@ -170,21 +172,21 @@
                 result = EvalTreeNode(left=result, right=right)
             else:
                 # get first token
                 result = EvalTreeNode(left=current_token)
         
         if tokens[index][0] == tokenlib.ENDMARKER:
             if prev_op == '(':
-                raise Exception('unclosed parentheses in tokens')
+                raise DefinitionSyntaxError('unclosed parentheses in tokens')
             if depth > 0 or prev_op:
                 # have to close recursion
                 return result, index
             else:
                 # recursion all closed, so just return the final result
                 return result
             
         if index + 1 >= len(tokens):
             # should hit ENDMARKER before this ever happens
-            raise Exception('unexpected end to tokens')
-        
+            raise DefinitionSyntaxError('unexpected end to tokens')
+
         index += 1
```

### Comparing `Pint-0.8.1/pint/quantity.py` & `Pint-0.9/pint/quantity.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 import datetime
 import math
 import operator
 import functools
 import bisect
 import warnings
 import numbers
+import re
 
 from .formatting import (remove_custom_flags, siunitx_format_unit, ndarray_to_latex,
                          ndarray_to_latex_parts)
 from .errors import (DimensionalityError, OffsetUnitCalculusError,
-                     UndefinedUnitError)
+                     UndefinedUnitError, UnitStrippedWarning)
 from .definitions import UnitDefinition
 from .compat import string_types, ndarray, np, _to_magnitude, long_type
-from .util import (logger, UnitsContainer, SharedRegistryObject,
+from .util import (PrettyIPython, logger, UnitsContainer, SharedRegistryObject,
                    to_units_container, infer_base_unit,
                    fix_str_conversions)
 from pint.compat import Loc
 
-
 def _eq(first, second, check_all):
     """Comparison of scalars and arrays
     """
     out = first == second
     if check_all and isinstance(out, ndarray):
         return np.all(out)
     return out
@@ -45,31 +45,44 @@
         self.internal = internal
 
 
 def reduce_dimensions(f):
     def wrapped(self, *args, **kwargs):
         result = f(self, *args, **kwargs)
         if result._REGISTRY.auto_reduce_dimensions:
-            return result.to_root_units()
+            return result.to_reduced_units()
         else:
             return result
     return wrapped
 
 
 def ireduce_dimensions(f):
     def wrapped(self, *args, **kwargs):
         result = f(self, *args, **kwargs)
         if result._REGISTRY.auto_reduce_dimensions:
-            result.ito_root_units()
+            result.ito_reduced_units()
+        return result
+    return wrapped
+
+def check_implemented(f):
+    def wrapped(self, *args, **kwargs):
+        other=args[0]
+        if other.__class__.__name__ in ["PintArray", "Series"]:
+            return NotImplemented
+        # pandas often gets to arrays of quantities [ Q_(1,"m"), Q_(2,"m")]
+        # and expects Quantity * array[Quantity] should return NotImplemented
+        elif isinstance(other, list) and isinstance(other[0], type(self)):
+            return NotImplemented
+        result = f(self, *args, **kwargs)
         return result
     return wrapped
 
 
 @fix_str_conversions
-class _Quantity(SharedRegistryObject):
+class _Quantity(PrettyIPython, SharedRegistryObject):
     """Implements a class to describe a physical quantity:
     the product of a numerical value and a unit of measurement.
 
     :param value: value of the physical quantity to be created.
     :type value: str, Quantity or any numeric type.
     :param units: units of the physical quantity to be created.
     :type units: UnitsContainer, str or Quantity.
@@ -111,20 +124,30 @@
                                'Quantity as units.')
             else:
                 inst = object.__new__(cls)
                 inst._units = units._units
             inst._magnitude = _to_magnitude(value, inst.force_ndarray)
         else:
             raise TypeError('units must be of type str, Quantity or '
-                            'UnitsContainer; not {0}.'.format(type(units)))
+                            'UnitsContainer; not {}.'.format(type(units)))
 
         inst.__used = False
         inst.__handling = None
+        # Only instances where the magnitude is iterable should have __iter__()
+        if hasattr(inst._magnitude,"__iter__"):
+            inst.__iter__ = cls._iter
         return inst
 
+    def _iter(self):
+        """
+        Will be become __iter__() for instances with iterable magnitudes
+        """
+        # # Allow exception to propagate in case of non-iterable magnitude
+        it_mag = iter(self.magnitude)
+        return iter((self.__class__(mag, self._units) for mag in it_mag))
     @property
     def debug_used(self):
         return self.__used
 
     def __copy__(self):
         ret = self.__class__(copy.copy(self._magnitude), self._units)
         ret.__used = self.__used
@@ -136,23 +159,32 @@
         ret.__used = self.__used
         return ret
 
     def __str__(self):
         return format(self)
 
     def __repr__(self):
-        return "<Quantity({0}, '{1}')>".format(self._magnitude, self._units)
+        return "<Quantity({}, '{}')>".format(self._magnitude, self._units)
+
+    def __hash__(self):
+        self_base = self.to_base_units()
+        if self_base.dimensionless:
+            return hash(self_base.magnitude)
+        else:
+            return hash((self_base.__class__, self_base.magnitude, self_base.units))
+
+    _exp_pattern = re.compile(r"([0-9]\.?[0-9]*)e(-?)\+?0*([0-9]+)")
 
     def __format__(self, spec):
         spec = spec or self.default_format
 
         if 'L' in spec:
-            allf = plain_allf = r'{0}\ {1}'
+            allf = plain_allf = r'{}\ {}'
         else:
-            allf = plain_allf = '{0} {1}'
+            allf = plain_allf = '{} {}'
 
         mstr, ustr = None, None
 
         # If Compact is selected, do it at the beginning
         if '#' in spec:
             spec = spec.replace('#', '')
             obj = self.to_compact()
@@ -161,66 +193,72 @@
 
         # the LaTeX siunitx code
         if 'Lx' in spec:
             spec = spec.replace('Lx','')
             # todo: add support for extracting options
             opts = ''
             ustr = siunitx_format_unit(obj.units)
-            allf = r'\SI[%s]{{{0}}}{{{1}}}'% opts
+            allf = r'\SI[%s]{{{}}}{{{}}}'% opts
         else:
             ustr = format(obj.units, spec)
 
         mspec = remove_custom_flags(spec)
         if isinstance(self.magnitude, ndarray):
             if 'L' in spec:
                 mstr = ndarray_to_latex(obj.magnitude, mspec)
             elif 'H' in spec:
                 # this is required to have the magnitude and unit in the same line
-                allf = r'\[{0} {1}\]'
+                allf = r'\[{} {}\]'
                 parts = ndarray_to_latex_parts(obj.magnitude, mspec)
 
                 if len(parts) > 1:
                     return '\n'.join(allf.format(part, ustr) for part in parts)
 
                 mstr = parts[0]
             else:
                 mstr = format(obj.magnitude, mspec).replace('\n', '')
         else:
             mstr = format(obj.magnitude, mspec).replace('\n', '')
 
+        if 'L' in spec:
+            mstr = self._exp_pattern.sub(r"\1\\times 10^{\2\3}", mstr)
+        elif 'H' in spec:
+            mstr = self._exp_pattern.sub(r"\1×10<sup>\2\3</sup>", mstr)
+
         if allf == plain_allf and ustr.startswith('1 /'):
             # Write e.g. "3 / s" instead of "3 1 / s"
             ustr = ustr[2:]
         return allf.format(mstr, ustr).strip()
 
+    def _repr_pretty_(self, p, cycle):
+        if cycle:
+            super(_Quantity, self)._repr_pretty_(p, cycle)
+        else:
+            p.pretty(self.magnitude)
+            p.text(" ")
+            p.pretty(self.units)
+
     def format_babel(self, spec='', **kwspec):
         spec = spec or self.default_format
 
         # standard cases
         if '#' in spec:
             spec = spec.replace('#', '')
             obj = self.to_compact()
         else:
             obj = self
         kwspec = dict(kwspec)
         if 'length' in kwspec:
             kwspec['babel_length'] = kwspec.pop('length')
         kwspec['locale'] = Loc.parse(kwspec['locale'])
         kwspec['babel_plural_form'] = kwspec['locale'].plural_form(obj.magnitude)
-        return '{0} {1}'.format(
+        return '{} {}'.format(
             format(obj.magnitude, remove_custom_flags(spec)),
             obj.units.format_babel(spec, **kwspec)).replace('\n', '')
 
-    # IPython related code
-    def _repr_html_(self):
-        return self.__format__('H')
-
-    def _repr_latex_(self):
-        return "$" + self.__format__('L') + "$"
-
     @property
     def magnitude(self):
         """Quantity's magnitude. Long form for `m`
         """
         return self._magnitude
 
     @property
@@ -274,14 +312,19 @@
         """Quantity's dimensionality (e.g. {length: 1, time: -1})
         """
         if self._dimensionality is None:
             self._dimensionality = self._REGISTRY._get_dimensionality(self._units)
 
         return self._dimensionality
 
+    def check(self, dimension):
+        """Return true if the quantity's dimension matches passed dimension.
+        """
+        return self.dimensionality == self._REGISTRY.get_dimensionality(dimension)
+
     @classmethod
     def from_tuple(cls, tup):
         return cls(tup[0], UnitsContainer(tup[1]))
 
     def to_tuple(self):
         return self.m, tuple(self._units.items())
 
@@ -370,14 +413,50 @@
         _, other = self._REGISTRY._get_base_units(self._units)
 
         magnitude = self._convert_magnitude_not_inplace(other)
 
         return self.__class__(magnitude, other)
 
 
+    def ito_reduced_units(self):
+        """Return Quantity scaled in place to reduced units, i.e. one unit per
+        dimension. This will not reduce compound units (intentionally), nor
+        can it make use of contexts at this time.
+        """
+        #shortcuts in case we're dimensionless or only a single unit
+        if self.dimensionless:
+            return self.ito({})
+        if len(self._units) == 1:
+            return None
+
+        newunits = self._units.copy()
+        #loop through individual units and compare to each other unit
+        #can we do better than a nested loop here?
+        for unit1, exp in self._units.items():
+            for unit2 in newunits:
+                if unit1 != unit2:
+                    power = self._REGISTRY._get_dimensionality_ratio(unit1,
+                                                                     unit2)
+                    if power:
+                        newunits = newunits.add(unit2, exp/power).remove(unit1)
+                        break
+
+        return self.ito(newunits)
+
+    def to_reduced_units(self):
+        """Return Quantity scaled in place to reduced units, i.e. one unit per
+        dimension. This will not reduce compound units (intentionally), nor
+        can it make use of contexts at this time.
+        """
+        #can we make this more efficient?
+        newq = copy.copy(self)
+        newq.ito_reduced_units()
+        return newq
+
+
     def to_compact(self, unit=None):
         """Return Quantity rescaled to compact, human-readable units.
 
         To get output in terms of a different unit, use the unit parameter.
 
         >>> import pint
         >>> ureg = pint.UnitRegistry()
@@ -389,15 +468,15 @@
         if not isinstance(self.magnitude, numbers.Number):
             msg = ("to_compact applied to non numerical types "
                     "has an undefined behavior.")
             w = RuntimeWarning(msg)
             warnings.warn(w, stacklevel=2)
             return self
 
-        if (self.unitless or self.magnitude==0 or 
+        if (self.unitless or self.magnitude==0 or
             math.isnan(self.magnitude) or math.isinf(self.magnitude)):
             return self
 
         SI_prefixes = {}
         for prefix in self._REGISTRY._prefixes.values():
             try:
                 scale = prefix.converter.scale
@@ -414,17 +493,22 @@
 
         if unit is None:
             unit = infer_base_unit(self)
 
         q_base = self.to(unit)
 
         magnitude = q_base.magnitude
-        # Only changes the prefix on the first unit in the UnitContainer
-        unit_str = list(q_base._units.items())[0][0]
-        unit_power = list(q_base._units.items())[0][1]
+
+        units = list(q_base._units.items())
+        units_numerator = list(filter(lambda a: a[1]>0, units))
+
+        if len(units_numerator) > 0:
+            unit_str, unit_power = units_numerator[0]
+        else:
+            unit_str, unit_power = units[0]
 
         if unit_power > 0:
             power = int(math.floor(math.log10(abs(magnitude)) / unit_power / 3)) * 3
         else:
             power = int(math.ceil(math.log10(abs(magnitude)) / unit_power / 3)) * 3
 
         prefix = SI_bases[bisect.bisect_left(SI_powers, power)]
@@ -549,14 +633,15 @@
             self._magnitude = op(self._convert_magnitude(tu), other._magnitude)
             self._units = other._units
         else:
             raise OffsetUnitCalculusError(self._units, other._units)
 
         return self
 
+    @check_implemented
     def _add_sub(self, other, op):
         """Perform addition or subtraction operation and return the result.
 
         :param other: object to be added to / subtracted from self
         :type other: Quantity or any type accepted by :func:`_to_magnitude`
         :param op: operator function (e.g. operator.add, operator.isub)
         :type op: function
@@ -739,15 +824,16 @@
             other.ito_root_units()
 
         self._magnitude = magnitude_op(self._magnitude, other._magnitude)
         self._units = units_op(self._units, other._units)
 
         return self
 
-    @reduce_dimensions
+    @check_implemented
+    @ireduce_dimensions
     def _mul_div(self, other, magnitude_op, units_op=None):
         """Perform multiplication or division operation and return the result.
 
         :param other: object to be multiplied/divided with self
         :type other: Quantity or any type accepted by :func:`_to_magnitude`
         :param magnitude_op: operator function to perform on the magnitudes
             (e.g. operator.mul)
@@ -847,23 +933,25 @@
         elif self.dimensionless:
             self._magnitude = self.to('')._magnitude // other
         else:
             raise DimensionalityError(self._units, 'dimensionless')
         self._units = UnitsContainer({})
         return self
 
+    @check_implemented
     def __floordiv__(self, other):
         if self._check(other):
             magnitude = self._magnitude // other.to(self._units)._magnitude
         elif self.dimensionless:
             magnitude = self.to('')._magnitude // other
         else:
             raise DimensionalityError(self._units, 'dimensionless')
         return self.__class__(magnitude, UnitsContainer({}))
 
+    @check_implemented
     def __rfloordiv__(self, other):
         if self._check(other):
             magnitude = other._magnitude // self.to(other._units)._magnitude
         elif self.dimensionless:
             magnitude = other // self.to('')._magnitude
         else:
             raise DimensionalityError(self._units, 'dimensionless')
@@ -871,37 +959,41 @@
 
     def __imod__(self, other):
         if not self._check(other):
             other = self.__class__(other, UnitsContainer({}))
         self._magnitude %= other.to(self._units)._magnitude
         return self
 
+    @check_implemented
     def __mod__(self, other):
         if not self._check(other):
             other = self.__class__(other, UnitsContainer({}))
         magnitude = self._magnitude % other.to(self._units)._magnitude
         return self.__class__(magnitude, self._units)
 
+    @check_implemented
     def __rmod__(self, other):
         if self._check(other):
             magnitude = other._magnitude % self.to(other._units)._magnitude
             return self.__class__(magnitude, other._units)
         elif self.dimensionless:
             magnitude = other % self.to('')._magnitude
             return self.__class__(magnitude, UnitsContainer({}))
         else:
             raise DimensionalityError(self._units, 'dimensionless')
 
+    @check_implemented
     def __divmod__(self, other):
         if not self._check(other):
             other = self.__class__(other, UnitsContainer({}))
         q, r = divmod(self._magnitude, other.to(self._units)._magnitude)
         return (self.__class__(q, UnitsContainer({})),
                 self.__class__(r, self._units))
 
+    @check_implemented
     def __rdivmod__(self, other):
         if self._check(other):
             q, r = divmod(other._magnitude, self.to(other._units)._magnitude)
             unit = other._units
         elif self.dimensionless:
             q, r = divmod(other, self.to('')._magnitude)
             unit = UnitsContainer({})
@@ -947,24 +1039,25 @@
                 if not self._is_multiplicative:
                     if self._REGISTRY.autoconvert_offset_to_baseunit:
                         self.ito_base_units()
                     else:
                         raise OffsetUnitCalculusError(self._units)
 
                 if getattr(other, 'dimensionless', False):
-                    other = other.to_base_units()
-                    self._units **= other.magnitude
+                    other = other.to_base_units().magnitude
+                    self._units **= other
                 elif not getattr(other, 'dimensionless', True):
                     raise DimensionalityError(self._units, 'dimensionless')
                 else:
                     self._units **= other
 
             self._magnitude **= _to_magnitude(other, self.force_ndarray)
             return self
 
+    @check_implemented
     def __pow__(self, other):
         try:
             other_magnitude = _to_magnitude(other, self.force_ndarray)
         except TypeError:
             return NotImplemented
         else:
             if not self._ok_for_muldiv:
@@ -997,21 +1090,22 @@
                         new_self = self.to_root_units()
                     else:
                         raise OffsetUnitCalculusError(self._units)
 
                 if getattr(other, 'dimensionless', False):
                     units = new_self._units ** other.to_root_units().magnitude
                 elif not getattr(other, 'dimensionless', True):
-                    raise DimensionalityError(self._units, 'dimensionless')
+                    raise DimensionalityError(other._units, 'dimensionless')
                 else:
                     units = new_self._units ** other
 
             magnitude = new_self._magnitude ** _to_magnitude(other, self.force_ndarray)
             return self.__class__(magnitude, units)
 
+    @check_implemented
     def __rpow__(self, other):
         try:
             other_magnitude = _to_magnitude(other, self.force_ndarray)
         except TypeError:
             return NotImplemented
         else:
             if not self.dimensionless:
@@ -1030,18 +1124,33 @@
 
     def __pos__(self):
         return self.__class__(operator.pos(self._magnitude), self._units)
 
     def __neg__(self):
         return self.__class__(operator.neg(self._magnitude), self._units)
 
+    @check_implemented
     def __eq__(self, other):
         # We compare to the base class of Quantity because
         # each Quantity class is unique.
         if not isinstance(other, _Quantity):
+            if _eq(other, 0, True):
+                # Handle the special case in which we compare to zero
+                # (or an array of zeros)
+                if self._is_multiplicative:
+                    # compare magnitude
+                    return _eq(self._magnitude, other, False)
+                else:
+                    # compare the magnitude after converting the
+                    # non-multiplicative quantity to base units
+                    if self._REGISTRY.autoconvert_offset_to_baseunit:
+                        return _eq(self.to_base_units()._magnitude, other, False)
+                    else:
+                        raise OffsetUnitCalculusError(self._units)
+
             return (self.dimensionless and
                     _eq(self._convert_magnitude(UnitsContainer()), other, False))
 
         if _eq(self._magnitude, 0, True) and _eq(other._magnitude, 0, True):
             return self.dimensionality == other.dimensionality
 
         if self._units == other._units:
@@ -1055,20 +1164,34 @@
 
     def __ne__(self, other):
         out = self.__eq__(other)
         if isinstance(out, ndarray):
             return np.logical_not(out)
         return not out
 
+    @check_implemented
     def compare(self, other, op):
         if not isinstance(other, self.__class__):
             if self.dimensionless:
                 return op(self._convert_magnitude_not_inplace(UnitsContainer()), other)
+            elif _eq(other, 0, True):
+                # Handle the special case in which we compare to zero
+                # (or an array of zeros)
+                if self._is_multiplicative:
+                    # compare magnitude
+                    return op(self._magnitude, other)
+                else:
+                    # compare the magnitude after converting the
+                    # non-multiplicative quantity to base units
+                    if self._REGISTRY.autoconvert_offset_to_baseunit:
+                        return op(self.to_base_units()._magnitude, other)
+                    else:
+                        raise OffsetUnitCalculusError(self._units)
             else:
-                raise ValueError('Cannot compare Quantity and {0}'.format(type(other)))
+                raise ValueError('Cannot compare Quantity and {}'.format(type(other)))
 
         if self._units == other._units:
             return op(self._magnitude, other._magnitude)
         if self.dimensionality != other.dimensionality:
             raise DimensionalityError(self._units, other._units,
                                       self.dimensionality, other.dimensionality)
         return op(self.to_root_units().magnitude,
@@ -1205,15 +1328,15 @@
     def shape(self):
         return self._magnitude.shape
 
     @shape.setter
     def shape(self, value):
         self._magnitude.shape = value
 
-    def searchsorted(self, v, side='left'):
+    def searchsorted(self, v, side='left', sorter=None):
         if isinstance(v, self.__class__):
             v = v.to(self).magnitude
         elif self.dimensionless:
             v = self.__class__(v, '').to(self)
         else:
             raise DimensionalityError('dimensionless', self._units)
         return self.magnitude.searchsorted(v, side)
@@ -1243,23 +1366,19 @@
             return self.__class__(value, self._units ** tmp)
 
         return value
 
     def __len__(self):
         return len(self._magnitude)
 
-    def __iter__(self):
-        # Allow exception to propagate in case of non-iterable magnitude
-        it_mag = iter(self.magnitude)
-        return iter((self.__class__(mag, self._units) for mag in it_mag))
-
     def __getattr__(self, item):
         # Attributes starting with `__array_` are common attributes of NumPy ndarray.
         # They are requested by numpy functions.
         if item.startswith('__array_'):
+            warnings.warn("The unit of the quantity is stripped.", UnitStrippedWarning)
             if isinstance(self._magnitude, ndarray):
                 return getattr(self._magnitude, item)
             else:
                 # If an `__array_` attributes is requested but the magnitude is not an ndarray,
                 # we convert the magnitude to a numpy ndarray.
                 self._magnitude = _to_magnitude(self._magnitude, force_ndarray=True)
                 return getattr(self._magnitude, item)
@@ -1269,23 +1388,23 @@
             attr = getattr(self._magnitude, item)
             if callable(attr):
                 return functools.partial(self.__numpy_method_wrap, attr)
             return attr
         try:
             return getattr(self._magnitude, item)
         except AttributeError as ex:
-            raise AttributeError("Neither Quantity object nor its magnitude ({0}) "
-                                 "has attribute '{1}'".format(self._magnitude, item))
+            raise AttributeError("Neither Quantity object nor its magnitude ({}) "
+                                 "has attribute '{}'".format(self._magnitude, item))
 
     def __getitem__(self, key):
         try:
             value = self._magnitude[key]
             return self.__class__(value, self._units)
         except TypeError:
-            raise TypeError("Neither Quantity object nor its magnitude ({0})"
+            raise TypeError("Neither Quantity object nor its magnitude ({})"
                             "supports indexing".format(self._magnitude))
 
     def __setitem__(self, key, value):
         try:
             if math.isnan(value):
                 self._magnitude[key] = value
                 return
@@ -1305,24 +1424,129 @@
                                                         'access the magnitude directly as '
                                                         '`obj.magnitude[%s] = %s`' % (key, value))
                 self._magnitude[key] = factor.magnitude
             else:
                 self._magnitude[key] = factor
 
         except TypeError:
-            raise TypeError("Neither Quantity object nor its magnitude ({0})"
+            raise TypeError("Neither Quantity object nor its magnitude ({})"
                             "supports indexing".format(self._magnitude))
 
     def tolist(self):
         units = self._units
         return [self.__class__(value, units).tolist() if isinstance(value, list) else self.__class__(value, units)
                 for value in self._magnitude.tolist()]
 
     __array_priority__ = 17
 
+    def _call_ufunc(self, ufunc, *inputs, **kwargs):
+        # Store the destination units
+        dst_units = None
+        # List of magnitudes of Quantities with the right units
+        # to be used as argument of the ufunc
+        mobjs = None
+
+        if ufunc.__name__ in self.__require_units:
+            # ufuncs in __require_units
+            # require specific units
+            # This is more complex that it should be due to automatic
+            # conversion between radians/dimensionless
+            # TODO: maybe could be simplified using Contexts
+            dst_units = self.__require_units[ufunc.__name__]
+            if dst_units == 'radian':
+                mobjs = []
+                for other in inputs:
+                    unt = getattr(other, '_units', '')
+                    if unt == 'radian':
+                        mobjs.append(getattr(other, 'magnitude', other))
+                    else:
+                        factor, units = self._REGISTRY._get_root_units(unt)
+                        if units and units != UnitsContainer({'radian': 1}):
+                            raise DimensionalityError(units, dst_units)
+                        mobjs.append(getattr(other, 'magnitude', other) * factor)
+                mobjs = tuple(mobjs)
+            else:
+                dst_units = self._REGISTRY.parse_expression(dst_units)._units
+
+        elif len(inputs) > 1 and ufunc.__name__ not in self.__skip_other_args:
+            # ufunc with multiple arguments require that all inputs have
+            # the same arguments unless they are in __skip_other_args
+            dst_units = getattr(inputs[0], "_units", None)
+
+        # Do the conversion (if needed) and extract the magnitude for each input.
+        if mobjs is None:
+            if dst_units is not None:
+                mobjs = tuple(self._REGISTRY.convert(getattr(other, 'magnitude', other),
+                                                     getattr(other, 'units', ''),
+                                                     dst_units)
+                              for other in inputs)
+            else:
+                mobjs = tuple(getattr(other, 'magnitude', other)
+                              for other in inputs)
+
+        # call the ufunc
+        try:
+            return ufunc(*mobjs)
+        except Exception as ex:
+            raise _Exception(ex)
+
+
+    def _wrap_output(self, ufname, i, objs, out):
+        """we set the units of the output value"""
+        if i > 0:
+            ufname = "{}__{}".format(ufname, i)
+
+        if ufname in self.__set_units:
+            try:
+                out = self.__class__(out, self.__set_units[ufname])
+            except:
+                raise _Exception(ValueError)
+        elif ufname in self.__copy_units:
+            try:
+                out = self.__class__(out, self._units)
+            except:
+                raise _Exception(ValueError)
+        elif ufname in self.__prod_units:
+            tmp = self.__prod_units[ufname]
+            if tmp == 'size':
+                out = self.__class__(out, self._units ** self._magnitude.size)
+            elif tmp == 'div':
+                units1 = objs[0]._units if isinstance(objs[0], self.__class__) else UnitsContainer()
+                units2 = objs[1]._units if isinstance(objs[1], self.__class__) else UnitsContainer()
+                out = self.__class__(out, units1 / units2)
+            elif tmp == 'mul':
+                units1 = objs[0]._units if isinstance(objs[0], self.__class__) else UnitsContainer()
+                units2 = objs[1]._units if isinstance(objs[1], self.__class__) else UnitsContainer()
+                out = self.__class__(out, units1 * units2)
+            else:
+                out = self.__class__(out, self._units ** tmp)
+
+        return out
+
+
+    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+        if method != "__call__":
+            return NotImplemented
+
+        try:
+            out = self._call_ufunc(ufunc, *inputs, **kwargs)
+            if isinstance(out, tuple):
+                ret = tuple(self._wrap_output(ufunc.__name__, i, inputs, o)
+                            for i, o in enumerate(out))
+                return ret
+            else:
+                return self._wrap_output(ufunc.__name__, 0, inputs, out)
+        except (DimensionalityError, UndefinedUnitError):
+            raise
+        except _Exception as ex:
+            raise ex.internal
+        except:
+            return NotImplemented
+
+
     def __array_prepare__(self, obj, context=None):
         # If this uf is handled by Pint, write it down in the handling dictionary.
 
         # name of the ufunc, argument of the ufunc, domain of the ufunc
         # In ufuncs with multiple outputs, domain indicates which output
         # is currently being prepared (eg. see modf).
         # In ufuncs with a single output, domain is 0
@@ -1330,120 +1554,44 @@
 
         if uf.__name__ in self.__handled and i_out == 0:
             # Only one ufunc should be handled at a time.
             # If a ufunc is already being handled (and this is not another domain),
             # something is wrong..
             if self.__handling:
                 raise Exception('Cannot handled nested ufuncs.\n'
-                                'Current: {0}\n'
-                                'New: {1}'.format(context, self.__handling))
+                                'Current: {}\n'
+                                'New: {}'.format(context, self.__handling))
             self.__handling = context
 
         return obj
 
     def __array_wrap__(self, obj, context=None):
         uf, objs, i_out = context
 
         # if this ufunc is not handled by Pint, pass it to the magnitude.
         if uf.__name__ not in self.__handled:
             return self.magnitude.__array_wrap__(obj, context)
 
         try:
-            ufname = uf.__name__ if i_out == 0 else '{0}__{1}'.format(uf.__name__, i_out)
-
             # First, we check the units of the input arguments.
 
             if i_out == 0:
-                # Do this only when the wrap is called for the first ouput.
-
-                # Store the destination units
-                dst_units = None
-                # List of magnitudes of Quantities with the right units
-                # to be used as argument of the ufunc
-                mobjs = None
-
-                if uf.__name__ in self.__require_units:
-                    # ufuncs in __require_units
-                    # require specific units
-                    # This is more complex that it should be due to automatic
-                    # conversion between radians/dimensionless
-                    # TODO: maybe could be simplified using Contexts
-                    dst_units = self.__require_units[uf.__name__]
-                    if dst_units == 'radian':
-                        mobjs = []
-                        for other in objs:
-                            unt = getattr(other, '_units', '')
-                            if unt == 'radian':
-                                mobjs.append(getattr(other, 'magnitude', other))
-                            else:
-                                factor, units = self._REGISTRY._get_root_units(unt)
-                                if units and units != UnitsContainer({'radian': 1}):
-                                    raise DimensionalityError(units, dst_units)
-                                mobjs.append(getattr(other, 'magnitude', other) * factor)
-                        mobjs = tuple(mobjs)
-                    else:
-                        dst_units = self._REGISTRY.parse_expression(dst_units)._units
-
-                elif len(objs) > 1 and uf.__name__ not in self.__skip_other_args:
-                    # ufunc with multiple arguments require that all inputs have
-                    # the same arguments unless they are in __skip_other_args
-                    dst_units = objs[0]._units
-
-                # Do the conversion (if needed) and extract the magnitude for each input.
-                if mobjs is None:
-                    if dst_units is not None:
-                        mobjs = tuple(self._REGISTRY.convert(getattr(other, 'magnitude', other),
-                                                             getattr(other, 'units', ''),
-                                                             dst_units)
-                                      for other in objs)
-                    else:
-                        mobjs = tuple(getattr(other, 'magnitude', other)
-                                      for other in objs)
-
-                # call the ufunc
-                out = uf(*mobjs)
-
+                out = self._call_ufunc(uf, *objs)
                 # If there are multiple outputs,
                 # store them in __handling (uf, objs, i_out, out0, out1, ...)
                 # and return the first
                 if uf.nout > 1:
                     self.__handling += out
                     out = out[0]
             else:
                 # If this is not the first output,
                 # just grab the result that was previously calculated.
                 out = self.__handling[3 + i_out]
 
-            # Second, we set the units of the output value.
-            if ufname in self.__set_units:
-                try:
-                    out = self.__class__(out, self.__set_units[ufname])
-                except:
-                    raise _Exception(ValueError)
-            elif ufname in self.__copy_units:
-                try:
-                    out = self.__class__(out, self._units)
-                except:
-                    raise _Exception(ValueError)
-            elif ufname in self.__prod_units:
-                tmp = self.__prod_units[ufname]
-                if tmp == 'size':
-                    out = self.__class__(out, self._units ** self._magnitude.size)
-                elif tmp == 'div':
-                    units1 = objs[0]._units if isinstance(objs[0], self.__class__) else UnitsContainer()
-                    units2 = objs[1]._units if isinstance(objs[1], self.__class__) else UnitsContainer()
-                    out = self.__class__(out, units1 / units2)
-                elif tmp == 'mul':
-                    units1 = objs[0]._units if isinstance(objs[0], self.__class__) else UnitsContainer()
-                    units2 = objs[1]._units if isinstance(objs[1], self.__class__) else UnitsContainer()
-                    out = self.__class__(out, units1 * units2)
-                else:
-                    out = self.__class__(out, self._units ** tmp)
-
-            return out
+            return self._wrap_output(uf.__name__, i_out, objs, out)
         except (DimensionalityError, UndefinedUnitError) as ex:
             raise ex
         except _Exception as ex:
             raise ex.internal
         except Exception as ex:
             print(ex)
         finally:
@@ -1520,14 +1668,15 @@
                 is_ok = False
         return is_ok
 
     def to_timedelta(self):
         return datetime.timedelta(microseconds=self.to('microseconds').magnitude)
 
 
+
 def build_quantity_class(registry, force_ndarray=False):
 
     class Quantity(_Quantity):
         pass
 
     Quantity._REGISTRY = registry
     Quantity.force_ndarray = force_ndarray
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Pint-0.8.1/pint/registry.py` & `Pint-0.9/pint/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     - Convert between units.
     - Find dimensionality of a unit.
     - Parse units with prefix and/or suffix.
     - Parse expressions.
     - Parse a definition file.
     - Allow extending the definition file parser by registering @ directives.
 
-    :param filename: path of the units definition file to load.
+    :param filename: path of the units definition file to load or line iterable object.
                      Empty to load the default definition file.
                      None to leave the UnitRegistry empty.
     :type filename: str | None
     :param force_ndarray: convert any input, scalar or not to a numpy.ndarray.
     :param on_redefinition: action to take in case a unit is redefined.
                             'warn', 'raise', 'ignore'
     :type on_redefinition: str
@@ -263,15 +263,15 @@
 
                     self.define(DimensionDefinition(dimension, '', (), None, is_base=True))
 
         elif isinstance(definition, PrefixDefinition):
             d, di = self._prefixes, None
 
         else:
-            raise TypeError('{0} is not a valid definition.'.format(definition))
+            raise TypeError('{} is not a valid definition.'.format(definition))
 
         # define "delta_" units for units with an offset
         if getattr(definition.converter, "offset", 0.0) != 0.0:
 
             if definition.name.startswith('['):
                 d_name = '[delta_' + definition.name[1:]
             else:
@@ -361,15 +361,15 @@
                         return self.load_definitions(fp, is_resource)
             except (RedefinitionError, DefinitionSyntaxError) as e:
                 if e.filename is None:
                     e.filename = file
                 raise e
             except Exception as e:
                 msg = getattr(e, 'message', '') or str(e)
-                raise ValueError('While opening {0}\n{1}'.format(file, msg))
+                raise ValueError('While opening {}\n{}'.format(file, msg))
 
         ifile = SourceIterator(file)
         for no, line in ifile:
             if line and line[0] == '@':
                 if line.startswith('@import'):
                     if is_resource:
                         path = line[7:].strip()
@@ -398,46 +398,49 @@
                 try:
                     self.define(Definition.from_string(line))
                 except DefinitionSyntaxError as ex:
                     if ex.lineno is None:
                         ex.lineno = no
                     raise ex
                 except Exception as ex:
-                    logger.error("In line {0}, cannot add '{1}' {2}".format(no, line, ex))
+                    logger.error("In line {}, cannot add '{}' {}".format(no, line, ex))
 
     def _build_cache(self):
         """Build a cache of dimensionality and base units.
         """
+        self._dimensional_equivalents = dict()
 
         deps = dict((name, set(definition.reference.keys() if definition.reference else {}))
                     for name, definition in self._units.items())
 
         for unit_names in solve_dependencies(deps):
             for unit_name in unit_names:
-                prefixed = False
-                for p in self._prefixes.keys():
-                    if p and unit_name.startswith(p):
-                        prefixed = True
-                        break
                 if '[' in unit_name:
                     continue
+                parsed_names = tuple(self.parse_unit_name(unit_name))
+                _prefix = None
+                if parsed_names:
+                    _prefix, base_name, _suffix = parsed_names[0]
+                else:
+                    base_name = unit_name
+                prefixed = True if _prefix else False
                 try:
-                    uc = ParserHelper.from_word(unit_name)
+                    uc = ParserHelper.from_word(base_name)
 
                     bu = self._get_root_units(uc)
                     di = self._get_dimensionality(uc)
 
                     self._root_units_cache[uc] = bu
                     self._dimensionality_cache[uc] = di
 
                     if not prefixed:
                         if di not in self._dimensional_equivalents:
                             self._dimensional_equivalents[di] = set()
 
-                        self._dimensional_equivalents[di].add(self._units[unit_name]._name)
+                        self._dimensional_equivalents[di].add(self._units[base_name]._name)
 
                 except Exception as e:
                     logger.warning('Could not resolve {0}: {1!r}'.format(unit_name, e))
 
     def _dedup_candidates(self, candidates):
         """Given a list of unit triplets (prefix, name, suffix),
         remove those with different names but equal value.
@@ -472,16 +475,16 @@
 
         candidates = self._dedup_candidates(self.parse_unit_name(name_or_alias, case_sensitive))
         if not candidates:
             raise UndefinedUnitError(name_or_alias)
         elif len(candidates) == 1:
             prefix, unit_name, _ = candidates[0]
         else:
-            logger.warning('Parsing {0} yield multiple results. '
-                           'Options are: {1}'.format(name_or_alias, candidates))
+            logger.warning('Parsing {} yield multiple results. '
+                           'Options are: {}'.format(name_or_alias, candidates))
             prefix, unit_name, _ = candidates[0]
 
         if prefix:
             name = prefix + unit_name
             symbol = self.get_symbol(name)
             prefix_def = self._prefixes[prefix]
             self._units[name] = UnitDefinition(name, symbol, (), prefix_def.converter,
@@ -554,14 +557,36 @@
                 elif reg.reference is not None:
                     self._get_dimensionality_recurse(reg.reference, exp2, accumulator)
             else:
                 reg = self._units[self.get_name(key)]
                 if reg.reference is not None:
                     self._get_dimensionality_recurse(reg.reference, exp2, accumulator)
 
+    def _get_dimensionality_ratio(self, unit1, unit2):
+        """ Get the exponential ratio between two units, i.e. solve unit2 = unit1**x for x.
+        :param unit1: first unit
+        :type unit1: UnitsContainer compatible (str, Unit, UnitsContainer, dict)
+        :param unit2: second unit
+        :type unit2: UnitsContainer compatible (str, Unit, UnitsContainer, dict)
+        :returns: exponential proportionality or None if the units cannot be converted
+        """
+        #shortcut in case of equal units
+        if unit1 == unit2:
+            return 1
+
+        dim1, dim2 = (self.get_dimensionality(unit) for unit in (unit1, unit2))
+        if not dim1 or not dim2 or dim1.keys() != dim2.keys(): #not comparable
+            return None
+
+        ratios = (dim2[key]/val for key, val in dim1.items())
+        first = next(ratios)
+        if all(r == first for r in ratios): #all are same, we're good
+            return first
+        return None
+
     def get_root_units(self, input_units, check_nonmult=True):
         """Convert unit or dict of units to the root units.
 
         If any unit is non multiplicative and check_converter is True,
         then None is returned as the multiplicative factor.
 
         :param input_units: units
@@ -906,14 +931,41 @@
         l = self._dedup_candidates(self.parse_unit_name(u))
         try:
             u = l[0][1]
             return self._units[u].is_multiplicative
         except KeyError:
             raise UndefinedUnitError(u)
 
+    def _validate_and_extract(self, units):
+
+        nonmult_units = [(u, e) for u, e in units.items()
+                         if not self._is_multiplicative(u)]
+
+        # Let's validate source offset units
+        if len(nonmult_units) > 1:
+            # More than one src offset unit is not allowed
+            raise ValueError('more than one offset unit.')
+
+        elif len(nonmult_units) == 1:
+            # A single src offset unit is present. Extract it
+            # But check that:
+            # - the exponent is 1
+            # - is not used in multiplicative context
+            nonmult_unit, exponent = nonmult_units.pop()
+
+            if exponent != 1:
+                raise ValueError('offset units in higher order.')
+
+            if len(units) > 1 and not self.autoconvert_offset_to_baseunit:
+                raise ValueError('offset unit used in multiplicative context.')
+
+            return nonmult_unit
+
+        return None
+
     def _convert(self, value, src, dst, inplace=False):
         """Convert value from some source to destination units.
 
         In addition to what is done by the BaseRegistry,
         converts between non-multiplicative units.
 
         :param value: value
@@ -923,78 +975,52 @@
         :type dst: UnitsContainer
 
         :return: converted value
         """
 
         # Conversion needs to consider if non-multiplicative (AKA offset
         # units) are involved. Conversion is only possible if src and dst
-        # have at most one offset unit per dimension.
-        src_offset_units = [(u, e) for u, e in src.items()
-                            if not self._is_multiplicative(u)]
-        dst_offset_units = [(u, e) for u, e in dst.items()
-                            if not self._is_multiplicative(u)]
+        # have at most one offset unit per dimension. Other rules are applied
+        # by validate and extract.
+        try:
+            src_offset_unit = self._validate_and_extract(src)
+        except ValueError as ex:
+            raise DimensionalityError(src, dst, extra_msg=' - In source units, %s ' % ex)
+
+        try:
+            dst_offset_unit = self._validate_and_extract(dst)
+        except ValueError as ex:
+            raise DimensionalityError(src, dst, extra_msg=' - In destination units, %s ' % ex)
 
-        if not (src_offset_units or dst_offset_units):
+        if not (src_offset_unit or dst_offset_unit):
             return super(NonMultiplicativeRegistry, self)._convert(value, src, dst, inplace)
 
         src_dim = self._get_dimensionality(src)
         dst_dim = self._get_dimensionality(dst)
 
         # If the source and destination dimensionality are different,
         # then the conversion cannot be performed.
         if src_dim != dst_dim:
             raise DimensionalityError(src, dst, src_dim, dst_dim)
 
-        # For offset units we need to check if the conversion is allowed.
-        if src_offset_units or dst_offset_units:
-
-            # Validate that not more than one offset unit is present
-            if len(src_offset_units) > 1 or len(dst_offset_units) > 1:
-                raise DimensionalityError(
-                    src, dst, src_dim, dst_dim,
-                    extra_msg=' - more than one offset unit.')
-
-            # validate that offset unit is not used in multiplicative context
-            if ((len(src_offset_units) == 1 and len(src) > 1)
-                    or (len(dst_offset_units) == 1 and len(dst) > 1)
-                    and not self.autoconvert_offset_to_baseunit):
-                raise DimensionalityError(
-                    src, dst, src_dim, dst_dim,
-                    extra_msg=' - offset unit used in multiplicative context.')
-
-            # Validate that order of offset unit is exactly one.
-            if src_offset_units:
-                if src_offset_units[0][1] != 1:
-                    raise DimensionalityError(
-                        src, dst, src_dim, dst_dim,
-                        extra_msg=' - offset units in higher order.')
-            else:
-                if dst_offset_units[0][1] != 1:
-                    raise DimensionalityError(
-                        src, dst, src_dim, dst_dim,
-                        extra_msg=' - offset units in higher order.')
-
-        # Here we convert only the offset quantities. Any remaining scaled
-        # quantities will be converted later.
-
-        # TODO: Shouldn't this (until factor, units) be inside the If above?
-
         # clean src from offset units by converting to reference
-        for u, e in src_offset_units:
-            value = self._units[u].converter.to_reference(value, inplace)
-        src = src.remove([u for u, e in src_offset_units])
+        if src_offset_unit:
+            value = self._units[src_offset_unit].converter.to_reference(value, inplace)
+
+        src = src.remove([src_offset_unit])
 
         # clean dst units from offset units
-        dst = dst.remove([u for u, e in dst_offset_units])
+        dst = dst.remove([dst_offset_unit])
 
+        # Convert non multiplicative units to the dst.
         value = super(NonMultiplicativeRegistry, self)._convert(value, src, dst, inplace, False)
 
         # Finally convert to offset units specified in destination
-        for u, e in dst_offset_units:
-            value = self._units[u].converter.from_reference(value, inplace)
+        if dst_offset_unit:
+            value = self._units[dst_offset_unit].converter.from_reference(value, inplace)
 
         return value
 
 
 class ContextRegistry(BaseRegistry):
     """Handle of Contexts.
 
@@ -1023,15 +1049,15 @@
         self._register_parser('@context', self._parse_context)
 
     def _parse_context(self, ifile):
         try:
             self.add_context(Context.from_lines(ifile.block_iter(),
                                                 self.get_dimensionality))
         except KeyError as e:
-            raise DefinitionSyntaxError('unknown dimension {0} in context'.format(str(e)))
+            raise DefinitionSyntaxError('unknown dimension {} in context'.format(str(e)))
 
     def add_context(self, context):
         """Add a context object to the registry.
 
         The context will be accessible by its name and aliases.
 
         Notice that this method will NOT enable the context. Use `enable_contexts`.
@@ -1067,16 +1093,16 @@
         """
 
         # If present, copy the defaults from the containing contexts
         if self._active_ctx.defaults:
             kwargs = dict(self._active_ctx.defaults, **kwargs)
 
         # For each name, we first find the corresponding context
-        ctxs = tuple((self._contexts[name] if isinstance(name, string_types) else name)
-                     for name in names_or_contexts)
+        ctxs = list((self._contexts[name] if isinstance(name, string_types) else name)
+                    for name in names_or_contexts)
 
         # Check if the contexts have been checked first, if not we make sure
         # that dimensions are expressed in terms of base dimensions.
         for ctx in ctxs:
             if getattr(ctx, '_checked', False):
                 continue
             for (src, dst), func in ctx.funcs.items():
@@ -1089,21 +1115,23 @@
 
         # and create a new one with the new defaults.
         ctxs = tuple(Context.from_context(ctx, **kwargs)
                      for ctx in ctxs)
 
         # Finally we add them to the active context.
         self._active_ctx.insert_contexts(*ctxs)
+        self._build_cache()
 
     def disable_contexts(self, n=None):
         """Disable the last n enabled contexts.
         """
         if n is None:
             n = len(self._contexts)
         self._active_ctx.remove_contexts(n)
+        self._build_cache()
 
     @contextmanager
     def context(self, *names, **kwargs):
         """Used as a context manager, this function enables to activate a context
         which is removed after usage.
 
         :param names: name of the context.
@@ -1219,15 +1247,14 @@
 
         src_dim = self._get_dimensionality(input_units)
 
         ret = super(ContextRegistry, self)._get_compatible_units(input_units, group_or_system)
 
         if self._active_ctx:
             nodes = find_connected_nodes(self._active_ctx.graph, src_dim)
-            ret = set()
             if nodes:
                 for node in nodes:
                     ret |= self._dimensional_equivalents[node]
 
         return ret
 
 
@@ -1428,15 +1455,15 @@
 
         return ret
 
 
 class UnitRegistry(SystemRegistry, ContextRegistry, NonMultiplicativeRegistry):
     """The unit registry stores the definitions and relationships between units.
 
-    :param filename: path of the units definition file to load.
+    :param filename: path of the units definition file to load or line-iterable object.
                      Empty to load the default definition file.
                      None to leave the UnitRegistry empty.
     :param force_ndarray: convert any input, scalar or not to a numpy.ndarray.
     :param default_as_delta: In the context of a multiplication of units, interpret
                              non-multiplicative units as their *delta* counterparts.
     :param autoconvert_offset_to_baseunit: If True converts offset units in quantites are
                                            converted to their base units in multiplicative
@@ -1463,14 +1490,23 @@
         """Builds dimensionless quantities using the Buckingham π theorem
         :param quantities: mapping between variable name and units
         :type quantities: dict
         :return: a list of dimensionless quantities expressed as dicts
         """
         return pi_theorem(quantities, self)
 
+    def setup_matplotlib(self, enable=True):
+        """Set up handlers for matplotlib's unit support.
+        :param enable: whether support should be enabled or disabled
+        :type enable: bool
+        """
+        # Delays importing matplotlib until it's actually requested
+        from .matplotlib import setup_matplotlib_handlers
+        setup_matplotlib_handlers(self, enable)
+
     wraps = registry_helpers.wraps
 
     check = registry_helpers.check
 
 
 class LazyRegistry(object):
```

### Comparing `Pint-0.8.1/pint/registry_helpers.py` & `Pint-0.9/pint/registry_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 import functools
 
 from .compat import string_types, zip_longest
 from .errors import DimensionalityError
 from .util import to_units_container, UnitsContainer
 
+try:
+    from inspect import signature
+except ImportError:
+    # Python2 does not have the inspect library. Import the backport.
+    from funcsigs import signature
+
 
 def _replace_units(original_units, values_by_name):
     """Convert a unit compatible type to a UnitsContainer.
 
     :param original_units: a UnitsContainer instance.
     :param values_by_name: a map between original names and the new values.
     """
@@ -114,20 +120,34 @@
                 new_values[ndx] = ureg._convert(values[ndx]._magnitude,
                                                 values[ndx]._units,
                                                 args_as_uc[ndx][0])
             else:
                 if strict:
                     raise ValueError('A wrapped function using strict=True requires '
                                      'quantity for all arguments with not None units. '
-                                     '(error found for {0}, {1})'.format(args_as_uc[ndx][0], new_values[ndx]))
+                                     '(error found for {}, {})'.format(args_as_uc[ndx][0], new_values[ndx]))
 
         return new_values, values_by_name
 
     return _converter
 
+def _apply_defaults(func, args, kwargs):
+    """Apply default keyword arguments.
+
+    Named keywords may have been left blank. This function applies the default
+    values so that every argument is defined.
+    """
+
+    sig = signature(func)
+    bound_arguments = sig.bind(*args, **kwargs)
+    for param in sig.parameters.values():
+        if param.name not in bound_arguments.arguments:
+            bound_arguments.arguments[param.name] = param.default
+    args = [bound_arguments.arguments[key] for key in sig.parameters.keys()]
+    return args, {} 
 
 def wraps(ureg, ret, args, strict=True):
     """Wraps a function to become pint-aware.
 
     Use it when a function requires a numerical value but in some specific
     units. The wrapper function will take a pint quantity, convert to the units
     specified in `args` and then call the wrapped function with the resulting
@@ -161,14 +181,16 @@
     def decorator(func):
         assigned = tuple(attr for attr in functools.WRAPPER_ASSIGNMENTS if hasattr(func, attr))
         updated = tuple(attr for attr in functools.WRAPPER_UPDATES if hasattr(func, attr))
 
         @functools.wraps(func, assigned=assigned, updated=updated)
         def wrapper(*values, **kw):
 
+            values, kw = _apply_defaults(func, values, kw)
+                
             # In principle, the values are used as is
             # When then extract the magnitudes when needed.
             new_values, values_by_name = converter(ureg, values, strict)
 
             result = func(*new_values, **kw)
 
             if container:
@@ -197,22 +219,31 @@
 
     :param ureg: a UnitRegistry instance.
     :param args: iterable of input units.
     :return: the wrapped function.
     :raises:
         :class:`DimensionalityError` if the parameters don't match dimensions
     """
-    dimensions = [ureg.get_dimensionality(dim) for dim in args]
+    dimensions = [ureg.get_dimensionality(dim) if dim is not None else None for dim in args]
 
     def decorator(func):
         assigned = tuple(attr for attr in functools.WRAPPER_ASSIGNMENTS if hasattr(func, attr))
         updated = tuple(attr for attr in functools.WRAPPER_UPDATES if hasattr(func, attr))
 
         @functools.wraps(func, assigned=assigned, updated=updated)
-        def wrapper(*values, **kwargs):
-            for dim, value in zip_longest(dimensions, values):
-                if dim and value.dimensionality != dim:
+        def wrapper(*args, **kwargs):
+            list_args, empty = _apply_defaults(func, args, kwargs)
+            if len(dimensions) > len(list_args):
+                raise TypeError("%s takes %i parameters, but %i dimensions were passed"
+                % (func.__name__, len(list_args), len(dimensions)))
+            for dim, value in zip(dimensions, list_args):
+
+                if dim is None:
+                    continue
+
+                if not ureg.Quantity(value).check(dim):
+                    val_dim = ureg.get_dimensionality(value)
                     raise DimensionalityError(value, 'a quantity of',
-                                              value.dimensionality, dim)
-            return func(*values, **kwargs)
+                                              val_dim, dim)
+            return func(*args, **kwargs)
         return wrapper
     return decorator
```

### Comparing `Pint-0.8.1/pint/systems.py` & `Pint-0.9/pint/systems.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         if self._computed_members is None:
             self._computed_members = set()
 
             for group_name in self._used_groups:
                 try:
                     self._computed_members |= d[group_name].members
                 except KeyError:
-                    logger.warning('Could not resolve {0} in System {1}'.format(group_name, self.name))
+                    logger.warning('Could not resolve {} in System {}'.format(group_name, self.name))
 
             self._computed_members = frozenset(self._computed_members)
 
         return self._computed_members
 
     def invalidate_members(self):
         """Invalidate computed members in this Group and all parent nodes.
@@ -339,15 +339,15 @@
         """
         self._used_groups -= set(group_names)
 
         self.invalidate_members()
 
     def format_babel(self, locale):
         """translate the name of the system
-        
+
         :type locale: Locale
         """
         if locale and self.name in _babel_systems:
             name = _babel_systems[self.name]
             locale = Loc.parse(locale)
             return locale.measurement_systems[name]
         return self.name
```

### Comparing `Pint-0.8.1/pint/testsuite/__init__.py` & `Pint-0.9/pint/testsuite/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from __future__ import division, unicode_literals, print_function, absolute_import
 
 import doctest
 import logging
 import os
 import sys
+import unittest
 
 from contextlib import contextmanager
 
 from pint.compat import ndarray, np
 
 from pint import logger, UnitRegistry
 from pint.quantity import _Quantity
-from pint.testsuite.compat import unittest
 from pint.testsuite.helpers import PintOutputChecker
 from logging.handlers import BufferingHandler
 
 
 class TestHandler(BufferingHandler):
 
     def __init__(self, only_warnings=False):
```

### Comparing `Pint-0.8.1/pint/testsuite/helpers.py` & `Pint-0.9/pint/testsuite/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from __future__ import division, unicode_literals, print_function, absolute_import
 
 
 import doctest
 from distutils.version import StrictVersion
 import re
+import unittest
 
 from pint.compat import HAS_NUMPY, HAS_PROPER_BABEL, HAS_UNCERTAINTIES, NUMPY_VER, PYTHON3
-from pint.testsuite.compat import unittest
 
 
 def requires_numpy18():
     if not HAS_NUMPY:
         return unittest.skip('Requires NumPy')
     return unittest.skipUnless(StrictVersion(NUMPY_VER) >= StrictVersion('1.8'), 'Requires NumPy >= 1.8')
```

### Comparing `Pint-0.8.1/pint/testsuite/parameterized.py` & `Pint-0.9/pint/testsuite/parameterized.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,17 @@
 #                ("3+5", 8),
 #                ("6*9", 54),
 #            ]
 #        )
 #        def test_eval(self, input, expected_output):
 #            self.assertEqual(eval(input), expected_output)
 
-from pint.testsuite.compat import unittest
-
 from functools import wraps
 import collections
-
+import unittest
 
 def add_metaclass(metaclass):
     """Class decorator for creating a class with a metaclass."""
     def wrapper(cls):
         orig_vars = cls.__dict__.copy()
         orig_vars.pop('__dict__', None)
         orig_vars.pop('__weakref__', None)
```

### Comparing `Pint-0.8.1/pint/testsuite/test_babel.py` & `Pint-0.9/pint/testsuite/test_babel.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_contexts.py` & `Pint-0.9/pint/testsuite/test_contexts.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,52 +15,52 @@
     a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[time]': -1})
     d = Context('lc')
     d.add_transformation(a, b, lambda ureg, x: ureg.speed_of_light / x)
     d.add_transformation(b, a, lambda ureg, x: ureg.speed_of_light / x)
 
     ureg.add_context(d)
 
-    a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[current]': -1})
+    a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[current]': 1})
     d = Context('ab')
-    d.add_transformation(a, b, lambda ureg, x: 1 / x)
-    d.add_transformation(b, a, lambda ureg, x: 1 / x)
+    d.add_transformation(a, b, lambda ureg, x: ureg.ampere * ureg.meter / x)
+    d.add_transformation(b, a, lambda ureg, x: ureg.ampere * ureg.meter / x)
 
     ureg.add_context(d)
 
 
 def add_arg_ctxs(ureg):
     a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[time]': -1})
     d = Context('lc')
     d.add_transformation(a, b, lambda ureg, x, n: ureg.speed_of_light / x / n)
     d.add_transformation(b, a, lambda ureg, x, n: ureg.speed_of_light / x / n)
 
     ureg.add_context(d)
 
-    a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[current]': -1})
+    a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[current]': 1})
     d = Context('ab')
-    d.add_transformation(a, b, lambda ureg, x: 1 / x)
-    d.add_transformation(b, a, lambda ureg, x: 1 / x)
+    d.add_transformation(a, b, lambda ureg, x: ureg.ampere * ureg.meter / x)
+    d.add_transformation(b, a, lambda ureg, x: ureg.ampere * ureg.meter / x)
 
     ureg.add_context(d)
 
 
 def add_argdef_ctxs(ureg):
     a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[time]': -1})
     d = Context('lc', defaults=dict(n=1))
     assert d.defaults == dict(n=1)
 
     d.add_transformation(a, b, lambda ureg, x, n: ureg.speed_of_light / x / n)
     d.add_transformation(b, a, lambda ureg, x, n: ureg.speed_of_light / x / n)
 
     ureg.add_context(d)
 
-    a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[current]': -1})
+    a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[current]': 1})
     d = Context('ab')
-    d.add_transformation(a, b, lambda ureg, x: 1 / x)
-    d.add_transformation(b, a, lambda ureg, x: 1 / x)
+    d.add_transformation(a, b, lambda ureg, x: ureg.ampere * ureg.meter / x)
+    d.add_transformation(b, a, lambda ureg, x: ureg.ampere * ureg.meter / x)
 
     ureg.add_context(d)
 
 
 def add_sharedargdef_ctxs(ureg):
     a, b = UnitsContainer({'[length]': 1}), UnitsContainer({'[time]': -1})
     d = Context('lc', defaults=dict(n=1))
@@ -118,15 +118,15 @@
         self.assertFalse(ureg._active_ctx.graph)
 
     def test_graph(self):
         ureg = UnitRegistry()
         add_ctxs(ureg)
         l = UnitsContainer({'[length]': 1.})
         t = UnitsContainer({'[time]': -1.})
-        c = UnitsContainer({'[current]': -1.})
+        c = UnitsContainer({'[current]': 1.})
 
         g_sp = defaultdict(set)
         g_sp.update({l: set((t,)),
                      t: set((l,))})
 
         g_ab = defaultdict(set)
         g_ab.update({l: set((c,)),
@@ -161,15 +161,15 @@
             self.assertEqual(ureg._active_ctx.graph, g)
 
     def test_graph_enable(self):
         ureg = UnitRegistry()
         add_ctxs(ureg)
         l = UnitsContainer({'[length]': 1.})
         t = UnitsContainer({'[time]': -1.})
-        c = UnitsContainer({'[current]': -1.})
+        c = UnitsContainer({'[current]': 1.})
 
         g_sp = defaultdict(set)
         g_sp.update({l: set((t,)),
                      t: set((l,))})
 
         g_ab = defaultdict(set)
         g_ab.update({l: set((c,)),
@@ -274,31 +274,44 @@
         ureg = UnitRegistry()
 
         add_ctxs(ureg)
 
         q = 500 * ureg.meter
         s = (ureg.speed_of_light / q).to('Hz')
 
+        meter_units = ureg.get_compatible_units(ureg.meter)
+        hertz_units = ureg.get_compatible_units(ureg.hertz)
+
         self.assertRaises(ValueError, q.to, 'Hz')
         with ureg.context('lc'):
             self.assertEqual(q.to('Hz'), s)
+            self.assertEqual(ureg.get_compatible_units(q), meter_units | hertz_units)
         self.assertRaises(ValueError, q.to, 'Hz')
+        self.assertEqual(ureg.get_compatible_units(q), meter_units)
+
 
     def test_multiple_context(self):
         ureg = UnitRegistry()
 
         add_ctxs(ureg)
 
         q = 500 * ureg.meter
         s = (ureg.speed_of_light / q).to('Hz')
 
+        meter_units = ureg.get_compatible_units(ureg.meter)
+        hertz_units = ureg.get_compatible_units(ureg.hertz)
+        ampere_units = ureg.get_compatible_units(ureg.ampere)
+
         self.assertRaises(ValueError, q.to, 'Hz')
         with ureg.context('lc', 'ab'):
             self.assertEqual(q.to('Hz'), s)
+            self.assertEqual(ureg.get_compatible_units(q), meter_units | hertz_units | ampere_units)
         self.assertRaises(ValueError, q.to, 'Hz')
+        self.assertEqual(ureg.get_compatible_units(q), meter_units)
+
 
     def test_nested_context(self):
         ureg = UnitRegistry()
 
         add_ctxs(ureg)
 
         q = 500 * ureg.meter
@@ -608,22 +621,40 @@
                     if x == 1:
                         a = a.to_base_units()
                         b = b.to_base_units()
                     da, db = Context.__keytransform__(a.dimensionality,
                                                       b.dimensionality)
                     p = find_shortest_path(ureg._active_ctx.graph, da, db)
                     self.assertTrue(p)
-                    msg = '{0} <-> {1}'.format(a, b)
+                    msg = '{} <-> {}'.format(a, b)
                     # assertAlmostEqualRelError converts second to first
                     self.assertQuantityAlmostEqual(b, a, rtol=0.01, msg=msg)
 
 
         for a, b in itertools.product(eq, eq):
             self.assertQuantityAlmostEqual(a.to(b.units, 'sp'), b, rtol=0.01)
 
+    def test_textile(self):
+        ureg = self.ureg
+        qty_direct = 1.331 * ureg.tex
+        with self.assertRaises(errors.DimensionalityError):
+            qty_indirect = qty_direct.to('Nm')
+
+        with ureg.context('textile'):
+            from pint.util import find_shortest_path
+            qty_indirect = qty_direct.to('Nm')
+            a = qty_direct.to_base_units()
+            b = qty_indirect.to_base_units()
+            da, db = Context.__keytransform__(a.dimensionality,
+                                              b.dimensionality)
+            p = find_shortest_path(ureg._active_ctx.graph, da, db)
+            self.assertTrue(p)
+            msg = '{} <-> {}'.format(a, b)
+            self.assertQuantityAlmostEqual(b, a, rtol=0.01, msg=msg)
+
     def test_decorator(self):
         ureg = self.ureg
 
         a = 532. * ureg.nm
         with ureg.context('sp'):
             b = a.to('terahertz')
 
@@ -652,8 +683,8 @@
 
         @ureg.with_context('sp')
         @ureg.check('[length]')
         def g(wl):
             return wl.to('terahertz')
 
         self.assertEqual(b, f(a))
-        self.assertEqual(b, g(a))
+        self.assertEqual(b, g(a))
```

### Comparing `Pint-0.8.1/pint/testsuite/test_converters.py` & `Pint-0.9/pint/testsuite/test_converters.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_definitions.py` & `Pint-0.9/pint/testsuite/test_definitions.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_errors.py` & `Pint-0.9/pint/testsuite/test_errors.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_formatter.py` & `Pint-0.9/pint/testsuite/test_formatter.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_infer_base_unit.py` & `Pint-0.9/pint/testsuite/test_infer_base_unit.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_issues.py` & `Pint-0.9/pint/testsuite/test_issues.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import division, unicode_literals, print_function, absolute_import
 
 import math
 import copy
+import unittest
 
 from pint import UnitRegistry
 from pint.unit import UnitsContainer
 from pint.util import ParserHelper
 
 from pint.compat import np, long_type
 from pint.errors import UndefinedUnitError, DimensionalityError
 from pint.testsuite import QuantityTestCase, helpers
-from pint.testsuite.compat import unittest
 
 
 class TestIssues(QuantityTestCase):
 
     FORCE_NDARRAY = False
 
     def setup(self):
@@ -35,15 +35,14 @@
         self.assertEqual(x, ureg.Quantity(10, {'%': 1}))
         y = ureg.parse_expression('10 ‰')
         self.assertEqual(y, ureg.Quantity(10, {'‰': 1}))
         self.assertEqual(x.to('‰'), ureg.Quantity(1, {'‰': 1}))
 
     def test_issue29(self):
         ureg = UnitRegistry()
-        ureg.define('molar = mole / liter = M')
         t = 4 * ureg('mM')
         self.assertEqual(t.magnitude, 4)
         self.assertEqual(t._units, UnitsContainer(millimolar=1))
         self.assertEqual(t.to('mole / liter'), 4e-3 * ureg('M'))
 
     def test_issue52(self):
         u1 = UnitRegistry()
@@ -557,8 +556,124 @@
         self.assertEquals(z, ureg.Quantity(1., 'meter * kilogram'))
 
     def test_issue483(self):
         ureg = self.ureg
         a = np.asarray([1, 2, 3])
         q = [1, 2, 3] * ureg.dimensionless
         p = (q ** q).m
-        np.testing.assert_array_equal(p, a ** a)
+        np.testing.assert_array_equal(p, a ** a)
+
+    def test_issue532(self):
+        ureg = self.ureg
+
+        @ureg.check(ureg(''))
+        def f(x):
+            return 2 * x
+
+        self.assertEqual(f(ureg.Quantity(1, '')), 2)
+        self.assertRaises(DimensionalityError, f, ureg.Quantity(1, 'm'))
+
+    def test_issue625a(self):
+        try:
+            from inspect import signature
+        except ImportError:
+            # Python2 does not have the inspect library. Import the backport.
+            from funcsigs import signature
+
+        ureg = UnitRegistry()
+        Q_ = ureg.Quantity
+        from math import sqrt
+
+        @ureg.wraps(ureg.second, (ureg.meters, ureg.meters/ureg.second**2))
+        def calculate_time_to_fall(height, gravity=Q_(9.8, 'm/s^2')):
+            """Calculate time to fall from a height h with a default gravity.
+
+            By default, the gravity is assumed to be earth gravity,
+            but it can be modified.
+
+            d = .5 * g * t**2
+            t = sqrt(2 * d / g)
+            """
+            return sqrt(2 * height / gravity)
+
+        lunar_module_height = Q_(10, 'm')
+        t1 = calculate_time_to_fall(lunar_module_height)
+        print(t1)
+        self.assertAlmostEqual(t1, Q_(1.4285714285714286, 's'))
+
+        moon_gravity = Q_(1.625, 'm/s^2')
+        t2 = calculate_time_to_fall(lunar_module_height, moon_gravity)
+        self.assertAlmostEqual(t2, Q_(3.508232077228117, 's'))
+
+    def test_issue625b(self):
+        try:
+            from inspect import signature
+        except ImportError:
+            # Python2 does not have the inspect library. Import the backport.
+            from funcsigs import signature
+
+        ureg = UnitRegistry()
+        Q_ = ureg.Quantity
+
+        @ureg.wraps('=A*B', ('=A', '=B'))
+        def get_displacement(time, rate=Q_(1, 'm/s')):
+            """Calculates displacement from a duration and default rate.
+            """
+            return time * rate
+
+        d1 = get_displacement(Q_(2, 's'))
+        self.assertAlmostEqual(d1, Q_(2, 'm'))
+
+        d2 = get_displacement(Q_(2, 's'), Q_(1, 'deg/s'))
+        self.assertAlmostEqual(d2, Q_(2,' deg'))
+
+    def test_issue625c(self):        
+        try:
+            from inspect import signature
+        except ImportError:
+            # Python2 does not have the inspect library. Import the backport.
+            from funcsigs import signature
+
+        u = UnitRegistry()
+
+        @u.wraps('=A*B*C', ('=A', '=B', '=C'))
+        def get_product(a=2*u.m, b=3*u.m, c=5*u.m):
+            return a*b*c
+
+        self.assertEqual(get_product(a=3*u.m), 45*u.m**3)
+        self.assertEqual(get_product(b=2*u.m), 20*u.m**3)
+        self.assertEqual(get_product(c=1*u.dimensionless), 6*u.m**2)
+
+    def test_issue655a(self):
+        ureg = UnitRegistry()
+        distance = 1 * ureg.m
+        time = 1 * ureg.s
+        velocity = distance / time
+        self.assertEqual(distance.check('[length]'), True)
+        self.assertEqual(distance.check('[time]'), False)
+        self.assertEqual(velocity.check('[length] / [time]'), True)
+        self.assertEqual(velocity.check('1 / [time] * [length]'), True)
+
+    def test_issue(self):
+        import math
+        try:
+            from inspect import signature
+        except ImportError:
+            # Python2 does not have the inspect library. Import the backport
+            from funcsigs import signature
+
+        ureg = UnitRegistry()
+        Q_ = ureg.Quantity
+        @ureg.check('[length]', '[length]/[time]^2')
+        def pendulum_period(length, G=Q_(1, 'standard_gravity')):
+            print(length)
+            return (2*math.pi*(length/G)**.5).to('s')
+        l = 1 * ureg.m
+        # Assume earth gravity
+        t = pendulum_period(l)
+        self.assertAlmostEqual(t, Q_('2.0064092925890407 second'))
+        # Use moon gravity
+        moon_gravity = Q_(1.625, 'm/s^2')
+        t = pendulum_period(l, moon_gravity)
+        self.assertAlmostEqual(t, Q_('4.928936075204336 second'))
+
+
```

### Comparing `Pint-0.8.1/pint/testsuite/test_measurement.py` & `Pint-0.9/pint/testsuite/test_measurement.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_numpy.py` & `Pint-0.9/pint/testsuite/test_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import division, unicode_literals, print_function, absolute_import
 
 import copy
 import operator as op
+import unittest
 
 from pint import DimensionalityError, set_application_registry
 from pint.compat import np
 from pint.testsuite import QuantityTestCase, helpers
-from pint.testsuite.compat import unittest
 from pint.testsuite.test_umath import TestUFuncs
 
 
 @helpers.requires_numpy()
 class TestNumpyMethods(QuantityTestCase):
 
     FORCE_NDARRAY = True
@@ -109,14 +109,20 @@
     def test_searchsorted(self):
         q = self.q.flatten()
         np.testing.assert_array_equal(q.searchsorted([1.5, 2.5] * self.ureg.m),
                                       [1, 2])
         q = self.q.flatten()
         self.assertRaises(ValueError, q.searchsorted, [1.5, 2.5])
 
+    def test_searchsorted_numpy_func(self):
+        """Test searchsorted as numpy function."""
+        q = self.q.flatten()
+        np.testing.assert_array_equal(np.searchsorted(q, [1.5, 2.5] * self.ureg.m),
+                                      [1, 2])
+
     def test_nonzero(self):
         q = [1, 0, 5, 6, 0, 9] * self.ureg.m
         np.testing.assert_array_equal(q.nonzero()[0], [0, 2, 3, 5])
 
     def test_max(self):
         self.assertEqual(self.q.max(), 4*self.ureg.m)
 
@@ -418,15 +424,15 @@
         self._test2(np.right_shift,
                     self.q1,
                     (self.qless, 2),
                     (self.q1, self.q2, self.qs, ),
                     'same')
 
 
-class TestNDArrayQunatityMath(QuantityTestCase):
+class TestNDArrayQuantityMath(QuantityTestCase):
 
     @helpers.requires_numpy()
     def test_exponentiation_array_exp(self):
         arr = np.array(range(3), dtype=np.float)
         q = self.Q_(arr, 'meter')
 
         for op_ in [op.pow, op.ipow]:
```

### Comparing `Pint-0.8.1/pint/testsuite/test_pint_eval.py` & `Pint-0.9/pint/testsuite/test_pint_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import division, unicode_literals, print_function, absolute_import
+import unittest
 
 from pint.compat import tokenizer
 from pint.pint_eval import build_eval_tree
-from pint.testsuite.compat import unittest
 
 
 class TestPintEval(unittest.TestCase):
 
     def _test_one(self, input_text, parsed):
         self.assertEqual(build_eval_tree(tokenizer(input_text)).to_string(), parsed)
```

### Comparing `Pint-0.8.1/pint/testsuite/test_pitheorem.py` & `Pint-0.9/pint/testsuite/test_pitheorem.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/testsuite/test_quantity.py` & `Pint-0.9/pint/testsuite/test_quantity.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,14 +86,30 @@
         self.assertEqual(self.Q_(1000, 'millimeter/min'), self.Q_(1000/60, 'millimeter/s'))
 
     def test_quantity_repr(self):
         x = self.Q_(4.2, UnitsContainer(meter=1))
         self.assertEqual(str(x), '4.2 meter')
         self.assertEqual(repr(x), "<Quantity(4.2, 'meter')>")
 
+    def test_quantity_hash(self):
+        x = self.Q_(4.2, 'meter')
+        x2 = self.Q_(4200, 'millimeter')
+        y = self.Q_(2, 'second')
+        z = self.Q_(0.5, 'hertz')
+        self.assertEqual(hash(x), hash(x2))
+
+        # Dimensionless equality
+        self.assertEqual(hash(y * z), hash(1.0))
+
+        # Dimensionless equality from a different unit registry
+        ureg2 = UnitRegistry(force_ndarray=self.FORCE_NDARRAY)
+        y2 = ureg2.Quantity(2, 'second')
+        z2 = ureg2.Quantity(0.5, 'hertz')
+        self.assertEqual(hash(y * z), hash(y2 * z2))
+
     def test_quantity_format(self):
         x = self.Q_(4.12345678, UnitsContainer(meter=2, kilogram=1, second=-1))
         for spec, result in (('{0}', str(x)), ('{0!s}', str(x)), ('{0!r}', repr(x)),
                              ('{0.magnitude}',  str(x.magnitude)), ('{0.units}',  str(x.units)),
                              ('{0.magnitude!s}',  str(x.magnitude)), ('{0.units!s}',  str(x.units)),
                              ('{0.magnitude!r}',  repr(x.magnitude)), ('{0.units!r}',  repr(x.units)),
                              ('{0:.4f}', '{0:.4f} {1!s}'.format(x.magnitude, x.units)),
@@ -146,14 +162,56 @@
                              ('P~', '4.12345678 kg·m²/s'),
                              ('H~', '4.12345678 kg m<sup>2</sup>/s'),
                              ('C~', '4.12345678 kg*m**2/s'),
                              ):
             ureg.default_format = spec
             self.assertEqual('{0}'.format(x), result)
 
+    def test_exponent_formatting(self):
+        ureg = UnitRegistry()
+        x = ureg.Quantity(1e20, UnitsContainer(meter=1))
+        self.assertEqual("{:~H}".format(x), "1×10<sup>20</sup> m")
+        self.assertEqual("{:~L}".format(x), r"1\times 10^{20}\ \mathrm{m}")
+        x /= 1e40
+        self.assertEqual("{:~H}".format(x), "1×10<sup>-20</sup> m")
+        self.assertEqual("{:~L}".format(x), r"1\times 10^{-20}\ \mathrm{m}")
+
+    def test_ipython(self):
+        alltext = []
+
+        class Pretty(object):
+            @staticmethod
+            def text(text):
+                alltext.append(text)
+
+            @classmethod
+            def pretty(cls, data):
+                try:
+                    data._repr_pretty_(cls, False)
+                except AttributeError:
+                    alltext.append(str(data))
+
+        ureg = UnitRegistry()
+        x = 3.5 * ureg.Unit(UnitsContainer(meter=2, kilogram=1, second=-1))
+        self.assertEqual(x._repr_html_(),
+                         "3.5 kilogram meter<sup>2</sup>/second")
+        self.assertEqual(x._repr_latex_(),
+                         r'$3.5\ \frac{\mathrm{kilogram} \cdot '
+                         r'\mathrm{meter}^{2}}{\mathrm{second}}$')
+        x._repr_pretty_(Pretty, False)
+        self.assertEqual("".join(alltext), "3.5 kilogram·meter²/second")
+        ureg.default_format = "~"
+        self.assertEqual(x._repr_html_(), "3.5 kg m<sup>2</sup>/s")
+        self.assertEqual(x._repr_latex_(),
+                         r'$3.5\ \frac{\mathrm{kg} \cdot '
+                         r'\mathrm{m}^{2}}{\mathrm{s}}$')
+        alltext = []
+        x._repr_pretty_(Pretty, False)
+        self.assertEqual("".join(alltext), "3.5 kg·m²/s")
+
     def test_to_base_units(self):
         x = self.Q_('1*inch')
         self.assertQuantityAlmostEqual(x.to_base_units(), self.Q_(0.0254, 'meter'))
         x = self.Q_('1*inch*inch')
         self.assertQuantityAlmostEqual(x.to_base_units(), self.Q_(0.0254 ** 2.0, 'meter*meter'))
         x = self.Q_('1*inch/minute')
         self.assertQuantityAlmostEqual(x.to_base_units(), self.Q_(0.0254 / 60., 'meter/second'))
@@ -185,14 +243,34 @@
             q = self.Q_(a, src)
             qac = self.Q_(ac, src).to(dst)
             r = q.to(dst)
             self.assertQuantityAlmostEqual(qac, r)
             self.assertIsNot(r, q)
             self.assertIsNot(r._magnitude, a)
 
+    def test_convert_from(self):
+        x = self.Q_('2*inch')
+        meter = self.ureg.meter
+
+        # from quantity
+        self.assertQuantityAlmostEqual(meter.from_(x), self.Q_(2. * 0.0254, 'meter'))
+        self.assertQuantityAlmostEqual(meter.m_from(x), 2. * 0.0254)
+
+        # from unit
+        self.assertQuantityAlmostEqual(meter.from_(self.ureg.inch), self.Q_(0.0254, 'meter'))
+        self.assertQuantityAlmostEqual(meter.m_from(self.ureg.inch), 0.0254)
+
+        # from number
+        self.assertQuantityAlmostEqual(meter.from_(2, strict=False), self.Q_(2., 'meter'))
+        self.assertQuantityAlmostEqual(meter.m_from(2, strict=False), 2.)
+
+        # from number (strict mode)
+        self.assertRaises(ValueError, meter.from_, 2)
+        self.assertRaises(ValueError, meter.m_from, 2)
+
     @helpers.requires_numpy()
     def test_retain_unit(self):
         # Test that methods correctly retain units and do not degrade into
         # ordinary ndarrays.  List contained in __copy_units.
         a = np.ones((3, 2))
         q = self.Q_(a, "km")
         self.assertEqual(q.u, q.reshape(2, 3).u)
@@ -303,14 +381,20 @@
         self.compareQuantity_compact(100e9/ureg.m, 100/ureg.nm)
 
     def test_inverse_square_units(self):
         ureg = self.ureg
         self.compareQuantity_compact(1/ureg.m**2, 1/ureg.m**2)
         self.compareQuantity_compact(1e11/ureg.m**2, 1e5/ureg.mm**2)
 
+    def test_fractional_units(self):
+        ureg = self.ureg
+        # Typing denominator first to provoke potential error
+        self.compareQuantity_compact(20e3*ureg('hr^(-1) m'),
+            20*ureg.km/ureg.hr)
+
     def test_fractional_exponent_units(self):
         ureg = self.ureg
         self.compareQuantity_compact(1*ureg.m**0.5, 1*ureg.m**0.5)
         self.compareQuantity_compact(1e-2*ureg.m**0.5, 10*ureg.um**0.5)
 
     def test_derived_units(self):
         ureg = self.ureg
@@ -1203,14 +1287,18 @@
         ureg = UnitRegistry(auto_reduce_dimensions=True)
         x = (10 * ureg.feet) / (3 * ureg.inches)
         self.assertEqual(x.units, UnitsContainer({}))
         ureg = UnitRegistry(auto_reduce_dimensions=False)
         x = (10 * ureg.feet) / (3 * ureg.inches)
         self.assertEqual(x.units, ureg.feet / ureg.inches)
 
+    def test_nocoerce_creation(self):
+        ureg = UnitRegistry(auto_reduce_dimensions=True)
+        x = 1 * ureg.foot
+        self.assertEqual(x.units, ureg.foot)
 
 class TestTimedelta(QuantityTestCase):
     def test_add_sub(self):
         d = datetime.datetime(year=1968, month=1, day=10, hour=3, minute=42, second=24)
         after = d + 3 * self.ureg.second
         self.assertEqual(d + datetime.timedelta(seconds=3), after)
         after = 3 * self.ureg.second + d
@@ -1230,7 +1318,111 @@
         self.assertEqual(d + datetime.timedelta(seconds=3), after)
         after = copy.copy(d)
         after -= 3 * self.ureg.second
         self.assertEqual(d - datetime.timedelta(seconds=3), after)
         after = 3 * self.ureg.second
         with self.assertRaises(DimensionalityError):
             after -= d
+
+
+class TestCompareZero(QuantityTestCase):
+    """This test case checks the special treatment that the zero value
+    receives in the comparisons: pint>=0.9 supports comparisons against zero
+    even for non-dimensionless quantities
+    """
+
+    def test_equal_zero(self):
+        ureg = self.ureg
+        ureg.autoconvert_offset_to_baseunit = False
+        self.assertTrue(ureg.Quantity(0, ureg.J) == 0)
+        self.assertFalse(ureg.Quantity(0, ureg.J) == ureg.Quantity(0, ''))
+        self.assertFalse(ureg.Quantity(5, ureg.J) == 0)
+
+    @helpers.requires_numpy()
+    def test_equal_zero_NP(self):
+        ureg = self.ureg
+        ureg.autoconvert_offset_to_baseunit = False
+        aeq = np.testing.assert_array_equal
+        aeq(ureg.Quantity(0, ureg.J) == np.zeros(3),
+            np.asarray([True, True, True]))
+        aeq(ureg.Quantity(5, ureg.J) == np.zeros(3),
+            np.asarray([False, False, False]))
+        aeq(ureg.Quantity(np.arange(3), ureg.J) == np.zeros(3),
+            np.asarray([True, False, False]))
+        self.assertFalse(ureg.Quantity(np.arange(4), ureg.J) == np.zeros(3))
+
+    def test_offset_equal_zero(self):
+        ureg =  self.ureg
+        ureg.autoconvert_offset_to_baseunit = False
+        q0 = ureg.Quantity(-273.15, 'degC')
+        q1 = ureg.Quantity(0, 'degC')
+        q2 = ureg.Quantity(5, 'degC')
+        self.assertRaises(OffsetUnitCalculusError, q0.__eq__, 0)
+        self.assertRaises(OffsetUnitCalculusError, q1.__eq__, 0)
+        self.assertRaises(OffsetUnitCalculusError, q2.__eq__, 0)
+        self.assertFalse(q0 == ureg.Quantity(0, ''))
+
+    def test_offset_autoconvert_equal_zero(self):
+        ureg =  self.ureg
+        ureg.autoconvert_offset_to_baseunit = True
+        q0 = ureg.Quantity(-273.15, 'degC')
+        q1 = ureg.Quantity(0, 'degC')
+        q2 = ureg.Quantity(5, 'degC')
+        self.assertTrue(q0 == 0)
+        self.assertFalse(q1 == 0)
+        self.assertFalse(q2 == 0)
+        self.assertFalse(q0 == ureg.Quantity(0, ''))
+
+    def test_gt_zero(self):
+        ureg = self.ureg
+        ureg.autoconvert_offset_to_baseunit = False
+        q0 = ureg.Quantity(0, 'J')
+        q0m = ureg.Quantity(0, 'm')
+        q0less = ureg.Quantity(0, '')
+        qpos = ureg.Quantity(5, 'J')
+        qneg = ureg.Quantity(-5, 'J')
+        self.assertTrue(qpos > q0)
+        self.assertTrue(qpos > 0)
+        self.assertFalse(qneg > 0)
+        self.assertRaises(DimensionalityError, qpos.__gt__, q0less)
+        self.assertRaises(DimensionalityError, qpos.__gt__, q0m)
+
+    @helpers.requires_numpy()
+    def test_gt_zero_NP(self):
+        ureg = self.ureg
+        ureg.autoconvert_offset_to_baseunit = False
+        qpos = ureg.Quantity(5, 'J')
+        qneg = ureg.Quantity(-5, 'J')
+        aeq = np.testing.assert_array_equal
+        aeq(qpos > np.zeros(3), np.asarray([True, True, True]))
+        aeq(qneg > np.zeros(3), np.asarray([False, False, False]))
+        aeq(ureg.Quantity(np.arange(-1, 2), ureg.J) > np.zeros(3),
+            np.asarray([False, False, True]))
+        aeq(ureg.Quantity(np.arange(-1, 2), ureg.J) > np.zeros(3),
+            np.asarray([False, False, True]))
+        self.assertRaises(ValueError,
+                          ureg.Quantity(np.arange(-1, 2), ureg.J).__gt__,
+                          np.zeros(4))
+
+    def test_offset_gt_zero(self):
+        ureg =  self.ureg
+        ureg.autoconvert_offset_to_baseunit = False
+        q0 = ureg.Quantity(-273.15, 'degC')
+        q1 = ureg.Quantity(0, 'degC')
+        q2 = ureg.Quantity(5, 'degC')
+        self.assertRaises(OffsetUnitCalculusError, q0.__gt__, 0)
+        self.assertRaises(OffsetUnitCalculusError, q1.__gt__, 0)
+        self.assertRaises(OffsetUnitCalculusError, q2.__gt__, 0)
+        self.assertRaises(DimensionalityError, q1.__gt__,
+                          ureg.Quantity(0, ''))
+
+    def test_offset_autoconvert_gt_zero(self):
+        ureg =  self.ureg
+        ureg.autoconvert_offset_to_baseunit = True
+        q0 = ureg.Quantity(-273.15, 'degC')
+        q1 = ureg.Quantity(0, 'degC')
+        q2 = ureg.Quantity(5, 'degC')
+        self.assertFalse(q0 > 0)
+        self.assertTrue(q1 > 0)
+        self.assertTrue(q2 > 0)
+        self.assertRaises(DimensionalityError, q1.__gt__,
+                          ureg.Quantity(0, ''))
```

### Comparing `Pint-0.8.1/pint/testsuite/test_systems.py` & `Pint-0.9/pint/testsuite/test_systems.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     def test_units_programatically(self):
         ureg, root = self._build_empty_reg_root()
         d  = ureg._groups
 
         self.assertEqual(root._used_groups, set())
         self.assertEqual(root._used_by, set())
         root.add_units('meter', 'second', 'meter')
-        self.assertEqual(root._unit_names, set(['meter', 'second']))
-        self.assertEqual(root.members, set(['meter', 'second']))
+        self.assertEqual(root._unit_names, {'meter', 'second'})
+        self.assertEqual(root.members, {'meter', 'second'})
 
-        self.assertEqual(set(d.keys()), set(['root']))
+        self.assertEqual(set(d.keys()), {'root'})
 
     def test_cyclic(self):
         ureg, root = self._build_empty_reg_root()
         g2 = ureg.Group('g2')
         g3 = ureg.Group('g3')
         g2.add_groups('g3')
 
@@ -40,56 +40,56 @@
         self.assertRaises(ValueError, g3.add_groups, 'root')
 
     def test_groups_programatically(self):
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
         g2 = ureg.Group('g2')
 
-        self.assertEqual(set(d.keys()), set(['root', 'g2']))
+        self.assertEqual(set(d.keys()), {'root', 'g2'})
 
-        self.assertEqual(root._used_groups, set(['g2']))
+        self.assertEqual(root._used_groups, {'g2'})
         self.assertEqual(root._used_by, set())
 
         self.assertEqual(g2._used_groups, set())
-        self.assertEqual(g2._used_by, set(['root']))
+        self.assertEqual(g2._used_by, {'root'})
 
 
     def test_simple(self):
         lines = ['@group mygroup',
                  'meter',
                  'second',
                  ]
 
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
 
         grp = ureg.Group.from_lines(lines, lambda x: None)
 
-        self.assertEqual(set(d.keys()), set(['root', 'mygroup']))
+        self.assertEqual(set(d.keys()), {'root', 'mygroup'})
 
         self.assertEqual(grp.name, 'mygroup')
-        self.assertEqual(grp._unit_names, set(['meter', 'second']))
+        self.assertEqual(grp._unit_names, {'meter', 'second'})
         self.assertEqual(grp._used_groups, set())
-        self.assertEqual(grp._used_by, set([root.name]))
+        self.assertEqual(grp._used_by, {root.name})
         self.assertEqual(grp.members, frozenset(['meter', 'second']))
 
     def test_using1(self):
         lines = ['@group mygroup using group1',
                  'meter',
                  'second',
                  ]
 
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
 
         g = ureg.Group('group1')
         grp = ureg.Group.from_lines(lines, lambda x: None)
         self.assertEqual(grp.name, 'mygroup')
-        self.assertEqual(grp._unit_names, set(['meter', 'second']))
-        self.assertEqual(grp._used_groups, set(['group1']))
+        self.assertEqual(grp._unit_names, {'meter', 'second'})
+        self.assertEqual(grp._used_groups, {'group1'})
         self.assertEqual(grp.members, frozenset(['meter', 'second']))
 
     def test_using2(self):
         lines = ['@group mygroup using group1,group2',
                  'meter',
                  'second',
                  ]
@@ -97,16 +97,16 @@
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
 
         ureg.Group('group1')
         ureg.Group('group2')
         grp = ureg.Group.from_lines(lines, lambda x: None)
         self.assertEqual(grp.name, 'mygroup')
-        self.assertEqual(grp._unit_names, set(['meter', 'second']))
-        self.assertEqual(grp._used_groups, set(['group1', 'group2']))
+        self.assertEqual(grp._unit_names, {'meter', 'second'})
+        self.assertEqual(grp._used_groups, {'group1', 'group2'})
         self.assertEqual(grp.members, frozenset(['meter', 'second']))
 
     def test_spaces(self):
         lines = ['@group   mygroup   using   group1 , group2',
                  ' meter ',
                  ' second  ',
                  ]
@@ -114,16 +114,16 @@
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
 
         ureg.Group('group1')
         ureg.Group('group2')
         grp = ureg.Group.from_lines(lines, lambda x: None)
         self.assertEqual(grp.name, 'mygroup')
-        self.assertEqual(grp._unit_names, set(['meter', 'second']))
-        self.assertEqual(grp._used_groups, set(['group1', 'group2']))
+        self.assertEqual(grp._unit_names, {'meter', 'second'})
+        self.assertEqual(grp._used_groups, {'group1', 'group2'})
         self.assertEqual(grp.members, frozenset(['meter', 'second']))
 
     def test_invalidate_members(self):
         lines = ['@group mygroup using group1',
                  'meter',
                  'second',
                  ]
@@ -210,28 +210,28 @@
                  'second',
                  ]
 
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
 
         s = ureg.System.from_lines(lines, lambda x: x)
-        s._used_groups = set(['root'])
+        s._used_groups = {'root'}
 
     def test_simple_using(self):
         lines = ['@system mks using g1',
                  'meter',
                  'kilogram',
                  'second',
                  ]
 
         ureg, root = self._build_empty_reg_root()
         d = ureg._groups
 
         s = ureg.System.from_lines(lines, lambda x: x)
-        s._used_groups = set(['root', 'g1'])
+        s._used_groups = {'root', 'g1'}
 
 
     def test_members_group(self):
         lines = ['@system mk',
                  'meter',
                  'kilogram',
                  ]
@@ -340,8 +340,8 @@
         c = ureg.get_base_units('kph', system=sysname)
         self.assertAlmostEqual(c[0], 0.6213, places=3)
         self.assertEqual(c[1], {'mph': 1})
 
     def test_members_nowarning(self):
         ureg = self.ureg
         for name in dir(ureg.sys):
-            s = dir(getattr(ureg.sys, name))
+            s = dir(getattr(ureg.sys, name))
```

### Comparing `Pint-0.8.1/pint/testsuite/test_umath.py` & `Pint-0.9/pint/testsuite/test_umath.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
     @property
     def qi(self):
         return np.asarray([1 + 1j, 2 + 2j, 3 + 3j, 4 + 4j]) * self.ureg.m
 
     def assertRaisesMsg(self, msg, ExcType, func, *args, **kwargs):
         try:
             func(*args, **kwargs)
-            self.assertFalse(True, msg='Exception {0} not raised {1}'.format(ExcType, msg))
+            self.assertFalse(True, msg='Exception {} not raised {}'.format(ExcType, msg))
         except ExcType as e:
             pass
         except Exception as e:
-            self.assertFalse(True, msg='{0} not raised but {1}\n{2}'.format(ExcType, e, msg))
+            self.assertFalse(True, msg='{} not raised but {}\n{}'.format(ExcType, e, msg))
 
     def _test1(self, func,  ok_with, raise_with=(), output_units='same', results=None, rtol=1e-6):
         """Test function that takes a single argument and returns Quantity.
 
         :param func: function callable.
         :param ok_with: iterables of values that work fine.
         :param raise_with: iterables of values that raise exceptions.
@@ -64,15 +64,15 @@
                         If None, the result will be obtained by applying
                         func to each ok_with value
         :param rtol: relative tolerance.
         """
         if results is None:
             results = [None, ] * len(ok_with)
         for x1, res in zip(ok_with, results):
-            err_msg = 'At {0} with {1}'.format(func.__name__, x1)
+            err_msg = 'At {} with {}'.format(func.__name__, x1)
             if output_units == 'same':
                 ou = x1.units
             elif isinstance(output_units, (int, float)):
                 ou = x1.units ** output_units
             else:
                 ou = output_units
 
@@ -81,15 +81,15 @@
                 res = func(x1.magnitude)
                 if ou is not None:
                     res = self.Q_(res, ou)
 
             self.assertQuantityAlmostEqual(qm, res, rtol=rtol, msg=err_msg)
 
         for x1 in raise_with:
-            self.assertRaisesMsg('At {0} with {1}'.format(func.__name__, x1),
+            self.assertRaisesMsg('At {} with {}'.format(func.__name__, x1),
                                  ValueError, func, x1)
 
     def _testn(self, func,  ok_with, raise_with=(), results=None):
         """Test function that takes a single argument and returns and ndarray (not a Quantity)
 
         :param func: function callable.
         :param ok_with: iterables of values that work fine.
@@ -117,15 +117,15 @@
                         func to each ok_with value
         :param rtol: relative tolerance.
         """
 
         if results is None:
             results = [None, ] * len(ok_with)
         for x1, res in zip(ok_with, results):
-            err_msg = 'At {0} with {1}'.format(func.__name__, x1)
+            err_msg = 'At {} with {}'.format(func.__name__, x1)
             qms = func(x1)
             if res is None:
                 res = func(x1.magnitude)
 
             for ndx, (qm, re, ou) in enumerate(zip(qms, res, output_units)):
                 if ou == 'same':
                     ou = x1.units
@@ -134,15 +134,15 @@
 
                 if ou is not None:
                     re = self.Q_(re, ou)
 
                 self.assertQuantityAlmostEqual(qm, re, rtol=rtol, msg=err_msg)
 
         for x1 in raise_with:
-            self.assertRaisesMsg('At {0} with {1}'.format(func.__name__, x1),
+            self.assertRaisesMsg('At {} with {}'.format(func.__name__, x1),
                                  ValueError, func, x1)
 
     def _test2(self, func, x1, ok_with, raise_with=(), output_units='same', rtol=1e-6, convert2=True):
         """Test function that takes two arguments and return a Quantity.
 
         :param func: function callable.
         :param x1: first argument of func.
@@ -155,15 +155,15 @@
                              'second': x1.units * ok_with[n]
                              None: no output units, the result should be an ndarray.
                              Other value will be parsed as unit.
         :param rtol: relative tolerance.
         :param convert2: if the ok_with[n] should be converted to x1.units.
         """
         for x2 in ok_with:
-            err_msg = 'At {0} with {1} and {2}'.format(func.__name__, x1, x2)
+            err_msg = 'At {} with {} and {}'.format(func.__name__, x1, x2)
             if output_units == 'same':
                 ou = x1.units
             elif output_units == 'prod':
                 ou = x1.units * x2.units
             elif output_units == 'div':
                 ou = x1.units / x2.units
             elif output_units == 'second':
@@ -181,15 +181,15 @@
             res = func(x1.magnitude, m2)
             if ou is not None:
                 res = self.Q_(res, ou)
 
             self.assertQuantityAlmostEqual(qm, res, rtol=rtol, msg=err_msg)
 
         for x2 in raise_with:
-            self.assertRaisesMsg('At {0} with {1} and {2}'.format(func.__name__, x1, x2),
+            self.assertRaisesMsg('At {} with {} and {}'.format(func.__name__, x1, x2),
                                  ValueError, func, x1, x2)
 
     def _testn2(self, func, x1, ok_with, raise_with=()):
         """Test function that takes two arguments and return a ndarray.
 
         :param func: function callable.
         :param x1: first argument of func.
@@ -609,15 +609,15 @@
                     (self.q1, self.qm, self.qless))
 
     def test_iscomplex(self):
         self._testn(np.iscomplex,
                     (self.q1, self.qm, self.qless))
 
     def test_isfinite(self):
-        self._testn(np.isreal,
+        self._testn(np.isfinite,
                     (self.q1, self.qm, self.qless))
 
     def test_isinf(self):
         self._testn(np.isinf,
                     (self.q1, self.qm, self.qless))
 
     def test_isnan(self):
```

### Comparing `Pint-0.8.1/pint/testsuite/test_unit.py` & `Pint-0.9/pint/testsuite/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     def test_creation(self):
         for arg in ('meter', UnitsContainer(meter=1), self.U_('m')):
             self.assertEqual(self.U_(arg)._units, UnitsContainer(meter=1))
         self.assertRaises(TypeError, self.U_, 1)
 
     def test_deepcopy(self):
-      x = self.U_(UnitsContainer(meter=1))
-      self.assertEqual(x, copy.deepcopy(x))
+        x = self.U_(UnitsContainer(meter=1))
+        self.assertEqual(x, copy.deepcopy(x))
 
     def test_unit_repr(self):
         x = self.U_(UnitsContainer(meter=1))
         self.assertEqual(str(x), 'meter')
         self.assertEqual(repr(x), "<Unit('meter')>")
 
     def test_unit_formatting(self):
@@ -59,14 +59,37 @@
                              ('H~', 'kg m<sup>2</sup>/s'),
                              ('C~', 'kg*m**2/s'),
                              ):
             ureg.default_format = spec
             self.assertEqual('{0}'.format(x), result,
                              'Failed for {0}, {1}'.format(spec, result))
 
+    def test_ipython(self):
+        alltext = []
+
+        class Pretty(object):
+            @staticmethod
+            def text(text):
+                alltext.append(text)
+
+        ureg = UnitRegistry()
+        x = ureg.Unit(UnitsContainer(meter=2, kilogram=1, second=-1))
+        self.assertEqual(x._repr_html_(), "kilogram meter<sup>2</sup>/second")
+        self.assertEqual(x._repr_latex_(), r'$\frac{\mathrm{kilogram} \cdot '
+                                           r'\mathrm{meter}^{2}}{\mathrm{second}}$')
+        x._repr_pretty_(Pretty, False)
+        self.assertEqual("".join(alltext), "kilogram·meter²/second")
+        ureg.default_format = "~"
+        self.assertEqual(x._repr_html_(), "kg m<sup>2</sup>/s")
+        self.assertEqual(x._repr_latex_(),
+                         r'$\frac{\mathrm{kg} \cdot \mathrm{m}^{2}}{\mathrm{s}}$')
+        alltext = []
+        x._repr_pretty_(Pretty, False)
+        self.assertEqual("".join(alltext), "kg·m²/s")
+
     def test_unit_mul(self):
         x = self.U_('m')
         self.assertEqual(x*1, self.Q_(1, 'm'))
         self.assertEqual(x*0.5, self.Q_(0.5, 'm'))
         self.assertEqual(x*self.Q_(1, 'm'), self.Q_(1, 'm**2'))
         self.assertEqual(1*x, self.Q_(1, 'm'))
 
@@ -201,15 +224,14 @@
         self.assertEqual(self.ureg.parse_expression('kilometer'), self.Q_(1, UnitsContainer(kilometer=1.)))
         #self.assertEqual(self.ureg._units['kilometer'], self.Q_(1000., UnitsContainer(meter=1.)))
 
     def test_parse_complex(self):
         self.assertEqual(self.ureg.parse_expression('kilometre'), self.Q_(1, UnitsContainer(kilometer=1.)))
         self.assertEqual(self.ureg.parse_expression('kilometres'), self.Q_(1, UnitsContainer(kilometer=1.)))
 
-
     def test_str_errors(self):
         self.assertEqual(str(UndefinedUnitError('rabbits')), "'{0!s}' is not defined in the unit registry".format('rabbits'))
         self.assertEqual(str(UndefinedUnitError(('rabbits', 'horses'))), "'{0!s}' are not defined in the unit registry".format(('rabbits', 'horses')))
         self.assertEqual(u(str(DimensionalityError('meter', 'second'))),
                          "Cannot convert from 'meter' to 'second'")
         self.assertEqual(str(DimensionalityError('meter', 'second', 'length', 'time')),
                          "Cannot convert from 'meter' (length) to 'second' (time)")
@@ -245,15 +267,15 @@
         parse = self.ureg.parse_units
         self.assertEqual(parse('kelvin', as_delta=True), UnitsContainer(kelvin=1))
         self.assertEqual(parse('kelvin', as_delta=False), UnitsContainer(kelvin=1))
         self.assertEqual(parse('kelvin**(-1)', as_delta=True), UnitsContainer(kelvin=-1))
         self.assertEqual(parse('kelvin**(-1)', as_delta=False), UnitsContainer(kelvin=-1))
         self.assertEqual(parse('kelvin**2', as_delta=True), UnitsContainer(kelvin=2))
         self.assertEqual(parse('kelvin**2', as_delta=False), UnitsContainer(kelvin=2))
-        self.assertEqual(parse('kelvin*meter', as_delta=True), UnitsContainer(kelvin=1, meter= 1))
+        self.assertEqual(parse('kelvin*meter', as_delta=True), UnitsContainer(kelvin=1, meter=1))
         self.assertEqual(parse('kelvin*meter', as_delta=False), UnitsContainer(kelvin=1, meter=1))
 
     def test_name(self):
         self.assertRaises(UndefinedUnitError, self.ureg.get_name, 'asdf')
 
     def test_symbol(self):
         self.assertRaises(UndefinedUnitError, self.ureg.get_symbol, 'asdf')
@@ -387,45 +409,45 @@
     def test_check(self):
         def func(x):
             return x
 
         ureg = self.ureg
 
         f0 = ureg.check('[length]')(func)
-        self.assertRaises(AttributeError, f0, 3.)
+        self.assertRaises(DimensionalityError, f0, 3.)
         self.assertEqual(f0(3. * ureg.centimeter), 0.03 * ureg.meter)
         self.assertRaises(DimensionalityError, f0, 3. * ureg.kilogram)
 
         f0b = ureg.check(ureg.meter)(func)
-        self.assertRaises(AttributeError, f0b, 3.)
+        self.assertRaises(DimensionalityError, f0b, 3.)
         self.assertEqual(f0b(3. * ureg.centimeter), 0.03 * ureg.meter)
         self.assertRaises(DimensionalityError, f0b, 3. * ureg.kilogram)
 
         def gfunc(x, y):
             return x / y
 
         g0 = ureg.check(None, None)(gfunc)
         self.assertEqual(g0(6, 2), 3)
         self.assertEqual(g0(6 * ureg.parsec, 2), 3 * ureg.parsec)
 
         g1 = ureg.check('[speed]', '[time]')(gfunc)
-        self.assertRaises(AttributeError, g1, 3.0, 1)
+        self.assertRaises(DimensionalityError, g1, 3.0, 1)
         self.assertRaises(DimensionalityError, g1, 1 * ureg.parsec, 1 * ureg.angstrom)
         self.assertRaises(TypeError, g1, 1 * ureg.km / ureg.hour, 1 * ureg.hour, 3.0)
         self.assertEqual(g1(3.6 * ureg.km / ureg.hour, 1 * ureg.second), 1 * ureg.meter / ureg.second ** 2)
 
         g2 = ureg.check('[speed]')(gfunc)
-        self.assertRaises(AttributeError, g2, 3.0, 1)
-        self.assertRaises(DimensionalityError, g2, 2 * ureg.parsec)
+        self.assertRaises(DimensionalityError, g2, 3.0, 1)
+        self.assertRaises(TypeError, g2, 2 * ureg.parsec)
         self.assertRaises(DimensionalityError, g2, 2 * ureg.parsec, 1.0)
         self.assertEqual(g2(2.0 * ureg.km / ureg.hour, 2), 1 * ureg.km / ureg.hour)
 
         g3 = ureg.check('[speed]', '[time]', '[mass]')(gfunc)
-        self.assertRaises(DimensionalityError, g3, 1 * ureg.parsec, 1 * ureg.angstrom)
-        self.assertRaises(DimensionalityError, g3, 1 * ureg.parsec, 1 * ureg.angstrom, 1 * ureg.kilogram)
+        self.assertRaises(TypeError, g3, 1 * ureg.parsec, 1 * ureg.angstrom)
+        self.assertRaises(TypeError, g3, 1 * ureg.parsec, 1 * ureg.angstrom, 1 * ureg.kilogram)
 
     def test_to_ref_vs_to(self):
         self.ureg.autoconvert_offset_to_baseunit = True
         q = 8. * self.ureg.inch
         t = 8. * self.ureg.degF
         dt = 8. * self.ureg.delta_degF
         self.assertEqual(q.to('yard').magnitude, self.ureg._units['inch'].converter.to_reference(8.))
@@ -488,16 +510,21 @@
     def test_parse_units(self):
         ureg = self.ureg
         self.assertEqual(ureg.parse_units(''), ureg.Unit(''))
         self.assertRaises(ValueError, ureg.parse_units, '2 * meter')
 
 
 class TestCompatibleUnits(QuantityTestCase):
+    FORCE_NDARRAY = False
 
-    FORCE_NDARRAY= False
+    def setUp(self):
+        super(TestCompatibleUnits, self).setUp()
+        self.ureg = UnitRegistry(force_ndarray=self.FORCE_NDARRAY)
+        self.Q_ = self.ureg.Quantity
+        self.U_ = self.ureg.Unit
 
     def _test(self, input_units):
         gd = self.ureg.get_dimensionality
         dim = gd(input_units)
         equiv = self.ureg.get_compatible_units(input_units)
         for eq in equiv:
             self.assertEqual(gd(eq), dim)
```

### Comparing `Pint-0.8.1/pint/testsuite/test_util.py` & `Pint-0.9/pint/testsuite/test_util.py`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/pint/unit.py` & `Pint-0.9/pint/unit.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 
 from __future__ import division, unicode_literals, print_function, absolute_import
 
 import copy
 import operator
 from numbers import Number
 
-from .util import UnitsContainer, SharedRegistryObject, fix_str_conversions
+from .util import (
+    PrettyIPython, UnitsContainer, SharedRegistryObject, fix_str_conversions)
 
 from .compat import string_types, NUMERIC_TYPES, long_type
 from .formatting import siunitx_format_unit
 from .definitions import UnitDefinition
 
 
 @fix_str_conversions
-class _Unit(SharedRegistryObject):
+class _Unit(PrettyIPython, SharedRegistryObject):
     """Implements a class to describe a unit supporting math operations.
 
     :type units: UnitsContainer, str, Unit or Quantity.
 
     """
 
     #: Default formatting string.
@@ -43,15 +44,15 @@
             inst._units = units
         elif isinstance(units, string_types):
             inst._units = inst._REGISTRY.parse_units(units)._units
         elif isinstance(units, _Unit):
             inst._units = units._units
         else:
             raise TypeError('units must be of type str, Unit or '
-                            'UnitsContainer; not {0}.'.format(type(units)))
+                            'UnitsContainer; not {}.'.format(type(units)))
 
         inst.__used = False
         inst.__handling = None
         return inst
 
     @property
     def debug_used(self):
@@ -67,15 +68,15 @@
       ret.__used = self.__used
       return ret
 
     def __str__(self):
         return format(self)
 
     def __repr__(self):
-        return "<Unit('{0}')>".format(self._units)
+        return "<Unit('{}')>".format(self._units)
 
     def __format__(self, spec):
         spec = spec or self.default_format
         # special cases
         if 'Lx' in spec: # the LaTeX siunitx code
           opts = ''
           ustr = siunitx_format_unit(self)
@@ -106,21 +107,14 @@
                                    for key, value in self._units.items()))
             spec = spec.replace('~', '')
         else:
             units = self._units
 
         return '%s' % (units.format_babel(spec, **kwspec))
 
-    # IPython related code
-    def _repr_html_(self):
-        return self.__format__('H')
-
-    def _repr_latex_(self):
-        return "$" + self.__format__('L') + "$"
-
     @property
     def dimensionless(self):
         """Return true if the Unit is dimensionless.
 
         """
         return not bool(self.dimensionality)
 
@@ -258,14 +252,45 @@
         out = set()
         for uname in self._units.keys():
             for sname, sys in self._REGISTRY._systems.items():
                 if uname in sys.members:
                     out.add(sname)
         return frozenset(out)
 
+    def from_(self, value, strict=True, name='value'):
+        """Converts a numerical value or quantity to this unit
+
+        :param value: a Quantity (or numerical value if strict=False) to convert
+        :param strict: boolean to indicate that only quanities are accepted
+        :param name: descriptive name to use if an exception occurs
+        :return: The converted value as this unit
+        :raises:
+            :class:`ValueError` if strict and one of the arguments is not a Quantity.
+        """
+        if self._check(value):
+            if not isinstance(value, self._REGISTRY.Quantity):
+                value = self._REGISTRY.Quantity(1, value)
+            return value.to(self)
+        elif strict:
+            raise ValueError("%s must be a Quantity" % value)
+        else:
+            return value * self
+
+    def m_from(self, value, strict=True, name='value'):
+        """Converts a numerical value or quantity to this unit, then returns
+        the magnitude of the converted value
+
+        :param value: a Quantity (or numerical value if strict=False) to convert
+        :param strict: boolean to indicate that only quanities are accepted
+        :param name: descriptive name to use if an exception occurs
+        :return: The magnitude of the converted value
+        :raises:
+            :class:`ValueError` if strict and one of the arguments is not a Quantity.
+        """
+        return self.from_(value, strict=strict, name=name).magnitude
 
 def build_unit_class(registry):
 
     class Unit(_Unit):
         pass
 
     Unit._REGISTRY = registry
```

### Comparing `Pint-0.8.1/pint/util.py` & `Pint-0.9/pint/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,27 @@
 from decimal import Decimal
 import locale
 import sys
 import re
 import operator
 from numbers import Number
 from fractions import Fraction
-from collections import Mapping
+
+try:
+    from collections.abc import Mapping
+except ImportError:
+    from collections import Mapping
+
+from logging import NullHandler
 
 import logging
 from token import STRING, NAME, OP, NUMBER
 from tokenize import untokenize
 
-from .compat import string_types, tokenizer, lru_cache, NullHandler, maketrans, NUMERIC_TYPES
+from .compat import string_types, tokenizer, lru_cache, maketrans, NUMERIC_TYPES
 from .formatting import format_unit,siunitx_format_unit
 from .pint_eval import build_eval_tree
 from .errors import DefinitionSyntaxError
 
 logger = logging.getLogger(__name__)
 logger.addHandler(NullHandler())
 
@@ -145,15 +151,15 @@
         elif not hasattr(value, 'dimensionality'):
             dims = getdim(value)
         else:
             dims = value.dimensionality
 
         if not registry and any(not key.startswith('[') for key in dims):
             logger.warning('A non dimension was found and a registry was not provided. '
-                           'Assuming that it is a dimension name: {0}.'.format(dims))
+                           'Assuming that it is a dimension name: {}.'.format(dims))
 
         quant.append((name, dims))
         dimensions = dimensions.union(dims.keys())
 
     dimensions = list(dimensions)
 
     # Calculate dimensionless  quantities
@@ -249,17 +255,17 @@
     __slots__ = ('_d', '_hash')
 
     def __init__(self, *args, **kwargs):
         d = udict(*args, **kwargs)
         self._d = d
         for key, value in d.items():
             if not isinstance(key, string_types):
-                raise TypeError('key must be a str, not {0}'.format(type(key)))
+                raise TypeError('key must be a str, not {}'.format(type(key)))
             if not isinstance(value, Number):
-                raise TypeError('value must be a number, not {0}'.format(type(value)))
+                raise TypeError('value must be a number, not {}'.format(type(value)))
             if not isinstance(value, float):
                 d[key] = float(value)
         self._hash = hash(frozenset(self._d.items()))
 
     def copy(self):
         return self.__copy__()
 
@@ -319,54 +325,54 @@
 
         return dict.__eq__(self._d, other)
 
     def __str__(self):
         return self.__format__('')
 
     def __repr__(self):
-        tmp = '{%s}' % ', '.join(["'{0}': {1}".format(key, value)
+        tmp = '{%s}' % ', '.join(["'{}': {}".format(key, value)
                                   for key, value in sorted(self._d.items())])
-        return '<UnitsContainer({0})>'.format(tmp)
+        return '<UnitsContainer({})>'.format(tmp)
 
     def __format__(self, spec):
         return format_unit(self, spec)
 
     def format_babel(self, spec, **kwspec):
         return format_unit(self, spec, **kwspec)
 
     def __copy__(self):
         return UnitsContainer(self._d)
 
     def __mul__(self, other):
         d = udict(self._d)
         if not isinstance(other, self.__class__):
-            err = 'Cannot multiply UnitsContainer by {0}'
+            err = 'Cannot multiply UnitsContainer by {}'
             raise TypeError(err.format(type(other)))
         for key, value in other.items():
             d[key] += value
         keys = [key for key, value in d.items() if value == 0]
         for key in keys:
             del d[key]
 
         return UnitsContainer(d)
 
     __rmul__ = __mul__
 
     def __pow__(self, other):
         if not isinstance(other, NUMERIC_TYPES):
-            err = 'Cannot power UnitsContainer by {0}'
+            err = 'Cannot power UnitsContainer by {}'
             raise TypeError(err.format(type(other)))
         d = udict(self._d)
         for key, value in d.items():
             d[key] *= other
         return UnitsContainer(d)
 
     def __truediv__(self, other):
         if not isinstance(other, self.__class__):
-            err = 'Cannot divide UnitsContainer by {0}'
+            err = 'Cannot divide UnitsContainer by {}'
             raise TypeError(err.format(type(other)))
 
         d = udict(self._d)
 
         for key, value in other.items():
             d[key] -= value
 
@@ -374,15 +380,15 @@
         for key in keys:
             del d[key]
 
         return UnitsContainer(d)
 
     def __rtruediv__(self, other):
         if not isinstance(other, self.__class__) and other != 1:
-            err = 'Cannot divide {0} by UnitsContainer'
+            err = 'Cannot divide {} by UnitsContainer'
             raise TypeError(err.format(type(other)))
 
         return self**-1
 
 
 class ParserHelper(UnitsContainer):
     """ The ParserHelper stores in place the product of variables and
@@ -411,15 +417,15 @@
 
         """
         return cls(1, [(input_word, 1)])
 
     @classmethod
     def from_string(cls, input_string):
         return cls._from_string(input_string)
-    
+
     @classmethod
     def eval_token(cls, token, use_decimal=False):
         token_type = token.type
         token_text = token.string
         if token_type == NUMBER:
             try:
                 return int(token_text)
@@ -427,15 +433,15 @@
                 if use_decimal:
                     return Decimal(token_text)
                 return float(token_text)
         elif token_type == NAME:
             return ParserHelper.from_word(token_text)
         else:
             raise Exception('unknown token type')
-    
+
     @classmethod
     @lru_cache()
     def _from_string(cls, input_string):
         """Parse linear expression mathematical units and return a quantity object.
 
         """
         if not input_string:
@@ -493,22 +499,22 @@
             keys = [key for key, value in d.items() if value == 0]
             for key in keys:
                 del d[key]
 
         return self.__class__(self.scale, d)
 
     def __str__(self):
-        tmp = '{%s}' % ', '.join(["'{0}': {1}".format(key, value)
+        tmp = '{%s}' % ', '.join(["'{}': {}".format(key, value)
                                   for key, value in sorted(self._d.items())])
-        return '{0} {1}'.format(self.scale, tmp)
+        return '{} {}'.format(self.scale, tmp)
 
     def __repr__(self):
-        tmp = '{%s}' % ', '.join(["'{0}': {1}".format(key, value)
+        tmp = '{%s}' % ', '.join(["'{}': {}".format(key, value)
                                   for key, value in sorted(self._d.items())])
-        return '<ParserHelper({0}, {1})>'.format(self.scale, tmp)
+        return '<ParserHelper({}, {})>'.format(self.scale, tmp)
 
     def __mul__(self, other):
         if isinstance(other, string_types):
             new = self.add(other, 1)
         elif isinstance(other, Number):
             new = self.copy()
             new.scale *= other
@@ -555,24 +561,24 @@
             new = new.operate(other.items(), operator.add)
         return new
 
 
 #: List of regex substitution pairs.
 _subs_re = [('\N{DEGREE SIGN}', " degree"),
             (r"([\w\.\-\+\*\\\^])\s+", r"\1 "), # merge multiple spaces
-            (r"({0}) squared", r"\1**2"),  # Handle square and cube
-            (r"({0}) cubed", r"\1**3"),
-            (r"cubic ({0})", r"\1**3"),
-            (r"square ({0})", r"\1**2"),
-            (r"sq ({0})", r"\1**2"),
+            (r"({}) squared", r"\1**2"),  # Handle square and cube
+            (r"({}) cubed", r"\1**3"),
+            (r"cubic ({})", r"\1**3"),
+            (r"square ({})", r"\1**2"),
+            (r"sq ({})", r"\1**2"),
             (r"\b([0-9]+\.?[0-9]*)(?=[e|E][a-zA-Z]|[a-df-zA-DF-Z])", r"\1*"),  # Handle numberLetter for multiplication
             (r"([\w\.\-])\s+(?=\w)", r"\1*"),  # Handle space for multiplication
             ]
 
-#: Compiles the regex and replace {0} by a regex that matches an identifier.
+#: Compiles the regex and replace {} by a regex that matches an identifier.
 _subs_re = [(re.compile(a.format(r"[_a-zA-Z][_a-zA-Z0-9]*")), b) for a, b in _subs_re]
 _pretty_table = maketrans('⁰¹²³⁴⁵⁶⁷⁸⁹·⁻', '0123456789*-')
 _pretty_exp_re = re.compile(r"⁻?[⁰¹²³⁴⁵⁶⁷⁸⁹]+(?:\.[⁰¹²³⁴⁵⁶⁷⁸⁹]*)?")
 
 
 def string_preprocessor(input_string):
 
@@ -614,20 +620,43 @@
         same unit registry.
 
         """
         if self._REGISTRY is getattr(other, '_REGISTRY', None):
             return True
 
         elif isinstance(other, SharedRegistryObject):
-            mess = 'Cannot operate with {0} and {1} of different registries.'
+            mess = 'Cannot operate with {} and {} of different registries.'
             raise ValueError(mess.format(self.__class__.__name__,
                                          other.__class__.__name__))
         else:
             return False
 
+
+class PrettyIPython(object):
+    """Mixin to add pretty-printers for IPython"""
+
+    def _repr_html_(self):
+        if "~" in self.default_format:
+            return "{:~H}".format(self)
+        else:
+            return "{:H}".format(self)
+
+    def _repr_latex_(self):
+        if "~" in self.default_format:
+            return "${:~L}$".format(self)
+        else:
+            return "${:L}$".format(self)
+
+    def _repr_pretty_(self, p, cycle):
+        if "~" in self.default_format:
+            p.text("{:~P}".format(self))
+        else:
+            p.text("{:P}".format(self))
+
+
 def to_units_container(unit_like, registry=None):
     """ Convert a unit compatible type to a UnitsContainer.
 
     """
     mro = type(unit_like).mro()
     if UnitsContainer in mro:
         return unit_like
```

### Comparing `Pint-0.8.1/pint/xtranslated.txt` & `Pint-0.9/pint/xtranslated.txt`

 * *Files identical despite different names*

### Comparing `Pint-0.8.1/Pint.egg-info/PKG-INFO` & `Pint-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Pint
-Version: 0.8.1
+Version: 0.9
 Summary: Physical quantities module
 Home-page: https://github.com/hgrecco/pint
 Author: Hernan E. Grecco
 Author-email: hernan.grecco@gmail.com
 License: BSD
 Description: Pint: makes units easy
         ======================
@@ -15,15 +15,15 @@
         to different units.
         
         It is distributed with a comprehensive list of physical units, prefixes
         and constants. Due to its modular design, you can extend (or even rewrite!)
         the complete list without changing the source code. It supports a lot of
         numpy mathematical operations **without monkey patching or wrapping numpy**.
         
-        It has a complete test coverage. It runs in Python 2.6 and 3.X
+        It has a complete test coverage. It runs in Python 2.7 and 3.3+
         with no other dependency. It is licensed under BSD.
         
         It is extremely easy and natural to use:
         
         .. code-block:: python
         
             >>> import pint
@@ -86,28 +86,29 @@
           PEP 3101 syntax. Extended conversion flags are given to provide latex and pretty
           formatting.
         
         - Small codebase: small and easy to maintain with a flat hierarchy.
         
         - Dependency free: it depends only on Python and its standard library.
         
-        - Python 2 and 3: A single codebase that runs unchanged in Python 2.6+ and Python 3.0+.
+        - Python 2 and 3: A single codebase that runs unchanged in Python 2.7 and Python 3.3+.
         
         - Advanced NumPy support: While NumPy is not a requirement for Pint,
           when available ndarray methods and ufuncs can be used in Quantity objects.
         
         
         Pint is written and maintained by Hernan E. Grecco <hernan.grecco@gmail.com>.
         
         Other contributors, listed alphabetically, are:
         
         * Aaron Coleman
         * Alexander Böhn <fish2000@gmail.com>
         * Ana Krivokapic <akrivokapic1@gmail.com>
         * Andrea Zonca <code@andreazonca.com>
+        * Andrew Savage <andrewgsavage@gmail.com>
         * Brend Wanders <b.wanders@utwente.nl>
         * choloepus
         * coutinho <coutinho@esrf.fr>
         * Daniel Sokolowski <daniel.sokolowski@danols.com>
         * Dave Brooks <dave@bcs.co.nz>
         * David Linke
         * Ed Schofield <ed@pythoncharmers.com>
@@ -126,26 +127,63 @@
         * Luke Campbell <luke.s.campbell@gmail.com>
         * Matthieu Dartiailh <marul@laposte.net>
         * Nate Bogdanowicz <natezb@gmail.com>
         * Peter Grayson <jpgrayson@gmail.com>
         * Richard Barnes <rbarnes@umn.edu>
         * Ryan Dwyer <ryanpdwyer@gmail.com>
         * Ryan Kingsbury <RyanSKingsbury@alumni.unc.edu>
+        * Ryan May
+        * Sigvald Marholm <sigvald@marebakken.com>
         * Sundar Raman <cybertoast@gmail.com>
         * Tiago Coutinho <coutinho@esrf.fr>
         * Thomas Kluyver <takowl@gmail.com>
         * Tom Ritchford <tom@swirly.com>
         * Virgil Dupras <virgil.dupras@savoirfairelinux.com>
+        * Zebedee Nicholls <zebedee.nicholls@climate-energy-college.org>
         
         (If you think that your name belongs here, please let the maintainer know)
         
         
         Pint Changelog
         ==============
         
+        0.9 (2019-01-12)
+        ----------------
+        
+        - Add support for registering with matplotlib's unit handling
+          (Issue #317, thanks dopplershift)
+        - Add converters for matplotlib's unit support.
+          (Issue #317, thanks Ryan May)
+        - Fix unwanted side effects in auto dimensionality reduction.
+          (Issue #516, thanks Ben Loer)
+        - Allow dimensionality check for non Quantity arguments.
+        - Make Quantity and UnitContainer objects hashable.
+          (Issue #286, thanks Nevada Sanchez)
+        - Fix unit tests errors with numpy >=1.13.
+          (Issue #577, thanks cpascual)
+        - Avoid error in in-place exponentiation with numpy > 1.11.
+          (Issue #577, thanks cpascual)
+        - fix compatible units in context.
+          (thanks enrico)
+        - Added warning for unsupported ufunc.
+          (Issue #626, thanks kanhua)
+        - Improve IPython pretty printers.
+          (Issue #590, thanks tecki)
+        - Drop Support for Python 2.6, 3.0, 3.1 and 3.2.
+          (Issue #567)
+        - Prepare for deprecation announced in Python 3.7
+          (Issue #747, thanks Simon Willison)
+        - Added several new units and Systems
+          (Issues #749, #737, )
+        - Started experimental pandas support
+          (Issue #746 and others. Thanks andrewgsavage, znicholls and others)  
+        - wraps and checks now supports kwargs and defaults.
+          (Issue #660, thanks jondoesntgit)
+        
+        
         0.8.1 (2017-06-05)
         ------------------
         
         - Add support for datetime math.
           (Issue #510, thanks robertd)
         - Fixed _repr_html_ in Python 2.7.
           (Issue #512)
@@ -165,15 +203,15 @@
           (Issue #483)
         - Wraps now gets the canonical name of the unit when passed as string.
           (Issue #468)
         - NumPy exp and log keeps the type
           (Issue #95)
         - Implemented a function decorator to ensure that a context is active (with_context)
           (Issue #465)
-        - Add warning when a System contains an unknown Group. 
+        - Add warning when a System contains an unknown Group.
           (Issue #472)
         - Add conda-forge installation snippet.
           (Issue #485, thanks stadelmanma)
         - Properly support floor division and modulo.
           (Issue #474, thanks tecki)
         - Measurement Correlated variable fix.
           (Issue #463, thanks tadhgmister)
@@ -188,15 +226,15 @@
           (Issue #425, thanks GloriaVictis)
         - Fixed issue with negative values in to_compact() method.
           (Issue #443, thanks nowox)
         - Improved defintions.
           (Issues #448, thanks gdonval)
         - Improved Parser to support capital "E" on scientific notation.
           (Issue #390, thanks javenoneal)
-        - Make sure that prefixed units are defined on the registry when unplicking.
+        - Make sure that prefixed units are defined on the registry when unpickling.
           (Issue #405)
         - Automatic unit names translation through babel.
           (Issue #338, thanks alexbodn)
         - Support pickling Unit objects.
           (Issue #349)
         - Add support for wavenumber/kayser in spectroscopy context.
           (Issue #321, thanks gerritholl)
@@ -365,15 +403,15 @@
           (Issue #111, thanks rec)
         - Default registry to lazy load, raise error on redefinition
           (Issue #108, thanks rec, aepsil0n)
         - Added condensed format.
           (Issue #107, thanks rec)
         - Added UnitRegistry () operator to parse expression replacing [].
           (Issue #106, thanks rec)
-        - Optional case insensitive unit parsing. 
+        - Optional case insensitive unit parsing.
           (Issue #105, thanks rec, jeremyfreeman, dbrnz)
         - Change the Quantity mutability depending on magnitude type.
           (Issue #104, thanks rec)
         - Implemented API to list compatible units.
           (Issue #89)
         - Implemented cache of key UnitRegistry methods.
         - Rewrote the Measurement class to use uncertainties.
@@ -578,15 +616,11 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `Pint-0.8.1/Pint.egg-info/SOURCES.txt` & `Pint-0.9/Pint.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 README
 README.rst
 setup.cfg
 setup.py
 Pint.egg-info/PKG-INFO
 Pint.egg-info/SOURCES.txt
 Pint.egg-info/dependency_links.txt
+Pint.egg-info/requires.txt
 Pint.egg-info/top_level.txt
 Pint.egg-info/zip-safe
 bench/bench.py
 bench/bench_base.yaml
 bench/bench_numpy.yaml
 docs/Makefile
 docs/conf.py
@@ -26,14 +27,15 @@
 docs/index.rst
 docs/make.bat
 docs/measurement.rst
 docs/nonmult.rst
 docs/numpy.rst
 docs/performance.rst
 docs/pitheorem.rst
+docs/plotting.rst
 docs/serialization.rst
 docs/systems.rst
 docs/tutorial.rst
 docs/wrapping.rst
 docs/_static/logo-full.jpg
 docs/_templates/sidebarintro.html
 docs/_templates/sidebarlogo.html
@@ -52,28 +54,28 @@
 pint/context.py
 pint/converters.py
 pint/default_en.txt
 pint/default_en_0.6.txt
 pint/definitions.py
 pint/errors.py
 pint/formatting.py
+pint/matplotlib.py
 pint/measurement.py
 pint/pint_eval.py
 pint/quantity.py
 pint/registry.py
 pint/registry_helpers.py
 pint/systems.py
 pint/unit.py
 pint/util.py
 pint/xtranslated.txt
 pint/compat/__init__.py
 pint/compat/chainmap.py
 pint/compat/lrucache.py
 pint/compat/meta.py
-pint/compat/nullhandler.py
 pint/compat/tokenize.py
 pint/testsuite/__init__.py
 pint/testsuite/helpers.py
 pint/testsuite/parameterized.py
 pint/testsuite/test_babel.py
 pint/testsuite/test_contexts.py
 pint/testsuite/test_converters.py
@@ -86,9 +88,8 @@
 pint/testsuite/test_numpy.py
 pint/testsuite/test_pint_eval.py
 pint/testsuite/test_pitheorem.py
 pint/testsuite/test_quantity.py
 pint/testsuite/test_systems.py
 pint/testsuite/test_umath.py
 pint/testsuite/test_unit.py
-pint/testsuite/test_util.py
-pint/testsuite/compat/__init__.py
+pint/testsuite/test_util.py
```

### Comparing `Pint-0.8.1/PKG-INFO` & `Pint-0.9/Pint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Pint
-Version: 0.8.1
+Version: 0.9
 Summary: Physical quantities module
 Home-page: https://github.com/hgrecco/pint
 Author: Hernan E. Grecco
 Author-email: hernan.grecco@gmail.com
 License: BSD
 Description: Pint: makes units easy
         ======================
@@ -15,15 +15,15 @@
         to different units.
         
         It is distributed with a comprehensive list of physical units, prefixes
         and constants. Due to its modular design, you can extend (or even rewrite!)
         the complete list without changing the source code. It supports a lot of
         numpy mathematical operations **without monkey patching or wrapping numpy**.
         
-        It has a complete test coverage. It runs in Python 2.6 and 3.X
+        It has a complete test coverage. It runs in Python 2.7 and 3.3+
         with no other dependency. It is licensed under BSD.
         
         It is extremely easy and natural to use:
         
         .. code-block:: python
         
             >>> import pint
@@ -86,28 +86,29 @@
           PEP 3101 syntax. Extended conversion flags are given to provide latex and pretty
           formatting.
         
         - Small codebase: small and easy to maintain with a flat hierarchy.
         
         - Dependency free: it depends only on Python and its standard library.
         
-        - Python 2 and 3: A single codebase that runs unchanged in Python 2.6+ and Python 3.0+.
+        - Python 2 and 3: A single codebase that runs unchanged in Python 2.7 and Python 3.3+.
         
         - Advanced NumPy support: While NumPy is not a requirement for Pint,
           when available ndarray methods and ufuncs can be used in Quantity objects.
         
         
         Pint is written and maintained by Hernan E. Grecco <hernan.grecco@gmail.com>.
         
         Other contributors, listed alphabetically, are:
         
         * Aaron Coleman
         * Alexander Böhn <fish2000@gmail.com>
         * Ana Krivokapic <akrivokapic1@gmail.com>
         * Andrea Zonca <code@andreazonca.com>
+        * Andrew Savage <andrewgsavage@gmail.com>
         * Brend Wanders <b.wanders@utwente.nl>
         * choloepus
         * coutinho <coutinho@esrf.fr>
         * Daniel Sokolowski <daniel.sokolowski@danols.com>
         * Dave Brooks <dave@bcs.co.nz>
         * David Linke
         * Ed Schofield <ed@pythoncharmers.com>
@@ -126,26 +127,63 @@
         * Luke Campbell <luke.s.campbell@gmail.com>
         * Matthieu Dartiailh <marul@laposte.net>
         * Nate Bogdanowicz <natezb@gmail.com>
         * Peter Grayson <jpgrayson@gmail.com>
         * Richard Barnes <rbarnes@umn.edu>
         * Ryan Dwyer <ryanpdwyer@gmail.com>
         * Ryan Kingsbury <RyanSKingsbury@alumni.unc.edu>
+        * Ryan May
+        * Sigvald Marholm <sigvald@marebakken.com>
         * Sundar Raman <cybertoast@gmail.com>
         * Tiago Coutinho <coutinho@esrf.fr>
         * Thomas Kluyver <takowl@gmail.com>
         * Tom Ritchford <tom@swirly.com>
         * Virgil Dupras <virgil.dupras@savoirfairelinux.com>
+        * Zebedee Nicholls <zebedee.nicholls@climate-energy-college.org>
         
         (If you think that your name belongs here, please let the maintainer know)
         
         
         Pint Changelog
         ==============
         
+        0.9 (2019-01-12)
+        ----------------
+        
+        - Add support for registering with matplotlib's unit handling
+          (Issue #317, thanks dopplershift)
+        - Add converters for matplotlib's unit support.
+          (Issue #317, thanks Ryan May)
+        - Fix unwanted side effects in auto dimensionality reduction.
+          (Issue #516, thanks Ben Loer)
+        - Allow dimensionality check for non Quantity arguments.
+        - Make Quantity and UnitContainer objects hashable.
+          (Issue #286, thanks Nevada Sanchez)
+        - Fix unit tests errors with numpy >=1.13.
+          (Issue #577, thanks cpascual)
+        - Avoid error in in-place exponentiation with numpy > 1.11.
+          (Issue #577, thanks cpascual)
+        - fix compatible units in context.
+          (thanks enrico)
+        - Added warning for unsupported ufunc.
+          (Issue #626, thanks kanhua)
+        - Improve IPython pretty printers.
+          (Issue #590, thanks tecki)
+        - Drop Support for Python 2.6, 3.0, 3.1 and 3.2.
+          (Issue #567)
+        - Prepare for deprecation announced in Python 3.7
+          (Issue #747, thanks Simon Willison)
+        - Added several new units and Systems
+          (Issues #749, #737, )
+        - Started experimental pandas support
+          (Issue #746 and others. Thanks andrewgsavage, znicholls and others)  
+        - wraps and checks now supports kwargs and defaults.
+          (Issue #660, thanks jondoesntgit)
+        
+        
         0.8.1 (2017-06-05)
         ------------------
         
         - Add support for datetime math.
           (Issue #510, thanks robertd)
         - Fixed _repr_html_ in Python 2.7.
           (Issue #512)
@@ -165,15 +203,15 @@
           (Issue #483)
         - Wraps now gets the canonical name of the unit when passed as string.
           (Issue #468)
         - NumPy exp and log keeps the type
           (Issue #95)
         - Implemented a function decorator to ensure that a context is active (with_context)
           (Issue #465)
-        - Add warning when a System contains an unknown Group. 
+        - Add warning when a System contains an unknown Group.
           (Issue #472)
         - Add conda-forge installation snippet.
           (Issue #485, thanks stadelmanma)
         - Properly support floor division and modulo.
           (Issue #474, thanks tecki)
         - Measurement Correlated variable fix.
           (Issue #463, thanks tadhgmister)
@@ -188,15 +226,15 @@
           (Issue #425, thanks GloriaVictis)
         - Fixed issue with negative values in to_compact() method.
           (Issue #443, thanks nowox)
         - Improved defintions.
           (Issues #448, thanks gdonval)
         - Improved Parser to support capital "E" on scientific notation.
           (Issue #390, thanks javenoneal)
-        - Make sure that prefixed units are defined on the registry when unplicking.
+        - Make sure that prefixed units are defined on the registry when unpickling.
           (Issue #405)
         - Automatic unit names translation through babel.
           (Issue #338, thanks alexbodn)
         - Support pickling Unit objects.
           (Issue #349)
         - Add support for wavenumber/kayser in spectroscopy context.
           (Issue #321, thanks gerritholl)
@@ -365,15 +403,15 @@
           (Issue #111, thanks rec)
         - Default registry to lazy load, raise error on redefinition
           (Issue #108, thanks rec, aepsil0n)
         - Added condensed format.
           (Issue #107, thanks rec)
         - Added UnitRegistry () operator to parse expression replacing [].
           (Issue #106, thanks rec)
-        - Optional case insensitive unit parsing. 
+        - Optional case insensitive unit parsing.
           (Issue #105, thanks rec, jeremyfreeman, dbrnz)
         - Change the Quantity mutability depending on magnitude type.
           (Issue #104, thanks rec)
         - Implemented API to list compatible units.
           (Issue #89)
         - Implemented cache of key UnitRegistry methods.
         - Rewrote the Measurement class to use uncertainties.
@@ -578,15 +616,11 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `Pint-0.8.1/README` & `Pint-0.9/README`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 to different units.
 
 It is distributed with a comprehensive list of physical units, prefixes
 and constants. Due to its modular design, you can extend (or even rewrite!)
 the complete list without changing the source code. It supports a lot of
 numpy mathematical operations **without monkey patching or wrapping numpy**.
 
-It has a complete test coverage. It runs in Python 2.6 and 3.X
+It has a complete test coverage. It runs in Python 2.7 and 3.3+
 with no other dependency. It is licensed under BSD.
 
 It is extremely easy and natural to use:
 
 .. code-block:: python
 
     >>> import pint
@@ -78,11 +78,11 @@
   PEP 3101 syntax. Extended conversion flags are given to provide latex and pretty
   formatting.
 
 - Small codebase: small and easy to maintain with a flat hierarchy.
 
 - Dependency free: it depends only on Python and its standard library.
 
-- Python 2 and 3: A single codebase that runs unchanged in Python 2.6+ and Python 3.0+.
+- Python 2 and 3: A single codebase that runs unchanged in Python 2.7 and Python 3.3+.
 
 - Advanced NumPy support: While NumPy is not a requirement for Pint,
   when available ndarray methods and ufuncs can be used in Quantity objects.
```

### Comparing `Pint-0.8.1/README.rst` & `Pint-0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 to different units.
 
 It is distributed with a comprehensive list of physical units, prefixes
 and constants. Due to its modular design, you can extend (or even rewrite!)
 the complete list without changing the source code. It supports a lot of
 numpy mathematical operations **without monkey patching or wrapping numpy**.
 
-It has a complete test coverage. It runs in Python 2.6 and 3.X
+It has a complete test coverage. It runs in Python 2.7 and 3.3+
 with no other dependency. It is licensed under BSD.
 
 It is extremely easy and natural to use:
 
 .. code-block:: python
 
     >>> import pint
@@ -107,11 +107,11 @@
   PEP 3101 syntax. Extended conversion flags are given to provide latex and pretty
   formatting.
 
 - Small codebase: small and easy to maintain with a flat hierarchy.
 
 - Dependency free: it depends only on Python and its standard library.
 
-- Python 2 and 3: A single codebase that runs unchanged in Python 2.6+ and Python 3.0+.
+- Python 2 and 3: A single codebase that runs unchanged in Python 2.7 and Python 3.3+.
 
 - Advanced NumPy support: While NumPy is not a requirement for Pint,
   when available ndarray methods and ufuncs can be used in Quantity objects.
```

### Comparing `Pint-0.8.1/setup.py` & `Pint-0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 try:
     from setuptools import setup
 except ImportError:
     print('Please install or upgrade setuptools or pip to continue')
     sys.exit(1)
 
-tests_require = []
-if sys.version_info < (2, 7):
-   tests_require.append('unittest2')
-
 import codecs
 
 
 def read(filename):
     return codecs.open(filename, encoding='utf-8').read()
 
 
@@ -29,23 +25,22 @@
                                 read('AUTHORS'),
                                 read('CHANGES')])
 
 __doc__ = long_description
 
 setup(
     name='Pint',
-    version='0.8.1',
+    version='0.9',
     description='Physical quantities module',
     long_description=long_description,
     keywords='physical quantities unit conversion science',
     author='Hernan E. Grecco',
     author_email='hernan.grecco@gmail.com',
     url='https://github.com/hgrecco/pint',
     test_suite='pint.testsuite.testsuite',
-    tests_require=tests_require,
     zip_safe=True,
     packages=['pint'],
     package_data={
         'pint': ['default_en.txt',
                  'constants_en.txt']
       },
     include_package_data=True,
@@ -57,16 +52,18 @@
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Programming Language :: Python',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development :: Libraries',
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.0',
-        'Programming Language :: Python :: 3.1',
-        'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
-    ])
+    ],
+    extras_require={
+        ':python_version == "2.7"': [
+            'funcsigs',
+        ],
+    },
+    )
```

