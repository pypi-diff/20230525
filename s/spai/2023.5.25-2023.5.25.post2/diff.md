# Comparing `tmp/spai-2023.5.25.tar.gz` & `tmp/spai-2023.5.25.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.25.tar", max compression
+gzip compressed data, was "spai-2023.5.25.post2.tar", max compression
```

## Comparing `spai-2023.5.25.tar` & `spai-2023.5.25.post2.tar`

### file list

```diff
@@ -1,28 +1,39 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25/README.md
--rw-r--r--   0        0        0      264 2023-05-25 06:41:35.471523 spai-2023.5.25/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25/spai/__init__.py
--rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25/spai/cli/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25/spai/cli/local.py
--rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     2129 2023-05-25 06:27:31.453555 spai-2023.5.25/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1264 2023-05-25 06:15:22.923801 spai-2023.5.25/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2434 2023-05-25 06:09:12.743073 spai-2023.5.25/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0       84 2023-05-25 05:50:35.998156 spai-2023.5.25/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       29 2023-05-25 06:31:59.119564 spai-2023.5.25/spai/image/__init__.py
--rw-r--r--   0        0        0      603 2023-05-25 06:36:00.653454 spai-2023.5.25/spai/image/utils.py
--rw-r--r--   0        0        0     3892 2023-05-19 06:36:13.726144 spai-2023.5.25/spai/main.bck
--rw-r--r--   0        0        0     1006 2023-05-22 09:43:14.295844 spai-2023.5.25/spai/main.py
--rw-r--r--   0        0        0       84 2023-05-25 06:27:12.053506 spai-2023.5.25/spai/models.py
--rw-r--r--   0        0        0      433 2023-05-25 06:28:52.517762 spai-2023.5.25/spai/storage/Storage.py
--rw-r--r--   0        0        0       29 2023-05-25 06:29:06.645887 spai-2023.5.25/spai/storage/__init__.py
--rw-r--r--   0        0        0      372 2023-05-25 05:43:36.956784 spai-2023.5.25/spai/storage/minio.py
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 spai-2023.5.25/setup.py
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 spai-2023.5.25/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25.post2/README.md
+-rw-r--r--   0        0        0      266 2023-05-25 10:34:34.765837 spai-2023.5.25.post2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25.post2/spai/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25.post2/spai/cli/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25.post2/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25.post2/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25.post2/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25.post2/spai/cli/local.py
+-rw-r--r--   0        0        0      647 2023-05-25 09:53:16.130678 spai-2023.5.25.post2/spai/cli/project-template/REDME.md
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:27.506558 spai-2023.5.25.post2/spai/cli/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:34.438575 spai-2023.5.25.post2/spai/cli/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:43.562598 spai-2023.5.25.post2/spai/cli/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0        0 2023-05-25 09:46:24.337697 spai-2023.5.25.post2/spai/cli/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:52:54.906626 spai-2023.5.25.post2/spai/cli/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      232 2023-05-25 09:54:34.271270 spai-2023.5.25.post2/spai/cli/project-template/spai.config.yml
+-rw-r--r--   0        0        0        0 2023-05-25 09:53:08.122658 spai-2023.5.25.post2/spai/cli/project-template/uis/map/main.py
+-rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25.post2/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25.post2/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25.post2/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.25.post2/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.25.post2/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.25.post2/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-25 08:29:38.312976 spai-2023.5.25.post2/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.25.post2/spai/image/utils.py
+-rw-r--r--   0        0        0     3892 2023-05-19 06:36:13.726144 spai-2023.5.25.post2/spai/main.bck
+-rw-r--r--   0        0        0     1473 2023-05-25 10:32:18.681715 spai-2023.5.25.post2/spai/main.py
+-rw-r--r--   0        0        0     1285 2023-05-25 09:18:40.109969 spai-2023.5.25.post2/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     2824 2023-05-25 09:09:16.519673 spai-2023.5.25.post2/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2042 2023-05-25 09:15:08.657120 spai-2023.5.25.post2/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.25.post2/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.25.post2/spai/storage/minio.py
+-rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 spai-2023.5.25.post2/setup.py
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.25.post2/PKG-INFO
```

### Comparing `spai-2023.5.25/spai/cli/cloud.py` & `spai-2023.5.25.post2/spai/cli/cloud.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25/spai/cli/local.py` & `spai-2023.5.25.post2/spai/cli/local.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25/spai/cli/validate.py` & `spai-2023.5.25.post2/spai/cli/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25/spai/data/satellite/explore.py` & `spai-2023.5.25.post2/spai/data/satellite/explore.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from .sentinelhub import SHExplorer
 import geopandas as gpd
 
 
