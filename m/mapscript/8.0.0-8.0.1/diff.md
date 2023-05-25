# Comparing `tmp/mapscript-8.0.0.tar.gz` & `tmp/mapscript-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapscript-8.0.0.tar", last modified: Fri Sep 23 08:10:19 2022, max compression
+gzip compressed data, was "mapscript-8.0.1.tar", last modified: Thu May 25 08:34:58 2023, max compression
```

## Comparing `mapscript-8.0.0.tar` & `mapscript-8.0.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.243231 mapscript-8.0.0/
--rw-rw-rw-   0        0        0    14112 2022-09-23 08:10:19.243231 mapscript-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13396 2022-09-23 08:09:41.000000 mapscript-8.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.196356 mapscript-8.0.0/mapscript/
--rw-rw-rw-   0        0        0     1310 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/__init__.py
--rw-rw-rw-   0        0        0  1051136 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/_mapscript.pyd
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.196356 mapscript-8.0.0/mapscript/examples/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/examples/__init__.py
--rw-rw-rw-   0        0        0     1670 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/examples/project_csv.py
--rw-rw-rw-   0        0        0     2074 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/examples/shpdump.py
--rw-rw-rw-   0        0        0     2909 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/examples/shpinfo.py
--rw-rw-rw-   0        0        0     1551 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/examples/wxs.py
--rw-rw-rw-   0        0        0   125441 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/mapscript.py
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.227606 mapscript-8.0.0/mapscript/tests/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/__init__.py
--rw-rw-rw-   0        0        0     4867 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/class_test.py
--rw-rw-rw-   0        0        0     3952 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/clone_test.py
--rw-rw-rw-   0        0        0     2492 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/cluster_test.py
--rw-rw-rw-   0        0        0     3244 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/color_test.py
--rw-rw-rw-   0        0        0     2597 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/config_test.py
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.227606 mapscript-8.0.0/mapscript/tests/data/
--rw-rw-rw-   0        0        0      463 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/cities.csv
--rw-rw-rw-   0        0        0       52 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/fonts.txt
--rw-rw-rw-   0        0        0     1268 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/home.png
--rw-rw-rw-   0        0        0      118 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/line.dbf
--rw-rw-rw-   0        0        0      188 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/line.shp
--rw-rw-rw-   0        0        0      108 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/line.shx
--rw-rw-rw-   0        0        0      893 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/mapserver-sample.conf
--rw-rw-rw-   0        0        0      118 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/point.dbf
--rw-rw-rw-   0        0        0      128 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/point.shp
--rw-rw-rw-   0        0        0      108 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/point.shx
--rw-rw-rw-   0        0        0      118 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/polygon.dbf
--rw-rw-rw-   0        0        0      236 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/polygon.shp
--rw-rw-rw-   0        0        0      108 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/polygon.shx
--rw-rw-rw-   0        0        0       47 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/raster.tfw
--rw-rw-rw-   0        0        0    27766 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/raster.tif
--rw-rw-rw-   0        0        0      348 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/symbols.txt
--rw-rw-rw-   0        0        0     3978 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/test.map
--rw-rw-rw-   0        0        0    11080 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/test.png
--rw-rw-rw-   0        0        0     1516 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/test_nofontset.map
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.243231 mapscript-8.0.0/mapscript/tests/data/vera/
--rw-rw-rw-   0        0        0     6078 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/vera/COPYRIGHT.TXT
--rw-rw-rw-   0        0        0      331 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/vera/README.TXT
--rw-rw-rw-   0        0        0     8274 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/vera/RELEASENOTES.TXT
--rw-rw-rw-   0        0        0    65932 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/vera/Vera.ttf
--rw-rw-rw-   0        0        0    58716 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/vera/VeraBd.ttf
--rw-rw-rw-   0        0        0     2329 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/data/xmarks.png
--rw-rw-rw-   0        0        0     3018 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/font_test.py
--rw-rw-rw-   0        0        0     5602 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/hash_test.py
--rw-rw-rw-   0        0        0     5563 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/image_test.py
--rw-rw-rw-   0        0        0     2439 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/label_test.py
--rw-rw-rw-   0        0        0    17948 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/layer_test.py
--rw-rw-rw-   0        0        0     3402 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/line_test.py
--rw-rw-rw-   0        0        0    13535 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/map_test.py
--rw-rw-rw-   0        0        0     4910 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/outputformat_test.py
--rw-rw-rw-   0        0        0     5637 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/ows_test.py
--rw-rw-rw-   0        0        0     4292 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/parentreference_test.py
--rw-rw-rw-   0        0        0     4945 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/pgtest.py
--rw-rw-rw-   0        0        0     5513 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/point_test.py
--rw-rw-rw-   0        0        0     5476 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/rect_test.py
--rw-rw-rw-   0        0        0    12334 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/refcount_test.py
--rw-rw-rw-   0        0        0     5495 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/resultcache_test.py
--rw-rw-rw-   0        0        0     7054 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/shape_test.py
--rw-rw-rw-   0        0        0     2365 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/shapefile_test.py
--rw-rw-rw-   0        0        0    11000 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/style_test.py
--rw-rw-rw-   0        0        0     6783 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/symbol_test.py
--rw-rw-rw-   0        0        0     6061 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/symbolset_test.py
--rw-rw-rw-   0        0        0     5852 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/testing.py
--rw-rw-rw-   0        0        0     6511 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/thread_test.py
--rw-rw-rw-   0        0        0     8360 2022-09-23 08:09:41.000000 mapscript-8.0.0/mapscript/tests/zoom_test.py
-drwxrwxrwx   0        0        0        0 2022-09-23 08:10:19.196356 mapscript-8.0.0/mapscript.egg-info/
--rw-rw-rw-   0        0        0    14112 2022-09-23 08:10:18.000000 mapscript-8.0.0/mapscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2102 2022-09-23 08:10:19.000000 mapscript-8.0.0/mapscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-23 08:10:18.000000 mapscript-8.0.0/mapscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-09-23 08:10:18.000000 mapscript-8.0.0/mapscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-23 08:10:19.243231 mapscript-8.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1672 2022-09-23 08:08:08.000000 mapscript-8.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.772476 mapscript-8.0.1/
+-rw-rw-rw-   0        0        0    14112 2023-05-25 08:34:58.772476 mapscript-8.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13396 2023-05-25 08:34:19.000000 mapscript-8.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.709972 mapscript-8.0.1/mapscript/
+-rw-rw-rw-   0        0        0     1310 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/__init__.py
+-rw-rw-rw-   0        0        0  1051136 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/_mapscript.pyd
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.709972 mapscript-8.0.1/mapscript/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/examples/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/examples/project_csv.py
+-rw-rw-rw-   0        0        0     2074 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/examples/shpdump.py
+-rw-rw-rw-   0        0        0     2909 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/examples/shpinfo.py
+-rw-rw-rw-   0        0        0     1551 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/examples/wxs.py
+-rw-rw-rw-   0        0        0   125266 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/mapscript.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.741221 mapscript-8.0.1/mapscript/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/__init__.py
+-rw-rw-rw-   0        0        0     4867 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/class_test.py
+-rw-rw-rw-   0        0        0     3952 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/clone_test.py
+-rw-rw-rw-   0        0        0     2492 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/cluster_test.py
+-rw-rw-rw-   0        0        0     3244 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/color_test.py
+-rw-rw-rw-   0        0        0     2597 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/config_test.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.756846 mapscript-8.0.1/mapscript/tests/data/
+-rw-rw-rw-   0        0        0      463 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/cities.csv
+-rw-rw-rw-   0        0        0       52 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/fonts.txt
+-rw-rw-rw-   0        0        0     1268 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/home.png
+-rw-rw-rw-   0        0        0      118 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/line.dbf
+-rw-rw-rw-   0        0        0      188 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/line.shp
+-rw-rw-rw-   0        0        0      108 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/line.shx
+-rw-rw-rw-   0        0        0      893 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/mapserver-sample.conf
+-rw-rw-rw-   0        0        0      118 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/point.dbf
+-rw-rw-rw-   0        0        0      128 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/point.shp
+-rw-rw-rw-   0        0        0      108 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/point.shx
+-rw-rw-rw-   0        0        0      118 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/polygon.dbf
+-rw-rw-rw-   0        0        0      236 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/polygon.shp
+-rw-rw-rw-   0        0        0      108 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/polygon.shx
+-rw-rw-rw-   0        0        0       47 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/raster.tfw
+-rw-rw-rw-   0        0        0    27766 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/raster.tif
+-rw-rw-rw-   0        0        0      348 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/symbols.txt
+-rw-rw-rw-   0        0        0     3978 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/test.map
+-rw-rw-rw-   0        0        0    11080 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/test.png
+-rw-rw-rw-   0        0        0     1516 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/test_nofontset.map
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.756846 mapscript-8.0.1/mapscript/tests/data/vera/
+-rw-rw-rw-   0        0        0     6078 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/vera/COPYRIGHT.TXT
+-rw-rw-rw-   0        0        0      331 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/vera/README.TXT
+-rw-rw-rw-   0        0        0     8274 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/vera/RELEASENOTES.TXT
+-rw-rw-rw-   0        0        0    65932 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/vera/Vera.ttf
+-rw-rw-rw-   0        0        0    58716 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/vera/VeraBd.ttf
+-rw-rw-rw-   0        0        0     2329 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/data/xmarks.png
+-rw-rw-rw-   0        0        0     3018 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/font_test.py
+-rw-rw-rw-   0        0        0     5602 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/hash_test.py
+-rw-rw-rw-   0        0        0     5563 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/image_test.py
+-rw-rw-rw-   0        0        0     2439 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/label_test.py
+-rw-rw-rw-   0        0        0    17948 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/layer_test.py
+-rw-rw-rw-   0        0        0     3402 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/line_test.py
+-rw-rw-rw-   0        0        0    13535 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/map_test.py
+-rw-rw-rw-   0        0        0     4908 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/outputformat_test.py
+-rw-rw-rw-   0        0        0     5637 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/ows_test.py
+-rw-rw-rw-   0        0        0     4292 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/parentreference_test.py
+-rw-rw-rw-   0        0        0     4945 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/pgtest.py
+-rw-rw-rw-   0        0        0     5513 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/point_test.py
+-rw-rw-rw-   0        0        0     5476 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/rect_test.py
+-rw-rw-rw-   0        0        0    12334 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/refcount_test.py
+-rw-rw-rw-   0        0        0     5495 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/resultcache_test.py
+-rw-rw-rw-   0        0        0     7054 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/shape_test.py
+-rw-rw-rw-   0        0        0     2365 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/shapefile_test.py
+-rw-rw-rw-   0        0        0    11000 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/style_test.py
+-rw-rw-rw-   0        0        0     6783 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/symbol_test.py
+-rw-rw-rw-   0        0        0     6061 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/symbolset_test.py
+-rw-rw-rw-   0        0        0     5852 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/testing.py
+-rw-rw-rw-   0        0        0     6511 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/thread_test.py
+-rw-rw-rw-   0        0        0     8360 2023-05-25 08:34:19.000000 mapscript-8.0.1/mapscript/tests/zoom_test.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:34:58.709972 mapscript-8.0.1/mapscript.egg-info/
+-rw-rw-rw-   0        0        0    14112 2023-05-25 08:34:58.000000 mapscript-8.0.1/mapscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2102 2023-05-25 08:34:58.000000 mapscript-8.0.1/mapscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:34:58.000000 mapscript-8.0.1/mapscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 08:34:58.000000 mapscript-8.0.1/mapscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 08:34:58.772476 mapscript-8.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1672 2023-05-25 08:31:34.000000 mapscript-8.0.1/setup.py
```

### Comparing `mapscript-8.0.0/PKG-INFO` & `mapscript-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapscript
-Version: 8.0.0
+Version: 8.0.1
 Summary: MapServer Python MapScript bindings
 Home-page: http://www.mapserver.org
 Author: Steve Lime
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mapscript-8.0.0/README.rst` & `mapscript-8.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/__init__.py` & `mapscript-8.0.1/mapscript/__init__.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/examples/project_csv.py` & `mapscript-8.0.1/mapscript/examples/project_csv.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/examples/shpdump.py` & `mapscript-8.0.1/mapscript/examples/shpdump.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/examples/shpinfo.py` & `mapscript-8.0.1/mapscript/examples/shpinfo.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/examples/wxs.py` & `mapscript-8.0.1/mapscript/examples/wxs.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/mapscript.py` & `mapscript-8.0.1/mapscript/mapscript.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.1.0
+# This file was automatically generated by SWIG (https://www.swig.org).
+# Version 4.1.1
 #
