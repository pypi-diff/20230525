# Comparing `tmp/osmnx-1.3.0.tar.gz` & `tmp/osmnx-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmnx-1.3.0.tar", last modified: Sun Jan  1 16:24:31 2023, max compression
+gzip compressed data, was "osmnx-1.3.1.tar", last modified: Wed May 24 21:55:50 2023, max compression
```

## Comparing `osmnx-1.3.0.tar` & `osmnx-1.3.1.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-01-01 16:24:31.935114 osmnx-1.3.0/
--rw-r--r--   0 geoff      (501) staff       (20)    18682 2022-12-28 21:40:22.000000 osmnx-1.3.0/CHANGELOG.md
--rw-r--r--   0 geoff      (501) staff       (20)     1111 2022-12-22 03:13:01.000000 osmnx-1.3.0/LICENSE.txt
--rw-r--r--   0 geoff      (501) staff       (20)       45 2022-12-14 16:25:06.000000 osmnx-1.3.0/MANIFEST.in
--rw-r--r--   0 geoff      (501) staff       (20)     2268 2023-01-01 16:24:31.935181 osmnx-1.3.0/PKG-INFO
--rw-r--r--   0 geoff      (501) staff       (20)     4357 2022-12-28 21:55:23.000000 osmnx-1.3.0/README.md
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-01-01 16:24:31.934081 osmnx-1.3.0/osmnx/
--rw-r--r--   0 geoff      (501) staff       (20)       73 2022-09-03 08:24:38.000000 osmnx-1.3.0/osmnx/__init__.py
--rw-r--r--   0 geoff      (501) staff       (20)     1993 2022-12-17 00:29:35.000000 osmnx-1.3.0/osmnx/_api.py
--rw-r--r--   0 geoff      (501) staff       (20)      505 2022-12-17 00:29:35.000000 osmnx-1.3.0/osmnx/_errors.py
--rw-r--r--   0 geoff      (501) staff       (20)     1758 2022-12-17 00:29:35.000000 osmnx-1.3.0/osmnx/_polygon_features.py
--rw-r--r--   0 geoff      (501) staff       (20)       52 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/_version.py
--rw-r--r--   0 geoff      (501) staff       (20)    12165 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/bearing.py
--rw-r--r--   0 geoff      (501) staff       (20)    17427 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/distance.py
--rw-r--r--   0 geoff      (501) staff       (20)    28472 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/downloader.py
--rw-r--r--   0 geoff      (501) staff       (20)     9178 2022-12-17 00:29:35.000000 osmnx-1.3.0/osmnx/elevation.py
--rw-r--r--   0 geoff      (501) staff       (20)     5725 2022-12-17 00:29:35.000000 osmnx-1.3.0/osmnx/folium.py
--rw-r--r--   0 geoff      (501) staff       (20)     8406 2022-12-17 00:29:35.000000 osmnx-1.3.0/osmnx/geocoder.py
--rw-r--r--   0 geoff      (501) staff       (20)    39973 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/geometries.py
--rw-r--r--   0 geoff      (501) staff       (20)    29069 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/graph.py
--rw-r--r--   0 geoff      (501) staff       (20)    14220 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/io.py
--rw-r--r--   0 geoff      (501) staff       (20)    14895 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/osm_xml.py
--rw-r--r--   0 geoff      (501) staff       (20)    27018 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/plot.py
--rw-r--r--   0 geoff      (501) staff       (20)     6343 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/projection.py
--rw-r--r--   0 geoff      (501) staff       (20)     7685 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/settings.py
--rw-r--r--   0 geoff      (501) staff       (20)    25488 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/simplification.py
--rw-r--r--   0 geoff      (501) staff       (20)     8409 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/speed.py
--rw-r--r--   0 geoff      (501) staff       (20)    12691 2022-12-22 03:13:01.000000 osmnx-1.3.0/osmnx/stats.py
--rw-r--r--   0 geoff      (501) staff       (20)     6740 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/truncate.py
--rw-r--r--   0 geoff      (501) staff       (20)    10525 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/utils.py
--rw-r--r--   0 geoff      (501) staff       (20)    16209 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/utils_geo.py
--rw-r--r--   0 geoff      (501) staff       (20)    17772 2022-12-17 00:29:36.000000 osmnx-1.3.0/osmnx/utils_graph.py
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-01-01 16:24:31.934989 osmnx-1.3.0/osmnx.egg-info/
--rw-r--r--   0 geoff      (501) staff       (20)     2268 2023-01-01 16:24:31.000000 osmnx-1.3.0/osmnx.egg-info/PKG-INFO
--rw-r--r--   0 geoff      (501) staff       (20)      671 2023-01-01 16:24:31.000000 osmnx-1.3.0/osmnx.egg-info/SOURCES.txt
--rw-r--r--   0 geoff      (501) staff       (20)        1 2023-01-01 16:24:31.000000 osmnx-1.3.0/osmnx.egg-info/dependency_links.txt
--rw-r--r--   0 geoff      (501) staff       (20)      229 2023-01-01 16:24:31.000000 osmnx-1.3.0/osmnx.egg-info/requires.txt
--rw-r--r--   0 geoff      (501) staff       (20)        6 2023-01-01 16:24:31.000000 osmnx-1.3.0/osmnx.egg-info/top_level.txt
--rw-r--r--   0 geoff      (501) staff       (20)      131 2022-12-20 17:38:47.000000 osmnx-1.3.0/requirements.txt
--rw-r--r--   0 geoff      (501) staff       (20)      405 2023-01-01 16:24:31.935462 osmnx-1.3.0/setup.cfg
--rw-r--r--   0 geoff      (501) staff       (20)     2961 2022-12-22 03:13:01.000000 osmnx-1.3.0/setup.py
+drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/
+-rw-r--r--   0 geoff     (1000) geoff     (1000)    19206 2023-05-24 21:42:36.000000 osmnx-1.3.1/CHANGELOG.md
+-rw-r--r--   0 geoff     (1000) geoff     (1000)     1111 2022-12-22 03:13:01.000000 osmnx-1.3.1/LICENSE.txt
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)       45 2022-12-14 16:25:06.000000 osmnx-1.3.1/MANIFEST.in
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     2268 2023-05-24 21:55:50.437286 osmnx-1.3.1/PKG-INFO
+-rw-r--r--   0 geoff     (1000) geoff     (1000)     4357 2022-12-28 21:55:23.000000 osmnx-1.3.1/README.md
+drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/osmnx/
+-rw-r--r--   0 geoff     (1000) geoff     (1000)       73 2022-09-03 08:24:38.000000 osmnx-1.3.1/osmnx/__init__.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     1993 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/_api.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)      505 2022-12-17 00:29:35.000000 osmnx-1.3.1/osmnx/_errors.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     1758 2022-12-17 00:29:35.000000 osmnx-1.3.1/osmnx/_polygon_features.py
+-rw-r--r--   0 geoff     (1000) geoff     (1000)       52 2023-05-24 21:42:36.000000 osmnx-1.3.1/osmnx/_version.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    12165 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/bearing.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    17675 2023-05-11 18:19:00.000000 osmnx-1.3.1/osmnx/distance.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    29369 2023-05-16 15:42:19.000000 osmnx-1.3.1/osmnx/downloader.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     9178 2022-12-17 00:29:35.000000 osmnx-1.3.1/osmnx/elevation.py
+-rw-r--r--   0 geoff     (1000) geoff     (1000)     5725 2023-05-24 16:21:01.000000 osmnx-1.3.1/osmnx/folium.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     8406 2023-01-14 20:32:17.000000 osmnx-1.3.1/osmnx/geocoder.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    39964 2023-05-24 17:58:29.000000 osmnx-1.3.1/osmnx/geometries.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    29082 2023-05-24 17:58:29.000000 osmnx-1.3.1/osmnx/graph.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    14242 2023-03-20 17:40:38.000000 osmnx-1.3.1/osmnx/io.py
+-rw-r--r--   0 geoff     (1000) geoff     (1000)    15244 2023-05-24 21:22:23.000000 osmnx-1.3.1/osmnx/osm_xml.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    27017 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/plot.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     6343 2022-12-17 00:29:36.000000 osmnx-1.3.1/osmnx/projection.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     7996 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/settings.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    25685 2023-03-20 17:40:38.000000 osmnx-1.3.1/osmnx/simplification.py
+-rw-r--r--   0 geoff     (1000) geoff     (1000)     9144 2023-05-22 03:49:01.000000 osmnx-1.3.1/osmnx/speed.py
+-rw-r--r--   0 geoff     (1000) geoff     (1000)    12691 2022-12-22 03:13:01.000000 osmnx-1.3.1/osmnx/stats.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)     6740 2022-12-17 00:29:36.000000 osmnx-1.3.1/osmnx/truncate.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    10547 2023-03-20 17:40:38.000000 osmnx-1.3.1/osmnx/utils.py
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)    16245 2023-02-22 17:24:42.000000 osmnx-1.3.1/osmnx/utils_geo.py
+-rw-r--r--   0 geoff     (1000) geoff     (1000)    17793 2023-05-24 16:21:01.000000 osmnx-1.3.1/osmnx/utils_graph.py
+drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/osmnx.egg-info/
+-rw-r--r--   0 geoff     (1000) geoff     (1000)     2268 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/PKG-INFO
+-rw-r--r--   0 geoff     (1000) geoff     (1000)      691 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/SOURCES.txt
+-rw-r--r--   0 geoff     (1000) geoff     (1000)        1 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/dependency_links.txt
+-rw-r--r--   0 geoff     (1000) geoff     (1000)      208 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/requires.txt
+-rw-r--r--   0 geoff     (1000) geoff     (1000)        6 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/top_level.txt
+-rw-r--r--   0 geoff     (1000) geoff     (1000)      110 2023-05-24 16:21:28.000000 osmnx-1.3.1/requirements.txt
+-rw-rw-r--   0 geoff     (1000) geoff     (1000)      405 2023-05-24 21:55:50.437286 osmnx-1.3.1/setup.cfg
+-rw-r--r--   0 geoff     (1000) geoff     (1000)     2961 2023-05-24 21:42:36.000000 osmnx-1.3.1/setup.py
+drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/tests/
+-rwxr--r--   0 geoff     (1000) geoff     (1000)    20089 2023-05-24 17:58:29.000000 osmnx-1.3.1/tests/test_osmnx.py
```

### Comparing `osmnx-1.3.0/CHANGELOG.md` & `osmnx-1.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # Change log
 