-# def download_satellite_image(location, date, sensor, options):
-def explore_satellite_images(time_interval):
+def explore_satellite_images(time_interval, sensor="S2L2A", **kargs):
     # aoi = retrieve_aoi_from_location(location)
     gdf = gpd.GeoDataFrame.from_features(
         {
             "type": "FeatureCollection",
             "features": [
                 {
                     "type": "Feature",
@@ -25,10 +24,10 @@
                         "type": "Polygon",
                     },
                 }
             ],
         },
         crs=4326,  # validate coords are lat/lon !
     )
-    explorer = SHExplorer(time_interval=time_interval, sensor="S2L2A", cloud_cover=0.2)
+    explorer = SHExplorer(time_interval, sensor, **kargs)
     results = explorer.search(gdf)
     return results
```

### Comparing `spai-2023.5.25/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
 from sentinelhub import SHConfig, SentinelHubCatalog
 from sentinelhub import CRS, BBox
 from sentinelhub.data_collections import DataCollection
 
 
 class SHExplorer:
-    def __init__(self, time_interval, sensor, cloud_cover):
+    def __init__(self, time_interval, sensor, **kargs):
         self.query, self.fields = None, {
             "include": ["id", "properties.datetime", "assets.thumbnail.href"],
             "exclude": [],
         }
         self.config = SHConfig()
         if sensor == "S1":
             self.data_collection = DataCollection.SENTINEL1
         elif sensor == "S2L1C" or sensor == "S2L2A":
             # no thumbnail for S2L2A, use the one for S2L1C
             self.data_collection = DataCollection.SENTINEL2_L1C
-            self.fields["include"].append("properties.eo:cloud_cover")
-            self.query = f"eo:cloud_cover < {cloud_cover}"
+            if "cloud_cover" in kargs:
+                cloud_cover = kargs["cloud_cover"]
+                self.query = f"eo:cloud_cover < {cloud_cover}"
+                self.fields["include"].append("properties.eo:cloud_cover")
         elif sensor == "S5P":
             self.data_collection = DataCollection.SENTINEL5P
             # self.data_collection = DataCollection.SENTINEL3_OLCI
             self.config.sh_base_url = DataCollection.SENTINEL5P.service_url
             # self.config.sh_base_url = DataCollection.SENTINEL3_OLCI.service_url
         else:
             raise Exception("Invalid sensor")
```

### Comparing `spai-2023.5.25/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.5.25.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25/spai/main.bck` & `spai-2023.5.25.post2/spai/main.bck`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25/spai/main.py` & `spai-2023.5.25.post2/spai/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 import typer
 from pathlib import Path
+import os
+import shutil
 
-from .cli.commands import hello
-from .cli import (
+from cli.commands import hello
+from cli import (
     load_and_validate_config,
     deploy_and_run_cloud,
     run_local,
     stop_local,
     list_local,
 )
 
 app = typer.Typer()
 app.add_typer(hello.app, name="hello")
 
 
 @app.command()
+def init():
+    # ask for project name
+    project = typer.prompt("Project name")
+    # copy template
+    template = Path(__file__).parent / "cli" / "project-template"
+    shutil.copytree(template, Path(project))
+    # change name to project in spai.config.yaml
+    config = Path(project) / "spai.config.yml"
+    os.system(f"sed -i 's/project-template/{project}/g' {config}")
+    return typer.echo(f"Project {project} created")
+
+
+@app.command()
 def run(
     dir: Path = typer.Option(Path("."), "-d"),
     cloud: bool = typer.Option(False, "-c", "--cloud"),
 ):
     # make sure dir is absolute
     dir = Path(dir).resolve()
     # load and validate config
```

### Comparing `spai-2023.5.25/setup.py` & `spai-2023.5.25.post2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['spai',
  'spai.cli',
  'spai.cli.commands',
+ 'spai.cli.project-template.apis.analytics',
+ 'spai.cli.project-template.apis.xyz',
+ 'spai.cli.project-template.scripts.downloader',
+ 'spai.cli.project-template.scripts.ndvi',
+ 'spai.cli.project-template.uis.map',
  'spai.data',
  'spai.data.satellite',
  'spai.data.satellite.sentinelhub',
  'spai.image',
  'spai.storage']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'spai.cli': ['project-template/*', 'project-template/notebooks/analytics/*']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.25',
+    'version': '2023.5.25.post2',
     'description': '',
     'long_description': '',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