-# Do not make changes to this file unless you know what you are doing--modify
+# Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 from sys import version_info as _swig_python_version_info
-if _swig_python_version_info < (2, 7, 0):
-    raise RuntimeError("Python 2.7 or later required")
-
 # Import the low-level C/C++ module
 if __package__ or "." in __name__:
     from . import _mapscript
 else:
     import _mapscript
 
 try:
@@ -25,18 +22,18 @@
     except __builtin__.Exception:
         strthis = ""
     return "<%s.%s; %s >" % (self.__class__.__module__, self.__class__.__name__, strthis,)
 
 
 def _swig_setattr_nondynamic_instance_variable(set):
     def set_instance_attr(self, name, value):
-        if name == "thisown":
-            self.this.own(value)
-        elif name == "this":
+        if name == "this":
             set(self, name, value)
+        elif name == "thisown":
+            self.this.own(value)
         elif hasattr(self, name) and isinstance(getattr(type(self), name), property):
             set(self, name, value)
         else:
             raise AttributeError("You cannot add instance attributes to %s" % self)
     return set_instance_attr
 
 
@@ -81,18 +78,14 @@
     @staticmethod
     def frompointer(t: "int *") -> "intarray *":
         return _mapscript.intarray_frompointer(t)
 
 # Register intarray in _mapscript:
 _mapscript.intarray_swigregister(intarray)
 
