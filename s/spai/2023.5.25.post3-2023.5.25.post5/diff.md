# Comparing `tmp/spai-2023.5.25.post3.tar.gz` & `tmp/spai-2023.5.25.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.25.post3.tar", max compression
+gzip compressed data, was "spai-2023.5.25.post5.tar", max compression
```

## Comparing `spai-2023.5.25.post3.tar` & `spai-2023.5.25.post5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25.post3/README.md
--rw-r--r--   0        0        0      344 2023-05-25 10:36:55.222035 spai-2023.5.25.post3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25.post3/spai/__init__.py
--rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25.post3/spai/cli/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25.post3/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25.post3/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25.post3/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25.post3/spai/cli/local.py
--rw-r--r--   0        0        0      647 2023-05-25 09:53:16.130678 spai-2023.5.25.post3/spai/cli/project-template/REDME.md
--rw-r--r--   0        0        0        0 2023-05-25 09:52:27.506558 spai-2023.5.25.post3/spai/cli/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:34.438575 spai-2023.5.25.post3/spai/cli/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:43.562598 spai-2023.5.25.post3/spai/cli/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0        0 2023-05-25 09:46:24.337697 spai-2023.5.25.post3/spai/cli/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:54.906626 spai-2023.5.25.post3/spai/cli/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      232 2023-05-25 09:54:34.271270 spai-2023.5.25.post3/spai/cli/project-template/spai.config.yml
--rw-r--r--   0        0        0        0 2023-05-25 09:53:08.122658 spai-2023.5.25.post3/spai/cli/project-template/uis/map/main.py
--rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25.post3/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25.post3/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25.post3/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.25.post3/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.25.post3/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.25.post3/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       41 2023-05-25 08:29:38.312976 spai-2023.5.25.post3/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.25.post3/spai/image/utils.py
--rw-r--r--   0        0        0     1473 2023-05-25 10:32:18.681715 spai-2023.5.25.post3/spai/main.py
--rw-r--r--   0        0        0     1285 2023-05-25 09:18:40.109969 spai-2023.5.25.post3/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     2824 2023-05-25 09:09:16.519673 spai-2023.5.25.post3/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2042 2023-05-25 09:15:08.657120 spai-2023.5.25.post3/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.25.post3/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.25.post3/spai/storage/minio.py
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 spai-2023.5.25.post3/setup.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.25.post3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25.post5/README.md
+-rw-r--r--   0        0        0      344 2023-05-25 11:55:02.356026 spai-2023.5.25.post5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25.post5/spai/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25.post5/spai/cli/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25.post5/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25.post5/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25.post5/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25.post5/spai/cli/local.py
+-rw-r--r--   0        0        0      647 2023-05-25 09:53:16.130678 spai-2023.5.25.post5/spai/cli/project-template/REDME.md
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:27.506558 spai-2023.5.25.post5/spai/cli/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:34.438575 spai-2023.5.25.post5/spai/cli/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:43.562598 spai-2023.5.25.post5/spai/cli/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0        0 2023-05-25 09:46:24.337697 spai-2023.5.25.post5/spai/cli/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:54.906626 spai-2023.5.25.post5/spai/cli/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      232 2023-05-25 09:54:34.271270 spai-2023.5.25.post5/spai/cli/project-template/spai.config.yml
+-rw-r--r--   0        0        0        0 2023-05-25 09:53:08.122658 spai-2023.5.25.post5/spai/cli/project-template/uis/map/main.py
+-rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25.post5/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25.post5/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25.post5/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.25.post5/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.25.post5/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.25.post5/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-25 08:29:38.312976 spai-2023.5.25.post5/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.25.post5/spai/image/utils.py
+-rw-r--r--   0        0        0     1631 2023-05-25 10:38:00.746147 spai-2023.5.25.post5/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-25 11:35:53.721248 spai-2023.5.25.post5/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-25 11:40:20.925888 spai-2023.5.25.post5/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2521 2023-05-25 11:38:44.845657 spai-2023.5.25.post5/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.25.post5/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.25.post5/spai/storage/minio.py
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 spai-2023.5.25.post5/setup.py
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.25.post5/PKG-INFO
```

### Comparing `spai-2023.5.25.post3/spai/cli/cloud.py` & `spai-2023.5.25.post5/spai/cli/cloud.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/cli/local.py` & `spai-2023.5.25.post5/spai/cli/local.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/cli/project-template/REDME.md` & `spai-2023.5.25.post5/spai/cli/project-template/REDME.md`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/cli/validate.py` & `spai-2023.5.25.post5/spai/cli/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/data/satellite/download.py` & `spai-2023.5.25.post5/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/data/satellite/explore.py` & `spai-2023.5.25.post5/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.5.25.post5/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/image/utils.py` & `spai-2023.5.25.post5/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/spai/main.py` & `spai-2023.5.25.post5/spai/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import typer
 from pathlib import Path
 import os
 import shutil
+import sys
+
+# Add the cli directory to the Python path
+spai_cli_dir = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(os.path.join(spai_cli_dir))
 
 from cli.commands import hello
 from cli import (
     load_and_validate_config,
     deploy_and_run_cloud,
     run_local,
     stop_local,
```

### Comparing `spai-2023.5.25.post3/spai/storage/BaseStorage.py` & `spai-2023.5.25.post5/spai/storage/BaseStorage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,57 @@
-import PIL
+from PIL import Image
 import numpy as np
+import pandas as pd
 
 
 class BaseStorage:
     def __init__(self):
         pass
 
     def create(self, data, name, **kwargs):
         if isinstance(data, str):  # puedo asumir que siempre será un path?
             return self.create_from_path(data, name)
