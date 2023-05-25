# Comparing `tmp/spai-2023.5.25.post2.tar.gz` & `tmp/spai-2023.5.25.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.25.post2.tar", max compression
+gzip compressed data, was "spai-2023.5.25.post3.tar", max compression
```

## Comparing `spai-2023.5.25.post2.tar` & `spai-2023.5.25.post3.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25.post2/README.md
--rw-r--r--   0        0        0      266 2023-05-25 10:34:34.765837 spai-2023.5.25.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25.post2/spai/__init__.py
--rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25.post2/spai/cli/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25.post2/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25.post2/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25.post2/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25.post2/spai/cli/local.py
--rw-r--r--   0        0        0      647 2023-05-25 09:53:16.130678 spai-2023.5.25.post2/spai/cli/project-template/REDME.md
--rw-r--r--   0        0        0        0 2023-05-25 09:52:27.506558 spai-2023.5.25.post2/spai/cli/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:34.438575 spai-2023.5.25.post2/spai/cli/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:43.562598 spai-2023.5.25.post2/spai/cli/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0        0 2023-05-25 09:46:24.337697 spai-2023.5.25.post2/spai/cli/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:54.906626 spai-2023.5.25.post2/spai/cli/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      232 2023-05-25 09:54:34.271270 spai-2023.5.25.post2/spai/cli/project-template/spai.config.yml
--rw-r--r--   0        0        0        0 2023-05-25 09:53:08.122658 spai-2023.5.25.post2/spai/cli/project-template/uis/map/main.py
--rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25.post2/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25.post2/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25.post2/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.25.post2/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.25.post2/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       41 2023-05-25 08:29:38.312976 spai-2023.5.25.post2/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.25.post2/spai/image/utils.py
--rw-r--r--   0        0        0     3892 2023-05-19 06:36:13.726144 spai-2023.5.25.post2/spai/main.bck
--rw-r--r--   0        0        0     1473 2023-05-25 10:32:18.681715 spai-2023.5.25.post2/spai/main.py
--rw-r--r--   0        0        0     1285 2023-05-25 09:18:40.109969 spai-2023.5.25.post2/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     2824 2023-05-25 09:09:16.519673 spai-2023.5.25.post2/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2042 2023-05-25 09:15:08.657120 spai-2023.5.25.post2/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.25.post2/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.25.post2/spai/storage/minio.py
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 spai-2023.5.25.post2/setup.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.25.post2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25.post3/README.md
+-rw-r--r--   0        0        0      344 2023-05-25 10:36:55.222035 spai-2023.5.25.post3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25.post3/spai/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25.post3/spai/cli/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25.post3/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25.post3/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25.post3/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25.post3/spai/cli/local.py
+-rw-r--r--   0        0        0      647 2023-05-25 09:53:16.130678 spai-2023.5.25.post3/spai/cli/project-template/REDME.md
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:27.506558 spai-2023.5.25.post3/spai/cli/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:34.438575 spai-2023.5.25.post3/spai/cli/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:43.562598 spai-2023.5.25.post3/spai/cli/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0        0 2023-05-25 09:46:24.337697 spai-2023.5.25.post3/spai/cli/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:54.906626 spai-2023.5.25.post3/spai/cli/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      232 2023-05-25 09:54:34.271270 spai-2023.5.25.post3/spai/cli/project-template/spai.config.yml
+-rw-r--r--   0        0        0        0 2023-05-25 09:53:08.122658 spai-2023.5.25.post3/spai/cli/project-template/uis/map/main.py
+-rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25.post3/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25.post3/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25.post3/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.25.post3/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.25.post3/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-25 08:29:38.312976 spai-2023.5.25.post3/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.25.post3/spai/image/utils.py
+-rw-r--r--   0        0        0     1473 2023-05-25 10:32:18.681715 spai-2023.5.25.post3/spai/main.py
+-rw-r--r--   0        0        0     1285 2023-05-25 09:18:40.109969 spai-2023.5.25.post3/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     2824 2023-05-25 09:09:16.519673 spai-2023.5.25.post3/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2042 2023-05-25 09:15:08.657120 spai-2023.5.25.post3/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.25.post3/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.25.post3/spai/storage/minio.py
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 spai-2023.5.25.post3/setup.py
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.25.post3/PKG-INFO
```

### Comparing `spai-2023.5.25.post2/spai/cli/cloud.py` & `spai-2023.5.25.post3/spai/cli/cloud.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/cli/local.py` & `spai-2023.5.25.post3/spai/cli/local.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/cli/project-template/REDME.md` & `spai-2023.5.25.post3/spai/cli/project-template/REDME.md`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/cli/validate.py` & `spai-2023.5.25.post3/spai/cli/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/data/satellite/download.py` & `spai-2023.5.25.post3/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/data/satellite/explore.py` & `spai-2023.5.25.post3/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/image/utils.py` & `spai-2023.5.25.post3/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/main.py` & `spai-2023.5.25.post3/spai/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/storage/BaseStorage.py` & `spai-2023.5.25.post3/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/storage/CloudStorage.py` & `spai-2023.5.25.post3/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/storage/Storage.py` & `spai-2023.5.25.post3/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/spai/storage/minio.py` & `spai-2023.5.25.post3/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post2/setup.py` & `spai-2023.5.25.post3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,28 @@
  'spai.image',
  'spai.storage']
 
 package_data = \
 {'': ['*'],
  'spai.cli': ['project-template/*', 'project-template/notebooks/analytics/*']}
 
+entry_points = \
+{'console_scripts': ['spai = spai.main:app']}
+
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.25.post2',
+    'version': '2023.5.25.post3',
     'description': '',
     'long_description': '',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