+## 1.3.1 (2023-05-24)
+
+  - improve DNS resolution when using proxies or on networks blocking DNS-over-HTTPS
+  - improve processing of per-lane values when adding edge speeds
+  - improve file writing in save_graph_xml function
+  - ensure node coordinates are non-null and covertible to float in the add_edge_lengths function
+  - ignore ways tagged highway=no or highway=razed in built-in filters
+  - do not assume an edge with key=0 exists between each node pair when simplifying graph
+  - drop dateutil package dependency
+
 ## 1.3.0 (2023-01-01)
+
   - fully support Shapely 2.0 and drop support for Shapely 1.x
   - drop RTree package dependency
   - much faster nearest edges search using STRTree index
   - allow using alternative Google Maps compatible elevation APIs, such as Open Topo Data
   - optionally track merged_edges as a new edge attribute in simplify_graph function
 
 ## 1.2.3 (2022-12-14)
```

### Comparing `osmnx-1.3.0/LICENSE.txt` & `osmnx-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/PKG-INFO` & `osmnx-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.3.0
+Version: 1.3.1
 Summary: Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data
 Home-page: https://github.com/gboeing/osmnx
 Author: Geoff Boeing
 Author-email: boeing@usc.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `osmnx-1.3.0/README.md` & `osmnx-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/_api.py` & `osmnx-1.3.1/osmnx/_api.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/_polygon_features.py` & `osmnx-1.3.1/osmnx/_polygon_features.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/bearing.py` & `osmnx-1.3.1/osmnx/bearing.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/distance.py` & `osmnx-1.3.1/osmnx/distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,16 +143,18 @@
 
     # extract edge IDs and corresponding coordinates from their nodes
     x = G.nodes(data="x")
     y = G.nodes(data="y")
     try:
         # two-dimensional array of coordinates: y0, x0, y1, x1
         c = np.array([(y[u], x[u], y[v], x[v]) for u, v, k in uvk])
-    except KeyError:  # pragma: no cover
-        raise KeyError("some edges missing nodes, possibly due to input data clipping issue")
+        # ensure all coordinates can be converted to float and are non-null
+        assert not np.isnan(c.astype(float)).any()
+    except (AssertionError, KeyError):  # pragma: no cover
+        raise ValueError("some edges missing nodes, possibly due to input data clipping issue")
 
     # calculate great circle distances, round, and fill nulls with zeros
     dists = great_circle_vec(c[:, 0], c[:, 1], c[:, 2], c[:, 3]).round(precision)
     dists[np.isnan(dists)] = 0
     nx.set_edge_attributes(G, values=dict(zip(uvk, dists)), name="length")
 
     utils.log("Added length attributes to graph edges")
@@ -286,30 +288,28 @@
 
     if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
         raise ValueError("`X` and `Y` cannot contain nulls")
     geoms = utils_graph.graph_to_gdfs(G, nodes=False)["geometry"]
 
     # if no interpolation distance was provided
     if interpolate is None:
-
         # build the r-tree spatial index by position for subsequent iloc
         rtree = STRtree(geoms)
 
         # use r-tree to find each point's nearest neighbor and distance
         points = [Point(xy) for xy in zip(X, Y)]
         pos, dist = rtree.query_nearest(points, all_matches=False, return_distance=True)
 
         # if user passed X/Y lists, the 2nd subarray contains geom indices
         if len(pos.shape) > 1:
             pos = pos[1]
         ne = geoms.iloc[pos].index
 
     # otherwise, if interpolation distance was provided
     else:
-
         # interpolate points along edges to index with k-d tree or ball tree
         uvk_xy = []
         for uvk, geom in zip(geoms.index, geoms.values):
             uvk_xy.extend((uvk, xy) for xy in utils_geo.interpolate_points(geom, interpolate))
         labels, xy = zip(*uvk_xy)
         vertices = pd.DataFrame(xy, index=labels, columns=["x", "y"])
 
@@ -345,15 +345,15 @@
 
 
 def _single_shortest_path(G, orig, dest, weight):
     """
     Solve the shortest path from an origin node to a destination node.
 
     This function is a convenience wrapper around networkx.shortest_path, with
-    exception handling for unsolvable paths.
+    exception handling for unsolvable paths. It uses Dijkstra's algorithm.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     orig : int
         origin node ID
@@ -364,31 +364,31 @@
 
     Returns
     -------
     path : list
         list of node IDs constituting the shortest path
     """
     try:
-        return nx.shortest_path(G, orig, dest, weight=weight)
+        return nx.shortest_path(G, orig, dest, weight=weight, method="dijkstra")
     except nx.exception.NetworkXNoPath:  # pragma: no cover
         utils.log(f"Cannot solve path from {orig} to {dest}")
         return None
 
 
 def shortest_path(G, orig, dest, weight="length", cpus=1):
     """
     Solve shortest path from origin node(s) to destination node(s).
 
-    If `orig` and `dest` are single node IDs, this will return a list of the
-    nodes constituting the shortest path between them.  If `orig` and `dest`
-    are lists of node IDs, this will return a list of lists of the nodes
-    constituting the shortest path between each origin-destination pair. If a
-    path cannot be solved, this will return None for that path. You can
-    parallelize solving multiple paths with the `cpus` parameter, but be
-    careful to not exceed your available RAM.
+    Uses Dijkstra's algorithm. If `orig` and `dest` are single node IDs, this
+    will return a list of the nodes constituting the shortest path between
+    them. If `orig` and `dest` are lists of node IDs, this will return a list
+    of lists of the nodes constituting the shortest path between each
+    origin-destination pair. If a path cannot be solved, this will return None
+    for that path. You can parallelize solving multiple paths with the `cpus`
+    parameter, but be careful to not exceed your available RAM.
 
     See also `k_shortest_paths` to solve multiple shortest paths between a
     single origin and destination. For additional functionality or different
     solver algorithms, use NetworkX directly.
 
     Parameters
     ----------
@@ -442,15 +442,16 @@
         raise ValueError("orig and dest must either both be iterable or neither must be iterable")
 
 
 def k_shortest_paths(G, orig, dest, k, weight="length"):
     """
     Solve `k` shortest paths from an origin node to a destination node.
 
-    See also `shortest_path` to get just the one shortest path.
+    Uses Yen's algorithm. See also `shortest_path` to solve just the one
+    shortest path.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     orig : int
         origin node ID
```

### Comparing `osmnx-1.3.0/osmnx/downloader.py` & `osmnx-1.3.1/osmnx/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Interact with the OSM APIs."""
 
-import datetime as dt
 import json
 import logging as lg
 import re
 import socket
 import time
 from collections import OrderedDict
+from datetime import datetime as dt
 from hashlib import sha1
 from pathlib import Path
 from urllib.parse import urlparse
 
 import numpy as np
 import requests
-from dateutil import parser as date_parser
 
 from . import projection
 from . import settings
 from . import utils
 from . import utils_geo
 from ._errors import CacheOnlyModeInterrupt
 