-        elif isinstance(data, PIL.Image.Image):
+        elif isinstance(data, Image.Image):
             return self.create_from_image(data, name)
         elif isinstance(data, np.ndarray):
             ext = name.split(".")[-1]
             if ext in ["tif", "tiff"]:
                 if "ds" in kwargs:
                     return self.create_from_rasterio(data, name, kwargs["ds"])
                 raise TypeError("Missing ds argument")
-            return self.create_from_array(data, name)
+            elif ext == "npy":
+                return self.create_from_array(data, name)
+            else:
+                raise TypeError("Not a valid array type")
+        elif isinstance(data, pd.core.frame.DataFrame):
+            ext = name.split(".")[-1]
+            if ext == "csv":
+                return self.create_from_csv(data, name)
+            elif ext == "json":
+                return self.create_from_json(data, name)
+            else:
+                raise TypeError("Not a valid dataframe type")
         else:
             raise TypeError("Not a valid type")
 
     def create_from_data(self, data, path):
         with open(path, "wb") as f:
             f.write(data.read())
         return path
 
     def read(self, name):
         ext = name.split(".")[-1]
         if ext == "npy":
             return self.read_from_array(name)
         elif ext in ["tif", "tiff"]:
             return self.read_from_rasterio(name)
+        elif ext == "csv":
+            return self.read_from_csv(name)
+        elif ext == "json":
+            return self.read_from_json(name)
         raise TypeError("Not a valid type")
 
     def update(self):
         pass
 
     def delete(self):
         pass
```

### Comparing `spai-2023.5.25.post3/spai/storage/CloudStorage.py` & `spai-2023.5.25.post5/spai/storage/CloudStorage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import fnmatch
 import rasterio as rio
 from io import BytesIO
 import numpy as np
 from rasterio.io import MemoryFile
+import pandas as pd
 
 from .minio import get_client
 from .BaseStorage import BaseStorage
 
 
 class CloudStorage(BaseStorage):
     # store in s3
@@ -61,21 +62,46 @@
         np.save(array_bytes, data)
         array_bytes.seek(0)
         self.client.put_object(
             self.bucket, name, array_bytes, len(array_bytes.getvalue())
         )
         return self.get_url(name)
 
+    def create_from_csv(self, data, name):
+        csv_bytes = BytesIO()
+        data.to_csv(csv_bytes, index=False)
+        csv_bytes.seek(0)
+        self.client.put_object(self.bucket, name, csv_bytes, len(csv_bytes.getvalue()))
+        return self.get_url(name)
+
+    def create_from_json(self, data, name):
+        json_bytes = BytesIO()
+        data.to_json(json_bytes)
+        json_bytes.seek(0)
+        self.client.put_object(
+            self.bucket, name, json_bytes, len(json_bytes.getvalue())
+        )
+        return self.get_url(name)
+
     def list(self, pattern="*"):
         return fnmatch.filter(  # need to test
             [
                 obj.object_name
                 for obj in self.client.list_objects(self.bucket, recursive=True)
             ],
             pattern,
         )
 
+    def read_object(self, name):
+        return BytesIO(self.client.get_object(self.bucket, name).read())
+
     def read_from_array(self, name):
-        return np.load(BytesIO(self.client.get_object(self.bucket, name).read()))
+        return np.load(self.read_object(name))
 
     def read_from_rasterio(self, name):
-        return rio.open(BytesIO(self.client.get_object(self.bucket, name).read()))
+        return rio.open(self.read_object(name))
+
+    def read_from_csv(self, name):
+        return pd.read_csv(self.read_object(name))
+
+    def read_from_json(self, name):
+        return pd.read_json(self.read_object(name))
```

### Comparing `spai-2023.5.25.post3/spai/storage/Storage.py` & `spai-2023.5.25.post5/spai/storage/Storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from glob import glob
 import rasterio as rio
 import numpy as np
+import pandas as pd
 
 from .BaseStorage import BaseStorage
 
 
 class Storage(BaseStorage):
     def __init__(self, path="data"):
         super().__init__()
@@ -47,19 +48,35 @@
         return dst_path
 
     def create_from_array(self, data, name):
         dst_path = self.get_path(name)
         np.save(dst_path, data)
         return dst_path
 
+    def create_from_csv(self, data, name):
+        dst_path = self.get_path(name)
+        data.to_csv(dst_path, index=False)
+        return dst_path
+
+    def create_from_json(self, data, name):
+        dst_path = self.get_path(name)
+        data.to_json(dst_path)
+        return dst_path
+
     def list(self, pattern="*"):
         paths = glob(os.path.join(self.path, pattern))
         # strip base path
         return [p.replace(self.path + "/", "") for p in paths]
 
     def read_from_array(self, name, path=None):
         if path is None:
             path = self.get_path(name)
         return np.load(path)
 
     def read_from_rasterio(self, name):
         return rio.open(self.get_path(name))
+
+    def read_from_csv(self, name):
+        return pd.read_csv(self.get_path(name))
+
+    def read_from_json(self, name):
+        return pd.read_json(self.get_path(name))
```

### Comparing `spai-2023.5.25.post3/spai/storage/minio.py` & `spai-2023.5.25.post5/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post3/setup.py` & `spai-2023.5.25.post5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'spai.cli': ['project-template/*', 'project-template/notebooks/analytics/*']}
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.25.post3',
+    'version': '2023.5.25.post5',
     'description': '',
     'long_description': '',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

