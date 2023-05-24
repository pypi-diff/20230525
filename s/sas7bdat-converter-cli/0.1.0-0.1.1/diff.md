# Comparing `tmp/sas7bdat_converter_cli-0.1.0.tar.gz` & `tmp/sas7bdat_converter_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sas7bdat_converter_cli-0.1.0.tar", max compression
+gzip compressed data, was "sas7bdat_converter_cli-0.1.1.tar", max compression
```

## Comparing `sas7bdat_converter_cli-0.1.0.tar` & `sas7bdat_converter_cli-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     2675 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/README.md
--rw-r--r--   0        0        0     1491 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/sas7bdat_converter_cli/__init__.py
--rw-r--r--   0        0        0      102 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/sas7bdat_converter_cli/__main__.py
--rw-r--r--   0        0        0     6899 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/sas7bdat_converter_cli/main.py
--rw-r--r--   0        0        0        0 2023-05-24 22:49:16.003423 sas7bdat_converter_cli-0.1.0/sas7bdat_converter_cli/py.typed
--rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 sas7bdat_converter_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2675 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/README.md
+-rw-r--r--   0        0        0     2164 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/sas7bdat_converter_cli/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/sas7bdat_converter_cli/__main__.py
+-rw-r--r--   0        0        0     6899 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/sas7bdat_converter_cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:22:22.328788 sas7bdat_converter_cli-0.1.1/sas7bdat_converter_cli/py.typed
+-rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 sas7bdat_converter_cli-0.1.1/PKG-INFO
```

### Comparing `sas7bdat_converter_cli-0.1.0/LICENSE` & `sas7bdat_converter_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter_cli-0.1.0/README.md` & `sas7bdat_converter_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter_cli-0.1.0/pyproject.toml` & `sas7bdat_converter_cli-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 [tool.poetry]
 name = "sas7bdat-converter-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLI to convert sas7bdat and xport files into other formats"
 authors = ["Paul Sanders <paul@pbsdatasolutions.com>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/pbs-data-solutions/sas7bdat-converter-cli"
+homepage = "https://github.com/pbs-data-solutions/sas7bdat-converter-cli"
+documentation = "https://github.com/pbs-data-solutions/sas7bdat-converter-cli"
+keywords = ["sas", "sas7bdat", "converter", "xpt", "XPort"]
+classifiers=[
+  "Intended Audience :: Science/Research",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Typing :: Typed",
+]
+include = ["sas7bdat_converter_cli/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = "0.9.0"
 sas7bdat-converter = {version = "1.3.0", extras = ["all"]}
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `sas7bdat_converter_cli-0.1.0/sas7bdat_converter_cli/main.py` & `sas7bdat_converter_cli-0.1.1/sas7bdat_converter_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sas7bdat_converter import to_csv as converter_to_csv
 from sas7bdat_converter import to_excel as converter_to_excel
 from sas7bdat_converter import to_json as converter_to_json
 from sas7bdat_converter import to_parquet as converter_to_parquet
 from sas7bdat_converter import to_xml as converter_to_xml
 from typer import Argument, Exit, Option, Typer, echo
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 app = Typer()
 
 
 @app.command()
 def to_csv(
     file_path: Path = Argument(..., help="Path to the file to convert", show_default=False),
```

### Comparing `sas7bdat_converter_cli-0.1.0/PKG-INFO` & `sas7bdat_converter_cli-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: sas7bdat-converter-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI to convert sas7bdat and xport files into other formats
+Home-page: https://github.com/pbs-data-solutions/sas7bdat-converter-cli
 License: MIT
+Keywords: sas,sas7bdat,converter,xpt,XPort
 Author: Paul Sanders
 Author-email: paul@pbsdatasolutions.com
 Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Dist: sas7bdat-converter[all] (==1.3.0)
 Requires-Dist: typer (==0.9.0)
+Project-URL: Documentation, https://github.com/pbs-data-solutions/sas7bdat-converter-cli
+Project-URL: Repository, https://github.com/pbs-data-solutions/sas7bdat-converter-cli
 Description-Content-Type: text/markdown
 
 # sas7bdat Converter CLI
 
 [![Tests Status](https://github.com/pbs-data-solutions/sas7bdat-converter-cli/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/pbs-data-solutions/sas7bdat-converter-cli/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pbs-data-solutions/sas7bdat-converter-cli/main.svg)](https://results.pre-commit.ci/latest/github/pbs-data-solutions/sas7bdat-converter-cli/main)
 [![Coverage](https://codecov.io/github/pbs-data-solutions/sas7bdat-converter-cli/coverage.svg?branch=main)](https://codecov.io/gh/pbs-data-solutions/sas7bdat-converter-cli)
```

