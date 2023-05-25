# Comparing `tmp/pyhgtmap-3.0.tar.gz` & `tmp/pyhgtmap-3.1.tar.gz`

## Comparing `pyhgtmap-3.0.tar` & `pyhgtmap-3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    31760 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/NASASRTMUtil.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/configUtil.py
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/contour.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/logger.py
--rw-r--r--   0        0        0    23328 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/main.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/varint.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/hgt/__init__.py
--rw-r--r--   0        0        0    27082 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/hgt/file.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/hgt/processor.py
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/hgt/tile.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/output/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/output/factory.py
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/output/o5mUtil.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/output/osmUtil.py
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyhgtmap/output/pbfUtil.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pyhgtmap-3.0/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyhgtmap-3.0/LICENSE.md
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 pyhgtmap-3.0/README.md
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 pyhgtmap-3.0/pyproject.toml
--rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 pyhgtmap-3.0/PKG-INFO
+-rw-r--r--   0        0        0    31759 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/NASASRTMUtil.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/configUtil.py
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/contour.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/logger.py
+-rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/main.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/varint.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/__init__.py
+-rw-r--r--   0        0        0    27460 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/file.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/processor.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/tile.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/factory.py
+-rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/o5mUtil.py
+-rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/osmUtil.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/pbfUtil.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pyhgtmap-3.1/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyhgtmap-3.1/LICENSE.md
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 pyhgtmap-3.1/README.md
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyproject.toml
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 pyhgtmap-3.1/PKG-INFO
```

### Comparing `pyhgtmap-3.0/pyhgtmap/NASASRTMUtil.py` & `pyhgtmap-3.1/pyhgtmap/NASASRTMUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import print_function
 
-
 import base64
 import os
 import sys
 import urllib
 import zipfile
 from http import cookiejar as cookielib
```

### Comparing `pyhgtmap-3.0/pyhgtmap/configUtil.py` & `pyhgtmap-3.1/pyhgtmap/configUtil.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/pyhgtmap/contour.py` & `pyhgtmap-3.1/pyhgtmap/contour.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/pyhgtmap/logger.py` & `pyhgtmap-3.1/pyhgtmap/logger.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/pyhgtmap/main.py` & `pyhgtmap-3.1/pyhgtmap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,16 @@
         metavar="WAY-ID",
     )
     parser.add_option(
         "--max-nodes-per-tile",
         help="specify an integer as a maximum"
         "\nnumber of nodes per generated tile.  It defaults to 1000000,"
         "\nwhich is approximately the maximum number of nodes handled properly"
-        "\nby mkgmap.  For bigger tiles, try higher values.",
+        "\nby mkgmap.  For bigger tiles, try higher values. For a single file"
+        "\noutput, say 0 here (this disables any parallelization).",
         dest="maxNodesPerTile",
         type="int",
         default=1000000,
         action="store",
     )
     parser.add_option(
         "--max-nodes-per-way",
@@ -582,14 +583,14 @@
             for arg in args
             if os.path.splitext(arg)[1].lower() in (".hgt", ".tif", ".tiff", ".vrt")
         ]
         opts.area = ":".join(
             [str(i) for i in calcHgtArea(hgtDataFiles, opts.srtmCorrx, opts.srtmCorry)]
         )
 
