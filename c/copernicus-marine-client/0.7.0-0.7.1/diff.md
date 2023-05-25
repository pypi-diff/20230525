# Comparing `tmp/copernicus_marine_client-0.7.0.tar.gz` & `tmp/copernicus_marine_client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.7.0.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.7.1.tar", max compression
```

## Comparing `copernicus_marine_client-0.7.0.tar` & `copernicus_marine_client-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     3142 2023-05-12 06:57:25.897183 copernicus_marine_client-0.7.0/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.7.0/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22578 2023-05-12 06:57:25.899181 copernicus_marine_client-0.7.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6275 2023-05-12 06:57:25.901181 copernicus_marine_client-0.7.0/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3282 2023-05-04 11:59:08.729763 copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     6727 2023-05-12 06:57:25.903183 copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    15676 2023-05-12 06:57:25.906185 copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     7691 2023-05-10 15:49:41.108051 copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     3856 2023-05-12 06:57:25.908292 copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0    10327 2023-05-12 06:57:25.911185 copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     7123 2023-05-10 15:49:41.112053 copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     6419 2023-05-12 06:57:25.913182 copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0      870 2023-05-12 07:14:21.397040 copernicus_marine_client-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    14302 2023-05-12 06:57:25.895201 copernicus_marine_client-0.7.0/README.md
--rw-r--r--   0        0        0    15555 1970-01-01 00:00:00.000000 copernicus_marine_client-0.7.0/setup.py
--rw-r--r--   0        0        0    14824 1970-01-01 00:00:00.000000 copernicus_marine_client-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3142 2023-05-12 06:57:25.897183 copernicus_marine_client-0.7.1/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22578 2023-05-12 06:57:25.899181 copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6275 2023-05-12 06:57:25.901181 copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3282 2023-05-04 11:59:08.729763 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     6727 2023-05-12 06:57:25.903183 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    15676 2023-05-12 06:57:25.906185 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     7691 2023-05-10 15:49:41.108051 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     3856 2023-05-12 06:57:25.908292 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0    10327 2023-05-12 06:57:25.911185 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     7365 2023-05-25 07:55:34.881556 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     6419 2023-05-12 06:57:25.913182 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_zarr.py
+-rwxr-xr-x   0        0        0 16950784 2022-07-05 02:58:00.000000 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/s5cmd.exe
+-rw-r--r--   0        0        0      887 2023-05-25 13:42:10.141400 copernicus_marine_client-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    14302 2023-05-12 06:57:25.895201 copernicus_marine_client-0.7.1/README.md
+-rw-r--r--   0        0        0    15574 1970-01-01 00:00:00.000000 copernicus_marine_client-0.7.1/setup.py
+-rw-r--r--   0        0        0    14857 1970-01-01 00:00:00.000000 copernicus_marine_client-0.7.1/PKG-INFO
```

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_motu.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import subprocess
 from multiprocessing.pool import ThreadPool
 from subprocess import CompletedProcess
 from typing import Tuple
 
 import click
 from numpy import append, arange
@@ -85,16 +86,18 @@
 def get_filenames_recursively(
     endpoint_url: str,
     path: str,
     files_already_found: list[tuple[str, str]] = [],
 ) -> list[tuple[str, str]]:
     if not path.endswith("/"):
         path += "/"
+    path_to_s5cmd_exe = os.path.join(os.path.dirname(__file__), r".\s5cmd.exe")
     bash_command: str = (
-        f"s5cmd --endpoint-url {endpoint_url} --no-sign-request ls {path}"
+        f"{path_to_s5cmd_exe} --endpoint-url {endpoint_url}"
+        f" --no-sign-request ls {path}"
     )
     raw_output: CompletedProcess[bytes] = subprocess.run(
         bash_command, shell=True, capture_output=True
     )
     cleaned_output: str = raw_output.stdout.decode("utf-8").strip()
     lines: list[str] = [
         substr.strip() for substr in cleaned_output.split("\n")
@@ -127,16 +130,19 @@
 ) -> str:
     def _s3native_file_download(
         endpoint_url: str, file_in: str, file_out: str
     ) -> str:
         """
         Download ONE file and return a string of the result
         """
+        path_to_s5cmd_exe = os.path.join(
+            os.path.dirname(__file__), r".\s5cmd.exe"
+        )
         bash_command = (
-            f"s5cmd --endpoint-url {endpoint_url} --no-sign-request "
+            f"{path_to_s5cmd_exe} --endpoint-url {endpoint_url} --no-sign-request "
             f"cp --no-clobber {file_in} {file_out}"
         )
         with tqdm(desc=file_in.split("/")[-1]) as t:
             """
             Comment: for now s5cmd does not seem to have a way to display progress
             (see https://github.com/peak/s5cmd/issues/51)
             """
```

