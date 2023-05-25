# Comparing `tmp/cognite_cdffs-0.2.2.tar.gz` & `tmp/cognite_cdffs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_cdffs-0.2.2.tar", max compression
+gzip compressed data, was "cognite_cdffs-0.2.3.tar", max compression
```

## Comparing `cognite_cdffs-0.2.2.tar` & `cognite_cdffs-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2423 2023-05-22 08:02:27.349744 cognite_cdffs-0.2.2/README.md
--rw-r--r--   0        0        0      205 2023-05-22 08:02:27.349744 cognite_cdffs-0.2.2/cognite/cdffs/__init__.py
--rw-r--r--   0        0        0     3907 2023-05-22 08:02:27.349744 cognite_cdffs-0.2.2/cognite/cdffs/credentials.py
--rw-r--r--   0        0        0     3134 2023-05-22 08:02:27.349744 cognite_cdffs-0.2.2/cognite/cdffs/file_handler.py
--rw-r--r--   0        0        0    26358 2023-05-22 08:02:27.349744 cognite_cdffs-0.2.2/cognite/cdffs/spec.py
--rw-r--r--   0        0        0     1655 2023-05-22 08:02:27.349744 cognite_cdffs-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.2/setup.py
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2423 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/README.md
+-rw-r--r--   0        0        0      205 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/__init__.py
+-rw-r--r--   0        0        0     3907 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/credentials.py
+-rw-r--r--   0        0        0     3134 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/file_handler.py
+-rw-r--r--   0        0        0    26358 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/spec.py
+-rw-r--r--   0        0        0     1638 2023-05-25 10:04:47.541252 cognite_cdffs-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.3/setup.py
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.3/PKG-INFO
```

### Comparing `cognite_cdffs-0.2.2/README.md` & `cognite_cdffs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.2/cognite/cdffs/credentials.py` & `cognite_cdffs-0.2.3/cognite/cdffs/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.2/cognite/cdffs/file_handler.py` & `cognite_cdffs-0.2.3/cognite/cdffs/file_handler.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.2/cognite/cdffs/spec.py` & `cognite_cdffs-0.2.3/cognite/cdffs/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.2/pyproject.toml` & `cognite_cdffs-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 [tool.poetry]
 name = "cognite-cdffs"
-version = "0.2.2"
+version = "0.2.3"
 description = "File System Interface for CDF Files"
 license = "Apache-2.0"
 authors = ["Infant Alex <infant.alex@cognite.com>"]
 readme = "README.md"
 packages = [
     { include="cognite", from="." },
 ]
 [tool.poetry.group.test.dependencies]
 pandas = "^1.5.1"
-geopandas = "^0.12.1"
-pyarrow = "^11.0.0"
+geopandas = "^0.13.0"
+pyarrow = "^12.0.0"
 zarr = "^2.13.3"
 dask = "^2023.5.0"
 xarray = "^2023.5.0"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.11.5"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 black = "^23.3.0"
 responses = "^0.23.1"
 flake8 = "6.0.0"
 pre-commit = "^3.2.2"
 flake8-pyproject = "^1.2.3"
-sphinx-rtd-theme = "^1.1.1"
 twine = "^4.0.2"
-sphinx = "6.2.1"
 toml = "^0.10.2"
+sphinx-rtd-theme = "^1.2.1"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
 include = '\.py$'
 
 [tool.flake8]