-    HgtFilesProcessor(opts.nJobs, opts.startId, opts.startWayId).process_files(
-        hgtDataFiles, opts
+    HgtFilesProcessor(opts.nJobs, opts.startId, opts.startWayId, opts).process_files(
+        hgtDataFiles
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyhgtmap-3.0/pyhgtmap/varint.py` & `pyhgtmap-3.1/pyhgtmap/varint.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/pyhgtmap/hgt/__init__.py` & `pyhgtmap-3.1/pyhgtmap/hgt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/pyhgtmap/hgt/file.py` & `pyhgtmap-3.1/pyhgtmap/hgt/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 from .tile import hgtTile
 
 meters2Feet = 1.0 / 0.3048
 
 logger = logging.getLogger(__name__)
 
+GEOTIFF_ERROR = "GeoTiff optional support not enabled; please install with 'pip install pyhgtmap[geotiff]'"
+
 
 class hgtError(Exception):
     """is the main class of visible exceptions from this file."""
 
 
 class filenameError(hgtError):
     """is raised when parsing bad filenames."""
@@ -113,15 +115,18 @@
 
 
 # Coordinates transformation function prototype
 TransformFunType = Callable[[List[Tuple[float, float]]], List[Tuple[float, float]]]
 
 
 def getTransform(o, reverse=False) -> Optional[TransformFunType]:
-    from osgeo import osr
+    try:
+        from osgeo import osr
+    except ModuleNotFoundError:
+        raise ImportError(GEOTIFF_ERROR)
 
     n = osr.SpatialReference()
     n.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
     n.ImportFromEPSG(4326)
     oAuth = o.GetAttrValue("AUTHORITY", 1)
     nAuth = n.GetAttrValue("AUTHORITY", 1)
     if nAuth == oAuth:
@@ -141,16 +146,18 @@
 
         return transform
 
 
 def parseGeotiffBbox(
     filename: str, corrx: float, corry: float, doTransform: bool
 ) -> Tuple[float, float, float, float]:
-    from osgeo import gdal, osr
-
+    try:
+        from osgeo import gdal, osr
+    except ModuleNotFoundError:
+        raise ImportError(GEOTIFF_ERROR)
     try:
         g = gdal.Open(filename)
         geoTransform = g.GetGeoTransform()
         if geoTransform[2] != 0 or geoTransform[4] != 0:
             sys.stderr.write(
                 "Can't handle geotiff {!s} with geo transform {!s}\n".format(
                     filename, geoTransform
@@ -401,15 +408,18 @@
             self.transform = None
             self.reverseTransform = None
 
     def initAsGeotiff(
         self, corrx, corry, polygon, checkPoly, voidMax, smooth_ratio: float
     ) -> None:
         """init this hgtFile instance with data from a geotiff image."""
-        from osgeo import gdal, osr
+        try:
+            from osgeo import gdal, osr
+        except ModuleNotFoundError:
+            raise ImportError(GEOTIFF_ERROR)
 
         try:
             g = gdal.Open(self.fullFilename)
             geoTransform = g.GetGeoTransform()
             # we don't need to check for the geo transform, this was already done when
             # calculating the area name from main.py
             fileProj = osr.SpatialReference()
```

### Comparing `pyhgtmap-3.0/pyhgtmap/hgt/tile.py` & `pyhgtmap-3.1/pyhgtmap/hgt/tile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from functools import cache
+from functools import lru_cache
 from typing import Any, Dict, Iterable, List, NamedTuple, Tuple
 
 import numpy
 import numpy.typing
 
 from pyhgtmap.contour import ContoursGenerator, build_contours
 from pyhgtmap.hgt import makeBBoxString, transformLonLats
@@ -43,14 +43,17 @@
         self.mask = tile_data["mask"]
         self.transform = tile_data["transform"]
         self.xData = numpy.arange(self.numOfCols) * self.lonIncrement + self.minLon
         self.yData = numpy.arange(self.numOfRows) * self.latIncrement * -1 + self.maxLat
         self.minEle, self.maxEle = self.getElevRange()
         self.elevations = None
         self.contourData = None
+        # Use cache local to this instance to avoid memory leak
+        # https://stackoverflow.com/a/68550238
+        self.get_contours = lru_cache(maxsize=16)(self._get_contours)
 
     def get_stats(self) -> str:
         """Get some statistics about the tile."""
         minLon, minLat, maxLon, maxLat = transformLonLats(
             self.minLon, self.minLat, self.maxLon, self.maxLat, self.transform
         )
         result = (
@@ -147,16 +150,15 @@
             raise IOError("could not open plot file {0:s} for writing".format(filename))
         for latIndex, row in enumerate(self.zData):
             lat = self.maxLat - latIndex * self.latIncrement
             for lonIndex, height in enumerate(row):
                 lon = self.minLon + lonIndex * self.lonIncrement
                 plotFile.write("{0:.7f} {1:.7f} {2:d}\n".format(lon, lat, height))
 
-    @cache
-    def get_contours(
+    def _get_contours(
         self,
         step_cont=20,
         max_nodes_per_way=0,
         no_zero=False,
         min_cont=None,
         max_cont=None,
         rdp_epsilon=None,
```

### Comparing `pyhgtmap-3.0/pyhgtmap/output/__init__.py` & `pyhgtmap-3.1/pyhgtmap/output/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from typing import Callable, List, NamedTuple, Tuple
 
 import numpy
 
 from pyhgtmap.hgt.tile import TileContours
 
+logger = logging.getLogger(__name__)
+
 # First node ID, number of nodes, closed loop, elevation
 WayType = NamedTuple(
     "WayType",
     [
         ("first_node_id", int),
         ("nb_nodes", int),
         ("closed_loop", bool),
@@ -35,35 +38,45 @@
 
 
 class Output:
     """Base class for all output modules."""
 
     def __init__(self) -> None:
         self.timestampString: str
+        self.ways_pending_write: List[Tuple[List[WayType], int]] = []
 
-    def writeNodes(
+    def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
     ) -> Tuple[int, List[WayType]]:
         """
         Write nodes and prepare associated ways.
         Return (latest_node_id, [ways]) tuple.
         """
         raise NotImplementedError
 
-    def writeWays(self, ways: List[WayType], start_way_id: int) -> None:
-        """Write ways previously prepared by writeNodes."""
+    def write_ways(self, ways: List[WayType], start_way_id: int) -> None:
+        """
+        Add ways previously prepared by write_nodes to be written later
+        (as ways should ideally be written after all nodes).
+        """
+        self.ways_pending_write.append((ways, start_way_id))
+
+    def _write_ways(self, ways: List[WayType], start_way_id: int) -> None:
+        """Actually write ways, upon output finalization via done()."""
         raise NotImplementedError
 
     def done(self) -> None:
         """Finalize and close file."""
-        raise NotImplementedError
+        logger.debug("done() - Writing pending ways")
+        for ways, start_way_id in self.ways_pending_write:
+            self._write_ways(ways, start_way_id)
 
     def flush(self) -> None:
         """Flush file to disk."""
         raise NotImplementedError
 
 
 class Id(object):
```

### Comparing `pyhgtmap-3.0/pyhgtmap/output/factory.py` & `pyhgtmap-3.1/pyhgtmap/output/factory.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/pyhgtmap/output/o5mUtil.py` & `pyhgtmap-3.1/pyhgtmap/output/o5mUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Callable, List, Tuple
 
 import pyhgtmap.output
 from pyhgtmap import output
 from pyhgtmap.hgt.tile import TileContours
 from pyhgtmap.varint import int2str, join, sint2str, writableInt, writableString
 
-
 HUNDREDNANO = 10000000
 
 
 class StringTable(object):
     def __init__(self):
         self.table = []
         self.maxStringRef = 15000
@@ -39,15 +38,16 @@
         self,
         filename,
         osmVersion,
         pyhgtmap_version,
         bbox: Tuple[float, float, float, float],
         elevClassifier: Callable[[int], str],
         writeTimestamp=False,
-    ):
+    ) -> None:
+        super().__init__()
         self.outf = open(filename, "wb")
         self.bbox = bbox
         self.elevClassifier = elevClassifier
         self.stringTable = StringTable()
         self.writeTimestamp = writeTimestamp
         self.timestamp = int(time.mktime(time.localtime()))
         self.timestampString = ""  # dummy attribute, needed by main.py
@@ -169,15 +169,15 @@
             deltaLon = sint2str(lon)
             deltaLat = sint2str(lat)
         data.append(deltaLon)
         data.append(deltaLat)
         # no tags, so data is complete now
         return join(data)
 
-    def writeWays(self, ways, startWayId):
+    def _write_ways(self, ways, startWayId):
         """writes ways to self.outf.  ways shall be a list of
         (<startNodeId>, <length>, <isCycle>, <elevation>) tuples.
         """
         if len(ways) == 0:
             return
         # write a reset byte
         self.writeReset()
@@ -246,21 +246,22 @@
         startNodeId, nodes = eval(nodeString.strip())
         self.writeNodesO5m(nodes, startNodeId)
 
     def flush(self) -> None:
         self.outf.flush()
 
     def done(self) -> None:
+        super().done()
         self.outf.write(writableInt(0xFE))
         self.__del__()
 
     def __del__(self):
         self.outf.close()
 
-    def writeNodes(
+    def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
     ) -> Tuple[int, List[output.WayType]]:
         return writeNodes(self, tile_contours, timestamp_string, start_node_id)
```

### Comparing `pyhgtmap-3.0/pyhgtmap/output/osmUtil.py` & `pyhgtmap-3.1/pyhgtmap/output/osmUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         osmVersion: float,
         pyhgtmap_version: str,
         boundsTag: str,
         gzip: int,
         elevClassifier: Callable[[int], str],
         timestamp=False,
     ) -> None:
+        super().__init__()
         self.outF: IOBase
         if 0 < gzip < 10:
             import gzip as Gzip
 
             self.outF = Gzip.open(fName, "wb", gzip)
         else:
             self.outF = open(fName, "wb")
@@ -65,24 +66,25 @@
             '<osm version="{0:s}" generator="pyhgtmap {1:s}">\n'.format(
                 self.osmVersion, self.pyhgtmap_version
             )
         )
         self.write(self.boundsTag + "\n")
 
     def done(self) -> None:
+        super().done()
         self.write("</osm>\n")
         self.outF.close()
 
     def write(self, output):
         self.outF.write(writableString(output))
 
     def flush(self) -> None:
         self.outF.flush()
 
-    def writeWays(self, ways, startWayId):
+    def _write_ways(self, ways, startWayId):
         IDCounter = pyhgtmap.output.Id(startWayId)
         for startNodeId, length, isCycle, elevation in ways:
             IDCounter.curId += 1
             nodeIds = list(range(startNodeId, startNodeId + length))
             if isCycle:
                 nodeIds.append(nodeIds[0])
             nodeRefs = ('<nd ref="{:d}"/>\n' * len(nodeIds)).format(*nodeIds)
@@ -97,15 +99,15 @@
                     self.timestampString,
                     nodeRefs,
                     elevation,
                     self.elevClassifier(elevation),
                 )
             )
 
-    def writeNodes(
+    def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
     ) -> Tuple[int, List[pyhgtmap.output.WayType]]:
         return writeXML(
```

### Comparing `pyhgtmap-3.0/pyhgtmap/output/pbfUtil.py` & `pyhgtmap-3.1/pyhgtmap/output/pbfUtil.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import logging
 import os
 import time
 from typing import Callable, List, Tuple
 
 import numpy
 import numpy.typing
-import osmium
-import osmium.io
-import osmium.osm
-import osmium.osm.mutable
+import npyosmium
+import npyosmium.io
+import npyosmium.osm
+import npyosmium.osm.mutable
 
 import pyhgtmap.output
 from pyhgtmap.hgt.tile import TileContours
 
 logger = logging.getLogger(__name__)
 
 BUFFER_SIZE: int = 4096 * 1024
@@ -32,55 +32,56 @@
         self,
         filename,
         osmVersion,
         pyhgtmap_version,
         bbox: Tuple[float, float, float, float],
         elevClassifier: Callable[[int], str],
     ):
+        super().__init__()
         self.bbox = bbox
         # SimpleWriter doesn't support overwriting file...
         if os.path.exists(filename):
             os.remove(filename)
-        self.osm_writer = osmium.SimpleWriter(
+        self.osm_writer = npyosmium.SimpleWriter(
             filename, BUFFER_SIZE, self.makeHeader(pyhgtmap_version)
         )
         # self.outf = open(filename, "wb")
         self.granularity = 100
         self.date_granularity = 1000
         self.elevClassifier = elevClassifier
         self.maxNodesPerNodeBlock = 8000
         self.maxNodesPerWayBlock = 32000
         self.timestamp = int(time.mktime(time.localtime()))
         self.timestampString: str = ""  # dummy attribute, needed by main.py
 
-    def makeHeader(self, pyhgtmap_version) -> osmium.io.Header:
+    def makeHeader(self, pyhgtmap_version) -> npyosmium.io.Header:
         """Prepare Header object"""
-        osm_header = osmium.io.Header()
+        osm_header = npyosmium.io.Header()
         left, bottom, right, top = self.bbox
         osm_header.add_box(
-            osmium.osm.Box(
-                osmium.osm.Location(left, bottom), osmium.osm.Location(right, top)
+            npyosmium.osm.Box(
+                npyosmium.osm.Location(left, bottom), npyosmium.osm.Location(right, top)
             )
         )
         osm_header.set(
             key="generator",
             value="pyhgtmap {0:s}".format(pyhgtmap_version),
         )
 
         return osm_header
 
-    def writeWays(self, ways: List[pyhgtmap.output.WayType], startWayId) -> None:
+    def _write_ways(self, ways: List[pyhgtmap.output.WayType], startWayId) -> None:
         """writes ways to self.outf.  ways shall be a list of
         (<startNodeId>, <length>, <isCycle>, <elevation>) tuples.
 
         The waylist is split up to make sure the pbf blobs will not be too big.
         """
         for ind, way in enumerate(ways):
             closed_loop_id: list[int] = [way.first_node_id] if way.closed_loop else []
-            osm_way = osmium.osm.mutable.Way(
+            osm_way = npyosmium.osm.mutable.Way(
                 id=startWayId + ind,
                 tags=(
                     ("ele", str(way.elevation)),
                     ("contour", "elevation"),
                     ("contour_ext", self.elevClassifier(way.elevation)),
                 ),
                 nodes=list(range(way.first_node_id, way.first_node_id + way.nb_nodes))
@@ -88,17 +89,18 @@
             )
             self.osm_writer.add_way(osm_way)
 
     def flush(self) -> None:
         pass
 
     def done(self) -> None:
+        super().done()
         self.osm_writer.close()
 
-    def writeNodes(
+    def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
     ) -> Tuple[int, List[pyhgtmap.output.WayType]]:
         logger.debug(f"writeNodes - startId: {start_node_id}")
@@ -113,23 +115,15 @@
                 continue
             for contour in contour_list:
                 # Add the points corresponding to the individual contour, and prepare the way for later step
                 is_closed_way: bool = bool(numpy.all(contour[0] == contour[-1]))
                 if is_closed_way:
                     # Close way by re-using first node instead of a new one; last node is not needed
                     contour = contour[:-1]
-                for node_id, location in zip(
-                    range(next_node_id, next_node_id + len(contour)), contour
-                ):
-                    self.osm_writer.add_node(
-                        osmium.osm.mutable.Node(
-                            id=node_id,
-                            location=(location[0], location[1]),
-                        )
-                    )
+                self.osm_writer.add_locations(contour, next_node_id)
 
                 ways.append(
                     pyhgtmap.output.WayType(
                         next_node_id, len(contour), is_closed_way, elevation
                     )
                 )
                 # Bump ID for next iteration
```

### Comparing `pyhgtmap-3.0/LICENSE.md` & `pyhgtmap-3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.0/README.md` & `pyhgtmap-3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -28,25 +28,54 @@
 Note that the intended use is not to upload generated contour OSM data to the
 OSM servers but to use it for fancy maps.
 
 # Installation
 
 For ubuntu-like system:
 
+## Ligther deployment (without GeoTiff support)
+
+GDAL dependency is required only to add GeoTiff support, and is quite painful to install.
+If you don't need GeoTiff support, simply install the default version of pyhgtmap:
+
+```bash
+sudo apt update
+sudo apt install python3 python3-pip python3-venv
+python3 -m venv my_venv
+# Switch to venv
+. ./my_venv/bin/activate
+# Install pyhgtmap with dependencies from PyPi
+pip install pyhgtmap
+```
+
+## With GeoTiff optional support
+
 ```bash
 sudo apt update
 sudo apt install python3 python3-pip python3-venv
 # Install GDAL via system package, as it's painful to install through PIP
 sudo apt install python3-gdal 
 # Create virtual env (allow --system-site-packages to use system's GDAL)
 python3 -m venv --system-site-packages my_venv
 # Switch to venv
 . ./my_venv/bin/activate
 # Install pyhgtmap with dependencies from PyPi
-pip install pyhgtmap
+pip install pyhgtmap[geotiff]
+```
+
+## Install directly from GitHub (useful to test non-released fixes)
+
+```bash
+sudo apt update
+sudo apt install python3 python3-pip python3-venv git
+python3 -m venv my_venv
+# Switch to venv
+. ./my_venv/bin/activate
+# Install latest pyhgtmap development version from github
+pip install -U git+https://github.com/agrenott/pyhgtmap.git
 ```
 
 # Usage
 
 For a detailed help, run `pyhgtmap --help` on the console.
 
 ## Example output
```

### Comparing `pyhgtmap-3.0/pyproject.toml` & `pyhgtmap-3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,35 @@
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
   "bs4>=0.0.1",
   "colorlog>=6.7.0",
-  "contourpy>=1.0.7", # Do NOT pin GDAL version to ease installing it via OS package manager (due to many dependencies)
-  "GDAL",
+  "contourpy>=1.0.7",
   "matplotlib>=3.4.3",
   "numpy>=1.24.2",
-  "osmium>=3.6.0",
+  "npyosmium>=3.6.1",
   "pybind11-rdp>=0.1.3",
   "scipy>=1.8.0",
   "shapely>=2.0.1",
 ]
 description = "Creates OpenStreetMap suitable contour lines from NASA SRTM data"
 dynamic = ["version"]
 keywords = ["osm", "OpenStreetMap", "countour", "SRTM", "elevation"]
 license = "GPL-2.0-or-later"
 name = "pyhgtmap"
 readme = "README.md"
 
+[project.optional-dependencies]
+geotiff = [
+  # Do NOT pin GDAL version to ease installing it via OS package manager (due to many dependencies)
+  "GDAL",
+]
+
 [project.scripts]
 pyhgtmap = "pyhgtmap.main:main"
 
 [project.urls]
 repository = "https://github.com/agrenott/pyhgtmap"
 
 [tool.hatch.version]
@@ -57,17 +62,14 @@
   "coverage~=7.2.1",
   "black>=23.1.0",
   "mypy>=1.0.1",
   "mypy-extensions~=1.0.0",
   "ruff>=0.0.259",
 ]
 
-# To allow using system's GDAL, which is painful to install
-system-packages = true
-
 [tool.hatch.envs.default.scripts]
 all = ["style", "typing", "test_cov"]
 fmt = [
   "black {args:pyhgtmap tests tools}",
   "ruff --fix {args:.}",
   "style",
 ]
@@ -83,14 +85,19 @@
   "coverage xml",
 ]
 typing = "mypy {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.9", "3.10"]
 
+[tool.hatch.envs.geotiff]
+# Env for optional geotiff dependencies
+# To allow using system's GDAL, which is painful to install
+system-packages = true
+
 [tool.black]
 
 [tool.isort]
 atomic = true
 known_first_party = ["pyhgtmap"]
 line_length = 88
 profile = "black"
```

### Comparing `pyhgtmap-3.0/PKG-INFO` & `pyhgtmap-3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgtmap
-Version: 3.0
+Version: 3.1
 Summary: Creates OpenStreetMap suitable contour lines from NASA SRTM data
 Project-URL: repository, https://github.com/agrenott/pyhgtmap
 Author-email: Adrian Dempwolff <phyghtmap@aldw.de>, Aurélien Grenotton <agrenott@gmail.com>
 License-Expression: GPL-2.0-or-later
 License-File: LICENSE.md
 Keywords: OpenStreetMap,SRTM,countour,elevation,osm
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,21 +14,22 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: colorlog>=6.7.0
 Requires-Dist: contourpy>=1.0.7
-Requires-Dist: gdal
 Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: npyosmium>=3.6.1
 Requires-Dist: numpy>=1.24.2
-Requires-Dist: osmium>=3.6.0
 Requires-Dist: pybind11-rdp>=0.1.3
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: shapely>=2.0.1
+Provides-Extra: geotiff
+Requires-Dist: gdal; extra == 'geotiff'
 Description-Content-Type: text/markdown
 
 [![Python: 3.9, 3.10](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)](https://www.python.org)
 ![GitHub](https://img.shields.io/github/license/agrenott/pyhgtmap)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/agrenott/pyhgtmap/pythonpackage.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
@@ -57,25 +58,54 @@
 Note that the intended use is not to upload generated contour OSM data to the
 OSM servers but to use it for fancy maps.
 
 # Installation
 
 For ubuntu-like system:
 
+## Ligther deployment (without GeoTiff support)
+
+GDAL dependency is required only to add GeoTiff support, and is quite painful to install.
+If you don't need GeoTiff support, simply install the default version of pyhgtmap:
+
+```bash
+sudo apt update
+sudo apt install python3 python3-pip python3-venv
+python3 -m venv my_venv
+# Switch to venv
+. ./my_venv/bin/activate
+# Install pyhgtmap with dependencies from PyPi
+pip install pyhgtmap
+```
+
+## With GeoTiff optional support
+
 ```bash
 sudo apt update
 sudo apt install python3 python3-pip python3-venv
 # Install GDAL via system package, as it's painful to install through PIP
 sudo apt install python3-gdal 
 # Create virtual env (allow --system-site-packages to use system's GDAL)
 python3 -m venv --system-site-packages my_venv
 # Switch to venv
 . ./my_venv/bin/activate
 # Install pyhgtmap with dependencies from PyPi
-pip install pyhgtmap
+pip install pyhgtmap[geotiff]
+```
+
+## Install directly from GitHub (useful to test non-released fixes)
+
+```bash
+sudo apt update
+sudo apt install python3 python3-pip python3-venv git
+python3 -m venv my_venv
+# Switch to venv
+. ./my_venv/bin/activate
+# Install latest pyhgtmap development version from github
+pip install -U git+https://github.com/agrenott/pyhgtmap.git
 ```
 
 # Usage
 
 For a detailed help, run `pyhgtmap --help` on the console.
 
 ## Example output
```