@@ -45,68 +44,70 @@
 
     # driving: filter out un-drivable roads, service roads, private ways, and
     # anything specifying motor=no. also filter out any non-service roads that
     # are tagged as providing certain services
     filters["drive"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|bridleway|bus_guideway|construction|corridor|cycleway|elevator|'
-        f"escalator|footway|path|pedestrian|planned|platform|proposed|raceway|service|"
+        f"escalator|footway|no|path|pedestrian|planned|platform|proposed|raceway|razed|service|"
         f'steps|track"]'
         f'["motor_vehicle"!~"no"]["motorcar"!~"no"]'
         f'["service"!~"alley|driveway|emergency_access|parking|parking_aisle|private"]'
     )
 
     # drive+service: allow ways tagged 'service' but filter out certain types
     filters["drive_service"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|bridleway|bus_guideway|construction|corridor|cycleway|elevator|'
-        f'escalator|footway|path|pedestrian|planned|platform|proposed|raceway|steps|track"]'
+        f"escalator|footway|no|path|pedestrian|planned|platform|proposed|raceway|razed|steps|"
+        f'track"]'
         f'["motor_vehicle"!~"no"]["motorcar"!~"no"]'
         f'["service"!~"emergency_access|parking|parking_aisle|private"]'
     )
 
     # walking: filter out cycle ways, motor ways, private ways, and anything
     # specifying foot=no. allow service roads, permitting things like parking
     # lot lanes, alleys, etc that you *can* walk on even if they're not
     # exactly pleasant walks. some cycleways may allow pedestrians, but this
     # filter ignores such cycleways.
     filters["walk"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
-        f'["highway"!~"abandoned|bus_guideway|construction|cycleway|motor|planned|platform|'
-        f'proposed|raceway"]'
+        f'["highway"!~"abandoned|bus_guideway|construction|cycleway|motor|no|planned|platform|'
+        f'proposed|raceway|razed"]'
         f'["foot"!~"no"]["service"!~"private"]'
     )
 
     # biking: filter out foot ways, motor ways, private ways, and anything
     # specifying biking=no
     filters["bike"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|bus_guideway|construction|corridor|elevator|escalator|footway|'
-        f'motor|planned|platform|proposed|raceway|steps"]'
+        f'motor|no|planned|platform|proposed|raceway|razed|steps"]'
         f'["bicycle"!~"no"]["service"!~"private"]'
     )
 
     # to download all ways, just filter out everything not currently in use or
     # that is private-access only
     filters["all"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
-        f'["highway"!~"abandoned|construction|planned|platform|proposed|raceway"]'
+        f'["highway"!~"abandoned|construction|no|planned|platform|proposed|raceway|razed"]'
         f'["service"!~"private"]'
     )
 
     # to download all ways, including private-access ones, just filter out
     # everything not currently in use
-    filters[
-        "all_private"
-    ] = '["highway"]["area"!~"yes"]["highway"!~"abandoned|construction|planned|platform|proposed|raceway"]'
+    filters["all_private"] = (
+        '["highway"]["area"!~"yes"]["highway"!~"abandoned|construction|no|planned|platform|'
+        'proposed|raceway|razed"]'
+    )
 
     if network_type in filters:
         osm_filter = filters[network_type]
     else:  # pragma: no cover
-        raise ValueError(f'Unrecognized network_type "{network_type}"')
+        raise ValueError(f"Unrecognized network_type {network_type!r}")
 
     return osm_filter
 
 
 def _save_to_cache(url, response_json, sc):
     """
     Save a HTTP response JSON object to a file in the cache folder.
@@ -133,15 +134,14 @@
         the response's HTTP status code
 
     Returns
     -------
     None
     """
     if settings.use_cache:
-
         if sc != 200:
             utils.log(f"Did not save to cache because status code is {sc}")
 
         elif response_json is None:
             utils.log("Did not save to cache because response_json is None")
 
         else:
@@ -152,15 +152,15 @@
             # hash the url to make the filename succinct but unique
             # sha1 digest is 160 bits = 20 bytes = 40 hexadecimal characters
             filename = sha1(url.encode("utf-8")).hexdigest() + ".json"
             cache_filepath = cache_folder / filename
 
             # dump to json, and save to file
             cache_filepath.write_text(json.dumps(response_json), encoding="utf-8")
-            utils.log(f'Saved response to cache file "{cache_filepath}"')
+            utils.log(f"Saved response to cache file {cache_filepath!r}")
 
 
 def _url_in_cache(url):
     """
     Determine if a URL's response exists in the cache.
 
     Calculates the checksum of url to determine the cache file's name.
@@ -198,27 +198,26 @@
     Returns
     -------
     response_json : dict
         cached response for url if it exists in the cache, otherwise None
     """
     # if the tool is configured to use the cache
     if settings.use_cache:
-
         # return cached response for this url if exists, otherwise return None
         cache_filepath = _url_in_cache(url)
         if cache_filepath is not None:
             response_json = json.loads(cache_filepath.read_text(encoding="utf-8"))
 
             # return None if check_remark is True and there is a server
             # remark in the cached response
             if check_remark and "remark" in response_json:
-                utils.log(f'Found remark, so ignoring cache file "{cache_filepath}"')
+                utils.log(f"Found remark, so ignoring cache file {cache_filepath!r}")
                 return None
 
-            utils.log(f'Retrieved response from cache file "{cache_filepath}"')
+            utils.log(f"Retrieved response from cache file {cache_filepath!r}")
             return response_json
 
 
 def _get_http_headers(user_agent=None, referer=None, accept_language=None):
     """
     Update the default requests HTTP headers with OSMnx info.
 
@@ -246,56 +245,66 @@
     headers = requests.utils.default_headers()
     headers.update(
         {"User-Agent": user_agent, "referer": referer, "Accept-Language": accept_language}
     )
     return headers
 
 
-def _get_host_by_name(host):
+def _resolve_host_via_doh(hostname):
     """
-    Resolve IP address from host using Google's public API for DNS over HTTPS.
+    Resolve hostname to IP address via Google's public DNS-over-HTTPS API.
 
     Necessary fallback as socket.gethostbyname will not always work when using
     a proxy. See https://developers.google.com/speed/public-dns/docs/doh/json
+    If the user has set `settings.doh_url_template=None` or if resolution
+    fails (e.g., due to local network blocking DNS-over-HTTPS) the hostname
+    itself will be returned instead. Note that this means that server slot
+    management may be violated: see `_config_dns` documentation for details.
 
     Parameters
     ----------
-    host : string
-        the host to consistently resolve the IP address of
+    hostname : string
+        the hostname to consistently resolve the IP address of
 
     Returns
     -------
     ip_address : string
-        resolved IP address
+        resolved IP address of host, or hostname itself if resolution failed
     """
-    dns_url = f"https://8.8.8.8/resolve?name={host}"
-    response = requests.get(dns_url)
-    data = response.json()
-
-    # status = 0 means NOERROR: standard DNS response code
-    if response.ok and data["Status"] == 0:
-        ip_address = data["Answer"][0]["data"]
-        utils.log(f"Google resolved '{host}' to '{ip_address}'")
-        return ip_address
+    if settings.doh_url_template is None:
+        # if user has set the url template to None, return hostname itself
+        utils.log("User set `doh_url_template=None`, requesting host by name", level=lg.WARNING)
+        return hostname
 
-    # in case host could not be resolved return the host itself
-    else:
-        utils.log(f"Google could not resolve '{host}'. Response status: {data['Status']}")
-        return host
+    try:
+        response = requests.get(settings.doh_url_template.format(hostname=hostname))
+        data = response.json()
+        if response.ok and data["Status"] == 0:
+            # status 0 means NOERROR, so return the IP address
+            return data["Answer"][0]["data"]
+        else:
+            raise requests.exceptions.RequestException
+
+    # if we cannot reach DoH server or cannot resolve host, return hostname itself
+    except requests.exceptions.RequestException:
+        utils.log(
+            f"Failed to resolve {hostname!r} IP via DoH, requesting host by name", level=lg.ERROR
+        )
+        return hostname
 
 
 def _config_dns(url):
     """
-    Force socket.getaddrinfo to use IP address instead of host.
+    Force socket.getaddrinfo to use IP address instead of hostname.
 
     Resolves the URL's domain to an IP address so that we use the same server
     for both 1) checking the necessary pause duration and 2) sending the query
     itself even if there is round-robin redirecting among multiple server
     machines on the server-side. Mutates the getaddrinfo function so it uses
-    the same IP address everytime it finds the host name in the URL.
+    the same IP address everytime it finds the hostname in the URL.
 
     For example, the domain overpass-api.de just redirects to one of its
     subdomains (currently z.overpass-api.de and lz4.overpass-api.de). So if we
     check the status endpoint of overpass-api.de, we may see results for
     subdomain z, but when we submit the query itself it gets redirected to
     subdomain lz4. This could result in violating server lz4's slot management
     timing.
