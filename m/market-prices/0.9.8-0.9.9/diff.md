# Comparing `tmp/market_prices-0.9.8.tar.gz` & `tmp/market_prices-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_prices-0.9.8.tar", last modified: Mon Oct  3 17:28:13 2022, max compression
+gzip compressed data, was "market_prices-0.9.9.tar", last modified: Mon Oct  3 22:01:56 2022, max compression
```

## Comparing `market_prices-0.9.8.tar` & `market_prices-0.9.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.979387 market_prices-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-03 17:28:00.000000 market_prices-0.9.8/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-10-03 17:28:00.000000 market_prices-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-03 17:28:00.000000 market_prices-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-10-03 17:28:00.000000 market_prices-0.9.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-03 17:28:00.000000 market_prices-0.9.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-03 17:28:00.000000 market_prices-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    22647 2022-10-03 17:28:13.979387 market_prices-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19897 2022-10-03 17:28:00.000000 market_prices-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.967387 market_prices-0.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.967387 market_prices-0.9.8/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (121)    11195 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/developers/other_internals.md
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/developers/releases.md
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/developers/serving_data.md
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/developers/testing.md
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/developers/typing_doc.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.967387 market_prices-0.9.8/docs/media/
--rw-r--r--   0 runner    (1001) docker     (121)    32073 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/media/readme_pt.png
--rw-r--r--   0 runner    (1001) docker     (121)    72514 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/media/splash.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.971387 market_prices-0.9.8/docs/public/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/public/method_doc.md
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/public/parsing.md
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/public/typing.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.971387 market_prices-0.9.8/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)   351080 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/anchor.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   135219 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/data_availability.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    95320 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/intervals.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   161202 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/other_get_options.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    28571 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/other_prices_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   284524 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/periods.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27166 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/prices.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   360128 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/pt_accessor.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   187320 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    89425 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials/specific_query_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-10-03 17:28:00.000000 market_prices-0.9.8/docs/tutorials_docs.md
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-10-03 17:28:00.000000 market_prices-0.9.8/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-10-03 17:28:00.000000 market_prices-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-03 17:28:00.000000 market_prices-0.9.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-10-03 17:28:00.000000 market_prices-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-10-03 17:28:00.000000 market_prices-0.9.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 17:28:13.979387 market_prices-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-03 17:28:00.000000 market_prices-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.967387 market_prices-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.975387 market_prices-0.9.8/src/market_prices/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-03 17:28:13.000000 market_prices-0.9.8/src/market_prices/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    24787 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    45825 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/daterange.py
--rw-r--r--   0 runner    (1001) docker     (121)    25918 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    14201 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15454 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/intervals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11403 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/mptypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    17101 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.975387 market_prices-0.9.8/src/market_prices/prices/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   169672 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/prices/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.975387 market_prices-0.9.8/src/market_prices/prices/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/prices/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/prices/config/config_yahoo.py
--rw-r--r--   0 runner    (1001) docker     (121)    47148 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/prices/yahoo.py
--rw-r--r--   0 runner    (1001) docker     (121)    97716 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/pt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.975387 market_prices-0.9.8/src/market_prices/support/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9876 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/support/tutorial_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.979387 market_prices-0.9.8/src/market_prices/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42137 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/utils/calendar_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    31145 2022-10-03 17:28:00.000000 market_prices-0.9.8/src/market_prices/utils/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:28:13.975387 market_prices-0.9.8/src/market_prices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22647 2022-10-03 17:28:13.000000 market_prices-0.9.8/src/market_prices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-10-03 17:28:13.000000 market_prices-0.9.8/src/market_prices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 17:28:13.000000 market_prices-0.9.8/src/market_prices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-03 17:28:13.000000 market_prices-0.9.8/src/market_prices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-03 17:28:13.000000 market_prices-0.9.8/src/market_prices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.025422 market_prices-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-03 22:01:40.000000 market_prices-0.9.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-10-03 22:01:40.000000 market_prices-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-03 22:01:40.000000 market_prices-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-10-03 22:01:40.000000 market_prices-0.9.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-03 22:01:40.000000 market_prices-0.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-03 22:01:40.000000 market_prices-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    22647 2022-10-03 22:01:56.025422 market_prices-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19897 2022-10-03 22:01:40.000000 market_prices-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.009421 market_prices-0.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.013421 market_prices-0.9.9/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (121)    11195 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/developers/other_internals.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/developers/releases.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/developers/serving_data.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/developers/testing.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/developers/typing_doc.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.013421 market_prices-0.9.9/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (121)    32073 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/media/readme_pt.png
+-rw-r--r--   0 runner    (1001) docker     (121)    72514 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/media/splash.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.013421 market_prices-0.9.9/docs/public/
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/public/method_doc.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/public/parsing.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/public/typing.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.017421 market_prices-0.9.9/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (121)   351080 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/anchor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   135219 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/data_availability.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    95320 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/intervals.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   161202 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/other_get_options.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    28571 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/other_prices_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   284524 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/periods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    27166 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/prices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   360128 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/pt_accessor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   187320 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    89425 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials/specific_query_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-10-03 22:01:40.000000 market_prices-0.9.9/docs/tutorials_docs.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-10-03 22:01:40.000000 market_prices-0.9.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-10-03 22:01:40.000000 market_prices-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-03 22:01:40.000000 market_prices-0.9.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-10-03 22:01:40.000000 market_prices-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-10-03 22:01:40.000000 market_prices-0.9.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 22:01:56.025422 market_prices-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-03 22:01:40.000000 market_prices-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.005421 market_prices-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.021422 market_prices-0.9.9/src/market_prices/
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-03 22:01:55.000000 market_prices-0.9.9/src/market_prices/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24787 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45825 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25918 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14201 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15454 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11403 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/mptypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17101 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.021422 market_prices-0.9.9/src/market_prices/prices/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   169672 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/prices/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.021422 market_prices-0.9.9/src/market_prices/prices/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/prices/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/prices/config/config_yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47148 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/prices/yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97716 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/pt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.025422 market_prices-0.9.9/src/market_prices/support/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9876 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/support/tutorial_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.025422 market_prices-0.9.9/src/market_prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42137 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/utils/calendar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31145 2022-10-03 22:01:40.000000 market_prices-0.9.9/src/market_prices/utils/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 22:01:56.021422 market_prices-0.9.9/src/market_prices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22647 2022-10-03 22:01:55.000000 market_prices-0.9.9/src/market_prices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-10-03 22:01:56.000000 market_prices-0.9.9/src/market_prices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 22:01:55.000000 market_prices-0.9.9/src/market_prices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-03 22:01:55.000000 market_prices-0.9.9/src/market_prices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-03 22:01:55.000000 market_prices-0.9.9/src/market_prices.egg-info/top_level.txt
```

### Comparing `market_prices-0.9.8/.flake8` & `market_prices-0.9.9/.flake8`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/.gitignore` & `market_prices-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/.pre-commit-config.yaml` & `market_prices-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/.pylintrc` & `market_prices-0.9.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/LICENSE.txt` & `market_prices-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/PKG-INFO` & `market_prices-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market_prices
-Version: 0.9.8
+Version: 0.9.9
 Summary: Meaningful OHLCV datasets
 Author: Marcus Read
 Author-email: marcusaread@gmail.com
 License: MIT License
         
         Copyright (c) 2022, Marcus Read
```