### Comparing `copernicus_marine_client-0.7.0/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/pyproject.toml` & `copernicus_marine_client-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
@@ -18,16 +18,15 @@
 cachier = ">=2.0.2"
 pystac = ">=1.7.2"
 xarray = ">=2023.3.0"
 tqdm = ">=4.65.0"
 zarr = ">=2.13.3"
 pydap = ">=3.2.2"
 dask = ">=2022.1.1"
-
-
+netCDF4 = ">=1.6.3"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.20.0"
 types-requests = "2.27.11"
 
 [tool.poetry.scripts]
 copernicus-marine = 'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface'
```

### Comparing `copernicus_marine_client-0.7.0/README.md` & `copernicus_marine_client-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.7.0/setup.py` & `copernicus_marine_client-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 install_requires = \
 ['aiohttp>=3.8.3',
  'cachier>=2.0.2',
  'click>=8.0.4',
  'dask>=2022.1.1',
  'motuclient==1.8.4',
+ 'netCDF4>=1.6.3',
  'numpy>=1.0',
  'owslib>=0.27.2',
  'pydap>=3.2.2',
  'pystac>=1.7.2',
  'requests>=2.27.1',
  'setuptools>=62.0.0',
  'tqdm>=4.65.0',
@@ -28,15 +29,15 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': '',
     'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Login:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of \'dataset-\n  id\' or \'dataset-url\' is required     (can be found via the \'copernicus-\n  marine describe\' command).     The arguments value passed individually\n  through the CLI take precedence     over the values from the "motu-api-\n  request" option, which takes precedence     over the ones from the "request-\n  file" option\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X\n    0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --login TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset. Requires a\n                                  float whithin this range:  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset. Requires a\n                                  float whithin this range:  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset. Requires a\n                                  float whithin this range:  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset. Requires a\n                                  float whithin this range:  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset. Requires a\n                                  float whithin this range:  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset. Requires a\n                                  float whithin this range:  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output directory)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'.\n  --motu-api-request TEXT         Option to pass a complete MOTU api request\n                                  as a string. Caution, user has to replace\n                                  double quotes " with single quotes \' in the\n                                  request\n  --help                          Show this message and exit.\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Login:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --login TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example:\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = \'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\'\nassert(dataset_id in cmc.get_all_dataset_ids())\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [variable for variable in dataset.variables if variable.short_name in [\'zooc\']][0]\ncoordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n  dataset_id=\'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\',\n  start_datetime="2023-04-20",\n  end_datetime=\'2023-04-21\',\n  minimal_latitude= 30.0,\n  maximal_latitude=30.1,\n  minimal_longitude=0.1,\n  maximal_longitude=0.2,\n  minimal_depth=100,\n  maximal_depth=1000,\n  variables = [\'zooc\'],\n  force_protocol = "zarr-map",\n  output_directory = \'data_folder\',\n  output_filename = \'datastore.zarr\',\n  assume_yes = True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(login=\'FAKE_LOGIN\', password=\'FAKE_PASSWORD\', subset_request=subset_request)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine=\'zarr\', out_type=\'xarray\')\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `copernicus_marine_client-0.7.0/PKG-INFO` & `copernicus_marine_client-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: cachier (>=2.0.2)
 Requires-Dist: click (>=8.0.4)
 Requires-Dist: dask (>=2022.1.1)
 Requires-Dist: motuclient (==1.8.4)
+Requires-Dist: netCDF4 (>=1.6.3)
 Requires-Dist: numpy (>=1.0)
 Requires-Dist: owslib (>=0.27.2)
 Requires-Dist: pydap (>=3.2.2)
 Requires-Dist: pystac (>=1.7.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: setuptools (>=62.0.0)
 Requires-Dist: tqdm (>=4.65.0)
```

