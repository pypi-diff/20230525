# Comparing `tmp/gwcloud-python-1.9.0.tar.gz` & `tmp/gwcloud-python-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcloud-python-1.9.0.tar", max compression
+gzip compressed data, was "gwcloud-python-1.9.1.tar", max compression
```

## Comparing `gwcloud-python-1.9.0.tar` & `gwcloud-python-1.9.1.tar`

### file list

```diff
@@ -1,66 +1,24 @@
--rw-r--r--   0        0        0     1076 2021-06-16 03:50:42.140497 gwcloud-python-1.9.0/LICENSE
--rw-r--r--   0        0        0     1040 2021-07-20 08:05:58.060259 gwcloud-python-1.9.0/README.rst
--rw-r--r--   0        0        0    53248 2022-01-27 11:15:06.126532 gwcloud-python-1.9.0/gwcloud_python/.coverage
--rw-r--r--   0        0        0       37 2021-06-25 01:52:38.644204 gwcloud-python-1.9.0/gwcloud_python/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-06-25 01:52:38.644204 gwcloud-python-1.9.0/gwcloud_python/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-06-25 01:52:38.644204 gwcloud-python-1.9.0/gwcloud_python/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-03-22 03:11:12.858533 gwcloud-python-1.9.0/gwcloud_python/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2507 2022-05-26 02:43:38.182262 gwcloud-python-1.9.0/gwcloud_python/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-05-26 02:43:38.182262 gwcloud-python-1.9.0/gwcloud_python/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      378 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/gwcloud_python/__init__.py
--rw-r--r--   0        0        0     3557 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/gwcloud_python/bilby_job.py
--rw-r--r--   0        0        0      259 2022-01-27 23:38:14.457797 gwcloud-python-1.9.0/gwcloud_python/event_id.py
--rw-r--r--   0        0        0    24988 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/gwcloud_python/gwcloud.py
--rw-r--r--   0        0        0      240 2022-03-25 04:01:33.050930 gwcloud-python-1.9.0/gwcloud_python/settings.py
--rw-r--r--   0        0        0    53248 2021-07-06 05:23:13.844636 gwcloud-python-1.9.0/gwcloud_python/tests/.coverage
--rw-r--r--   0        0        0       37 2021-07-06 04:04:58.722620 gwcloud-python-1.9.0/gwcloud_python/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-07-06 04:04:58.722620 gwcloud-python-1.9.0/gwcloud_python/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-07-06 04:04:58.722620 gwcloud-python-1.9.0/gwcloud_python/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       36 2022-06-01 02:02:28.421121 gwcloud-python-1.9.0/gwcloud_python/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      622 2022-06-01 02:02:28.421121 gwcloud-python-1.9.0/gwcloud_python/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-06-01 02:02:28.421121 gwcloud-python-1.9.0/gwcloud_python/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2021-06-15 05:08:29.478516 gwcloud-python-1.9.0/gwcloud_python/tests/__init__.py
--rw-r--r--   0        0        0      168 2021-06-15 11:34:34.025373 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    13238 2022-06-06 06:33:56.653783 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/test_bilby_job.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     4641 2022-03-16 05:35:10.420858 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/test_bilby_job.cpython-38.pyc
--rw-r--r--   0        0        0      175 2022-05-25 06:40:43.586953 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/test_file_reference.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     1955 2022-03-16 05:35:10.480857 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/test_file_reference.cpython-38.pyc
--rw-r--r--   0        0        0    13617 2022-06-06 06:33:56.673783 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/test_gwcloud_python.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     4243 2022-03-16 05:35:10.480857 gwcloud-python-1.9.0/gwcloud_python/tests/__pycache__/test_gwcloud_python.cpython-38.pyc
--rw-r--r--   0        0        0     7464 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/gwcloud_python/tests/test_bilby_job.py
--rw-r--r--   0        0        0     9386 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/gwcloud_python/tests/test_gwcloud_python.py
--rw-r--r--   0        0        0       37 2021-07-12 06:21:29.263812 gwcloud-python-1.9.0/gwcloud_python/utils/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-07-12 06:21:29.263812 gwcloud-python-1.9.0/gwcloud_python/utils/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-07-12 06:21:29.263812 gwcloud-python-1.9.0/gwcloud_python/utils/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2021-07-12 06:21:36.876107 gwcloud-python-1.9.0/gwcloud_python/utils/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      212 2021-07-12 06:21:36.876107 gwcloud-python-1.9.0/gwcloud_python/utils/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2021-07-12 06:21:36.876107 gwcloud-python-1.9.0/gwcloud_python/utils/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       81 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/gwcloud_python/utils/__init__.py
--rw-r--r--   0        0        0      275 2022-06-07 07:02:46.582054 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1772 2022-03-25 05:19:11.969216 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/file_download.cpython-38.pyc
--rw-r--r--   0        0        0     4422 2022-05-30 03:22:12.305344 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/file_filters.cpython-38.pyc
--rw-r--r--   0        0        0     4256 2021-07-11 11:57:23.878045 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/file_lists.cpython-38.pyc
--rw-r--r--   0        0        0      426 2022-04-01 04:50:46.824533 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/file_upload.cpython-38.pyc
--rw-r--r--   0        0        0     5133 2022-05-30 03:22:12.305344 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/identifiers.cpython-38.pyc
--rw-r--r--   0        0        0     1704 2022-06-06 00:22:04.860360 gwcloud-python-1.9.0/gwcloud_python/utils/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     1779 2022-03-25 04:01:33.050930 gwcloud-python-1.9.0/gwcloud_python/utils/file_download.py
--rw-r--r--   0        0        0     4720 2022-05-27 00:54:24.583260 gwcloud-python-1.9.0/gwcloud_python/utils/file_filters.py
--rw-r--r--   0        0        0      194 2022-03-30 03:43:22.231450 gwcloud-python-1.9.0/gwcloud_python/utils/file_upload.py
--rw-r--r--   0        0        0     4556 2022-05-27 00:54:24.583260 gwcloud-python-1.9.0/gwcloud_python/utils/identifiers.py
--rw-r--r--   0        0        0        0 2021-06-15 05:08:29.478516 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__init__.py
--rw-r--r--   0        0        0      174 2021-06-15 11:34:34.037373 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4219 2022-03-29 03:13:02.628276 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_file_download.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     8083 2022-06-01 01:47:50.585216 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_file_filters.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     4608 2022-03-16 05:35:10.484857 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_file_filters.cpython-38.pyc
--rw-r--r--   0        0        0     6090 2021-07-12 06:33:46.023729 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_file_lists.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     1436 2022-05-25 06:39:58.439494 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_file_upload.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     3973 2022-06-01 01:47:50.589216 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_identifiers.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     3278 2022-03-16 05:35:10.484857 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_identifiers.cpython-38.pyc
--rw-r--r--   0        0        0      364 2022-06-06 06:33:15.021472 gwcloud-python-1.9.0/gwcloud_python/utils/tests/__pycache__/test_utils.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0        0        0     2987 2022-03-25 04:01:33.050930 gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_file_download.py
--rw-r--r--   0        0        0     5434 2022-05-27 00:54:24.583260 gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_file_filters.py
--rw-r--r--   0        0        0      588 2022-03-30 03:43:22.231450 gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_file_upload.py
--rw-r--r--   0        0        0     3787 2022-05-27 00:54:24.583260 gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_identifiers.py
--rw-r--r--   0        0        0     1064 2022-06-08 05:45:35.309119 gwcloud-python-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     2367 2022-06-08 05:54:06.793205 gwcloud-python-1.9.0/setup.py
--rw-r--r--   0        0        0     2195 2022-06-08 05:54:06.793537 gwcloud-python-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-06-16 03:50:42.140497 gwcloud-python-1.9.1/LICENSE
+-rw-r--r--   0        0        0     1040 2021-07-20 08:05:58.060259 gwcloud-python-1.9.1/README.rst
+-rw-r--r--   0        0        0      378 2022-06-08 05:45:35.309119 gwcloud-python-1.9.1/gwcloud_python/__init__.py
+-rw-r--r--   0        0        0     3557 2022-06-08 05:45:35.309119 gwcloud-python-1.9.1/gwcloud_python/bilby_job.py
+-rw-r--r--   0        0        0      259 2022-01-27 23:38:14.457797 gwcloud-python-1.9.1/gwcloud_python/event_id.py
+-rw-r--r--   0        0        0      726 2022-06-23 04:27:31.298431 gwcloud-python-1.9.1/gwcloud_python/exceptions.py
+-rw-r--r--   0        0        0    25347 2022-06-23 03:52:31.274219 gwcloud-python-1.9.1/gwcloud_python/gwcloud.py
+-rw-r--r--   0        0        0      302 2022-06-22 05:59:30.658771 gwcloud-python-1.9.1/gwcloud_python/settings.py
+-rw-r--r--   0        0        0        0 2021-06-15 05:08:29.478516 gwcloud-python-1.9.1/gwcloud_python/tests/__init__.py
+-rw-r--r--   0        0        0     7464 2022-06-08 05:45:35.309119 gwcloud-python-1.9.1/gwcloud_python/tests/test_bilby_job.py
+-rw-r--r--   0        0        0     9428 2022-06-23 03:52:04.747204 gwcloud-python-1.9.1/gwcloud_python/tests/test_gwcloud_python.py
+-rw-r--r--   0        0        0       81 2022-06-08 05:45:35.309119 gwcloud-python-1.9.1/gwcloud_python/utils/__init__.py
+-rw-r--r--   0        0        0     1779 2022-03-25 04:01:33.050930 gwcloud-python-1.9.1/gwcloud_python/utils/file_download.py
+-rw-r--r--   0        0        0     4720 2022-05-27 00:54:24.583260 gwcloud-python-1.9.1/gwcloud_python/utils/file_filters.py
+-rw-r--r--   0        0        0      194 2022-03-30 03:43:22.231450 gwcloud-python-1.9.1/gwcloud_python/utils/file_upload.py
+-rw-r--r--   0        0        0     4556 2022-05-27 00:54:24.583260 gwcloud-python-1.9.1/gwcloud_python/utils/identifiers.py
+-rw-r--r--   0        0        0        0 2021-06-15 05:08:29.478516 gwcloud-python-1.9.1/gwcloud_python/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2987 2022-03-25 04:01:33.050930 gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_file_download.py
+-rw-r--r--   0        0        0     5434 2022-05-27 00:54:24.583260 gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_file_filters.py
+-rw-r--r--   0        0        0      588 2022-03-30 03:43:22.231450 gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_file_upload.py
+-rw-r--r--   0        0        0     3787 2022-05-27 00:54:24.583260 gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_identifiers.py
+-rw-r--r--   0        0        0     1064 2022-06-23 03:51:14.169093 gwcloud-python-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2154 2022-06-23 05:10:41.650042 gwcloud-python-1.9.1/setup.py
+-rw-r--r--   0        0        0     2195 2022-06-23 05:10:41.650305 gwcloud-python-1.9.1/PKG-INFO
```

### Comparing `gwcloud-python-1.9.0/LICENSE` & `gwcloud-python-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/README.rst` & `gwcloud-python-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/bilby_job.py` & `gwcloud-python-1.9.1/gwcloud_python/bilby_job.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/gwcloud.py` & `gwcloud-python-1.9.1/gwcloud_python/gwcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,47 @@
 from gwdc_python.files import FileReference, FileReferenceList
 from gwdc_python.helpers import TimeRange, Cluster
 from gwdc_python.utils import rename_dict_keys
 from gwdc_python.logger import create_logger
 
 from .bilby_job import BilbyJob
 from .event_id import EventID
