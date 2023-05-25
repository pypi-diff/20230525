# Comparing `tmp/pandas-indexing-0.2.5.tar.gz` & `tmp/pandas-indexing-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.5.tar", last modified: Tue May  9 06:15:10 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.6.tar", last modified: Thu May 25 16:41:15 2023, max compression
```

## Comparing `pandas-indexing-0.2.5.tar` & `pandas-indexing-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.868255 pandas-indexing-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.868255 pandas-indexing-0.2.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   362406 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.868255 pandas-indexing-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.872255 pandas-indexing-0.2.5/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.967780 pandas-indexing-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.967780 pandas-indexing-0.2.6/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   362791 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.959780 pandas-indexing-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.971780 pandas-indexing-0.2.6/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.971780 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.5/CHANGELOG.rst` & `pandas-indexing-0.2.6/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.2.6 (2023-05-25)
+------------------------------------------------------------
+* :func:`~core.extractlevel` can be used on non-multiindex, like
+  f.ex. ``extractlevel(df, "{sector}|{gas}")`` :pull:`17`
+* :func:`~selectors.isin` accepts callable filters :pull:`16`, f.ex.
+  ``df.loc[isin(year=lambda s: s>2000)]``
+* New function :func:`~core.concat` makes concatenation level aware :pull:`14`
+
 v0.2.5 (2023-05-04)
 ------------------------------------------------------------
 * :func:`~core.formatlevel` and :func:`~core.extractlevel` (or their equivalents
   :meth:`~accessors.DataFrameIdxAccessor.format` and
   :meth:`~accessors.DataFrameIdxAccessor.extract`) make it easy to combine or split
   index levels using format-string like templates; check examples in the guide
   (:ref:`Selecting data`) :pull:`13`
```

### Comparing `pandas-indexing-0.2.5/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/CONTRIBUTING.rst` & `pandas-indexing-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/LICENSE` & `pandas-indexing-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/PKG-INFO` & `pandas-indexing-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.5
+Version: 0.2.6
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.5/README.rst` & `pandas-indexing-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/docs/api.rst` & `pandas-indexing-0.2.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/docs/conf.py` & `pandas-indexing-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.6/docs/notebooks/introduction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952510245901639%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(3, '\\n'), (5, '   \\n'), (10, '2. convenience accessors "*

 * *            "that are hooking into pandas as extensions, like\\n'), (11, '   \\n')], delete: [9, "*

 * *            "3]}}, 57: {'source': ['# Additional helpful multi-index helpers']}, 59: "*

 * *            "{'execution_count': None, 'outputs': {0: {'execution_count': 33}}}, 60: "*

 * *            "{'execution_count': None, 'outputs': {0: {'execution_count': 34}}}, insert: [(55, "*

 * *            "OrderedDict([('attachments', Or […]*

```diff
@@ -357,21 +357,23 @@
             "cell_type": "markdown",
             "id": "0d61c065",
             "metadata": {},
             "source": [
                 "# Usage styles\n",
                 "\n",
                 "`pandas-indexing` defines two different usage styles:\n",
-                "There are:\n",
+                "\n",
                 "1. functions that can be imported from the toplevel module, like\n",
+                "   \n",
                 "   ```python\n",
                 "   from pandas_indexing import assignlevel\n",
                 "   assignlevel(df, unit=\"Mt CO2e/yr\")\n",
                 "   ```\n",
-                "2. convenience accessors that are hooking into pandas as extensions\n",
+                "2. convenience accessors that are hooking into pandas as extensions, like\n",
+                "   \n",
                 "   ```python\n",
                 "   import pandas_indexing.accessors\n",
                 "   df.idx.assign(unit=\"Mt CO2e/yr)\n",
                 "   ```\n",
                 "\n",
                 "Most of the functionality is available with both styles under slightly different names. I'll present the functional style here first (and add the alternative as comments)"
             ]
@@ -5683,34 +5685,53 @@
                 "    ]\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "c91c2ef3",