@@ -305,25 +314,29 @@
     url : string
         the URL to consistently resolve the IP address of
 
     Returns
     -------
     None
     """
-    host = urlparse(url).netloc.split(":")[0]
+    hostname = urlparse(url).netloc.split(":")[0]
     try:
-        ip = socket.gethostbyname(host)
+        ip = socket.gethostbyname(hostname)
     except socket.gaierror:  # pragma: no cover
-        # this error occurs sometimes when using a proxy. instead, you must
-        # get IP address using google's public JSON API for DNS over HTTPS
-        ip = _get_host_by_name(host)[0]
+        # may occur when using a proxy, so instead resolve IP address via DoH
+        utils.log(
+            f"Encountered gaierror while trying to resolve {hostname!r}, trying again via DoH...",
+            level=lg.ERROR,
+        )
+        ip = _resolve_host_via_doh(hostname)
 
+    # mutate socket.getaddrinfo to map hostname -> IP address
     def _getaddrinfo(*args):
-        if args[0] == host:
-            utils.log(f"Resolved {host} to {ip}")
+        if args[0] == hostname:
+            utils.log(f"Resolved {hostname!r} to {ip!r}")
             return _original_getaddrinfo(ip, *args[1:])
         else:
             return _original_getaddrinfo(*args)
 
     socket.getaddrinfo = _getaddrinfo
 
 
@@ -374,27 +387,27 @@
         _ = int(status_first_token)  # number of available slots
         pause = 0
 
     except Exception:  # pragma: no cover
         # if first token is 'Slot', it tells you when your slot will be free
         if status_first_token == "Slot":
             utc_time_str = status.split(" ")[3]
-            utc_time = date_parser.parse(utc_time_str).replace(tzinfo=None)
-            pause = int(np.ceil((utc_time - dt.datetime.utcnow()).total_seconds()))
+            utc_time = dt.strptime(utc_time_str, "%Y-%m-%dT%H:%M:%SZ,")
+            pause = int(np.ceil((utc_time - dt.utcnow()).total_seconds()))
             pause = max(pause, 1)
 
         # if first token is 'Currently', it is currently running a query so
         # check back in recursive_delay seconds
         elif status_first_token == "Currently":
             time.sleep(recursive_delay)
             pause = _get_pause(base_endpoint)
 
         # any other status is unrecognized: log error, return default duration
         else:
-            utils.log(f'Unrecognized server status: "{status}"', level=lg.ERROR)
+            utils.log(f"Unrecognized server status: {status!r}", level=lg.ERROR)
             return default_duration
 
     return pause
 
 
 def _make_overpass_settings():
     """
@@ -458,15 +471,14 @@
     # make sure every value in dict is bool, str, or list of str
     error_msg = "tags must be a dict with values of bool, str, or list of str"
     if not isinstance(tags, dict):  # pragma: no cover
         raise TypeError(error_msg)
 
     tags_dict = {}
     for key, value in tags.items():
-
         if isinstance(value, bool):
             tags_dict[key] = value
 
         elif isinstance(value, str):
             tags_dict[key] = [value]
 
         elif isinstance(value, list):
@@ -486,21 +498,20 @@
             for value_item in value:
                 tags_list.append({key: value_item})
 
     # add node/way/relation query components one at a time
     components = []
     for d in tags_list:
         for key, value in d.items():
-
             if isinstance(value, bool):
                 # if bool (ie, True) just pass the key, no value
-                tag_str = f"['{key}'](poly:'{polygon_coord_str}');(._;>;);"
+                tag_str = f"[{key!r}](poly:{polygon_coord_str!r});(._;>;);"
             else:
                 # otherwise, pass "key"="value"
-                tag_str = f"['{key}'='{value}'](poly:'{polygon_coord_str}');(._;>;);"
+                tag_str = f"[{key!r}={value!r}](poly:{polygon_coord_str!r});(._;>;);"
 
             for kind in ("node", "way", "relation"):
                 components.append(f"({kind}{tag_str});")
 
     # finalize query and return
     components = "".join(components)
     query = f"{overpass_settings};({components});out;"
@@ -540,15 +551,15 @@
 
     # subdivide query polygon to get list of sub-divided polygon coord strings
     polygon_coord_strs = _make_overpass_polygon_coord_strs(polygon)
 
     # pass each polygon exterior coordinates in the list to the API, one at a
     # time. The '>' makes it recurse so we get ways and the ways' nodes.
     for polygon_coord_str in polygon_coord_strs:
-        query_str = f"{overpass_settings};(way{osm_filter}(poly:'{polygon_coord_str}');>;);out;"
+        query_str = f"{overpass_settings};(way{osm_filter}(poly:{polygon_coord_str!r});>;);out;"
         response_json = overpass_request(data={"data": query_str})
         response_jsons.append(response_json)
     utils.log(
         f"Got all network data within polygon from API in {len(polygon_coord_strs)} request(s)"
     )
 
     if settings.cache_only_mode:  # pragma: no cover
@@ -779,15 +790,15 @@
         size_kb = len(response.content) / 1000
         domain = re.findall(r"(?s)//(.*?)/", url)[0]
         utils.log(f"Downloaded {size_kb:,.1f}kB from {domain}")
 
         try:
             response_json = response.json()
             if "remark" in response_json:
-                utils.log(f'Server remark: "{response_json["remark"]}"', level=lg.WARNING)
+                utils.log(f'Server remark: {response_json["remark"]!r}', level=lg.WARNING)
 
         except Exception:  # pragma: no cover
             if sc in {429, 504}:
                 # 429 is 'too many requests' and 504 is 'gateway timeout' from
                 # server overload: handle these by pausing then recursively
                 # re-trying until we get a valid response from the server
                 this_pause = error_pause + _get_pause(base_endpoint)
```

### Comparing `osmnx-1.3.0/osmnx/elevation.py` & `osmnx-1.3.1/osmnx/elevation.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/folium.py` & `osmnx-1.3.1/osmnx/folium.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/geocoder.py` & `osmnx-1.3.1/osmnx/geocoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     response_json = downloader.nominatim_request(params=params)
 
     # if results were returned, parse lat and lng out of the result
     if response_json and "lat" in response_json[0] and "lon" in response_json[0]:
         lat = float(response_json[0]["lat"])
         lng = float(response_json[0]["lon"])
         point = (lat, lng)
-        utils.log(f'Geocoded "{query}" to {point}')
+        utils.log(f"Geocoded {query!r} to {point}")
         return point
     else:
-        raise ValueError(f'Nominatim could not geocode query "{query}"')
+        raise ValueError(f"Nominatim could not geocode query {query!r}")
 
 
 def geocode_to_gdf(query, which_result=None, by_osmid=False, buffer_dist=None):
     """
     Retrieve place(s) by name or ID from the Nominatim API as a GeoDataFrame.
 
     You can query by place name or OSM ID. If querying by place name, the
@@ -152,15 +152,15 @@
         limit = which_result
 
     results = downloader._osm_place_download(query, by_osmid=by_osmid, limit=limit)
 
     # choose the right result from the JSON response
     if not results:
         # if no results were returned, raise error
-        raise ValueError(f'Nominatim geocoder returned 0 results for query "{query}"')
+        raise ValueError(f"Nominatim geocoder returned 0 results for query {query!r}")
 
     elif by_osmid:
         # if searching by OSM ID, always take the first (ie, only) result
         result = results[0]
 
     elif which_result is None:
         # else, if which_result=None, auto-select the first (Multi)Polygon
@@ -168,21 +168,21 @@
 
     elif len(results) >= which_result:
         # else, if we got at least which_result results, choose that one
         result = results[which_result - 1]
 
     else:  # pragma: no cover
         # else, we got fewer results than which_result, raise error
-        msg = f'Nominatim geocoder only returned {len(results)} result(s) for query "{query}"'
+        msg = f"Nominatim geocoder only returned {len(results)} result(s) for query {query!r}"
         raise ValueError(msg)
 
     # if we got a non (Multi)Polygon geometry type (like a point), log warning
     geom_type = result["geojson"]["type"]
     if geom_type not in {"Polygon", "MultiPolygon"}:
-        msg = f'Nominatim geocoder returned a {geom_type} as the geometry for query "{query}"'
+        msg = f"Nominatim geocoder returned a {geom_type} as the geometry for query {query!r}"
         utils.log(msg, level=lg.WARNING)
 
     # build the GeoJSON feature from the chosen result
     south, north, west, east = result["boundingbox"]
     feature = {
         "type": "Feature",
         "geometry": result["geojson"],
@@ -224,8 +224,8 @@
     """
     polygon_types = {"Polygon", "MultiPolygon"}
     for result in results:
         if "geojson" in result and result["geojson"]["type"] in polygon_types:
             return result
 
     # if we never found a polygon, throw an error
