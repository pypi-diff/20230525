# Comparing `tmp/sas7bdat_converter-1.3.0.tar.gz` & `tmp/sas7bdat_converter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sas7bdat_converter-1.3.0.tar", max compression
+gzip compressed data, was "sas7bdat_converter-2.0.0.tar", max compression
```

## Comparing `sas7bdat_converter-1.3.0.tar` & `sas7bdat_converter-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1074 2022-12-07 02:51:23.112654 sas7bdat_converter-1.3.0/LICENSE
--rw-r--r--   0        0        0    15839 2022-12-07 02:51:23.112654 sas7bdat_converter-1.3.0/README.md
--rw-r--r--   0        0        0     2079 2022-12-07 02:51:23.112654 sas7bdat_converter-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      695 2022-12-07 02:51:23.112654 sas7bdat_converter-1.3.0/sas7bdat_converter/__init__.py
--rw-r--r--   0        0        0    22713 2022-12-07 02:51:23.112654 sas7bdat_converter-1.3.0/sas7bdat_converter/converter.py
--rw-r--r--   0        0        0        0 2022-12-07 02:51:23.112654 sas7bdat_converter-1.3.0/sas7bdat_converter/py.typed
--rw-r--r--   0        0        0    17303 1970-01-01 00:00:00.000000 sas7bdat_converter-1.3.0/setup.py
--rw-r--r--   0        0        0    17093 1970-01-01 00:00:00.000000 sas7bdat_converter-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 02:34:47.895068 sas7bdat_converter-2.0.0/LICENSE
+-rw-r--r--   0        0        0    15839 2023-05-25 02:34:47.895068 sas7bdat_converter-2.0.0/README.md
+-rw-r--r--   0        0        0     2016 2023-05-25 02:34:47.895068 sas7bdat_converter-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-05-25 02:34:47.895068 sas7bdat_converter-2.0.0/sas7bdat_converter/__init__.py
+-rw-r--r--   0        0        0    23411 2023-05-25 02:34:47.895068 sas7bdat_converter-2.0.0/sas7bdat_converter/converter.py
+-rw-r--r--   0        0        0        0 2023-05-25 02:34:47.895068 sas7bdat_converter-2.0.0/sas7bdat_converter/py.typed
+-rw-r--r--   0        0        0    17028 1970-01-01 00:00:00.000000 sas7bdat_converter-2.0.0/PKG-INFO
```

### Comparing `sas7bdat_converter-1.3.0/LICENSE` & `sas7bdat_converter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter-1.3.0/README.md` & `sas7bdat_converter-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter-1.3.0/pyproject.toml` & `sas7bdat_converter-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "sas7bdat_converter"
-version = "1.3.0"
+version = "2.0.0"
 description = "Convert sas7bdat and xport files into other formats"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/sas7bdat-converter"
 homepage = "https://github.com/sanders41/sas7bdat-converter"
 documentation = "https://github.com/sanders41/sas7bdat-converter"
 keywords = ["sas", "sas7bdat", "converter", "xpt", "XPort"]
 classifiers=[
+  "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
+  "Typing :: Typed",
 ]
 include = ["sas7bdat_converter/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 pandas = ">=1.2.0"
 openpyxl = {version = ">=3.0.5", optional = true}
@@ -27,21 +29,20 @@
 [tool.poetry.extras]
 excel = ["openpyxl"]
 parquet = ["pyarrow"]
 all = ["openpyxl", "pyarrow"]
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.8.0"
-isort = ">=5.10.1"
 mypy = ">=0.981"
 pre-commit = ">=2.20.0"
 pytest = ">=7.1.3"
 pytest-cov = ">=4.0.0"
-ruff = "^0.0.141"
-tox = ">=3.26.0"
+ruff = ">=0.0.253"
+pandas-stubs = ">=2.0.1.230501"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
@@ -61,31 +62,28 @@
   | buck-out
   | build
   | dist
   | setup.py
 )/
 '''
 
-[tool.isort]
-profile = "black"
-line_length = 100
-src_paths = ["sas7bdat_converter", "tests"]
-
 [tool.mypy]
 disallow_untyped_defs = true
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
-module = ["numpy.*", "pandas.*", "pyarrow.*"]
+module = ["pyarrow.*"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov=sas7bdat_converter --cov-report term-missing"
 
 [tool.ruff]
-select=["T201", "T203"]
-ignore=["E501", "D100", "D101", "D102", "D103", "D104", "D105", "D106", "D107"]
+select = ["E", "F", "T201", "T203", "I001"]
+ignore = ["E501"]
+line-length = 100
+fix = true
```

### Comparing `sas7bdat_converter-1.3.0/sas7bdat_converter/__init__.py` & `sas7bdat_converter-2.0.0/sas7bdat_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter-1.3.0/sas7bdat_converter/converter.py` & `sas7bdat_converter-2.0.0/sas7bdat_converter/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,218 +1,236 @@
 from __future__ import annotations
 
 import csv
-import logging
 from pathlib import Path
 from xml.sax.saxutils import escape
 
 import numpy as np
 import pandas as pd
 
-logging.basicConfig(format="%(asctime)s: %(levelname)s: %(message)s")
-logging.root.setLevel(level=logging.INFO)
-logger = logging.getLogger(__name__)
-
-__FILE_DICT_REQUIRED_KEYS = [
+_FILE_DICT_REQUIRED_KEYS = [
     "sas7bdat_file",
     "export_file",
 ]
 
 
 def batch_to_csv(
     file_dicts: list[dict[str, str | Path]],
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts a batch of sas7bdat and/or xpt files to csv files.
 
     Args:
         file_dicts: A list dictionaries containing the files to convert. The dictionary should
-                    contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
-                    file) and 'export_file' containing the path and name of the export csv).
-                    Example: file_dict = [{
-                                              'sas7bdat_file': 'sas_file1.sas7bdat',
-                                              'export_file': 'converted_file1.csv',
-                                          },
-                                          {
-                                              'sas7bdat_file': 'sas_file2.sas7bdat',
-                                              'export_file': 'converted_file2.csv',
-                                          }]
+            contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
+            file) and 'export_file' containing the path and name of the export csv).
+            Example: file_dict = [{
+                                      'sas7bdat_file': 'sas_file1.sas7bdat',
+                                      'export_file': 'converted_file1.csv',
+                                  },
+                                  {
+                                      'sas7bdat_file': 'sas_file2.sas7bdat',
+                                      'export_file': 'converted_file2.csv',
+                                  }]
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                    a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
     for file_dict in file_dicts:
         _rise_on_invalid_file_dict(file_dict)
 
-        xpt = _format_path(file_dict["sas7bdat_file"])
+        sas7bdat = _format_path(file_dict["sas7bdat_file"])
         export = _format_path(file_dict["export_file"])
         try:
-            to_csv(sas7bdat_file=xpt, export_file=export)
+            to_csv(sas7bdat_file=sas7bdat, export_file=export)
         except:  # noqa: E722
-            if continue_on_error:
-                logger.info(f"Error converting {xpt}")
+            if continue_on_error and verbose:
+                print(f"Error converting {sas7bdat}")  # noqa: T201
+            elif continue_on_error:
+                pass
             else:
                 raise
 
 
 def batch_to_parquet(
     file_dicts: list[dict[str, str | Path]],
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts a batch of sas7bdat and/or xpt files to parquet files.
 
     Args:
         file_dicts: A list dictionaries containing the files to convert. The dictionary should
-                    contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
-                    file) and 'export_file' containing the path and name of the export parquet).
-                    Example: file_dict = [{
-                                              'sas7bdat_file': 'sas_file1.sas7bdat',
-                                              'export_file': 'converted_file1.parquet',
-                                          },
-                                          {
-                                              'sas7bdat_file': 'sas_file2.sas7bdat',
-                                              'export_file': 'converted_file2.parquet',
-                                          }]
+            contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
+            file) and 'export_file' containing the path and name of the export parquet).
+            Example: file_dict = [{
+                                      'sas7bdat_file': 'sas_file1.sas7bdat',
+                                      'export_file': 'converted_file1.parquet',
+                                  },
+                                  {
+                                      'sas7bdat_file': 'sas_file2.sas7bdat',
+                                      'export_file': 'converted_file2.parquet',
+                                  }]
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                    a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
     for file_dict in file_dicts:
         _rise_on_invalid_file_dict(file_dict)
 
-        xpt = _format_path(file_dict["sas7bdat_file"])
+        sas7bdat = _format_path(file_dict["sas7bdat_file"])
         export = _format_path(file_dict["export_file"])
         try:
-            to_parquet(sas7bdat_file=xpt, export_file=export)
+            to_parquet(sas7bdat_file=sas7bdat, export_file=export)
         except:  # noqa: E722
-            if continue_on_error:
-                logger.info(f"Error converting {xpt}")
+            if continue_on_error and verbose:
+                print(f"Error converting {sas7bdat}")  # noqa: T201
+            elif continue_on_error:
+                pass
             else:
                 raise
 
 
 def batch_to_excel(
     file_dicts: list[dict[str, str | Path]],
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts a batch of sas7bdat and/or xpt files to xlsx files.
 
     Args:
         file_dicts: A list of dictionaries containing the files to convert. The dictionary should
-                    contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
-                    file) and 'export_file' containing the path and name of the export xlsx).
-                    Example: file_dict = [{
-                                              'sas7bdat_file': 'sas_file1.sas7bdat',
-                                              'export_file': 'converted_file1.xlsx',
-                                          },
-                                          {
-                                              'sas7bdat_file': 'sas_file2.sas7bdat',
-                                              'export_file': 'converted_file2.xlxs',
-                                          }]
+            contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
+            file) and 'export_file' containing the path and name of the export xlsx).
+            Example: file_dict = [{
+                                      'sas7bdat_file': 'sas_file1.sas7bdat',
+                                      'export_file': 'converted_file1.xlsx',
+                                  },
+                                  {
+                                      'sas7bdat_file': 'sas_file2.sas7bdat',
+                                      'export_file': 'converted_file2.xlxs',
+                                  }]
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                    a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
     for file_dict in file_dicts:
         _rise_on_invalid_file_dict(file_dict)
 
         sas7bdat = _format_path(file_dict["sas7bdat_file"])
         export = _format_path(file_dict["export_file"])
         try:
             to_excel(sas7bdat_file=sas7bdat, export_file=export)
         except:  # noqa: 722
-            if continue_on_error:
-                logger.info(f"Error converting {sas7bdat}")
+            if continue_on_error and verbose:
+                print(f"Error converting {sas7bdat}")  # noqa: T201
+            elif continue_on_error:
+                pass
             else:
                 raise
 
 
 def batch_to_json(
     file_dicts: list[dict[str, str | Path]],
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts a batch of sas7bdat and/or xpt files to json files.
 
     Args:
         file_dicts: A list dictionaries containing the files to convert. The dictionary should
-                    contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
-                    file) and 'export_file' containing the path and name of the export json).
-                    Example: file_dict = [{
-                                              'sas7bdat_file': 'sas_file1.sas7bdat',
-                                              'export_file': 'converted_file1.json',
-                                          },
-                                          {
-                                              'sas7bdat_file': 'sas_file2.sas7bdat',
-                                              'export_file': 'converted_file2.json',
-                                          }]
+            contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
+            file) and 'export_file' containing the path and name of the export json).
+            Example: file_dict = [{
+                                      'sas7bdat_file': 'sas_file1.sas7bdat',
+                                      'export_file': 'converted_file1.json',
+                                  },
+                                  {
+                                      'sas7bdat_file': 'sas_file2.sas7bdat',
+                                      'export_file': 'converted_file2.json',
+                                  }]
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                    a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
     for file_dict in file_dicts:
         _rise_on_invalid_file_dict(file_dict)
 
         sas7bdat = _format_path(file_dict["sas7bdat_file"])
         export = _format_path(file_dict["export_file"])
         try:
             to_json(sas7bdat_file=sas7bdat, export_file=export)
         except:  # noqa: 722
-            if continue_on_error:
-                logger.info(f"Error converting {sas7bdat}")
+            if continue_on_error and verbose:
+                print(f"Error converting {sas7bdat}")  # noqa: T201
+            elif continue_on_error:
+                pass
             else:
                 raise
 
 
 def batch_to_xml(
     file_dicts: list[dict[str, str | Path]],
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts a batch of sas7bdat and/or xpt files to xml files.
 
     Args:
         file_dicts: A list dictionaries containing the files to convert. The dictionary should
-                    contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
-                    file) and 'export_file' containing the path and name of the export xml).
-                    Optinallly the dictionary can also contain 'root_node' (containing the name for
-                    the root node in the xml file, and 'first_node' (containing the name for the
-                    first node in the xml file).
-                    Examples: file_dict = [{'sas7bdat_file': 'sas_file1.sas7bdat',
-                                            'export_file': 'converted_file1.xlsx'},
-                                           {'sas7bdat_file': 'sas_file2.sas7bdat',
-                                            'export_file': 'converted_file2.xlxs'}]
-
-                              file_dict = [{'sas7bdat_file': 'sas_file1.sas7bdat',
-                                            'export_file': 'converted_file1.xml',
-                                            'root_node': 'my_root',
-                                            'first_node': 'my_first'},
-                                           {'sas7bdat_file': 'sas_file2.sas7bdat',
-                                            'export_file': 'converted_file2.xml',
-                                            'root_node': 'another_root',
-                                            'first_node': 'another_first'}]
+            contain the keys 'sas7bdat_file' (containing the path and name to the sas7bdat
+            file) and 'export_file' containing the path and name of the export xml).
+            Optinallly the dictionary can also contain 'root_node' (containing the name for
+            the root node in the xml file, and 'first_node' (containing the name for the
+            first node in the xml file).
+            Examples: file_dict = [{'sas7bdat_file': 'sas_file1.sas7bdat',
+                                    'export_file': 'converted_file1.xlsx'},
+                                   {'sas7bdat_file': 'sas_file2.sas7bdat',
+                                    'export_file': 'converted_file2.xlxs'}]
+
+                      file_dict = [{'sas7bdat_file': 'sas_file1.sas7bdat',
+                                    'export_file': 'converted_file1.xml',
+                                    'root_node': 'my_root',
+                                    'first_node': 'my_first'},
+                                   {'sas7bdat_file': 'sas_file2.sas7bdat',
+                                    'export_file': 'converted_file2.xml',
+                                    'root_node': 'another_root',
+                                    'first_node': 'another_first'}]
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                    a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
     optional_keys = [
         "root_node",
         "first_node",
     ]
     for file_dict in file_dicts:
         error = False
-        if len(set(file_dict).intersection(__FILE_DICT_REQUIRED_KEYS)) != len(
-            __FILE_DICT_REQUIRED_KEYS
-        ) or len(set(file_dict).intersection(__FILE_DICT_REQUIRED_KEYS)) > len(
-            __FILE_DICT_REQUIRED_KEYS
+        if len(set(file_dict).intersection(_FILE_DICT_REQUIRED_KEYS)) != len(
+            _FILE_DICT_REQUIRED_KEYS
+        ) or len(set(file_dict).intersection(_FILE_DICT_REQUIRED_KEYS)) > len(
+            _FILE_DICT_REQUIRED_KEYS
         ) + len(
             optional_keys
         ):
             error = True
         elif len(set(file_dict).intersection(optional_keys)) != len(file_dict) - len(
-            __FILE_DICT_REQUIRED_KEYS
+            _FILE_DICT_REQUIRED_KEYS
         ):
             error = True
 
         if error:
             message = _invalid_key_exception_message(
-                required_keys=__FILE_DICT_REQUIRED_KEYS, optional_keys=optional_keys
+                required_keys=_FILE_DICT_REQUIRED_KEYS, optional_keys=optional_keys
             )
             raise KeyError(message)
 
         sas7bdat = _format_path(file_dict["sas7bdat_file"])
         export = _format_path(file_dict["export_file"])
         root_node = None
         first_node = None
@@ -232,111 +250,130 @@
             elif root_node:
                 to_xml(sas7bdat_file=sas7bdat, export_file=export, root_node=str(root_node))
             elif first_node:
                 to_xml(sas7bdat_file=sas7bdat, export_file=export, first_node=str(first_node))
             else:
                 to_xml(sas7bdat_file=sas7bdat, export_file=export)
         except:  # noqa: 722
-            if continue_on_error:
-                logger.info(f"Error converting {sas7bdat}")
+            if continue_on_error and verbose:
+                print(f"Error converting {sas7bdat}")  # noqa: T201
+            elif continue_on_error:
+                pass
             else:
                 raise
 
 
 def dir_to_csv(
     dir_path: str | Path,
     export_path: str | Path | None = None,
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts all sas7bdat and/or xpt files in a directory into csv files.
 
     args:
         dir_path: The path to the directory that contains the sas7bdat files
-                for conversion.
+            for conversion.
         export_path (optional): If used this can specify a new directory to create
-                the converted files into. If not supplied then the files will be
-                created into the same directory as dir_path. Default = None
+            the converted files into. If not supplied then the files will be
+            created into the same directory as dir_path. Default = None
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
-    _walk_dir("csv", dir_path, continue_on_error, export_path)
+    _walk_dir("csv", dir_path, export_path, continue_on_error, verbose)
 
 
 def dir_to_excel(
     dir_path: str | Path,
     export_path: str | Path | None = None,
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts all sas7bdat and/or xpt files in a directory into xlsx files.
 
     args:
         dir_path: The path to the directory that contains the sas7bdat files
-                for conversion.
+            for conversion.
         export_path (optional): If used this can specify a new directory to create
-                the converted files into. If not supplied then the files will be
-                created into the same directory as dir_path. Default = None
+            the converted files into. If not supplied then the files will be
+            created into the same directory as dir_path. Default = None
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
-    _walk_dir("xlsx", dir_path, continue_on_error, export_path)
+    _walk_dir("xlsx", dir_path, export_path, continue_on_error, verbose)
 
 
 def dir_to_json(
     dir_path: str | Path,
     export_path: str | Path | None = None,
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts all sas7bdat and/or xpt files in a directory into json files.
 
     args:
         dir_path: The path to the directory that contains the sas7bdat files
-                for conversion.
+            for conversion.
         export_path (optional): If used this can specify a new directory to create
-                the converted files into. If not supplied then the files will be
-                created into the same directory as dir_path. Default = None
+            the converted files into. If not supplied then the files will be
+            created into the same directory as dir_path. Default = None
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
-    _walk_dir("json", dir_path, continue_on_error, export_path)
+    _walk_dir("json", dir_path, export_path, continue_on_error, verbose)
 
 
 def dir_to_parquet(
-    dir_path: str | Path, export_path: str | Path | None = None, continue_on_error: bool = False
+    dir_path: str | Path,
+    export_path: str | Path | None = None,
+    *,
+    continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts all sas7bdat and/or xpt files in a directory into a parquet files.
 
     args:
         dir_path: The path to the directory that contains the sas7bdat files
-                for conversion.
+            for conversion.
         export_path (optional): If used this can specify a new directory to create
-                the converted files into. If not supplied then the files will be
-                created into the same directory as dir_path. Default = None
+            the converted files into. If not supplied then the files will be
+            created into the same directory as dir_path. Default = None
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
-    _walk_dir("parquet", dir_path, continue_on_error, export_path)
+    _walk_dir("parquet", dir_path, export_path, continue_on_error, verbose)
 
 
 def dir_to_xml(
     dir_path: str | Path,
     export_path: str | Path | None = None,
+    *,
     continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     """Converts all sas7bdat and/or xpt files in a directory into xml files.
 
     args:
         dir_path: The path to the directory that contains the sas7bdat files
-                for conversion.
+            for conversion.
         export_path (optional): If used this can specify a new directory to create
-                the converted files into. If not supplied then the files will be
-                created into the same directory as dir_path. Default = None
+            the converted files into. If not supplied then the files will be
+            created into the same directory as dir_path. Default = None
         continue_on_error: If set to true processing of files in a batch will continue if there is
-                a file conversion error instead of raising an exception. Default = False
+            a file conversion error instead of raising an exception. Default = False
+        verbose: Increases the output. Default = True
     """
-    _walk_dir("xml", dir_path, continue_on_error, export_path)
+    _walk_dir("xml", dir_path, export_path, continue_on_error, verbose)
 
 
 def to_csv(sas7bdat_file: str | Path, export_file: str | Path) -> None:
     """Converts a sas7bdat and/or xpt file into a csv file.
 
     args:
         sas7bdat_file: The name, including the path, for the sas7bdat file.
@@ -385,15 +422,15 @@
 
     return:
         A pandas dataframe containing the data from the sas7bdat file.
     """
     df = pd.read_sas(sas7bdat_file)
 
     # convert binary strings to utf-8
-    str_df = df.select_dtypes([np.dtype(object)])
+    str_df = df.select_dtypes([str(np.dtype(object))])
     if len(str_df.columns) > 0:
         str_df = str_df.stack().str.decode("utf-8").unstack()
 
         for col in str_df:
             df[col] = str_df[col]
     # end conversion to utf-8
 
@@ -509,26 +546,25 @@
 
 
 def _format_path(path: str | Path) -> str:
     return str(path) if isinstance(path, Path) else path
 
 
 def _rise_on_invalid_file_dict(file_dict: dict[str, str | Path]) -> None:
-    if len(set(file_dict).intersection(__FILE_DICT_REQUIRED_KEYS)) != len(
-        __FILE_DICT_REQUIRED_KEYS
-    ):
-        message = _invalid_key_exception_message(required_keys=__FILE_DICT_REQUIRED_KEYS)
+    if len(set(file_dict).intersection(_FILE_DICT_REQUIRED_KEYS)) != len(_FILE_DICT_REQUIRED_KEYS):
+        message = _invalid_key_exception_message(required_keys=_FILE_DICT_REQUIRED_KEYS)
         raise KeyError(message)
 
 
 def _walk_dir(
     file_type: str,
     dir_path: str | Path,
-    continue_on_error: bool,
     export_path: str | Path | None = None,
+    continue_on_error: bool = False,
+    verbose: bool = True,
 ) -> None:
     path = dir_path if isinstance(dir_path, Path) else Path(dir_path)
     for file_name in path.iterdir():
         if file_name.suffix in [".sas7bdat", ".xpt"]:
             export_file = Path(f"{file_name.stem}.{file_type}")
             if export_path:
                 export_file = Path(export_path).joinpath(export_file)
@@ -545,11 +581,13 @@
                 elif file_type == "xlsx":
                     to_excel(str(sas7bdat_file), str(export_file))
                 elif file_type == "xml":
                     to_xml(str(sas7bdat_file), str(export_file))
                 elif file_type == "parquet":
                     to_parquet(str(sas7bdat_file), str(export_file))
             except:  # noqa: 722
-                if continue_on_error:
-                    logger.info(f"Error converting {sas7bdat_file}")
+                if continue_on_error and verbose:
+                    print(f"Error converting {sas7bdat_file}")  # noqa: T201
+                elif continue_on_error:
+                    pass
                 else:
                     raise
```

### Comparing `sas7bdat_converter-1.3.0/setup.py` & `sas7bdat_converter-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,405 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sas7bdat-converter
+Version: 2.0.0
+Summary: Convert sas7bdat and xport files into other formats
+Home-page: https://github.com/sanders41/sas7bdat-converter
+License: MIT
+Keywords: sas,sas7bdat,converter,xpt,XPort
+Author: Paul Sanders
+Author-email: psanders1@gmail.com
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Provides-Extra: all
+Provides-Extra: excel
+Provides-Extra: parquet
+Requires-Dist: openpyxl (>=3.0.5) ; extra == "excel" or extra == "all"
+Requires-Dist: pandas (>=1.2.0)
+Requires-Dist: pyarrow (>=9.0.0) ; extra == "parquet" or extra == "all"
+Project-URL: Documentation, https://github.com/sanders41/sas7bdat-converter
+Project-URL: Repository, https://github.com/sanders41/sas7bdat-converter
+Description-Content-Type: text/markdown
 
-packages = \
-['sas7bdat_converter']
+# sas7bdat-converter: Convert sas7bdat files into other formats
 
-package_data = \
-{'': ['*']}
+[![Tests Status](https://github.com/sanders41/sas7bdat-converter/workflows/Tests/badge.svg?branch=main&event=push)](https://github.com/sanders41/sas7bdat-converter/actions?query=workflow%3ATests+branch%3Amain+event%3Apush)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/sas7bdat-converter/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/sas7bdat-converter/main)
+[![Coverage](https://codecov.io/github/sanders41/sas7bdat-converter/coverage.svg?branch=main)](https://codecov.io/gh/sanders41/sas7bdat-converter)
+[![PyPI version](https://badge.fury.io/py/sas7bdat-converter.svg)](https://badge.fury.io/py/sas7bdat-converter)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sas7bdat-converter?color=5cc141)](https://github.com/sanders41/sas7bdat-converter)
 
-install_requires = \
-['pandas>=1.2.0']
-
-extras_require = \
-{'all': ['openpyxl>=3.0.5', 'pyarrow>=9.0.0'],
- 'excel': ['openpyxl>=3.0.5'],
- 'parquet': ['pyarrow>=9.0.0']}
-
-setup_kwargs = {
-    'name': 'sas7bdat-converter',
-    'version': '1.3.0',
-    'description': 'Convert sas7bdat and xport files into other formats',
-    'long_description': '# sas7bdat-converter: Convert sas7bdat files into other formats\n\n[![Tests Status](https://github.com/sanders41/sas7bdat-converter/workflows/Tests/badge.svg?branch=main&event=push)](https://github.com/sanders41/sas7bdat-converter/actions?query=workflow%3ATests+branch%3Amain+event%3Apush)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/sas7bdat-converter/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/sas7bdat-converter/main)\n[![Coverage](https://codecov.io/github/sanders41/sas7bdat-converter/coverage.svg?branch=main)](https://codecov.io/gh/sanders41/sas7bdat-converter)\n[![PyPI version](https://badge.fury.io/py/sas7bdat-converter.svg)](https://badge.fury.io/py/sas7bdat-converter)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sas7bdat-converter?color=5cc141)](https://github.com/sanders41/sas7bdat-converter)\n\nConverts proprietary sas7bdat and/or xport files from SAS into formats such as csv, json, and Excel useable\nby other programs. Currently supported conversiaions are csv, Excel (xlsx format), json, Pandas\nDataFrame, Parquet and XML.\n\nConversions can be done on either a single file, an entire directory, or a batch of specified files.\n\n## Install\n\n`pip install sas7bdat-converter`\n\nIf you would like to be able to convert to Excel files you will need to install with the extra Excel dependency.\n\n`pip install sas7bdat-converter[excel]`\n\nIf you would like to be able to convert to Parquet files you will need to install with the extra parquet dependency.\n\n`pip install sas7bdat-converter[parquet]`\n\nIf you would like to use Conda, it includes both the extras required to convert to Excel & Parquet files.\n\n`conda install -c conda-forge sas7bdat-converter`\n\n## Usage\n\nIn all cases either sas7bdat or xport files can be converted. Examples below all use the .sas7bdat\nextension, xport files with a .xpt extension will also work.\n\n* **batch_to_csv(file_dicts)** - Convert multiple sas7bdat files into csv files at once.\n  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required\n  to contain \'sas7bdat_file\' containing the path and name for the sas7bdat file, and \'export_file\'\n  containing the path and name for the csv files. The csv file extension should be .csv. File paths\n  can be sent as either strings or Path objects.\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  file_dicts = [\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_1.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_1.csv\',\n    },\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_2.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_2.csv\',\n    },\n  ]\n  sas7bdat_converter.batch_to_csv(file_dicts)\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example_1.sas7bdat`.\n\n* **batch_to_excel(file_dicts)** - Convert multiple sas7bdat files into Excel files at once.\n  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required\n  to contain \'sas7bdat_file\' containing the path and name for the sas7bdat file, and \'export_file\'\n  containing the path and name for the excel files. The Excel file extension should be .xlsx. File\n  paths can be sent as either strings or Path objects.\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  file_dicts = [\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_1.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_1.xlsx\',\n    },\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_2.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_2.xlsx\',\n    },\n  ]\n  sas7bdat_converter.batch_to_excel(file_dicts)\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example_1.sas7bdat`.\n\n* **batch_to_parquet(file_dicts)** - Convert multiple sas7bdat files into Parquet files at once.\n  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required\n  to contain \'sas7bdat_file\' containing the path and name for the sas7bdat file, and \'export_file\'\n  containing the path and name for the perquet files. The Perquet file extension should be .perquet. File\n  paths can be sent as either strings or Path objects.\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  file_dicts = [\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_1.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_1.parquet\',\n    },\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_2.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_2.parquet\',\n    },\n  ]\n  sas7bdat_converter.batch_to_parquet(file_dicts)\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example_1.sas7bdat`.\n\n* **batch_to_json(file_dicts)** - Convert multiple sas7bdat files into json files at once.\n  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required\n  to contain \'sas7bdat_file\' containing the path and name for the sas7bdat file, and \'export_file\'\n  containing the path and name for the json files. The json file extension should be .json. File\n  paths can be sent as either strings or Path objects.\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  file_dicts = [\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_1.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_1.json\',\n    },\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_2.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_2.json\',\n    },\n  ]\n  sas7bdat_converter.batch_to_json(file_dicts)\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example_1.sas7bdat`.\n\n* **batch_to_xml(file_dicts)** - Convert multiple sas7bdat files into XML files at once.\n  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required\n  to contain \'sas7bdat_file\' containing the path and name for the sas7bdat file, and \'export_file\'\n  containing the path and name for the xml files. The XML file extension should be .xml. File paths\n  can be sent as either strings or Path objects.\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  file_dicts = [\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_1.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_1.xml\',\n    },\n    {\n      \'sas7bdat_file\': \'/path/to/sas7bdat/files/example_2.sas7bdat\',\n      \'export_file\': \'/path/to/new/files/example_2.xml\',\n    },\n  ]\n  sas7bdat_converter.batch_to_xml(file_dicts)\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example_1.sas7bdat`.\n\n* **dir_to_csv(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into csv\nfiles at once. File paths can be sent as either strings or Path objects.\n  * dir_path = The dictionary that contains the sas7bdat file to convert.\n  * export_path = Optional path for the converted files. If no path is supplied the new files will\n  be put into the dir_path directory with the sas7bdat files. File paths can be sent as either\n  strings or Path objects. Default = None\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  # Option 1: put the converted files in the same directory as the sas7bdat files\n  sas7bdat_converter.dir_to_csv(\'/path/to/sas7bdat/files\')\n\n  # Option 2: put the converted fiels in a diffferent directory\n  sas7bdat_converter.dir_to_csv(\'/path/to/sas7bdat/files\', \'path/for/new/files\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files`.\n\n* **dir_to_excel(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into\nExcel files at once. File paths can be sent as either strings or Path objects.\n  * dir_path = The dictionary that contains the sas7bdat file to convert.\n  * export_path = Optional path for the converted files. If no path is supplied the new files will\n  be put into the dir_path directory with the sas7bdat files Default = None\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  # Option 1: put the converted files in the same directory as the sas7bdat files\n  sas7bdat_converter.dir_to_excel(\'/path/to/sas7bdat/files\')\n\n  # Option 2: put the converted fiels in a diffferent directory\n  sas7bdat_converter.dir_to_excel(\'/path/to/sas7bdat/files\', \'path/for/new/files\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files`.\n\n* **dir_to_json(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into json\n  files at once. File paths can be sent as either strings or Path objects.\n  * dir_path = The dictionary that contains the sas7bdat file to convert.\n  * export_path = Optional path for the converted files. If no path is supplied the new files will\n  be put into the dir_path directory with the sas7bdat files. Default = None\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  # Option 1: put the converted files in the same directory as the sas7bdat files\n  sas7bdat_converter.dir_to_json(\'/path/to/sas7bdat/files\')\n\n  # Option 2: put the converted fiels in a diffferent directory\n  sas7bdat_converter.dir_to_json(\'/path/to/sas7bdat/files\', \'path/for/new/files\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files`.\n\n* **dir_to_xml(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into XML\n  files at once. File paths can be sent as either strings or Path objects.\n  * dir_path = The dictionary that contains the sas7bdat file to convert.\n  * export_path = Optional path for the converted files. If no path is supplied the new files will\n  be put into the dir_path directory with the sas7bdat files. Default = None\n  * continue_on_error = If set to true processing of files in a batch will continue if there is a\n  file conversion error instead of raising an exception. Default = False\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  # Option 1: put the converted files in the same directory as the sas7bdat files\n  sas7bdat_converter.dir_to_xml(\'/path/to/sas7bdat/files\')\n\n  # Option 2: put the converted fiels in a diffferent directory\n  sas7bdat_converter.dir_to_xml(\'/path/to/sas7bdat/files\', \'path/for/new/files\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files`.\n\n* **to_csv(sas7bdat_file, export_file)** - convert a sas7bdat file into a csv file. File path can be\n  sent as either a string or Path objects.\n  * sas7bdat_file = the path and name for sas7bdat file to convert.\n  * export_file = the path and name for the csv file. The csv file extension should be .csv.\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  sas7bdat_converter.to_csv(\'/path/to/sas7bdat/file/example.sas7bdat\', \'path/to/new/file/example.csv\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example.sas7bdat`.\n\n* **to_dataframe(sas7bdat_file)** - Convert a sas7bdat file into a Pandas DataFrame. File path can\n  be sent as either a string or Path objects.\n  * sas7bdat_file = The path and name for sas7bdat file to convert.\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  sas7bdat_converter.to_dataframe(\'/path/to/sas7bdat/file/example.sas7bdat\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example_1.sas7bdat`.\n\n* **to_excel(sas7bdat_file, export_file)** - convert a sas7bdat file into a Excel file. File path\n  can be sent as either a string or Path objects.\n  * sas7bdat_file = the path and name for sas7bdat file to convert.\n  * export_file = the path and name for the Excel file. The Excel file extension should be .xlsx.\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  sas7bdat_converter.to_excel(\'/path/to/sas7bdat/file/example.sas7bdat\',\n  \'path/to/new/file/example.xlsx\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example.sas7bdat`.\n\n* **to_parquet(sas7bdat_file, export_file)** - convert a sas7bdat file into a Parquet file. File path\n  can be sent as either a string or Path objects.\n  * sas7bdat_file = the path and name for sas7bdat file to convert.\n  * export_file = the path and name for the Parquet file. The Parquet file extension should be .parquet.\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  sas7bdat_converter.to_parquet(\'/path/to/sas7bdat/file/example.sas7bdat\',\n  \'path/to/new/file/example.parquet\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example.sas7bdat`.\n\n* **to_json(sas7bdat_file, export_file)** - convert a sas7bdat file into a json file. File path can\n  be sent as either a string or Path objects.\n  * sas7bdat_file = the path and name for sas7bdat file to convert.\n  * export_file = the path and name for the json file. the json file extension should be .json.\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  sas7bdat_converter.to_json(\'/path/to/sas7bdat/file/example.sas7bdat\', \'path/to/new/file/example.json\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example.sas7bdat`.\n\n* **to_xml(sas7bdat_file, export_file, root_node=\'root\', first_node=\'item\')** - convert a sas7bdat\n  file into a XML file. File path can be sent as either a string or Path objects.\n  * sas7bdat_file = the path and name for sas7bdat file to convert.\n  * export_file = the path and name for the XML file. The XML file extension should be .xlm.\n  * root_node = The name to uses for the top level node. If no name is supplied "root" will be used.\n  * first_node = The name to use for the first node under root. If no name is supplied "item" will be used.\n\n  **Example**\n\n  ```py\n  import sas7bdat_converter\n\n  sas7bdat_converter.to_xml(\'/path/to/sas7bdat/file/example.sas7bdat\', \'path/to/new/file/example.xml\')\n  ```\n\n  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like\n  `c:\\path\\to\\sas7bdat\\files\\example.sas7bdat`.\n\n## Contributing\n\nIf you are interesting in contributing to this project please see our [contributing guide](CONTRIBUTING.md)\n',
-    'author': 'Paul Sanders',
-    'author_email': 'psanders1@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sanders41/sas7bdat-converter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8.0,<4.0.0',
-}
+Converts proprietary sas7bdat and/or xport files from SAS into formats such as csv, json, and Excel useable
+by other programs. Currently supported conversiaions are csv, Excel (xlsx format), json, Pandas
+DataFrame, Parquet and XML.
 
+Conversions can be done on either a single file, an entire directory, or a batch of specified files.
+
+## Install
+
+`pip install sas7bdat-converter`
+
+If you would like to be able to convert to Excel files you will need to install with the extra Excel dependency.
+
+`pip install sas7bdat-converter[excel]`
+
+If you would like to be able to convert to Parquet files you will need to install with the extra parquet dependency.
+
+`pip install sas7bdat-converter[parquet]`
+
+If you would like to use Conda, it includes both the extras required to convert to Excel & Parquet files.
+
+`conda install -c conda-forge sas7bdat-converter`
+
+## Usage
+
+In all cases either sas7bdat or xport files can be converted. Examples below all use the .sas7bdat
+extension, xport files with a .xpt extension will also work.
+
+* **batch_to_csv(file_dicts)** - Convert multiple sas7bdat files into csv files at once.
+  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required
+  to contain 'sas7bdat_file' containing the path and name for the sas7bdat file, and 'export_file'
+  containing the path and name for the csv files. The csv file extension should be .csv. File paths
+  can be sent as either strings or Path objects.
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  file_dicts = [
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_1.sas7bdat',
+      'export_file': '/path/to/new/files/example_1.csv',
+    },
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_2.sas7bdat',
+      'export_file': '/path/to/new/files/example_2.csv',
+    },
+  ]
+  sas7bdat_converter.batch_to_csv(file_dicts)
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example_1.sas7bdat`.
+
+* **batch_to_excel(file_dicts)** - Convert multiple sas7bdat files into Excel files at once.
+  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required
+  to contain 'sas7bdat_file' containing the path and name for the sas7bdat file, and 'export_file'
+  containing the path and name for the excel files. The Excel file extension should be .xlsx. File
+  paths can be sent as either strings or Path objects.
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  file_dicts = [
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_1.sas7bdat',
+      'export_file': '/path/to/new/files/example_1.xlsx',
+    },
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_2.sas7bdat',
+      'export_file': '/path/to/new/files/example_2.xlsx',
+    },
+  ]
+  sas7bdat_converter.batch_to_excel(file_dicts)
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example_1.sas7bdat`.
+
+* **batch_to_parquet(file_dicts)** - Convert multiple sas7bdat files into Parquet files at once.
+  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required
+  to contain 'sas7bdat_file' containing the path and name for the sas7bdat file, and 'export_file'
+  containing the path and name for the perquet files. The Perquet file extension should be .perquet. File
+  paths can be sent as either strings or Path objects.
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  file_dicts = [
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_1.sas7bdat',
+      'export_file': '/path/to/new/files/example_1.parquet',
+    },
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_2.sas7bdat',
+      'export_file': '/path/to/new/files/example_2.parquet',
+    },
+  ]
+  sas7bdat_converter.batch_to_parquet(file_dicts)
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example_1.sas7bdat`.
+
+* **batch_to_json(file_dicts)** - Convert multiple sas7bdat files into json files at once.
+  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required
+  to contain 'sas7bdat_file' containing the path and name for the sas7bdat file, and 'export_file'
+  containing the path and name for the json files. The json file extension should be .json. File
+  paths can be sent as either strings or Path objects.
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  file_dicts = [
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_1.sas7bdat',
+      'export_file': '/path/to/new/files/example_1.json',
+    },
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_2.sas7bdat',
+      'export_file': '/path/to/new/files/example_2.json',
+    },
+  ]
+  sas7bdat_converter.batch_to_json(file_dicts)
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example_1.sas7bdat`.
+
+* **batch_to_xml(file_dicts)** - Convert multiple sas7bdat files into XML files at once.
+  * file_dicts = A list containing a dictionary for each file to convert. The dictionary is required
+  to contain 'sas7bdat_file' containing the path and name for the sas7bdat file, and 'export_file'
+  containing the path and name for the xml files. The XML file extension should be .xml. File paths
+  can be sent as either strings or Path objects.
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  file_dicts = [
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_1.sas7bdat',
+      'export_file': '/path/to/new/files/example_1.xml',
+    },
+    {
+      'sas7bdat_file': '/path/to/sas7bdat/files/example_2.sas7bdat',
+      'export_file': '/path/to/new/files/example_2.xml',
+    },
+  ]
+  sas7bdat_converter.batch_to_xml(file_dicts)
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example_1.sas7bdat`.
+
+* **dir_to_csv(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into csv
+files at once. File paths can be sent as either strings or Path objects.
+  * dir_path = The dictionary that contains the sas7bdat file to convert.
+  * export_path = Optional path for the converted files. If no path is supplied the new files will
+  be put into the dir_path directory with the sas7bdat files. File paths can be sent as either
+  strings or Path objects. Default = None
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  # Option 1: put the converted files in the same directory as the sas7bdat files
+  sas7bdat_converter.dir_to_csv('/path/to/sas7bdat/files')
+
+  # Option 2: put the converted fiels in a diffferent directory
+  sas7bdat_converter.dir_to_csv('/path/to/sas7bdat/files', 'path/for/new/files')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files`.
+
+* **dir_to_excel(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into
+Excel files at once. File paths can be sent as either strings or Path objects.
+  * dir_path = The dictionary that contains the sas7bdat file to convert.
+  * export_path = Optional path for the converted files. If no path is supplied the new files will
+  be put into the dir_path directory with the sas7bdat files Default = None
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  # Option 1: put the converted files in the same directory as the sas7bdat files
+  sas7bdat_converter.dir_to_excel('/path/to/sas7bdat/files')
+
+  # Option 2: put the converted fiels in a diffferent directory
+  sas7bdat_converter.dir_to_excel('/path/to/sas7bdat/files', 'path/for/new/files')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files`.
+
+* **dir_to_json(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into json
+  files at once. File paths can be sent as either strings or Path objects.
+  * dir_path = The dictionary that contains the sas7bdat file to convert.
+  * export_path = Optional path for the converted files. If no path is supplied the new files will
+  be put into the dir_path directory with the sas7bdat files. Default = None
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  # Option 1: put the converted files in the same directory as the sas7bdat files
+  sas7bdat_converter.dir_to_json('/path/to/sas7bdat/files')
+
+  # Option 2: put the converted fiels in a diffferent directory
+  sas7bdat_converter.dir_to_json('/path/to/sas7bdat/files', 'path/for/new/files')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files`.
+
+* **dir_to_xml(dir_path, export_path=None)** - Convert all sas7bdat files in a directory into XML
+  files at once. File paths can be sent as either strings or Path objects.
+  * dir_path = The dictionary that contains the sas7bdat file to convert.
+  * export_path = Optional path for the converted files. If no path is supplied the new files will
+  be put into the dir_path directory with the sas7bdat files. Default = None
+  * continue_on_error = If set to true processing of files in a batch will continue if there is a
+  file conversion error instead of raising an exception. Default = False
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  # Option 1: put the converted files in the same directory as the sas7bdat files
+  sas7bdat_converter.dir_to_xml('/path/to/sas7bdat/files')
+
+  # Option 2: put the converted fiels in a diffferent directory
+  sas7bdat_converter.dir_to_xml('/path/to/sas7bdat/files', 'path/for/new/files')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files`.
+
+* **to_csv(sas7bdat_file, export_file)** - convert a sas7bdat file into a csv file. File path can be
+  sent as either a string or Path objects.
+  * sas7bdat_file = the path and name for sas7bdat file to convert.
+  * export_file = the path and name for the csv file. The csv file extension should be .csv.
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  sas7bdat_converter.to_csv('/path/to/sas7bdat/file/example.sas7bdat', 'path/to/new/file/example.csv')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example.sas7bdat`.
+
+* **to_dataframe(sas7bdat_file)** - Convert a sas7bdat file into a Pandas DataFrame. File path can
+  be sent as either a string or Path objects.
+  * sas7bdat_file = The path and name for sas7bdat file to convert.
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  sas7bdat_converter.to_dataframe('/path/to/sas7bdat/file/example.sas7bdat')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example_1.sas7bdat`.
+
+* **to_excel(sas7bdat_file, export_file)** - convert a sas7bdat file into a Excel file. File path
+  can be sent as either a string or Path objects.
+  * sas7bdat_file = the path and name for sas7bdat file to convert.
+  * export_file = the path and name for the Excel file. The Excel file extension should be .xlsx.
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  sas7bdat_converter.to_excel('/path/to/sas7bdat/file/example.sas7bdat',
+  'path/to/new/file/example.xlsx')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example.sas7bdat`.
+
+* **to_parquet(sas7bdat_file, export_file)** - convert a sas7bdat file into a Parquet file. File path
+  can be sent as either a string or Path objects.
+  * sas7bdat_file = the path and name for sas7bdat file to convert.
+  * export_file = the path and name for the Parquet file. The Parquet file extension should be .parquet.
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  sas7bdat_converter.to_parquet('/path/to/sas7bdat/file/example.sas7bdat',
+  'path/to/new/file/example.parquet')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example.sas7bdat`.
+
+* **to_json(sas7bdat_file, export_file)** - convert a sas7bdat file into a json file. File path can
+  be sent as either a string or Path objects.
+  * sas7bdat_file = the path and name for sas7bdat file to convert.
+  * export_file = the path and name for the json file. the json file extension should be .json.
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  sas7bdat_converter.to_json('/path/to/sas7bdat/file/example.sas7bdat', 'path/to/new/file/example.json')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example.sas7bdat`.
+
+* **to_xml(sas7bdat_file, export_file, root_node='root', first_node='item')** - convert a sas7bdat
+  file into a XML file. File path can be sent as either a string or Path objects.
+  * sas7bdat_file = the path and name for sas7bdat file to convert.
+  * export_file = the path and name for the XML file. The XML file extension should be .xlm.
+  * root_node = The name to uses for the top level node. If no name is supplied "root" will be used.
+  * first_node = The name to use for the first node under root. If no name is supplied "item" will be used.
+
+  **Example**
+
+  ```py
+  import sas7bdat_converter
+
+  sas7bdat_converter.to_xml('/path/to/sas7bdat/file/example.sas7bdat', 'path/to/new/file/example.xml')
+  ```
+
+  **Note:** Example uses Mac/Linux type file paths. For Windows use paths like
+  `c:\path\to\sas7bdat\files\example.sas7bdat`.
+
+## Contributing
+
+If you are interesting in contributing to this project please see our [contributing guide](CONTRIBUTING.md)
 
-setup(**setup_kwargs)
```