-def intarray_frompointer(t: "int *") -> "intarray *":
-    return _mapscript.intarray_frompointer(t)
-
-
 MapServerError = _mapscript.MapServerError
 MapServerChildError = _mapscript.MapServerChildError
 
 MS_TRUE = _mapscript.MS_TRUE
 MS_FALSE = _mapscript.MS_FALSE
 MS_UNKNOWN = _mapscript.MS_UNKNOWN
 MS_ON = _mapscript.MS_ON
@@ -292,30 +285,28 @@
 
     def __init__(self):
         _mapscript.CompositingFilter_swiginit(self, _mapscript.new_CompositingFilter())
     __swig_destroy__ = _mapscript.delete_CompositingFilter
 
 # Register CompositingFilter in _mapscript:
 _mapscript.CompositingFilter_swigregister(CompositingFilter)
-
 class LayerCompositer(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     comp_op: "CompositingOperation" = property(_mapscript.LayerCompositer_comp_op_get, _mapscript.LayerCompositer_comp_op_set)
     opacity: "int" = property(_mapscript.LayerCompositer_opacity_get, _mapscript.LayerCompositer_opacity_set)
     filter: "CompositingFilter *" = property(_mapscript.LayerCompositer_filter_get, _mapscript.LayerCompositer_filter_set)
     next: "struct _LayerCompositer *" = property(_mapscript.LayerCompositer_next_get, _mapscript.LayerCompositer_next_set)
 
     def __init__(self):
         _mapscript.LayerCompositer_swiginit(self, _mapscript.new_LayerCompositer())
     __swig_destroy__ = _mapscript.delete_LayerCompositer
 
 # Register LayerCompositer in _mapscript:
 _mapscript.LayerCompositer_swigregister(LayerCompositer)
-
 MS_STYLE_BINDING_LENGTH = _mapscript.MS_STYLE_BINDING_LENGTH
 MS_STYLE_BINDING_SIZE = _mapscript.MS_STYLE_BINDING_SIZE
 MS_STYLE_BINDING_WIDTH = _mapscript.MS_STYLE_BINDING_WIDTH
 MS_STYLE_BINDING_ANGLE = _mapscript.MS_STYLE_BINDING_ANGLE
 MS_STYLE_BINDING_COLOR = _mapscript.MS_STYLE_BINDING_COLOR
 MS_STYLE_BINDING_OUTLINECOLOR = _mapscript.MS_STYLE_BINDING_OUTLINECOLOR
 MS_STYLE_BINDING_SYMBOL = _mapscript.MS_STYLE_BINDING_SYMBOL
@@ -347,15 +338,14 @@
 
     def __init__(self):
         _mapscript.fontSetObj_swiginit(self, _mapscript.new_fontSetObj())
     __swig_destroy__ = _mapscript.delete_fontSetObj
 
 # Register fontSetObj in _mapscript:
 _mapscript.fontSetObj_swigregister(fontSetObj)
-
 MS_TOKEN_LOGICAL_AND = _mapscript.MS_TOKEN_LOGICAL_AND
 MS_TOKEN_LOGICAL_OR = _mapscript.MS_TOKEN_LOGICAL_OR
 MS_TOKEN_LOGICAL_NOT = _mapscript.MS_TOKEN_LOGICAL_NOT
 MS_TOKEN_LITERAL_NUMBER = _mapscript.MS_TOKEN_LITERAL_NUMBER
 MS_TOKEN_LITERAL_STRING = _mapscript.MS_TOKEN_LITERAL_STRING
 MS_TOKEN_LITERAL_TIME = _mapscript.MS_TOKEN_LITERAL_TIME
 MS_TOKEN_LITERAL_SHAPE = _mapscript.MS_TOKEN_LITERAL_SHAPE
@@ -440,15 +430,14 @@
 
     def __init__(self):
         _mapscript.clusterObj_swiginit(self, _mapscript.new_clusterObj())
     __swig_destroy__ = _mapscript.delete_clusterObj
 
 # Register clusterObj in _mapscript:
 _mapscript.clusterObj_swigregister(clusterObj)
-
 class outputFormatObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numformatoptions: "int" = property(_mapscript.outputFormatObj_numformatoptions_get)
     name: "char *" = property(_mapscript.outputFormatObj_name_get, _mapscript.outputFormatObj_name_set)
     mimetype: "char *" = property(_mapscript.outputFormatObj_mimetype_get, _mapscript.outputFormatObj_mimetype_set)
     driver: "char *" = property(_mapscript.outputFormatObj_driver_get, _mapscript.outputFormatObj_driver_set)
@@ -482,15 +471,14 @@
         return _mapscript.outputFormatObj_getOptionAt(self, i)
 
     def attachDevice(self, device: "void *") -> "void":
         return _mapscript.outputFormatObj_attachDevice(self, device)
 
 # Register outputFormatObj in _mapscript:
 _mapscript.outputFormatObj_swigregister(outputFormatObj)
-
 MS_NOOVERRIDE = _mapscript.MS_NOOVERRIDE
 class queryMapObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     map: "struct mapObj *" = property(_mapscript.queryMapObj_map_get)
     height: "int" = property(_mapscript.queryMapObj_height_get, _mapscript.queryMapObj_height_set)
     width: "int" = property(_mapscript.queryMapObj_width_get, _mapscript.queryMapObj_width_set)
@@ -506,15 +494,14 @@
 
     def __init__(self):
         _mapscript.queryMapObj_swiginit(self, _mapscript.new_queryMapObj())
     __swig_destroy__ = _mapscript.delete_queryMapObj
 
 # Register queryMapObj in _mapscript:
 _mapscript.queryMapObj_swigregister(queryMapObj)
-
 class webObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     metadata: "hashTableObj" = property(_mapscript.webObj_metadata_get)
     validation: "hashTableObj" = property(_mapscript.webObj_validation_get)
     map: "struct mapObj *" = property(_mapscript.webObj_map_get)
     imagepath: "char *" = property(_mapscript.webObj_imagepath_get, _mapscript.webObj_imagepath_set)
@@ -541,15 +528,14 @@
         return _mapscript.webObj_updateFromString(self, snippet)
 
     def convertToString(self) -> "char *":
         return _mapscript.webObj_convertToString(self)
 
 # Register webObj in _mapscript:
 _mapscript.webObj_swigregister(webObj)
-
 class styleObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     refcount: "int" = property(_mapscript.styleObj_refcount_get)
     symbolname: "char *" = property(_mapscript.styleObj_symbolname_get)
     patternlength: "int" = property(_mapscript.styleObj_patternlength_get)
     angle: "double" = property(_mapscript.styleObj_angle_get, _mapscript.styleObj_angle_set)
@@ -625,15 +611,14 @@
 
     pattern = property(pattern_get, pattern_set, doc=r"""pattern : list **Python Only**""")
 
 
 
 # Register styleObj in _mapscript:
 _mapscript.styleObj_swigregister(styleObj)
-
 MS_STYLE_SINGLE_SIDED_OFFSET = _mapscript.MS_STYLE_SINGLE_SIDED_OFFSET
 MS_STYLE_DOUBLE_SIDED_OFFSET = _mapscript.MS_STYLE_DOUBLE_SIDED_OFFSET
 class labelLeaderObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numstyles: "int" = property(_mapscript.labelLeaderObj_numstyles_get)
     maxdistance: "int" = property(_mapscript.labelLeaderObj_maxdistance_get, _mapscript.labelLeaderObj_maxdistance_set)
@@ -641,15 +626,14 @@
 
     def __init__(self):
         _mapscript.labelLeaderObj_swiginit(self, _mapscript.new_labelLeaderObj())
     __swig_destroy__ = _mapscript.delete_labelLeaderObj
 
 # Register labelLeaderObj in _mapscript:
 _mapscript.labelLeaderObj_swigregister(labelLeaderObj)
-
 class labelObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     refcount: "int" = property(_mapscript.labelObj_refcount_get)
     font: "char *" = property(_mapscript.labelObj_font_get, _mapscript.labelObj_font_set)
     color: "colorObj" = property(_mapscript.labelObj_color_get, _mapscript.labelObj_color_set)
     outlinecolor: "colorObj" = property(_mapscript.labelObj_outlinecolor_get, _mapscript.labelObj_outlinecolor_set)
@@ -728,15 +712,14 @@
         return _mapscript.labelObj_moveStyleUp(self, index)
 
     def moveStyleDown(self, index: "int") -> "int":
         return _mapscript.labelObj_moveStyleDown(self, index)
 
 # Register labelObj in _mapscript:
 _mapscript.labelObj_swigregister(labelObj)
-
 MS_LABEL_PERPENDICULAR_OFFSET = _mapscript.MS_LABEL_PERPENDICULAR_OFFSET
 MS_LABEL_PERPENDICULAR_TOP_OFFSET = _mapscript.MS_LABEL_PERPENDICULAR_TOP_OFFSET
 class classObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     metadata: "hashTableObj" = property(_mapscript.classObj_metadata_get)
     validation: "hashTableObj" = property(_mapscript.classObj_validation_get)
@@ -817,15 +800,14 @@
         return _mapscript.classObj_moveStyleUp(self, index)
 
     def moveStyleDown(self, index: "int") -> "int":
         return _mapscript.classObj_moveStyleDown(self, index)
 
 # Register classObj in _mapscript:
 _mapscript.classObj_swigregister(classObj)
-
 class labelCacheMemberObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numtextsymbols: "int" = property(_mapscript.labelCacheMemberObj_numtextsymbols_get)
     layerindex: "int" = property(_mapscript.labelCacheMemberObj_layerindex_get)
     classindex: "int" = property(_mapscript.labelCacheMemberObj_classindex_get)
     status: "int" = property(_mapscript.labelCacheMemberObj_status_get)
@@ -837,28 +819,26 @@
 
     def __init__(self):
         _mapscript.labelCacheMemberObj_swiginit(self, _mapscript.new_labelCacheMemberObj())
     __swig_destroy__ = _mapscript.delete_labelCacheMemberObj
 
 # Register labelCacheMemberObj in _mapscript:
 _mapscript.labelCacheMemberObj_swigregister(labelCacheMemberObj)
-
 class markerCacheMemberObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     id: "int" = property(_mapscript.markerCacheMemberObj_id_get)
     bounds: "rectObj" = property(_mapscript.markerCacheMemberObj_bounds_get)
 
     def __init__(self):
         _mapscript.markerCacheMemberObj_swiginit(self, _mapscript.new_markerCacheMemberObj())
     __swig_destroy__ = _mapscript.delete_markerCacheMemberObj
 
 # Register markerCacheMemberObj in _mapscript:
 _mapscript.markerCacheMemberObj_swigregister(markerCacheMemberObj)
-
 class labelCacheSlotObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numlabels: "int" = property(_mapscript.labelCacheSlotObj_numlabels_get)
     cachesize: "int" = property(_mapscript.labelCacheSlotObj_cachesize_get)
     nummarkers: "int" = property(_mapscript.labelCacheSlotObj_nummarkers_get)
     markercachesize: "int" = property(_mapscript.labelCacheSlotObj_markercachesize_get)
@@ -867,45 +847,42 @@
 
     def __init__(self):
         _mapscript.labelCacheSlotObj_swiginit(self, _mapscript.new_labelCacheSlotObj())
     __swig_destroy__ = _mapscript.delete_labelCacheSlotObj
 
 # Register labelCacheSlotObj in _mapscript:
 _mapscript.labelCacheSlotObj_swigregister(labelCacheSlotObj)
-
 class labelCacheObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     num_rendered_members: "int" = property(_mapscript.labelCacheObj_num_rendered_members_get)
 
     def freeCache(self) -> "void":
         return _mapscript.labelCacheObj_freeCache(self)
 
     def __init__(self):
         _mapscript.labelCacheObj_swiginit(self, _mapscript.new_labelCacheObj())
     __swig_destroy__ = _mapscript.delete_labelCacheObj
 
 # Register labelCacheObj in _mapscript:
 _mapscript.labelCacheObj_swigregister(labelCacheObj)
-
 class resultObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     shapeindex: "long" = property(_mapscript.resultObj_shapeindex_get)
     tileindex: "int" = property(_mapscript.resultObj_tileindex_get)
     resultindex: "int" = property(_mapscript.resultObj_resultindex_get)
     classindex: "int" = property(_mapscript.resultObj_classindex_get)
 
     def __init__(self, shapeindex: "long"):
         _mapscript.resultObj_swiginit(self, _mapscript.new_resultObj(shapeindex))
     __swig_destroy__ = _mapscript.delete_resultObj
 
 # Register resultObj in _mapscript:
 _mapscript.resultObj_swigregister(resultObj)
-
 class resultCacheObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numresults: "int" = property(_mapscript.resultCacheObj_numresults_get)
     bounds: "rectObj" = property(_mapscript.resultCacheObj_bounds_get)
 
     def getResult(self, i: "int") -> "resultObj *":
@@ -913,15 +890,14 @@
 
     def __init__(self):
         _mapscript.resultCacheObj_swiginit(self, _mapscript.new_resultCacheObj())
     __swig_destroy__ = _mapscript.delete_resultCacheObj
 
 # Register resultCacheObj in _mapscript:
 _mapscript.resultCacheObj_swigregister(resultCacheObj)
-
 class symbolSetObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numsymbols: "int" = property(_mapscript.symbolSetObj_numsymbols_get)
     maxsymbols: "int" = property(_mapscript.symbolSetObj_maxsymbols_get)
     filename: "char *" = property(_mapscript.symbolSetObj_filename_get, _mapscript.symbolSetObj_filename_set)
     imagecachesize: "int" = property(_mapscript.symbolSetObj_imagecachesize_get, _mapscript.symbolSetObj_imagecachesize_set)
@@ -946,15 +922,14 @@
         return _mapscript.symbolSetObj_removeSymbol(self, index)
 
     def save(self, filename: "char const *") -> "int":
         return _mapscript.symbolSetObj_save(self, filename)
 
 # Register symbolSetObj in _mapscript:
 _mapscript.symbolSetObj_swigregister(symbolSetObj)
-
 class referenceMapObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     map: "struct mapObj *" = property(_mapscript.referenceMapObj_map_get)
     extent: "rectObj" = property(_mapscript.referenceMapObj_extent_get, _mapscript.referenceMapObj_extent_set)
     height: "int" = property(_mapscript.referenceMapObj_height_get, _mapscript.referenceMapObj_height_set)
     width: "int" = property(_mapscript.referenceMapObj_width_get, _mapscript.referenceMapObj_width_set)
@@ -976,15 +951,14 @@
 
     def __init__(self):
         _mapscript.referenceMapObj_swiginit(self, _mapscript.new_referenceMapObj())
     __swig_destroy__ = _mapscript.delete_referenceMapObj
 
 # Register referenceMapObj in _mapscript:
 _mapscript.referenceMapObj_swigregister(referenceMapObj)
-
 MS_SCALEBAR_INTERVALS_MIN = _mapscript.MS_SCALEBAR_INTERVALS_MIN
 MS_SCALEBAR_INTERVALS_MAX = _mapscript.MS_SCALEBAR_INTERVALS_MAX
 MS_SCALEBAR_WIDTH_MIN = _mapscript.MS_SCALEBAR_WIDTH_MIN
 MS_SCALEBAR_WIDTH_MAX = _mapscript.MS_SCALEBAR_WIDTH_MAX
 MS_SCALEBAR_HEIGHT_MIN = _mapscript.MS_SCALEBAR_HEIGHT_MIN
 MS_SCALEBAR_HEIGHT_MAX = _mapscript.MS_SCALEBAR_HEIGHT_MAX
 MS_SCALEBAR_OFFSET_MIN = _mapscript.MS_SCALEBAR_OFFSET_MIN
@@ -1018,15 +992,14 @@
 
     def __init__(self):
         _mapscript.scalebarObj_swiginit(self, _mapscript.new_scalebarObj())
     __swig_destroy__ = _mapscript.delete_scalebarObj
 
 # Register scalebarObj in _mapscript:
 _mapscript.scalebarObj_swigregister(scalebarObj)
-
 MS_LEGEND_KEYSIZE_MIN = _mapscript.MS_LEGEND_KEYSIZE_MIN
 MS_LEGEND_KEYSIZE_MAX = _mapscript.MS_LEGEND_KEYSIZE_MAX
 MS_LEGEND_KEYSPACING_MIN = _mapscript.MS_LEGEND_KEYSPACING_MIN
 MS_LEGEND_KEYSPACING_MAX = _mapscript.MS_LEGEND_KEYSPACING_MAX
 class legendObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -1054,15 +1027,14 @@
 
     def __init__(self):
         _mapscript.legendObj_swiginit(self, _mapscript.new_legendObj())
     __swig_destroy__ = _mapscript.delete_legendObj
 
 # Register legendObj in _mapscript:
 _mapscript.legendObj_swigregister(legendObj)
-
 class imageObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     width: "int" = property(_mapscript.imageObj_width_get)
     height: "int" = property(_mapscript.imageObj_height_get)
     resolution: "double" = property(_mapscript.imageObj_resolution_get)
     resolutionfactor: "double" = property(_mapscript.imageObj_resolutionfactor_get)
@@ -1084,43 +1056,40 @@
         return _mapscript.imageObj_getSize(self)
 
     def write(self, *args) -> "int":
         return _mapscript.imageObj_write(self, *args)
 
 # Register imageObj in _mapscript:
 _mapscript.imageObj_swigregister(imageObj)
-
 class scaleTokenEntryObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     minscale: "double" = property(_mapscript.scaleTokenEntryObj_minscale_get, _mapscript.scaleTokenEntryObj_minscale_set)
     maxscale: "double" = property(_mapscript.scaleTokenEntryObj_maxscale_get, _mapscript.scaleTokenEntryObj_maxscale_set)
     value: "char *" = property(_mapscript.scaleTokenEntryObj_value_get, _mapscript.scaleTokenEntryObj_value_set)
 
     def __init__(self):
         _mapscript.scaleTokenEntryObj_swiginit(self, _mapscript.new_scaleTokenEntryObj())
     __swig_destroy__ = _mapscript.delete_scaleTokenEntryObj
 
 # Register scaleTokenEntryObj in _mapscript:
 _mapscript.scaleTokenEntryObj_swigregister(scaleTokenEntryObj)
-
 class scaleTokenObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     name: "char *" = property(_mapscript.scaleTokenObj_name_get, _mapscript.scaleTokenObj_name_set)
     n_entries: "int" = property(_mapscript.scaleTokenObj_n_entries_get, _mapscript.scaleTokenObj_n_entries_set)
     tokens: "scaleTokenEntryObj *" = property(_mapscript.scaleTokenObj_tokens_get, _mapscript.scaleTokenObj_tokens_set)
 
     def __init__(self):
         _mapscript.scaleTokenObj_swiginit(self, _mapscript.new_scaleTokenObj())
     __swig_destroy__ = _mapscript.delete_scaleTokenObj
 
 # Register scaleTokenObj in _mapscript:
 _mapscript.scaleTokenObj_swigregister(scaleTokenObj)
-
 class layerObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     refcount: "int" = property(_mapscript.layerObj_refcount_get)
     numclasses: "int" = property(_mapscript.layerObj_numclasses_get)
     maxclasses: "int" = property(_mapscript.layerObj_maxclasses_get)
     index: "int" = property(_mapscript.layerObj_index_get)
@@ -1384,15 +1353,14 @@
         item_types = [self.getItemType(idx) for idx in range(0, self.numitems)]
         return zip(item_names, item_types)
 
 
 
 # Register layerObj in _mapscript:
 _mapscript.layerObj_swigregister(layerObj)
-
 MS_RESOLUTION_MAX = _mapscript.MS_RESOLUTION_MAX
 MS_RESOLUTION_MIN = _mapscript.MS_RESOLUTION_MIN
 class mapObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     refcount: "int" = property(_mapscript.mapObj_refcount_get)
     numlayers: "int" = property(_mapscript.mapObj_numlayers_get)
@@ -1703,29 +1671,28 @@
     height = property(get_height, set_height, doc = "See :ref:`SIZE <mapfile-map-size>`")
 
 
 
 # Register mapObj in _mapscript:
 _mapscript.mapObj_swigregister(mapObj)
 
-
 def msSaveImage(map: "mapObj", img: "imageObj", filename: "char const *") -> "int":
     return _mapscript.msSaveImage(map, img, filename)
 
 def msFreeImage(img: "imageObj") -> "void":
     return _mapscript.msFreeImage(img)
 
 def msSetup() -> "int":
     return _mapscript.msSetup()
 
 def msCleanup() -> "void":
     return _mapscript.msCleanup()
 
-def msLoadMapFromString(buffer: "char *", new_mappath: "char *") -> "mapObj *":
-    return _mapscript.msLoadMapFromString(buffer, new_mappath)
+def msLoadMapFromString(buffer: "char *", new_mappath: "char *", config: "configObj") -> "mapObj *":
+    return _mapscript.msLoadMapFromString(buffer, new_mappath, config)
 MS_VERSION_MAJOR = _mapscript.MS_VERSION_MAJOR
 MS_VERSION_MINOR = _mapscript.MS_VERSION_MINOR
 MS_VERSION_REV = _mapscript.MS_VERSION_REV
 MS_VERSION = _mapscript.MS_VERSION
 MS_VERSION_NUM = _mapscript.MS_VERSION_NUM
 class rectObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
@@ -1772,15 +1739,14 @@
         else:
             raise TypeError('__contains__ does not yet handle %s' % (item_type))
 
 
 
 # Register rectObj in _mapscript:
 _mapscript.rectObj_swigregister(rectObj)
-
 class pointObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     x: "double" = property(_mapscript.pointObj_x_get, _mapscript.pointObj_x_set)
     y: "double" = property(_mapscript.pointObj_y_get, _mapscript.pointObj_y_set)
     z: "double" = property(_mapscript.pointObj_z_get, _mapscript.pointObj_z_set)
     m: "double" = property(_mapscript.pointObj_m_get, _mapscript.pointObj_m_set)
@@ -1833,15 +1799,14 @@
 
         return {"type": "Point", "coordinates": coords}
 
 
 
 # Register pointObj in _mapscript:
 _mapscript.pointObj_swigregister(pointObj)
-
 class lineObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numpoints: "int" = property(_mapscript.lineObj_numpoints_get)
 
     def __init__(self):
         _mapscript.lineObj_swiginit(self, _mapscript.new_lineObj())
@@ -1872,15 +1837,14 @@
 
         return {"type": "LineString", "coordinates": coords}
 
 
 
 # Register lineObj in _mapscript:
 _mapscript.lineObj_swigregister(lineObj)
-
 class shapeObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numlines: "int" = property(_mapscript.shapeObj_numlines_get)
     numvalues: "int" = property(_mapscript.shapeObj_numvalues_get)
     bounds: "rectObj" = property(_mapscript.shapeObj_bounds_get, _mapscript.shapeObj_bounds_set)
     type: "int" = property(_mapscript.shapeObj_type_get, _mapscript.shapeObj_type_set)
@@ -2098,18 +2062,14 @@
     def itemdefinitions(self, item_definitions):
         self._item_definitions = item_definitions
 
 
 
 # Register shapeObj in _mapscript:
 _mapscript.shapeObj_swigregister(shapeObj)
-
-def shapeObj_fromWKT(wkt: "char *") -> "shapeObj *":
-    return _mapscript.shapeObj_fromWKT(wkt)
-
 MS_NOERR = _mapscript.MS_NOERR
 MS_IOERR = _mapscript.MS_IOERR
 MS_MEMERR = _mapscript.MS_MEMERR
 MS_TYPEERR = _mapscript.MS_TYPEERR
 MS_SYMERR = _mapscript.MS_SYMERR
 MS_REGEXERR = _mapscript.MS_REGEXERR
 MS_TTFERR = _mapscript.MS_TTFERR
@@ -2170,15 +2130,14 @@
 
     def next(self) -> "errorObj *":
         return _mapscript.errorObj_next(self)
 
 # Register errorObj in _mapscript:
 _mapscript.errorObj_swigregister(errorObj)
 
-
 def msGetErrorObj() -> "errorObj *":
     return _mapscript.msGetErrorObj()
 
 def msResetErrorList() -> "void":
     return _mapscript.msResetErrorList()
 
 def msGetVersion() -> "char *":
@@ -2229,15 +2188,14 @@
 
     def __init__(self):
         _mapscript.DBFInfo_swiginit(self, _mapscript.new_DBFInfo())
     __swig_destroy__ = _mapscript.delete_DBFInfo
 
 # Register DBFInfo in _mapscript:
 _mapscript.DBFInfo_swigregister(DBFInfo)
-
 FTString = _mapscript.FTString
 FTInteger = _mapscript.FTInteger
 FTDouble = _mapscript.FTDouble
 FTInvalid = _mapscript.FTInvalid
 class shapefileObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -2271,15 +2229,14 @@
         return _mapscript.shapefileObj_addPoint(self, point)
 
     def getDBF(self) -> "DBFInfo *":
         return _mapscript.shapefileObj_getDBF(self)
 
 # Register shapefileObj in _mapscript:
 _mapscript.shapefileObj_swigregister(shapefileObj)
-
 wkp_none = _mapscript.wkp_none
 wkp_lonlat = _mapscript.wkp_lonlat
 wkp_gmerc = _mapscript.wkp_gmerc
 class projectionObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numargs: "int" = property(_mapscript.projectionObj_numargs_get)
@@ -2294,26 +2251,24 @@
         return _mapscript.projectionObj_setWKTProjection(self, wkt)
 
     def getUnits(self) -> "int":
         return _mapscript.projectionObj_getUnits(self)
 
 # Register projectionObj in _mapscript:
 _mapscript.projectionObj_swigregister(projectionObj)
-
 class reprojectionObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, _in: "projectionObj", out: "projectionObj"):
         _mapscript.reprojectionObj_swiginit(self, _mapscript.new_reprojectionObj(_in, out))
     __swig_destroy__ = _mapscript.delete_reprojectionObj
 
 # Register reprojectionObj in _mapscript:
 _mapscript.reprojectionObj_swigregister(reprojectionObj)