-    raise ValueError(f'Nominatim could not geocode query "{query}" to polygonal boundaries')
+    raise ValueError(f"Nominatim could not geocode query {query!r} to polygonal boundaries")
```

### Comparing `osmnx-1.3.0/osmnx/geometries.py` & `osmnx-1.3.1/osmnx/geometries.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,15 +380,14 @@
 
         # extract geometries from the downloaded osm data
         for response_json in response_jsons:
             # Parses the JSON of OSM nodes, ways and (multipolygon) relations
             # to dictionaries of coordinates, Shapely Points, LineStrings,
             # Polygons and MultiPolygons
             for element in response_json["elements"]:
-
                 # id numbers are only unique within element types
                 # create unique id from combination of type and id
                 unique_id = f"{element['type']}/{element['id']}"
 
                 # add elements that are not nodes and that are without tags or
                 # with empty tags to the untagged_element_ids set (untagged
                 # nodes are not added to the geometries dict at all)
@@ -561,15 +560,14 @@
             )
             geometry = LineString()
 
     # if the OSM element is a closed way (i.e. first and last nodes are the
     # same) depending upon the tags the geometry could be a Shapely LineString
     # or Polygon
     elif element["nodes"][0] == element["nodes"][-1]:
-
         # determine if closed way represents LineString or Polygon
         if _is_closed_way_a_polygon(element):
             # if it is a Polygon
             try:
                 geometry = Polygon([(coords[node]["lon"], coords[node]["lat"]) for node in nodes])
             except (GEOSException, ValueError) as e:
                 # XMLs may include geometries that are incomplete, in which
@@ -632,28 +630,26 @@
     is_polygon = False
 
     # get the element's tags
     element_tags = element.get("tags")
 
     # if the element doesn't have any tags leave it as a Linestring
     if element_tags is not None:
-
         # if the element is specifically tagged 'area':'no' -> LineString
         if element_tags.get("area") == "no":
             pass
 
         # if the element has tags and is not tagged 'area':'no'
         # compare its tags with the polygon_features dict
         else:
             # identify common keys in element's tags and polygon_features dict
             intersecting_keys = element_tags.keys() & polygon_features.keys()
 
             # for each key in the intersecting keys (if any found)
             for key in intersecting_keys:
-
                 # Get the key's value from the element's tags
                 key_value = element_tags.get(key)
 
                 # Determine if the key is for a blocklist or passlist in
                 # polygon_features dict
                 blocklist_or_passlist = polygon_features.get(key).get("polygon")
 
@@ -663,24 +659,22 @@
                 # if all features with that key should be polygons -> Polygon
                 if blocklist_or_passlist == "all":
                     is_polygon = True
 
                 # if the key is for a blocklist i.e. tags that should not
                 # become Polygons
                 elif blocklist_or_passlist == "blocklist":
-
                     # if the value for that key in the element is not in
                     # the blocklist -> Polygon
                     if key_value not in polygon_features_values:
                         is_polygon = True
 
                 # if the key is for a passlist i.e. specific tags should
                 # become Polygons
                 elif blocklist_or_passlist == "passlist":
-
                     # if the value for that key in the element is in the
                     # passlist -> Polygon
                     if key_value in polygon_features_values:
                         is_polygon = True
 
     return is_polygon
 
@@ -903,21 +897,19 @@
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         the GeoDataFrame with .buffer(0) applied to invalid geometries
     """
     # only apply the filters if the GeoDataFrame is not empty
     if not gdf.empty:
-
         # create a filter for rows with invalid geometries
         invalid_geometry_filter = ~gdf["geometry"].is_valid
 
         # if there are invalid geometries
         if invalid_geometry_filter.any():
-
             # get their unique_ids from the index
             invalid_geometry_ids = gdf.loc[invalid_geometry_filter].index.to_list()
 
             # create a list of their urls and log them
             osm_url = "https://www.openstreetmap.org/"
             invalid_geom_urls = [osm_url + unique_id for unique_id in invalid_geometry_ids]
             utils.log(
@@ -954,15 +946,14 @@
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         final filtered GeoDataFrame
     """
     # only apply the filters if the GeoDataFrame is not empty
     if not gdf.empty:
-
         # create two filters, initially all True
         polygon_filter = pd.Series(True, index=gdf.index)
         combined_tag_filter = pd.Series(True, index=gdf.index)
 
         # if a polygon was supplied, create a filter that is True for
         # geometries that intersect with the polygon
         if polygon:
```

### Comparing `osmnx-1.3.0/osmnx/graph.py` & `osmnx-1.3.1/osmnx/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,15 @@
         # it's best to parameterize function with clean_periphery=True
         spn = stats.count_streets_per_node(G)
         nx.set_node_attributes(G, values=spn, name="street_count")
         msg = (
             "the graph-level street_count attribute will likely be inaccurate "
             "when you set clean_periphery=False"
         )
-        warnings.warn(msg)
+        warnings.warn(msg, stacklevel=1)
 
     utils.log(f"graph_from_polygon returned graph with {len(G)} nodes and {len(G.edges)} edges")
     return G
 
 
 def graph_from_xml(filepath, bidirectional=False, simplify=True, retain_all=False):
     """
@@ -751,15 +751,14 @@
     # travel can only occur in the opposite direction of the node order. see:
     # https://wiki.openstreetmap.org/wiki/Key:oneway
     # https://www.geofabrik.de/de/data/geofabrik-osm-gis-standard-0.7.pdf
     oneway_values = {"yes", "true", "1", "-1", "reverse", "T", "F"}
     reversed_values = {"-1", "reverse", "T"}
 
     for path in paths:
-
         # extract/remove the ordered list of nodes from this path element so
         # we don't add it as a superfluous attribute to the edge later
         nodes = path.pop("nodes")
 
         # reverse the order of nodes in the path if this path is both one-way
         # and only allows travel in the opposite direction of nodes' order
         is_one_way = _is_path_one_way(path, bidirectional, oneway_values)
```

### Comparing `osmnx-1.3.0/osmnx/io.py` & `osmnx-1.3.1/osmnx/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(utils_graph.get_undirected(G))
     gdf_nodes = _stringify_nonnumeric_cols(gdf_nodes)
     gdf_edges = _stringify_nonnumeric_cols(gdf_edges)
 
     # save the nodes and edges as GeoPackage layers
     gdf_nodes.to_file(filepath, layer="nodes", driver="GPKG", index=True, encoding=encoding)
     gdf_edges.to_file(filepath, layer="edges", driver="GPKG", index=True, encoding=encoding)
-    utils.log(f'Saved graph as GeoPackage at "{filepath}"')
+    utils.log(f"Saved graph as GeoPackage at {filepath!r}")
 
 
 def save_graph_shapefile(G, filepath=None, encoding="utf-8", directed=False):
     """
     Do not use: deprecated. Use the save_graph_geopackage function instead.
 
     The Shapefile format is proprietary and outdated. Instead, use the
@@ -83,15 +83,16 @@
     Returns
     -------
     None
     """
     warnings.warn(
         "The `save_graph_shapefile` function is deprecated and will be removed "
         "in a future release. Instead, use the `save_graph_geopackage` function "
-        "to save graphs as GeoPackage files for subsequent GIS analysis."
+        "to save graphs as GeoPackage files for subsequent GIS analysis.",
+        stacklevel=1,
     )
 
     # default filepath if none was provided
     if filepath is None:
         filepath = Path(settings.data_folder) / "graph_shapefile"
     else:
         filepath = Path(filepath)
@@ -109,15 +110,15 @@
         gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(utils_graph.get_undirected(G))
     gdf_nodes = _stringify_nonnumeric_cols(gdf_nodes)
     gdf_edges = _stringify_nonnumeric_cols(gdf_edges)
 
     # save the nodes and edges as separate ESRI shapefiles
     gdf_nodes.to_file(filepath_nodes, driver="ESRI Shapefile", index=True, encoding=encoding)
     gdf_edges.to_file(filepath_edges, driver="ESRI Shapefile", index=True, encoding=encoding)
-    utils.log(f'Saved graph as shapefiles at "{filepath}"')
+    utils.log(f"Saved graph as shapefiles at {filepath!r}")
 
 
 def save_graphml(G, filepath=None, gephi=False, encoding="utf-8"):
     """
     Save graph to disk as GraphML file.
 
     Parameters
@@ -166,15 +167,15 @@
 
     # stringify all the edge attribute values
     for _, _, data in G.edges(keys=False, data=True):
         for attr, value in data.items():
             data[attr] = str(value)
 
     nx.write_graphml(G, path=filepath, encoding=encoding)
