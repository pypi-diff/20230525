# Comparing `tmp/pidge-0.1.2.tar.gz` & `tmp/pidge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidge-0.1.2.tar", max compression
+gzip compressed data, was "pidge-0.2.0.tar", max compression
```

## Comparing `pidge-0.1.2.tar` & `pidge-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1070 2023-04-01 16:29:20.717592 pidge-0.1.2/LICENSE
--rw-r--r--   0        0        0     2939 2023-04-21 04:17:16.768589 pidge-0.1.2/README.md
--rw-r--r--   0        0        0       38 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/__init__.py
--rw-r--r--   0        0        0       65 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/__main__.py
--rw-r--r--   0        0        0     1974 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/core.py
--rw-r--r--   0        0        0      188 2023-03-30 16:12:14.803646 pidge-0.1.2/pidge/examples.py
--rw-r--r--   0        0        0      783 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/main.py
--rw-r--r--   0        0        0    13884 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/sample_data/fake_expenses.csv
--rw-r--r--   0        0        0        0 2023-03-30 16:12:14.803646 pidge-0.1.2/pidge/tests/__init__.py
--rw-r--r--   0        0        0       44 2023-03-30 16:12:14.803646 pidge-0.1.2/pidge/tests/conftest.py
--rw-r--r--   0        0        0      123 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      937 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/fixtures/data.py
--rw-r--r--   0        0        0      366 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/fixtures/mapper.py
--rw-r--r--   0        0        0     1076 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/fixtures/rules.py
--rw-r--r--   0        0        0     3319 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/test_core.py
--rw-r--r--   0        0        0      185 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/test_examples.py
--rw-r--r--   0        0        0       59 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/test_main.py
--rw-r--r--   0        0        0     2954 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/test_mapper.py
--rw-r--r--   0        0        0     3946 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/tests/test_ui.py
--rw-r--r--   0        0        0      114 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/ui/__init__.py
--rw-r--r--   0        0        0      859 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/ui/assets/favicon-16x16.png
--rw-r--r--   0        0        0     2209 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/ui/css/webui.css
--rw-r--r--   0        0        0     3256 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/ui/mapper.py
--rw-r--r--   0        0        0     7426 2023-04-21 04:32:42.658589 pidge-0.1.2/pidge/ui/ui.py
--rw-r--r--   0        0        0     6014 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/ui/web_ui_template.html
--rw-r--r--   0        0        0      638 2023-04-21 04:33:01.058589 pidge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 pidge-0.1.2/setup.py
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 pidge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-01 16:29:20.717592 pidge-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2939 2023-04-21 11:02:19.145236 pidge-0.2.0/README.md
+-rw-r--r--   0        0        0       38 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/__main__.py
+-rw-r--r--   0        0        0     1974 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/core.py
+-rw-r--r--   0        0        0      188 2023-03-30 16:12:14.803646 pidge-0.2.0/pidge/examples.py
+-rw-r--r--   0        0        0      783 2023-04-16 20:50:02.091384 pidge-0.2.0/pidge/main.py
+-rw-r--r--   0        0        0    13884 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/sample_data/fake_expenses.csv
+-rw-r--r--   0        0        0        0 2023-03-30 16:12:14.803646 pidge-0.2.0/pidge/tests/__init__.py
+-rw-r--r--   0        0        0       44 2023-03-30 16:12:14.803646 pidge-0.2.0/pidge/tests/conftest.py
+-rw-r--r--   0        0        0      123 2023-04-15 17:05:58.566718 pidge-0.2.0/pidge/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      937 2023-04-15 17:05:58.566718 pidge-0.2.0/pidge/tests/fixtures/data.py
+-rw-r--r--   0        0        0      366 2023-04-15 17:05:58.566718 pidge-0.2.0/pidge/tests/fixtures/mapper.py
+-rw-r--r--   0        0        0     1076 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/tests/fixtures/rules.py
+-rw-r--r--   0        0        0     3319 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/tests/test_core.py
+-rw-r--r--   0        0        0      185 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/tests/test_examples.py
+-rw-r--r--   0        0        0       59 2023-04-01 16:29:20.717592 pidge-0.2.0/pidge/tests/test_main.py
+-rw-r--r--   0        0        0     2954 2023-04-15 17:05:58.566718 pidge-0.2.0/pidge/tests/test_mapper.py
+-rw-r--r--   0        0        0     3946 2023-04-16 20:50:02.091384 pidge-0.2.0/pidge/tests/test_ui.py
+-rw-r--r--   0        0        0      114 2023-04-15 17:05:58.566718 pidge-0.2.0/pidge/ui/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-16 20:50:02.091384 pidge-0.2.0/pidge/ui/assets/favicon-16x16.png
+-rw-r--r--   0        0        0     2209 2023-04-16 20:50:02.091384 pidge-0.2.0/pidge/ui/css/webui.css
+-rw-r--r--   0        0        0     3256 2023-04-15 17:05:58.566718 pidge-0.2.0/pidge/ui/mapper.py
+-rw-r--r--   0        0        0     7426 2023-04-21 11:02:19.145236 pidge-0.2.0/pidge/ui/ui.py
+-rw-r--r--   0        0        0     6014 2023-04-16 20:50:02.091384 pidge-0.2.0/pidge/ui/web_ui_template.html
+-rw-r--r--   0        0        0      642 2023-05-25 12:21:41.840793 pidge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3469 1970-01-01 00:00:00.000000 pidge-0.2.0/PKG-INFO
```

### Comparing `pidge-0.1.2/LICENSE` & `pidge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/README.md` & `pidge-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/core.py` & `pidge-0.2.0/pidge/core.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/main.py` & `pidge-0.2.0/pidge/main.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/sample_data/fake_expenses.csv` & `pidge-0.2.0/pidge/sample_data/fake_expenses.csv`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/tests/fixtures/data.py` & `pidge-0.2.0/pidge/tests/fixtures/data.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/tests/fixtures/rules.py` & `pidge-0.2.0/pidge/tests/fixtures/rules.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/tests/test_core.py` & `pidge-0.2.0/pidge/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/tests/test_mapper.py` & `pidge-0.2.0/pidge/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/tests/test_ui.py` & `pidge-0.2.0/pidge/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/ui/assets/favicon-16x16.png` & `pidge-0.2.0/pidge/ui/assets/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/ui/css/webui.css` & `pidge-0.2.0/pidge/ui/css/webui.css`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/ui/mapper.py` & `pidge-0.2.0/pidge/ui/mapper.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/ui/ui.py` & `pidge-0.2.0/pidge/ui/ui.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pidge/ui/web_ui_template.html` & `pidge-0.2.0/pidge/ui/web_ui_template.html`

 * *Files identical despite different names*

### Comparing `pidge-0.1.2/pyproject.toml` & `pidge-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = [ "poetry-core>=1.2.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pidge"
-version = "0.1.2"
+version = "0.2.0"
 description = "pidge helps with the creation of mappings for tabular string data"
 readme = "README.md"
 authors = ["Konrad Wölms <konrad.woelms@gmail.com>",]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 panel = "^0.14.4"
-pandas = "^1.5.3"
+pandas = ">=1.5.3,<3"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.16.0"
 pytest = "^7.0.1"
 pytest-cov = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `pidge-0.1.2/setup.py` & `pidge-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,98 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pidge
+Version: 0.2.0
+Summary: pidge helps with the creation of mappings for tabular string data
+Author: Konrad Wölms
+Author-email: konrad.woelms@gmail.com
+Requires-Python: >=3.9,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=1.5.3,<3)
+Requires-Dist: panel (>=0.14.4,<0.15.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['pidge', 'pidge.tests', 'pidge.tests.fixtures', 'pidge.ui']
+# pidge
 
-package_data = \
-{'': ['*'],
- 'pidge': ['sample_data/fake_expenses.csv'],
- 'pidge.ui': ['assets/*', 'css/*']}
-
-install_requires = \
-['pandas>=1.5.3,<2.0.0', 'panel>=0.14.4,<0.15.0']
-
-setup_kwargs = {
-    'name': 'pidge',
-    'version': '0.1.2',
-    'description': 'pidge helps with the creation of mappings for tabular string data',
-    'long_description': "# pidge\n\npidge helps with the creation of mappings for tabular string data. The primary use cases for\nthis are data cleaning and data categorization.\n\npidge consists out of two parts:\n\n1. An interactive UI to help with the creation of mappings and assessing their completeness\n2. Library functionality to apply mappings inside of data pipelines, after they have been exported from the UI\n\n\n## Usage\n\n1. install `pidge`\n\n        pip install pidge\n\n1. Launch the UI in a notebook\n\n    ```python\n    from pidge import pidge_ui\n    import panel as pn\n\n    pn.extensions('tabulator','jsoneditor')\n\n    pidge_ui(my_input_dataframe)\n    ```\n\n1. Create and export a mapping named `pidge_mapping.json`\n\n1. In your data pipeline import `pidge` and apply the mapping\n\n    ```python\n    from pidge import pidge\n\n    transformed_data = pidge(my_input_dataframe,rule_file= 'pidge_mapping.json')\n    ```\n\n### The web-ui outside of Jupyter\n\nPidge can also run the UI as a standalone web server outside of jupyter, using the command.\n\n> python -m pidge\n\nThis starts up the UI in a local web server, which is primarily intended for illustration purposes.\nTherefore it starts up with example data already loaded. However new data can be loaded and the\npredefined rules can easily be reset. The main limitation at this moment, however, is the\nconstraint on the upload format for data. It only supports `.csv` and reads it with default\n`pandas.read_csv` settings.\n\n## Mapping Logic\n\nPidge mappings map a source string column to a newly created target string column. The logic can\nbe broken down as follows.\n\n1. One defines a possible value, a category, for the target column.\n1. One associates one or more patterns with that category.\n1. When a value of the source column matches one of the category's patterns, that category is chosen.\n1. Pattern matching checks whether the pattern is part of the source string. It is case insensitive\n    and allows for regular expressions.\n1. This is repeated for as many categories as desired.\n\n\n## Contribution\n\nPidge is in an early MVP stage. At this stage the following is particularly appreciated\n\n1. Any feedback regarding, bugs, issues usability feature requests etc. Ideally this can be done directly\n    as github issues.\n1. Any sharing of the project to potentially help with the previous point.\n\n## Known Limitations\n\nThere are a few known limitations particularly due to the MVP stage of the project. These\nwill be prioritized according to feedback and general usage of the project.\n\n- Mapping is not optimized for speed at all and might slow down for large dataframes\n- Patterns do not check for multiple inconsistent matches and simply the first applicable pattern\n    is chosen\n- the web-ui does only support small file uploads (around < 10Mb).\n- file uploads can only read in the data with `pandas.read_csv` default settings\n- The rule name used for the .json export can currently not be changed in the UI.\n",
-    'author': 'Konrad Wölms',
-    'author_email': 'konrad.woelms@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.12',
-}
+pidge helps with the creation of mappings for tabular string data. The primary use cases for
+this are data cleaning and data categorization.
 
+pidge consists out of two parts:
+
+1. An interactive UI to help with the creation of mappings and assessing their completeness
+2. Library functionality to apply mappings inside of data pipelines, after they have been exported from the UI
+
+
+## Usage
+
+1. install `pidge`
+
+        pip install pidge
+
+1. Launch the UI in a notebook
+
+    ```python
+    from pidge import pidge_ui
+    import panel as pn
+
+    pn.extensions('tabulator','jsoneditor')
+
+    pidge_ui(my_input_dataframe)
+    ```
+
+1. Create and export a mapping named `pidge_mapping.json`
+
+1. In your data pipeline import `pidge` and apply the mapping
+
+    ```python
+    from pidge import pidge
+
+    transformed_data = pidge(my_input_dataframe,rule_file= 'pidge_mapping.json')
+    ```
+
+### The web-ui outside of Jupyter
+
+Pidge can also run the UI as a standalone web server outside of jupyter, using the command.
+
+> python -m pidge
+
+This starts up the UI in a local web server, which is primarily intended for illustration purposes.
+Therefore it starts up with example data already loaded. However new data can be loaded and the
+predefined rules can easily be reset. The main limitation at this moment, however, is the
+constraint on the upload format for data. It only supports `.csv` and reads it with default
+`pandas.read_csv` settings.
+
+## Mapping Logic
+
+Pidge mappings map a source string column to a newly created target string column. The logic can
+be broken down as follows.
+
+1. One defines a possible value, a category, for the target column.
+1. One associates one or more patterns with that category.
+1. When a value of the source column matches one of the category's patterns, that category is chosen.
+1. Pattern matching checks whether the pattern is part of the source string. It is case insensitive
+    and allows for regular expressions.
+1. This is repeated for as many categories as desired.
+
+
+## Contribution
+
+Pidge is in an early MVP stage. At this stage the following is particularly appreciated
+
+1. Any feedback regarding, bugs, issues usability feature requests etc. Ideally this can be done directly
+    as github issues.
+1. Any sharing of the project to potentially help with the previous point.
+
+## Known Limitations
+
+There are a few known limitations particularly due to the MVP stage of the project. These
+will be prioritized according to feedback and general usage of the project.
+
+- Mapping is not optimized for speed at all and might slow down for large dataframes
+- Patterns do not check for multiple inconsistent matches and simply the first applicable pattern
+    is chosen
+- the web-ui does only support small file uploads (around < 10Mb).
+- file uploads can only read in the data with `pandas.read_csv` default settings
+- The rule name used for the .json export can currently not be changed in the UI.
 
-setup(**setup_kwargs)
```