+from .exceptions import custom_error_handler
 from .utils.file_download import _download_files, _save_file_map_fn, _get_file_map_fn
 from .utils.file_upload import check_file
-from .settings import GWCLOUD_ENDPOINT
+from .settings import GWCLOUD_ENDPOINT, GWCLOUD_AUTH_ENDPOINT
 
 logger = create_logger(__name__)
 
 
 class GWCloud:
     """
     GWCloud class provides an API for interacting with Bilby, allowing jobs to be submitted and acquired.
 
     Parameters
     ----------
     token : str
         API token for a Bilby user
+    auth_endpoint : str, optional
+        URL to which we send the authentication queries, by default GWCLOUD_AUTH_ENDPOINT
     endpoint : str, optional
         URL to which we send the queries, by default GWCLOUD_ENDPOINT
 
     Attributes
     ----------
     client : GWDC
         Handles a lot of the underlying logic surrounding the queries
     """
-    def __init__(self, token, endpoint=GWCLOUD_ENDPOINT):
-        self.client = GWDC(token=token, endpoint=endpoint)
+    def __init__(self, token, auth_endpoint=GWCLOUD_AUTH_ENDPOINT, endpoint=GWCLOUD_ENDPOINT):
+        self.client = GWDC(
+            token=token,
+            auth_endpoint=auth_endpoint,
+            endpoint=endpoint,
+            custom_error_handler=custom_error_handler
+        )
         self.request = self.client.request  # Setting shorthand for simplicity
 
     def _upload_supporting_files(self, tokens, file_paths):
         """
         Uploads supporting files for a job
 
         Parameters
```

### Comparing `gwcloud-python-1.9.0/gwcloud_python/tests/test_bilby_job.py` & `gwcloud-python-1.9.1/gwcloud_python/tests/test_bilby_job.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/tests/test_gwcloud_python.py` & `gwcloud-python-1.9.1/gwcloud_python/tests/test_gwcloud_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from gwdc_python.helpers import JobStatus
 import pytest
 from tempfile import TemporaryFile
 
 
 @pytest.fixture
 def mock_gwdc_init(mocker):
-    def mock_init(self, token, endpoint):
+    def mock_init(self, token, auth_endpoint, endpoint, custom_error_handler=None):
         pass
 
     mocker.patch('gwdc_python.gwdc.GWDC.__init__', mock_init)
 
 
 @pytest.fixture
 def setup_mock_gwdc(mocker, mock_gwdc_init):
```

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/file_download.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/file_download.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/file_filters.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/file_filters.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/identifiers.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/identifiers.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_file_download.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_file_download.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_file_filters.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_file_upload.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/gwcloud_python/utils/tests/test_identifiers.py` & `gwcloud-python-1.9.1/gwcloud_python/utils/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `gwcloud-python-1.9.0/pyproject.toml` & `gwcloud-python-1.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "gwcloud-python"
-version = "1.9.0"
+version = "1.9.1"
 description = "Wrapper of GWDC API, used for interacting with the GWCloud endpoints"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>"]
 license = "MIT"
 readme = "README.rst"
 documentation = "https://gwcloud-python.readthedocs.io/en/latest/"
 repository = "https://github.com/gravitationalwavedc/gwcloud_python"
 include = ["LICENSE",]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-gwdc-python = "^0.4.0"
+gwdc-python = "^0.4.1"
 requests = "^2.25.1"
 jwt = "^1.2.0"
 graphene-file-upload = "^1.3.0"
 importlib-metadata = "^4.5.0"
 Sphinx = {version = "^4.0.2", optional = true}
 sphinx-rtd-theme = {version = "^0.5.2", optional = true}
 tqdm = "^4.61.2"
```

### Comparing `gwcloud-python-1.9.0/setup.py` & `gwcloud-python-1.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,33 +4,30 @@
 packages = \
 ['gwcloud_python',
  'gwcloud_python.tests',
  'gwcloud_python.utils',
  'gwcloud_python.utils.tests']
 
 package_data = \
-{'': ['*'],
- 'gwcloud_python': ['.pytest_cache/*', '.pytest_cache/v/cache/*'],
- 'gwcloud_python.tests': ['.pytest_cache/*', '.pytest_cache/v/cache/*'],
- 'gwcloud_python.utils': ['.pytest_cache/*', '.pytest_cache/v/cache/*']}
+{'': ['*']}
 
 install_requires = \
 ['graphene-file-upload>=1.3.0,<2.0.0',
- 'gwdc-python>=0.4.0,<0.5.0',
+ 'gwdc-python>=0.4.1,<0.5.0',
  'importlib-metadata>=4.5.0,<5.0.0',
  'jwt>=1.2.0,<2.0.0',
  'requests>=2.25.1,<3.0.0',
  'tqdm>=4.61.2,<5.0.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.0.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
 
 setup_kwargs = {
     'name': 'gwcloud-python',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'Wrapper of GWDC API, used for interacting with the GWCloud endpoints',
     'long_description': "GWCloud Python API\n==================\n\n`GWCloud <https://gwcloud.org.au/>`_ is a service used to handle both the submission of `Bilby <https://pypi.org/project/bilby/>`_ jobs to a supercomputer queue and the obtaining of the results produced by these jobs.\nWhile there is a web interface for this service, which is recommended for beginners, this package can be used to allow Bilby job submission and manipulation from Python scripts.\n\nCheck out the `documentation <https://gwcloud-python.readthedocs.io/en/latest/>`_ for more information.\n\nInstallation\n------------\n\nThe gwcloud-python package can be installed with\n\n::\n\n    pip install gwcloud-python\n\n\nExample\n-------\n\n::\n\n    >>> from gwcloud_python import GWCloud\n    >>> gwc = GWCloud(token='<user_api_token_here>')\n    >>> job = gwc.get_preferred_job_list()[0]\n    >>> job.save_corner_plot_files()\n\n    100%|██████████████████████████████████████| 3.76M/3.76M [00:00<00:00, 5.20MB/s]\n    All 2 files saved!\n",
     'author': 'Thomas Reichardt',
     'author_email': 'treichardt@swin.edu.au',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/gravitationalwavedc/gwcloud_python',
```

### Comparing `gwcloud-python-1.9.0/PKG-INFO` & `gwcloud-python-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gwcloud-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: Wrapper of GWDC API, used for interacting with the GWCloud endpoints
 Home-page: https://github.com/gravitationalwavedc/gwcloud_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=4.0.2,<5.0.0); extra == "docs"
 Requires-Dist: graphene-file-upload (>=1.3.0,<2.0.0)
-Requires-Dist: gwdc-python (>=0.4.0,<0.5.0)
+Requires-Dist: gwdc-python (>=0.4.1,<0.5.0)
 Requires-Dist: importlib-metadata (>=4.5.0,<5.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "docs"
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
 Project-URL: Documentation, https://gwcloud-python.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/gravitationalwavedc/gwcloud_python
```