@@ -66,17 +65,17 @@
     coverage xml
 """
 
 [tool.poetry.dependencies]
 python = "^3.9.10"
 cognite-sdk = "^6.1.10"
 fsspec = "^2023.5.0"
-requests = "^2.30.0"
+requests = "^2.31.0"
 twine = "^4.0.2"
-pydantic = "^1.10.7"
+pydantic = "^1.10.8"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `cognite_cdffs-0.2.2/setup.py` & `cognite_cdffs-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cognite-sdk>=6.1.10,<7.0.0',
  'fsspec>=2023.5.0,<2024.0.0',
- 'pydantic>=1.10.7,<2.0.0',
+ 'pydantic>=1.10.8,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
- 'requests>=2.30.0,<3.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'twine>=4.0.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'cognite-cdffs',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'File System Interface for CDF Files',
     'long_description': '<a href="https://cognite.com/">\n  <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">\n</a>\n\n[![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/badge.svg)](https://codecov.io/gh/cognitedata/cdffs)\n![PyPI](https://img.shields.io/pypi/v/cognite-cdffs)\n\n# cdffs\n\nA file system interface (`cdffs`) to allow users to work with CDF Files using the [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) supported/compatible python packages (`pandas`, `xarray` etc).\n\n`fsspec` provides an abstract file system interface to work with local/cloud storages and based on the protocol name (example, `s3` or `abfs`) provided in the path, `fsspec` translates the incoming requests to storage specific implementations and send the responses back to the upstream package to work with the desired data.\n\nRefer [fsspec documentation](https://filesystem-spec.readthedocs.io/en/latest/#who-uses-fsspec) to get the list of all supported/compatible python packages.\n\n## Installation\n\n`cdffs` is available on PyPI. Install using,\n\n```shell\npip install cognite-cdffs\n```\n\n## Usage\n\nImportant steps to follow when working with CDF Files using the `fsspec` supported python packages.\n\n1) Import `cdffs` package\n```python\n  from cognite import cdffs  # noqa\n```\n\n2) Follow instructions from [Authentication](https://cdffs.readthedocs.io/en/latest/authentication.html) to authenticate.\n\n3) Read/write the files from/to CDF using `fsspec` supported packages. Example,\n\n    * Read `zarr` files using using `xarray`.\n\n    ```python\n    ds = xarray.open_zarr("cdffs://sample_data/test.zarr")\n    ```\n    * Write `zarr` files using `xarray`.\n\n    ```python\n    ds.to_zarr("cdffs://sample_data/test.zarr", storage_options={"file_metadata": metadata})\n    ```\n\nRefer [cdffs.readthedocs.io](https://cdffs.readthedocs.io) for more details.\n\n## Contributing\nWant to contribute? Check out [CONTRIBUTING](CONTRIBUTING.md).\n',
     'author': 'Infant Alex',
     'author_email': 'infant.alex@cognite.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '.'}
 packages = \ ['cognite', 'cognite.cdffs'] package_data = \ {'': ['*']}
 install_requires = \ ['cognite-sdk>=6.1.10,<7.0.0',
-'fsspec>=2023.5.0,<2024.0.0', 'pydantic>=1.10.7,<2.0.0', 'python-
-dotenv>=1.0.0,<2.0.0', 'requests>=2.30.0,<3.0.0', 'twine>=4.0.2,<5.0.0']
-setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.2', 'description':
+'fsspec>=2023.5.0,<2024.0.0', 'pydantic>=1.10.8,<2.0.0', 'python-
+dotenv>=1.0.0,<2.0.0', 'requests>=2.31.0,<3.0.0', 'twine>=4.0.2,<5.0.0']
+setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.3', 'description':
 'File System Interface for CDF Files', 'long_description': '\n_[Cognite]\n\n\n
 [![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://
 github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status]
 (https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/
```

### Comparing `cognite_cdffs-0.2.2/PKG-INFO` & `cognite_cdffs-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cognite-cdffs
-Version: 0.2.2
+Version: 0.2.3
 Summary: File System Interface for CDF Files
 License: Apache-2.0
 Author: Infant Alex
 Author-email: infant.alex@cognite.com
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cognite-sdk (>=6.1.10,<7.0.0)
 Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://cognite.com/">
   <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">
 </a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.2 Summary: File System
+Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.3 Summary: File System
 Interface for CDF Files License: Apache-2.0 Author: Infant Alex Author-email:
 infant.alex@cognite.com Requires-Python: >=3.9.10,<4.0.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: cognite-sdk
 (>=6.1.10,<7.0.0) Requires-Dist: fsspec (>=2023.5.0,<2024.0.0) Requires-Dist:
-pydantic (>=1.10.7,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-Dist: twine (>=4.0.2,<5.0.0)
+pydantic (>=1.10.8,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown [Cognite] [![GitHub](https://
 img.shields.io/github/license/cognitedata/cdffs)](https://github.com/
 cognitedata/cdffs/blob/main/LICENSE) [![Documentation Status](https://
 readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black) [![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/
```