-    utils.log(f'Saved graph as GraphML file at "{filepath}"')
+    utils.log(f"Saved graph as GraphML file at {filepath!r}")
 
 
 def load_graphml(
     filepath=None, graphml_str=None, node_dtypes=None, edge_dtypes=None, graph_dtypes=None
 ):
     """
     Load an OSMnx-saved GraphML file from disk or GraphML string.
@@ -267,15 +268,15 @@
 
     # convert graph/node/edge attribute data types
     utils.log("Converting node, edge, and graph-level attribute data types")
     G = _convert_graph_attr_types(G, default_graph_dtypes)
     G = _convert_node_attr_types(G, default_node_dtypes)
     G = _convert_edge_attr_types(G, default_edge_dtypes)
 
-    utils.log(f'Loaded graph with {len(G)} nodes and {len(G.edges)} edges from "{source}"')
+    utils.log(f"Loaded graph with {len(G)} nodes and {len(G.edges)} edges from {source!r}")
     return G
 
 
 def _convert_graph_attr_types(G, dtypes=None):
     """
     Convert graph-level attributes using a dict of data types.
 
@@ -334,15 +335,14 @@
 
     Returns
     -------
     G : networkx.MultiDiGraph
     """
     # for each edge in the graph, eval attribute value lists and convert types
     for _, _, data in G.edges(data=True, keys=False):
-
         # remove extraneous "id" attribute added by graphml saving
         data.pop("id", None)
 
         # first, eval stringified lists to convert them to list objects
         # edge attributes might have a single value, or a list if simplified
         for attr, value in data.items():
             if value.startswith("[") and value.endswith("]"):
@@ -388,15 +388,15 @@
     bool
     """
     if value in {"True", "False"}:
         return value == "True"
     elif isinstance(value, bool):
         return value
     else:  # pragma: no cover
-        raise ValueError(f'invalid literal for boolean: "{value}"')
+        raise ValueError(f"invalid literal for boolean: {value!r}")
 
 
 def _stringify_nonnumeric_cols(gdf):
     """
     Make every non-numeric GeoDataFrame column (besides geometry) a string.
 
     This allows proper serializing via Fiona of GeoDataFrames with mixed types
```

### Comparing `osmnx-1.3.0/osmnx/osm_xml.py` & `osmnx-1.3.1/osmnx/osm_xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,16 @@
     node_tags=settings.osm_xml_node_tags,
     node_attrs=settings.osm_xml_node_attrs,
     edge_tags=settings.osm_xml_way_tags,
     edge_attrs=settings.osm_xml_way_attrs,
     oneway=False,
     merge_edges=True,
     edge_tag_aggs=None,
+    api_version=0.6,
+    precision=6,
 ):
     """
     Save graph to disk as an OSM-formatted XML .osm file.
 
     This function exists only to allow serialization to the .osm file format
     for applications that require it, and has constraints to conform to that.
     As such, this function has a limited use case which does not include
@@ -159,14 +161,18 @@
         OSM way entry tags accurately represent the sum total of
         their component edge attributes. For example, if the user
         wants the OSM way to have a "length" attribute, the user must
         specify `edge_tag_aggs=[('length', 'sum')]` in order to tell
         this method to aggregate the lengths of the individual
         component edges. Otherwise, the length attribute will simply
         reflect the length of the first edge associated with the way.
+    api_version : float
+        OpenStreetMap API version to write to the XML file header
+    precision : int
+        number of decimal places to round latitude and longitude values
 
     Returns
     -------
     None
     """
     # default filepath if none was provided
     if filepath is None:
@@ -180,64 +186,62 @@
     if not settings.all_oneway:  # pragma: no cover
         import warnings
 
         msg = (
             "In order for save_graph_xml to behave properly the graph must "
             "have been created with the `all_oneway` setting set to True."
         )
-        warnings.warn(msg)
+        warnings.warn(msg, stacklevel=1)
 
     try:
         gdf_nodes, gdf_edges = data
     except ValueError:
         gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(
             data, node_geometry=False, fill_edge_geometry=False
         )
 
     # rename columns per osm specification
     gdf_nodes.rename(columns={"x": "lon", "y": "lat"}, inplace=True)
+    gdf_nodes["lon"] = gdf_nodes["lon"].round(precision)
+    gdf_nodes["lat"] = gdf_nodes["lat"].round(precision)
     gdf_nodes = gdf_nodes.reset_index().rename(columns={"osmid": "id"})
     if "id" in gdf_edges.columns:
         gdf_edges = gdf_edges[[col for col in gdf_edges if col != "id"]]
     if "uniqueid" in gdf_edges.columns:
         gdf_edges = gdf_edges.rename(columns={"uniqueid": "id"})
     else:
         gdf_edges = gdf_edges.reset_index().reset_index().rename(columns={"index": "id"})
 
     # add default values for required attributes
     for table in (gdf_nodes, gdf_edges):
         table["uid"] = "1"
         table["user"] = "osmnx"
         table["version"] = "1"
         table["changeset"] = "1"
-        table["timestamp"] = "2017-01-01T00:00:00Z"
-
-    # convert all datatypes to str
-    gdf_nodes = gdf_nodes.applymap(str)
-    gdf_edges = gdf_edges.applymap(str)
+        table["timestamp"] = utils.ts(template="{:%Y-%m-%dT%H:%M:%SZ}")
 
     # misc. string replacements to meet OSM XML spec
     if "oneway" in gdf_edges.columns:
         # fill blank oneway tags with default (False)
         gdf_edges.loc[pd.isnull(gdf_edges["oneway"]), "oneway"] = oneway
         gdf_edges.loc[:, "oneway"] = gdf_edges["oneway"].astype(str)
         gdf_edges.loc[:, "oneway"] = (
             gdf_edges["oneway"].str.replace("False", "no").replace("True", "yes")
         )
 
     # initialize XML tree with an OSM root element then append nodes/edges
-    root = etree.Element("osm", attrib={"version": "0.6", "generator": "OSMnx"})
+    root = etree.Element("osm", attrib={"version": str(api_version), "generator": "OSMnx"})
     root = _append_nodes_xml_tree(root, gdf_nodes, node_attrs, node_tags)
     root = _append_edges_xml_tree(
         root, gdf_edges, edge_attrs, edge_tags, edge_tag_aggs, merge_edges
     )
 
     # write to disk
-    etree.ElementTree(root).write(filepath)
-    utils.log(f'Saved graph as .osm file at "{filepath}"')
+    etree.ElementTree(root).write(filepath, encoding="utf-8", xml_declaration=True)
+    utils.log(f"Saved graph as .osm file at {filepath!r}")
 
 
 def _append_nodes_xml_tree(root, gdf_nodes, node_attrs, node_tags):
     """
     Append nodes to an XML tree.
 
     Parameters
@@ -253,17 +257,19 @@
 
     Returns
     -------
     root : ElementTree.Element
         xml tree with nodes appended
     """
     for _, row in gdf_nodes.iterrows():
-        node = etree.SubElement(root, "node", attrib=row[node_attrs].dropna().to_dict())
+        row = row.dropna().astype(str)
+        node = etree.SubElement(root, "node", attrib=row[node_attrs].to_dict())
+
         for tag in node_tags:
-            if tag in gdf_nodes.columns:
+            if tag in row:
                 etree.SubElement(node, "tag", attrib={"k": tag, "v": row[tag]})
     return root
 
 
 def _append_edges_xml_tree(root, gdf_edges, edge_attrs, edge_tags, edge_tag_aggs, merge_edges):
     """
     Append edges to an XML tree.
@@ -296,57 +302,57 @@
     Returns
     -------
     root : ElementTree.Element
         xml tree with edges appended
     """
     gdf_edges.reset_index(inplace=True)
     if merge_edges:
-
         for _, all_way_edges in gdf_edges.groupby("id"):
-            first = all_way_edges.iloc[0]
+            first = all_way_edges.iloc[0].dropna().astype(str)
             edge = etree.SubElement(root, "way", attrib=first[edge_attrs].dropna().to_dict())
 
             if len(all_way_edges) == 1:
                 etree.SubElement(edge, "nd", attrib={"ref": first["u"]})
                 etree.SubElement(edge, "nd", attrib={"ref": first["v"]})
             else:
                 # topological sort
                 ordered_nodes = _get_unique_nodes_ordered_from_way(all_way_edges)
                 for node in ordered_nodes:
-                    etree.SubElement(edge, "nd", attrib={"ref": node})
+                    etree.SubElement(edge, "nd", attrib={"ref": str(node)})
 
             if edge_tag_aggs is None:
                 for tag in edge_tags:
-                    if tag in all_way_edges.columns:
+                    if tag in first:
                         etree.SubElement(edge, "tag", attrib={"k": tag, "v": first[tag]})
             else:
                 for tag in edge_tags:
-                    if (tag in all_way_edges.columns) and (
-                        tag not in (t for t, agg in edge_tag_aggs)
-                    ):
+                    if (tag in first) and (tag not in (t for t, agg in edge_tag_aggs)):
                         etree.SubElement(edge, "tag", attrib={"k": tag, "v": first[tag]})
 
                 for tag, agg in edge_tag_aggs:
                     if tag in all_way_edges.columns:
                         etree.SubElement(
-                            edge, "tag", attrib={"k": tag, "v": all_way_edges[tag].aggregate(agg)}
+                            edge,
+                            "tag",
+                            attrib={"k": tag, "v": str(all_way_edges[tag].aggregate(agg))},
                         )
     else:
         # NOTE: this will generate separate OSM ways for each network edge,
         # even if the edges are all part of the same original OSM way. As
         # such, each way will be comprised of two nodes, and there will be
         # many ways with the same OSM id. This does not conform to the
         # OSM XML schema standard, however, the data will still comprise a
         # valid network and will be readable by *most* OSM tools.
         for _, row in gdf_edges.iterrows():
-            edge = etree.SubElement(root, "way", attrib=row[edge_attrs].dropna().to_dict())
+            row = row.dropna().astype(str)
+            edge = etree.SubElement(root, "way", attrib=row[edge_attrs].to_dict())
             etree.SubElement(edge, "nd", attrib={"ref": row["u"]})
             etree.SubElement(edge, "nd", attrib={"ref": row["v"]})
             for tag in edge_tags:
-                if tag in gdf_edges.columns:
+                if tag in row:
                     etree.SubElement(edge, "tag", attrib={"k": tag, "v": row[tag]})
 
     return root
 
 
 def _get_unique_nodes_ordered_from_way(df_way_edges):
     """