+            "id": "ac53aa0b",
+            "metadata": {},
+            "source": [
+                "Therefore, `pandas-indexing` brings a variant which does this automatically:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 31,
+            "id": "ef1d54c6",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "# Additional helpful multi-index helpers\n",
+                "from pandas_indexing import concat\n",
                 "\n",
-                "To know which labels exist in a given `level` the index's `unique` method is helpful:"
+                "concat([simple_fossil_series, simple_fossil_series.swaplevel()])"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "c91c2ef3",
+            "metadata": {},
+            "source": [
+                "# Additional helpful multi-index helpers"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "46c57e84",
             "metadata": {},
             "source": [
                 "MultiIndex rendering is often annoying to read, since the important information might get abbreviated away, then converting it into a dataframe is helpful"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": null,
             "id": "5b7cb7db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MultiIndex([('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
@@ -5724,26 +5745,26 @@
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...)],\n",
                             "           names=['model', 'scenario', 'variable'])"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 33,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series.index, [\"model\", \"scenario\", \"variable\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": null,
             "id": "5b7cb7db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -5858,15 +5879,15 @@
                             "7   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900      Gas\n",
                             "8   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "9   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "10  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "11  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 34,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series.index, [\"model\", \"scenario\", \"variable\"]).to_frame(\n",
                 "    index=False\n",
```

### Comparing `pandas-indexing-0.2.5/pyproject.toml` & `pandas-indexing-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.6/src/pandas_indexing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from . import core, datasets
 from .arithmetics import add, divide, multiply, subtract
 from .core import (
     alignlevel,
     alignlevels,
     assignlevel,
+    concat,
     describelevel,
     dropnalevel,
     extractlevel,
     formatlevel,
     index_names,
     projectlevel,
     semijoin,
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.6/src/pandas_indexing/accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 from typing import Any, Literal, Optional, Sequence, Union
 
 import pandas as pd
 from pandas import DataFrame, Index, MultiIndex, Series
 
 from . import arithmetics
 from .core import (
-    Data,
     assignlevel,
     describelevel,
     dropnalevel,
     extractlevel,
     formatlevel,
     isna,
     notna,
     projectlevel,
     semijoin,
     uniquelevel,
 )
-from .utils import Axis, doc
+from .types import Axis, Data
+from .utils import doc
 
 
 class _IdxAccessor:
     """
     Convenience accessor for accessing `pandas-indexing` functions.
     """
 
@@ -93,15 +93,15 @@
     @doc(isna, index_or_data="")
     def isna(
         self,
         subset: Optional[Sequence[str]] = None,
         how: Literal["any", "all"] = "any",
         axis: Axis = 0,
     ):
-        return ~isna(self._obj, subset=subset, how=how, axis=axis)
+        return isna(self._obj, subset=subset, how=how, axis=axis)
 
     @doc(dropnalevel, index_or_data="")
     def dropna(
         self,
         subset: Optional[Sequence[str]] = None,
         how: Literal["any", "all"] = "any",
         axis: Axis = 0,
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.6/src/pandas_indexing/arithmetics.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pandas.DataFrame.align
 """
 
 from typing import Any, Mapping, Tuple
 
 from pandas import DataFrame, Series
 
-from .core import Data
+from .types import Data
 
 
 def _needs_axis(df: Data, other: Data) -> bool:
     return (isinstance(df, DataFrame) and isinstance(other, Series)) or (
         isinstance(df, Series) and isinstance(other, DataFrame)
     )
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/core.py` & `pandas-indexing-0.2.6/src/pandas_indexing/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 Core module.
 """
 import re
 from functools import reduce
 from itertools import chain
 from operator import and_, or_
-from typing import Any, Literal, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Any, Iterable, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
+import pandas as pd
 from deprecated import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.core.indexes.frozen import FrozenList
 
-from .utils import Axis, doc, get_axis, print_list
-
-
-Data = Union[Series, DataFrame]
-T = TypeVar("T", bound=Union[Index, DataFrame, Series])
-S = TypeVar("S", bound=Union[DataFrame, Series])
+from .types import Axis, Data, S, T
+from .utils import doc, get_axis, print_list
 
 
 def _assignlevel(
     index: Index, frame: Optional[Data] = None, order: bool = False, **labels: Any
 ) -> MultiIndex:
     if isinstance(index, MultiIndex):
         new_levels = list(index.levels)
@@ -144,14 +141,91 @@
     if isinstance(index_or_data, Index):
         return _projectlevel(index_or_data, levels)
 
     index = get_axis(index_or_data.index, axis)
     return index_or_data.set_axis(_projectlevel(index, levels), axis=axis)
 
 
+def concat(
+    objs: Union[Iterable[S], Mapping[str, S]],
+    order: Optional[Sequence[str]] = None,
+    axis: Axis = 0,
+    keys: Union[None, str, Index, Sequence] = None,
+    copy: bool = False,
+    **concat_kwds,
+) -> S:
+    """Concatenate pandas objects along a particular axis.
+
+    In addition to the functionality provided by pd.concat, if the concat axis has a multiindex
+    then the level order is reordered consistently.
+
+    Parameters
+    ----------
+    objs : a sequence or mapping of Series or DataFrame objects
+        If a mapping is passed the keys will be used as a new index level
+        (with the name of the `keys` argument).
+    order : a sequence of str, default None
+        The order of level names in which to concatenate
+    axis : Axis
+        Axis along which to concatenate
+    keys : str or list-like of str
+        If `objs` is a mapping, a string-like value will be used as name of the new level,
+        otherwise it is passed on to pd.concat.
+    copy : bool, default False
+        Whether to copy the underlying data
+    **concat_kwds
+        Other arguments accepted by pd.concat
+
+    Returns
+    -------
+    Concatenated data
+
+    Raises
+    ------
+    ValueError
+        If the level names of `objs` do not match
+
+    See also
+    --------
+    pandas.concat
+    """
+
+    if isinstance(objs, dict):
+        objs = {k: v for k, v in objs.items() if v is not None}
+        keys = Index(objs.keys(), name=keys)
+        objs = list(objs.values())
+    else:
+        objs = [obj for obj in objs if obj is not None]
+
+    if not objs:
+        raise ValueError("Need at least one element to concatenate")
+
+    if order is None:
+        order = get_axis(objs[0], axis=axis).names
+    elif isinstance(keys, Index):
+        # make sure the order list does not include the new axis name
+        order = [o for o in order if o != keys.name]
+
+    orderset = frozenset(order)
+
+    def reorder(df_or_ser):
+        ax = get_axis(df_or_ser, axis=axis)
+        if ax.names == order:
+            return df_or_ser
+        elif not set(ax.names) == orderset:
+            raise ValueError(
+                "All objects need to have the same index levels, but "
+                f"{set(orderset)} != {set(ax.names)}"
+            )
+
+        return df_or_ser.set_axis(ax.reorder_levels(order), axis=axis, copy=False)
+
+    return pd.concat([reorder(o) for o in objs], keys=keys, copy=copy, **concat_kwds)
+
+
 def _notna(
     index: Index,
     subset: Optional[Sequence[str]] = None,
     how: Literal["any", "all"] = "any",
 ) -> np.ndarray:
     if not isinstance(index, MultiIndex):
         return index.notna()
@@ -476,19 +550,24 @@
             f"frame_or_series must derive from DataFrame or Series, but is {type(frame_or_series)}"
         )
 
     return cls(data, *axes).__finalize__(frame_or_series)
 
 
 def _extractlevel(
-    index: Index, drop: bool = False, **templates: str
+    index: Index, template: Optional[str] = None, drop: bool = False, **templates: str
 ) -> Tuple[Index, list[str]]:
     index = ensure_multiindex(index)
     all_identifiers = set()
 
+    if template is not None:
+        if len(index.names) > 1:
+            raise ValueError("``template`` may only be non-null for single index level")
+        templates[index.names[0]] = template
+
     for dim, template in templates.items():
         identifiers = re.findall(r"\{([a-zA-Z_]+)\}", template)
         all_identifiers.update(identifiers)
         if dim not in index.names:
             raise ValueError(f"{dim} not a dimension of index: {index.names}")
 
         levelnum = index.names.index(dim)
@@ -516,25 +595,29 @@
     index_or_data="""
     index_or_data : DataFrame, Series or Index
         Data to modify\
     """
 )
 def extractlevel(
     index_or_data: T,
+    template: Optional[str] = None,
+    *,
     drop: bool = False,
     dropna: bool = True,
     axis: Axis = 0,
     **templates: str,
 ) -> T:
     """Split an index ``dim`` ension into multiple ones based on a
     ``template``.
 
     Parameters
     ----------\
     {index_or_data}
+    template : str, optional
+        Extraction template for a single level
     drop : bool, default False
         Whether to keep the split dimension
     dropna : bool, default True
         Whether to drop the non-matching levels
     axis : {{0, 1, "index", "columns"}}, default 0
         Axis of DataFrame to extract from
     **templates : str
@@ -544,20 +627,24 @@
     -------
     Index, Series or DataFrame
 
     Raises
     ------
     ValueError
         If ``dim`` is not a dimension of ``index_or_series``
+    ValueError
+        If ``template`` is given, while index has more than one level
     """
     if isinstance(index_or_data, Index):
-        index_or_data, identifiers = _extractlevel(index_or_data, drop, **templates)
+        index_or_data, identifiers = _extractlevel(
+            index_or_data, template, drop, **templates
+        )
     else:
         index, identifiers = _extractlevel(
-            get_axis(index_or_data, axis), drop, **templates
+            get_axis(index_or_data, axis), template, drop, **templates
         )
         index_or_data = index_or_data.set_axis(index, axis=axis)
 
     if dropna:
         index_or_data = dropnalevel(index_or_data, subset=identifiers, axis=axis)
 
     return index_or_data
@@ -576,18 +663,29 @@
             string += template[prev_end:start] + projectlevel(index, level).astype(str)
             prev_end = end
             used_levels.add(level)
         string += template[prev_end:]
 
         levels[dim] = string
 
-    if drop:
-        used_levels.difference_update(templates)
-        if used_levels:
-            index = index.droplevel(list(used_levels))
+    used_levels.difference_update(templates)
+
+    if drop and used_levels:
+        if len(used_levels) == len(index.levels):
+            # none remain
+            def expand_to_array(val):
+                return (
+                    val if not np.isscalar(val) else np.full(len(index), fill_value=val)
+                )
+
+            return MultiIndex.from_arrays(
+                map(expand_to_array, levels.values()), names=levels.keys()
+            )
+
+        index = index.droplevel(list(used_levels))
 
     return assignlevel(index, **levels)
 
 
 @doc(
     index_or_data="""
     index_or_data : DataFrame, Series or Index
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.6/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.6/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.6/src/pandas_indexing/selectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from operator import and_
 from typing import Any, Mapping, Optional, Union
 
 import numpy as np
 from attrs import define, field
 from pandas import DataFrame, Index, Series
 
-from .core import Data
+from .types import Data
 from .utils import shell_pattern_to_regex
 
 
 def maybe_const(x):
     return x if isinstance(x, Selector) else Const(x)
 
 
@@ -80,16 +80,20 @@
         else:
             index = df.index
 
         filters = self.filters
         if self.ignore_missing_levels:
             filters = {k: v for k, v in filters.items() if k in index.names}
 
-        tests = (index.isin(np.atleast_1d(v), level=k) for k, v in filters.items())
-        return reduce(and_, tests)
+        def apply_filter(value, level):
+            if callable(value):
+                return value(index.get_level_values(level))
+            return index.isin(np.atleast_1d(value), level=level)
+
+        return reduce(and_, (apply_filter(v, k) for k, v in filters.items()))
 
 
 def isin(
     df: Optional[Data] = None, ignore_missing_levels: bool = False, **filters: Any
 ) -> Union[Isin, Series]:
     """Constructs a MultiIndex selector.
 
@@ -97,14 +101,15 @@
     ---------
     df : Data, optional
         Data on which to match, if missing an ``Isin`` object is returned
     ignore_missing_levels : bool, default False
         If set, levels missing in data index will be ignored
     **filters
         Filter to apply on given levels (lists are ``or`` ed, levels are ``and`` ed)
+        Callables are evaluated on the index level values.
 
     Returns
     -------
     Isin or Series
 
     Example
     -------
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing/utils.py` & `pandas-indexing-0.2.6/src/pandas_indexing/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Utils module.
 
 Simple utility functions not of greater interest
 """
-from typing import Literal, Union
+from typing import Union
 
 from pandas import DataFrame, Index, Series
 from pandas.util._decorators import doc  # noqa: F401
 
-
-Axis = Literal[0, 1, "index", "columns"]
+from .types import Axis
 
 
 def shell_pattern_to_regex(s):
     """
     Escape characters with specific regexp use.
     """
     return (
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.6/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.5
+Version: 0.2.6
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.5/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.6/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/usage.rst
 docs/notebooks/introduction.ipynb
 src/pandas_indexing/__init__.py
 src/pandas_indexing/accessors.py
 src/pandas_indexing/arithmetics.py
 src/pandas_indexing/core.py
 src/pandas_indexing/selectors.py
+src/pandas_indexing/types.py
 src/pandas_indexing/utils.py
 src/pandas_indexing.egg-info/PKG-INFO
 src/pandas_indexing.egg-info/SOURCES.txt
 src/pandas_indexing.egg-info/dependency_links.txt
 src/pandas_indexing.egg-info/requires.txt
 src/pandas_indexing.egg-info/top_level.txt
 src/pandas_indexing/datasets/__init__.py
```