### Comparing `market_prices-0.9.8/README.md` & `market_prices-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/developers/other_internals.md` & `market_prices-0.9.9/docs/developers/other_internals.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/developers/releases.md` & `market_prices-0.9.9/docs/developers/releases.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/developers/serving_data.md` & `market_prices-0.9.9/docs/developers/serving_data.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/developers/testing.md` & `market_prices-0.9.9/docs/developers/testing.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/developers/typing_doc.md` & `market_prices-0.9.9/docs/developers/typing_doc.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/media/readme_pt.png` & `market_prices-0.9.9/docs/media/readme_pt.png`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/media/splash.png` & `market_prices-0.9.9/docs/media/splash.png`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/public/method_doc.md` & `market_prices-0.9.9/docs/public/method_doc.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/public/parsing.md` & `market_prices-0.9.9/docs/public/parsing.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/public/typing.md` & `market_prices-0.9.9/docs/public/typing.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/anchor.ipynb` & `market_prices-0.9.9/docs/tutorials/anchor.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/data_availability.ipynb` & `market_prices-0.9.9/docs/tutorials/data_availability.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/intervals.ipynb` & `market_prices-0.9.9/docs/tutorials/intervals.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/other_get_options.ipynb` & `market_prices-0.9.9/docs/tutorials/other_get_options.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/other_prices_methods.ipynb` & `market_prices-0.9.9/docs/tutorials/other_prices_methods.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/periods.ipynb` & `market_prices-0.9.9/docs/tutorials/periods.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/prices.ipynb` & `market_prices-0.9.9/docs/tutorials/prices.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/pt_accessor.ipynb` & `market_prices-0.9.9/docs/tutorials/pt_accessor.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/quickstart.ipynb` & `market_prices-0.9.9/docs/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials/specific_query_methods.ipynb` & `market_prices-0.9.9/docs/tutorials/specific_query_methods.ipynb`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/docs/tutorials_docs.md` & `market_prices-0.9.9/docs/tutorials_docs.md`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/mypy.ini` & `market_prices-0.9.9/mypy.ini`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/pyproject.toml` & `market_prices-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/requirements.txt` & `market_prices-0.9.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/requirements_dev.txt` & `market_prices-0.9.9/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/__init__.py` & `market_prices-0.9.9/src/market_prices/__init__.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/data.py` & `market_prices-0.9.9/src/market_prices/data.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/daterange.py` & `market_prices-0.9.9/src/market_prices/daterange.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/errors.py` & `market_prices-0.9.9/src/market_prices/errors.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/helpers.py` & `market_prices-0.9.9/src/market_prices/helpers.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/intervals.py` & `market_prices-0.9.9/src/market_prices/intervals.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/mptypes.py` & `market_prices-0.9.9/src/market_prices/mptypes.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/parsing.py` & `market_prices-0.9.9/src/market_prices/parsing.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/prices/base.py` & `market_prices-0.9.9/src/market_prices/prices/base.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/prices/config/config_yahoo.py` & `market_prices-0.9.9/src/market_prices/prices/config/config_yahoo.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/prices/yahoo.py` & `market_prices-0.9.9/src/market_prices/prices/yahoo.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/pt.py` & `market_prices-0.9.9/src/market_prices/pt.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/support/tutorial_helpers.py` & `market_prices-0.9.9/src/market_prices/support/tutorial_helpers.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/utils/calendar_utils.py` & `market_prices-0.9.9/src/market_prices/utils/calendar_utils.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/utils/general_utils.py` & `market_prices-0.9.9/src/market_prices/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices/utils/pandas_utils.py` & `market_prices-0.9.9/src/market_prices/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `market_prices-0.9.8/src/market_prices.egg-info/PKG-INFO` & `market_prices-0.9.9/src/market_prices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-prices
-Version: 0.9.8
+Version: 0.9.9
 Summary: Meaningful OHLCV datasets
 Author: Marcus Read
 Author-email: marcusaread@gmail.com
 License: MIT License
         
         Copyright (c) 2022, Marcus Read
```

### Comparing `market_prices-0.9.8/src/market_prices.egg-info/SOURCES.txt` & `market_prices-0.9.9/src/market_prices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