```

### Comparing `osmnx-1.3.0/osmnx/plot.py` & `osmnx-1.3.1/osmnx/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -720,15 +720,14 @@
     fig, ax : tuple
         matplotlib figure, axis
     """
     fig.canvas.draw()
     fig.canvas.flush_events()
 
     if save:
-
         # default filepath, if none provided
         if filepath is None:
             filepath = Path(settings.imgs_folder) / "image.png"
         else:
             filepath = Path(filepath)
 
         # if save folder does not already exist, create it
```

### Comparing `osmnx-1.3.0/osmnx/projection.py` & `osmnx-1.3.1/osmnx/projection.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/settings.py` & `osmnx-1.3.1/osmnx/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,17 +40,21 @@
     is `"epsg:4326"`.
 default_referer : string
     HTTP header referer. Default is
     `"OSMnx Python package (https://github.com/gboeing/osmnx)"`.
 default_user_agent : string
     HTTP header user-agent. Default is
     `"OSMnx Python package (https://github.com/gboeing/osmnx)"`.
+doh_url_template : string
+    Endpoint to resolve DNS-over-HTTPS if local DNS resolution fails. Set to
+    None to disable DoH, but see `downloader._config_dns` documentation for
+    caveats. Default is: `"https://8.8.8.8/resolve?name={hostname}"`
 imgs_folder : string or pathlib.Path
     Path to folder in which to save plotted images by default. Default is
-    "./images".
+    `"./images"`.
 log_file : bool
     If True, save log output to a file in logs_folder. Default is `False`.
 log_filename : string
     Name of the log file, without file extension. Default is `"osmnx"`.
 log_console : bool
     If True, print log output to the console (terminal window). Default is
     `False`.
@@ -131,14 +135,15 @@
 cache_only_mode = False
 data_folder = "./data"
 default_accept_language = "en"
 default_access = '["access"!~"private"]'
 default_crs = "epsg:4326"
 default_referer = "OSMnx Python package (https://github.com/gboeing/osmnx)"
 default_user_agent = "OSMnx Python package (https://github.com/gboeing/osmnx)"
+doh_url_template = "https://8.8.8.8/resolve?name={hostname}"
 imgs_folder = "./images"
 log_console = False
 log_file = False
 log_filename = "osmnx"
 log_level = lg.INFO
 log_name = "OSMnx"
 logs_folder = "./logs"
```

### Comparing `osmnx-1.3.0/osmnx/simplification.py` & `osmnx-1.3.1/osmnx/simplification.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,35 +265,36 @@
     initial_node_count = len(G)
     initial_edge_count = len(G.edges)
     all_nodes_to_remove = []
     all_edges_to_add = []
 
     # generate each path that needs to be simplified
     for path in _get_paths_to_simplify(G, strict=strict):
-
         # add the interstitial edges we're removing to a list so we can retain
         # their spatial geometry
         merged_edges = []
         path_attributes = {}
         for u, v in zip(path[:-1], path[1:]):
-
             if track_merged:
                 # keep track of the edges that were merged
                 merged_edges.append((u, v))
 
             # there should rarely be multiple edges between interstitial nodes
             # usually happens if OSM has duplicate ways digitized for just one
             # street... we will keep only one of the edges (see below)
             edge_count = G.number_of_edges(u, v)
             if edge_count != 1:
                 utils.log(f"Found {edge_count} edges between {u} and {v} when simplifying")
 
             # get edge between these nodes: if multiple edges exist between
             # them (see above), we retain only one in the simplified graph
-            edge_data = G.edges[u, v, 0]
+            # We can't assume that there exists an edge from u to v
+            # with key=0, so we get a list of all edges from u to v
+            # and just take the first one.
+            edge_data = list(G.get_edge_data(u, v).values())[0]
             for attr in edge_data:
                 if attr in path_attributes:
                     # if this key already exists in the dict, append it to the
                     # value list
                     path_attributes[attr].append(edge_data[attr])
                 else:
                     # if this key doesn't already exist, set the value to a list
@@ -547,15 +548,14 @@
     H.graph = G.graph
 
     # STEP 5
     # create a new node for each cluster of merged nodes
     # regroup now that we potentially have new cluster labels from step 3
     groups = gdf.groupby("cluster")
     for cluster_label, nodes_subset in groups:
-
         osmids = nodes_subset.index.to_list()
         if len(osmids) == 1:
             # if cluster is a single node, add that node to new graph
             osmid = osmids[0]
             H.add_node(cluster_label, osmid_original=osmid, **G.nodes[osmid])
         else:
             # if cluster is multiple merged nodes, create one new node to
@@ -593,19 +593,17 @@
                 data["geometry"] = gdf_edges.loc[(u, v, k), "geometry"]
             H.add_edge(u2, v2, **data)
 
     # STEP 7
     # for every group of merged nodes with more than 1 node in it, extend the
     # edge geometries to reach the new node point
     for cluster_label, nodes_subset in groups:
-
         # but only if there were multiple nodes merged together,
         # otherwise it's the same old edge as in original graph
         if len(nodes_subset) > 1:
-
             # get coords of merged nodes point centroid to prepend or
             # append to the old edge geom's coords
             x = H.nodes[cluster_label]["x"]
             y = H.nodes[cluster_label]["y"]
             xy = [(x, y)]
 
             # for each edge incident on this new merged node, update its
```

### Comparing `osmnx-1.3.0/osmnx/speed.py` & `osmnx-1.3.1/osmnx/speed.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,40 +163,53 @@
     # add travel time attribute to graph edges
     edges["travel_time"] = travel_time.round(precision).values
     nx.set_edge_attributes(G, values=edges["travel_time"], name="travel_time")
 
     return G
 
 
-def _clean_maxspeed(value, convert_mph=True):
+def _clean_maxspeed(maxspeed, agg=np.mean, convert_mph=True):
     """
     Clean a maxspeed string and convert mph to kph if necessary.
 
+    If present, splits maxspeed on "|" (which denotes that the value contains
+    different speeds per lane) then aggregates the resulting values. Invalid
+    inputs return None. See https://wiki.openstreetmap.org/wiki/Key:maxspeed
+    for details on values and formats.
+
     Parameters
     ----------
-    value : string
-        an OSM way maxspeed value
+    maxspeed : string
+        a valid OpenStreetMap way maxspeed value
+    agg : function
+        aggregation function if maxspeed contains multiple values (default
+        is numpy.mean)
     convert_mph : bool
-        if True, convert mph to kph
+        if True, convert miles per hour to km per hour
 
     Returns
     -------
-    value_clean : string
+    clean_value : string
     """
-    MPH_TO_KPH = 1.60934
-    pattern = re.compile(r"[^\d\.,;]")
-
+    MILES_TO_KM = 1.60934
+    # regex adapted from OSM wiki
+    pattern = "^([0-9][\\.,0-9]+?)(?:[ ]?(?:km/h|kmh|kph|mph|knots))?$"
+    values = re.split(r"\|", maxspeed)  # creates a list even if it's a single value
     try:
-        # strip out everything but numbers, periods, commas, semicolons
-        value_clean = float(re.sub(pattern, "", value).replace(",", "."))
-        if convert_mph and "mph" in value.lower():
-            value_clean = value_clean * MPH_TO_KPH
-        return value_clean
+        clean_values = []
+        for value in values:
+            match = re.match(pattern, value)
+            clean_value = float(match.group(1).replace(",", "."))
+            if convert_mph and "mph" in maxspeed.lower():
+                clean_value = clean_value * MILES_TO_KM
+            clean_values.append(clean_value)
+        return agg(clean_values)
 
-    except ValueError:
+    except (ValueError, AttributeError):
+        # if invalid input, return None
         return None
 
 
 def _collapse_multiple_maxspeed_values(value, agg):
     """
     Collapse a list of maxspeed values to a single value.