-
 MS_SYMBOL_SIMPLE = _mapscript.MS_SYMBOL_SIMPLE
 MS_SYMBOL_VECTOR = _mapscript.MS_SYMBOL_VECTOR
 MS_SYMBOL_ELLIPSE = _mapscript.MS_SYMBOL_ELLIPSE
 MS_SYMBOL_PIXMAP = _mapscript.MS_SYMBOL_PIXMAP
 MS_SYMBOL_TRUETYPE = _mapscript.MS_SYMBOL_TRUETYPE
 MS_SYMBOL_HATCH = _mapscript.MS_SYMBOL_HATCH
 MS_SYMBOL_SVG = _mapscript.MS_SYMBOL_SVG
@@ -2343,15 +2298,14 @@
         return _mapscript.colorObj_setHex(self, psHexColor)
 
     def toHex(self) -> "char *":
         return _mapscript.colorObj_toHex(self)
 
 # Register colorObj in _mapscript:
 _mapscript.colorObj_swigregister(colorObj)
-
 class symbolObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     refcount: "int" = property(_mapscript.symbolObj_refcount_get)
     numpoints: "int" = property(_mapscript.symbolObj_numpoints_get)
     imagepath: "char *" = property(_mapscript.symbolObj_imagepath_get)
     name: "char *" = property(_mapscript.symbolObj_name_get, _mapscript.symbolObj_name_set)