```

### Comparing `osmnx-1.3.0/osmnx/stats.py` & `osmnx-1.3.1/osmnx/stats.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/truncate.py` & `osmnx-1.3.1/osmnx/truncate.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.0/osmnx/utils.py` & `osmnx-1.3.1/osmnx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if style == "datetime":
             template = "{:%Y-%m-%d %H:%M:%S}"
         elif style == "date":
             template = "{:%Y-%m-%d}"
         elif style == "time":
             template = "{:%H:%M:%S}"
         else:  # pragma: no cover
-            raise ValueError(f'unrecognized timestamp style "{style}"')
+            raise ValueError(f"unrecognized timestamp style {style!r}")
 
     ts = template.format(dt.datetime.now())
     return ts
 
 
 def config(
     all_oneway=settings.all_oneway,
@@ -189,15 +189,16 @@
     -------
     None
     """
     warnings.warn(
         "The `utils.config` function is deprecated and will be removed in a "
         "future release. Instead, use the `settings` module directly to "
         "configure a global setting's value. For example, "
-        "`ox.settings.log_console=True`."
+        "`ox.settings.log_console=True`.",
+        stacklevel=1,
     )
 
     # set each global setting to the argument value
     settings.all_oneway = all_oneway
     settings.bidirectional_network_types = bidirectional_network_types
     settings.cache_folder = cache_folder
     settings.cache_only_mode = cache_only_mode
@@ -311,15 +312,14 @@
     -------
     logger : logging.logger
     """
     logger = lg.getLogger(name)
 
     # if a logger with this name is not already set up
     if not getattr(logger, "handler_set", None):
-
         # get today's date and construct a log filename
         log_filename = Path(settings.logs_folder) / f'{filename}_{ts(style="date")}.log'
 
         # if the logs folder does not already exist, create it
         log_filename.parent.mkdir(parents=True, exist_ok=True)
 
         # create file handler and log formatter and set them up
```

### Comparing `osmnx-1.3.0/osmnx/utils_geo.py` & `osmnx-1.3.1/osmnx/utils_geo.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     Returns
     -------
     points : geopandas.GeoSeries
         the sampled points, multi-indexed by (u, v, key) of the edge from
         which each point was drawn
     """
     if nx.is_directed(G):  # pragma: no cover
-        warnings.warn("graph should be undirected to not oversample bidirectional edges")
+        warnings.warn(
+            "graph should be undirected to not oversample bidirectional edges", stacklevel=1
+        )
     gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)[["geometry", "length"]]
     weights = gdf_edges["length"] / gdf_edges["length"].sum()
     idx = np.random.choice(gdf_edges.index, size=n, p=weights)
     lines = gdf_edges.loc[idx, "geometry"]
     return lines.interpolate(np.random.rand(n), normalized=True)
```

### Comparing `osmnx-1.3.0/osmnx/utils_graph.py` & `osmnx-1.3.1/osmnx/utils_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         gdf_nodes or gdf_edges or tuple of (gdf_nodes, gdf_edges). gdf_nodes
         is indexed by osmid and gdf_edges is multi-indexed by u, v, key
         following normal MultiDiGraph structure.
     """
     crs = G.graph["crs"]
 
     if nodes:
-
         if not G.nodes:  # pragma: no cover
             raise ValueError("graph contains no nodes")
 
         nodes, data = zip(*G.nodes(data=True))
 
         if node_geometry:
             # convert node x/y attributes to Points for geometry column
@@ -55,22 +54,20 @@
         else:
             gdf_nodes = gpd.GeoDataFrame(data, index=nodes)
 
         gdf_nodes.index.rename("osmid", inplace=True)
         utils.log("Created nodes GeoDataFrame from graph")
 
     if edges:
-
         if not G.edges:  # pragma: no cover
             raise ValueError("graph contains no edges")
 
         u, v, k, data = zip(*G.edges(keys=True, data=True))
 
         if fill_edge_geometry:
-
             # subroutine to get geometry for every edge: if edge already has
             # geometry return it, otherwise create it using the incident nodes
             x_lookup = nx.get_node_attributes(G, "x")
             y_lookup = nx.get_node_attributes(G, "y")
 
             def make_geom(u, v, data, x=x_lookup, y=y_lookup):
                 if "geometry" in data:
@@ -149,15 +146,16 @@
             all_y_match = (gdf_nodes.geometry.y == gdf_nodes["y"]).all()
             assert all_x_match and all_y_match
         except (AssertionError, ValueError):  # pragma: no cover
             # AssertionError if x/y coords don't match geometry column
             # ValueError if geometry column contains non-point geometry types
             warnings.warn(
                 "discarding the gdf_nodes geometry column, though its "
-                "values differ from the coordinates in the x and y columns"
+                "values differ from the coordinates in the x and y columns",
+                stacklevel=1,
             )
         gdf_nodes = gdf_nodes.drop(columns=gdf_nodes.geometry.name)
 
     # create graph and add graph-level attribute dict
     if graph_attrs is None:
         graph_attrs = {"crs": gdf_edges.crs}
     G = nx.MultiDiGraph(**graph_attrs)
@@ -364,24 +362,20 @@
     H.add_edges_from(G.edges(keys=True, data=True))
 
     # the previous operation added all directed edges from G as undirected
     # edges in H. we now have duplicate edges for every bidirectional parallel
     # edge or self-loop. so, look through the edges and remove any duplicates.
     duplicate_edges = set()
     for u1, v1, key1, data1 in H.edges(keys=True, data=True):
-
         # if we haven't already flagged this edge as a duplicate
         if (u1, v1, key1) not in duplicate_edges:
-
             # look at every other edge between u and v, one at a time
             for key2 in H[u1][v1]:
-
                 # don't compare this edge to itself
                 if key1 != key2:
-
                     # compare the first edge's data to the second's
                     # if they match up, flag the duplicate for removal
                     data2 = H.edges[u1, v1, key2]
                     if _is_duplicate_edge(data1, data2):
                         duplicate_edges.add((u1, v1, key2))
 
     H.remove_edges_from(duplicate_edges)
@@ -410,15 +404,14 @@
     # if either edge's osmid contains multiple values (due to simplification)
     # compare them as sets to see if they contain the same values
     osmid1 = set(data1["osmid"]) if isinstance(data1["osmid"], list) else data1["osmid"]
     osmid2 = set(data2["osmid"]) if isinstance(data2["osmid"], list) else data2["osmid"]
 
     # if they contain the same osmid or set of osmids (due to simplification)
     if osmid1 == osmid2:
-
         # if both edges have geometry attributes and they match each other
         if ("geometry" in data1) and ("geometry" in data2):
             if _is_same_geometry(data1["geometry"], data2["geometry"]):
                 is_dupe = True
 
         # if neither edge has a geometry attribute
         elif ("geometry" not in data1) and ("geometry" not in data2):
@@ -486,18 +479,16 @@
     dupes = edges[mask].dropna(subset=["geometry"])
 
     different_streets = []
     groups = dupes[["geometry", "uvk"]].groupby("uvk")
 
     # for each group of duplicate edges
     for _, group in groups:
-
         # for each pair of edges within this group
         for geom1, geom2 in itertools.combinations(group["geometry"], 2):
-
             # if they don't have the same geometry, flag them as different
             # streets: flag edge uvk, but not edge vuk, otherwise we would
             # increment both their keys and they'll still duplicate each other
             if not _is_same_geometry(geom1, geom2):
                 different_streets.append(group.index[0])
 
     # for each unique different street, increment its key to make it unique
```

### Comparing `osmnx-1.3.0/osmnx.egg-info/PKG-INFO` & `osmnx-1.3.1/osmnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.3.0
+Version: 1.3.1
 Summary: Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data
 Home-page: https://github.com/gboeing/osmnx
 Author: Geoff Boeing
 Author-email: boeing@usc.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `osmnx-1.3.0/osmnx.egg-info/SOURCES.txt` & `osmnx-1.3.1/osmnx.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 osmnx/utils.py
 osmnx/utils_geo.py
 osmnx/utils_graph.py
 osmnx.egg-info/PKG-INFO
 osmnx.egg-info/SOURCES.txt
 osmnx.egg-info/dependency_links.txt
 osmnx.egg-info/requires.txt
-osmnx.egg-info/top_level.txt
+osmnx.egg-info/top_level.txt
+tests/test_osmnx.py
```

### Comparing `osmnx-1.3.0/setup.py` & `osmnx-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
 
 # now call setup
 setup(
     name="osmnx",
-    version="1.3.0",
+    version="1.3.1",
     description=DESC,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     classifiers=CLASSIFIERS,
     url="https://github.com/gboeing/osmnx",
     author="Geoff Boeing",
     author_email="boeing@usc.edu",
```