@@ -2388,15 +2342,14 @@
         return _mapscript.symbolObj_getImage(self, input_format)
 
     def setImage(self, image: "imageObj") -> "int":
         return _mapscript.symbolObj_setImage(self, image)
 
 # Register symbolObj in _mapscript:
 _mapscript.symbolObj_swigregister(symbolObj)
-
 MS_HASHSIZE = _mapscript.MS_HASHSIZE
 class hashTableObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     numitems: "int" = property(_mapscript.hashTableObj_numitems_get)
 
     def __init__(self):
@@ -2452,15 +2405,14 @@
 
         return keys
 
 
 
 # Register hashTableObj in _mapscript:
 _mapscript.hashTableObj_swigregister(hashTableObj)
-
 MS_CONFIG_SECTION = _mapscript.MS_CONFIG_SECTION
 MS_CONFIG_SECTION_ENV = _mapscript.MS_CONFIG_SECTION_ENV
 MS_CONFIG_SECTION_MAPS = _mapscript.MS_CONFIG_SECTION_MAPS
 MS_CONFIG_SECTION_PLUGINS = _mapscript.MS_CONFIG_SECTION_PLUGINS
 class configObj(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -2471,15 +2423,14 @@
     def __init__(self, filename: "char *"=None):
         _mapscript.configObj_swiginit(self, _mapscript.new_configObj(filename))
     __swig_destroy__ = _mapscript.delete_configObj
 
 # Register configObj in _mapscript:
 _mapscript.configObj_swigregister(configObj)
 
-
 def msLoadConfig(ms_config_file: "char const *") -> "configObj *":
     return _mapscript.msLoadConfig(ms_config_file)
 
 def msFreeConfig(config: "configObj") -> "void":
     return _mapscript.msFreeConfig(config)
 
 def msConfigGetEnv(config: "configObj", key: "char const *") -> "char const *":
@@ -2529,15 +2480,14 @@
 
     def getValueByName(self, name: "char const *") -> "char *":
         return _mapscript.OWSRequest_getValueByName(self, name)
 
 # Register OWSRequest in _mapscript:
 _mapscript.OWSRequest_swigregister(OWSRequest)
 
-
 def msConnPoolCloseUnreferenced() -> "void":
     return _mapscript.msConnPoolCloseUnreferenced()
 
 def msIO_resetHandlers() -> "void":
     return _mapscript.msIO_resetHandlers()
 
 def msIO_installStdoutToBuffer() -> "void":
@@ -2557,15 +2507,15 @@
 
 def msIO_getStdoutBufferBytes() -> "gdBuffer":
     return _mapscript.msIO_getStdoutBufferBytes()
 
 def msIO_getAndStripStdoutBufferMimeHeaders() -> "hashTableObj *":
     return _mapscript.msIO_getAndStripStdoutBufferMimeHeaders()
 
-def fromstring(data, mappath=None):
+def fromstring(data, mappath=None, configpath=None):
     """Creates map objects from mapfile strings.
 
     Parameters
     ==========
     data : string
         Mapfile in a string.
     mappath : string
@@ -2574,16 +2524,21 @@
     Example
     =======
     >>> mo = fromstring("MAP\nNAME 'test'\nEND")
     >>> mo.name
     'test'
     """
     import re
-    if re.search(r"^\s*MAP", data, re.I): 
-        return msLoadMapFromString(data, mappath)
+    if re.search(r"^\s*MAP", data, re.I):
+# create a config object if a path is supplied
+        if configpath:
+             config = configObj(configpath)
+        else:
+             config = None
+        return msLoadMapFromString(data, mappath, config)
     elif re.search(r"^\s*LAYER", data, re.I):
         ob = layerObj()
         ob.updateFromString(data)
         return ob
     elif re.search(r"^\s*CLASS", data, re.I):
         ob = classObj()
         ob.updateFromString(data)
@@ -2592,8 +2547,7 @@
         ob = styleObj()
         ob.updateFromString(data)
         return ob
     else:
         raise ValueError("No map, layer, class, or style found. Can not load from provided string")
 
 
-
```

### Comparing `mapscript-8.0.0/mapscript/tests/class_test.py` & `mapscript-8.0.1/mapscript/tests/class_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/clone_test.py` & `mapscript-8.0.1/mapscript/tests/clone_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/cluster_test.py` & `mapscript-8.0.1/mapscript/tests/cluster_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/color_test.py` & `mapscript-8.0.1/mapscript/tests/color_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/config_test.py` & `mapscript-8.0.1/mapscript/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/home.png` & `mapscript-8.0.1/mapscript/tests/data/home.png`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/mapserver-sample.conf` & `mapscript-8.0.1/mapscript/tests/data/mapserver-sample.conf`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/raster.tif` & `mapscript-8.0.1/mapscript/tests/data/raster.tif`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/test.map` & `mapscript-8.0.1/mapscript/tests/data/test.map`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/test.png` & `mapscript-8.0.1/mapscript/tests/data/test.png`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/test_nofontset.map` & `mapscript-8.0.1/mapscript/tests/data/test_nofontset.map`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/vera/COPYRIGHT.TXT` & `mapscript-8.0.1/mapscript/tests/data/vera/COPYRIGHT.TXT`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/vera/RELEASENOTES.TXT` & `mapscript-8.0.1/mapscript/tests/data/vera/RELEASENOTES.TXT`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/vera/Vera.ttf` & `mapscript-8.0.1/mapscript/tests/data/vera/Vera.ttf`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/vera/VeraBd.ttf` & `mapscript-8.0.1/mapscript/tests/data/vera/VeraBd.ttf`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/data/xmarks.png` & `mapscript-8.0.1/mapscript/tests/data/xmarks.png`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/font_test.py` & `mapscript-8.0.1/mapscript/tests/font_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/hash_test.py` & `mapscript-8.0.1/mapscript/tests/hash_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/image_test.py` & `mapscript-8.0.1/mapscript/tests/image_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/label_test.py` & `mapscript-8.0.1/mapscript/tests/label_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/layer_test.py` & `mapscript-8.0.1/mapscript/tests/layer_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/line_test.py` & `mapscript-8.0.1/mapscript/tests/line_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/map_test.py` & `mapscript-8.0.1/mapscript/tests/map_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/outputformat_test.py` & `mapscript-8.0.1/mapscript/tests/outputformat_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         num = self.map.numoutputformats
         new_format = mapscript.outputFormatObj('GDAL/GTiff', 'gtiffx')
         # assert new_format.refcount == 1, new_format.refcount
         self.map.appendOutputFormat(new_format)
         assert self.map.numoutputformats == num + 1
         # assert new_format.refcount == 2, new_format.refcount
         self.map.selectOutputFormat('gtiffx')
-        # self.map.save('testAppendNewOutputFormat.map')
+        self.map.save('testAppendNewOutputFormat.map')
         self.map.getLayerByName('INLINE-PIXMAP-RGBA').status = mapscript.MS_ON
         imgobj = self.map.draw()
         filename = 'testAppendNewOutputFormat.tif'
         imgobj.save(filename)
 
     def testRemoveOutputFormat(self):
         """testRemoveOutputFormat may fail depending on GD options"""
```

### Comparing `mapscript-8.0.0/mapscript/tests/ows_test.py` & `mapscript-8.0.1/mapscript/tests/ows_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,16 @@
     def testWFSPostRequest(self):
         """OWSRequestTestCase.testLoadWMSRequest: OWS can POST a WFS request"""
 
         self.map.web.metadata.set("ows_onlineresource", "http://dummy.org/")
         request = mapscript.OWSRequest()
         request.contenttype = "application/xml"
 
-        post_data = """<wfs:GetFeature xmlns:wfs="http://www.opengis.net/wfs" xmlns:ogc="http://www.opengis.net/ogc"
-        service="WFS" version="1.1.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
+        post_data = """<wfs:GetFeature xmlns:wfs="http://www.opengis.net/wfs" xmlns:ogc="http://www.opengis.net/ogc" service="WFS"
+        version="1.1.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
         <wfs:Query typeName="*:POINT" xmlns:feature="http://www.openplans.org/topp">
             <ogc:Filter>
                 <ogc:PropertyIsEqualTo>
                     <ogc:PropertyName>FID</ogc:PropertyName>
                     <ogc:Literal>1</ogc:Literal>
                 </ogc:PropertyIsEqualTo>
             </ogc:Filter>
```

### Comparing `mapscript-8.0.0/mapscript/tests/parentreference_test.py` & `mapscript-8.0.1/mapscript/tests/parentreference_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/pgtest.py` & `mapscript-8.0.1/mapscript/tests/pgtest.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/point_test.py` & `mapscript-8.0.1/mapscript/tests/point_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/rect_test.py` & `mapscript-8.0.1/mapscript/tests/rect_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/refcount_test.py` & `mapscript-8.0.1/mapscript/tests/refcount_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/resultcache_test.py` & `mapscript-8.0.1/mapscript/tests/resultcache_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/shape_test.py` & `mapscript-8.0.1/mapscript/tests/shape_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/shapefile_test.py` & `mapscript-8.0.1/mapscript/tests/shapefile_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/style_test.py` & `mapscript-8.0.1/mapscript/tests/style_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/symbol_test.py` & `mapscript-8.0.1/mapscript/tests/symbol_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/symbolset_test.py` & `mapscript-8.0.1/mapscript/tests/symbolset_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/testing.py` & `mapscript-8.0.1/mapscript/tests/testing.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/thread_test.py` & `mapscript-8.0.1/mapscript/tests/thread_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript/tests/zoom_test.py` & `mapscript-8.0.1/mapscript/tests/zoom_test.py`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/mapscript.egg-info/PKG-INFO` & `mapscript-8.0.1/mapscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapscript
-Version: 8.0.0
+Version: 8.0.1
 Summary: MapServer Python MapScript bindings
 Home-page: http://www.mapserver.org
 Author: Steve Lime
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mapscript-8.0.0/mapscript.egg-info/SOURCES.txt` & `mapscript-8.0.1/mapscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapscript-8.0.0/setup.py` & `mapscript-8.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         'Programming Language :: C++',
         'Topic :: Scientific/Engineering :: GIS',
         'Topic :: Scientific/Engineering :: Information Analysis',
     ],
     author = "Steve Lime",
     license = "MIT",
     url="http://www.mapserver.org",
-    version="8.0.0",
+    version="8.0.1",
     packages=find_packages(),
     package_data={
         # list the files to include starting with the most deeply nested folder or they are overwritten
         'mapscript': ['tests/data/vera/*.*', 'tests/data/*.*', '_mapscript.pyd']
         },
     distclass=BinaryDistribution
 )
```

