# Comparing `tmp/feffery_leaflet_components-0.0.1a8.tar.gz` & `tmp/feffery_leaflet_components-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_leaflet_components-0.0.1a8.tar", last modified: Sat Dec 10 14:02:34 2022, max compression
+gzip compressed data, was "feffery_leaflet_components-0.0.1a9.tar", last modified: Wed Mar 15 09:14:27 2023, max compression
```

## Comparing `feffery_leaflet_components-0.0.1a8.tar` & `feffery_leaflet_components-0.0.1a9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-12-10 14:02:34.191621 feffery_leaflet_components-0.0.1a8/
--rw-rw-rw-   0        0        0     1085 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/LICENSE
--rw-rw-rw-   0        0        0      504 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/MANIFEST.in
--rw-rw-rw-   0        0        0      242 2022-12-10 14:02:34.191621 feffery_leaflet_components-0.0.1a8/PKG-INFO
--rw-rw-rw-   0        0        0     1989 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-10 14:02:34.174174 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/
--rw-rw-rw-   0        0        0     2554 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletAntPath.py
--rw-rw-rw-   0        0        0     2394 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletCircle.py
--rw-rw-rw-   0        0        0     2411 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletCircleMarker.py
--rw-rw-rw-   0        0        0     2209 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletExport.py
--rw-rw-rw-   0        0        0     1958 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletFeatureGroup.py
--rw-rw-rw-   0        0        0     2914 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletFlowLayer.py
--rw-rw-rw-   0        0        0     1744 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletFullscreenControl.py
--rw-rw-rw-   0        0        0     5706 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletGeoJSON.py
--rw-rw-rw-   0        0        0     2057 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletHeatMap.py
--rw-rw-rw-   0        0        0     1595 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletLayerGroup.py
--rw-rw-rw-   0        0        0     5147 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMap.py
--rw-rw-rw-   0        0        0     2317 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMapAction.py
--rw-rw-rw-   0        0        0     2166 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMapListener.py
--rw-rw-rw-   0        0        0     3232 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMarker.py
--rw-rw-rw-   0        0        0     3387 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMiniMap.py
--rw-rw-rw-   0        0        0     2537 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletPolygon.py
--rw-rw-rw-   0        0        0     2975 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletPolyline.py
--rw-rw-rw-   0        0        0     2351 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletPopup.py
--rw-rw-rw-   0        0        0     2386 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletRectangle.py
--rw-rw-rw-   0        0        0     2038 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletStaticHeatMap.py
--rw-rw-rw-   0        0        0     3763 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletSuperCluster.py
--rw-rw-rw-   0        0        0     1812 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletTileLayer.py
--rw-rw-rw-   0        0        0     2748 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletTileSelect.py
--rw-rw-rw-   0        0        0     2182 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletTooltip.py
--rw-rw-rw-   0        0        0     2614 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/__init__.py
--rw-rw-rw-   0        0        0     1746 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/_imports_.py
--rw-rw-rw-   0        0        0     7819 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/coloring_utils.py
--rw-rw-rw-   0        0        0   891731 2022-12-10 14:02:05.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/feffery_leaflet_components.min.js
--rw-rw-rw-   0        0        0      110 2022-12-10 14:02:05.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/feffery_leaflet_components.min.js.map
--rw-rw-rw-   0        0        0    14910 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/geometry_utils.py
--rw-rw-rw-   0        0        0   100532 2022-12-10 14:02:08.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/metadata.json
--rw-rw-rw-   0        0        0     3028 2022-12-10 14:02:07.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/package-info.json
-drwxrwxrwx   0        0        0        0 2022-12-10 14:02:34.189623 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/
--rw-rw-rw-   0        0        0      242 2022-12-10 14:02:34.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1802 2022-12-10 14:02:34.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-10 14:02:34.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-12-10 14:02:34.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-12-10 14:02:34.000000 feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3028 2022-12-10 13:26:48.000000 feffery_leaflet_components-0.0.1a8/package.json
--rw-rw-rw-   0        0        0       42 2022-12-10 14:02:34.192867 feffery_leaflet_components-0.0.1a8/setup.cfg
--rw-rw-rw-   0        0        0      559 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-15 09:14:27.808741 feffery_leaflet_components-0.0.1a9/
+-rw-rw-rw-   0        0        0     1085 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a9/LICENSE
+-rw-rw-rw-   0        0        0      504 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a9/MANIFEST.in
+-rw-rw-rw-   0        0        0      242 2023-03-15 09:14:27.808741 feffery_leaflet_components-0.0.1a9/PKG-INFO
+-rw-rw-rw-   0        0        0     1989 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-15 09:14:27.801421 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/
+-rw-rw-rw-   0        0        0     2554 2023-03-15 09:09:36.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletAntPath.py
+-rw-rw-rw-   0        0        0     2394 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletCircle.py
+-rw-rw-rw-   0        0        0     2411 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletCircleMarker.py
+-rw-rw-rw-   0        0        0     2209 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletExport.py
+-rw-rw-rw-   0        0        0     1958 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletFeatureGroup.py
+-rw-rw-rw-   0        0        0     2914 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletFlowLayer.py
+-rw-rw-rw-   0        0        0     1744 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletFullscreenControl.py
+-rw-rw-rw-   0        0        0     5706 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletGeoJSON.py
+-rw-rw-rw-   0        0        0     2057 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletHeatMap.py
+-rw-rw-rw-   0        0        0     1675 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletLayerGroup.py
+-rw-rw-rw-   0        0        0     5147 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMap.py
+-rw-rw-rw-   0        0        0     2317 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMapAction.py
+-rw-rw-rw-   0        0        0     2166 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMapListener.py
+-rw-rw-rw-   0        0        0     3232 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMarker.py
+-rw-rw-rw-   0        0        0     3387 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMiniMap.py
+-rw-rw-rw-   0        0        0     2537 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletPolygon.py
+-rw-rw-rw-   0        0        0     2975 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletPolyline.py
+-rw-rw-rw-   0        0        0     2351 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletPopup.py
+-rw-rw-rw-   0        0        0     2386 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletRectangle.py
+-rw-rw-rw-   0        0        0     2038 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletStaticHeatMap.py
+-rw-rw-rw-   0        0        0     3763 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletSuperCluster.py
+-rw-rw-rw-   0        0        0     1812 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletTileLayer.py
+-rw-rw-rw-   0        0        0     2748 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletTileSelect.py
+-rw-rw-rw-   0        0        0     2182 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletTooltip.py
+-rw-rw-rw-   0        0        0     2614 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/__init__.py
+-rw-rw-rw-   0        0        0     1746 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/_imports_.py
+-rw-rw-rw-   0        0        0     7819 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/coloring_utils.py
+-rw-rw-rw-   0        0        0   891887 2023-03-15 09:09:34.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/feffery_leaflet_components.min.js
+-rw-rw-rw-   0        0        0      110 2023-03-15 09:09:34.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/feffery_leaflet_components.min.js.map
+-rw-rw-rw-   0        0        0    14910 2022-12-08 08:31:30.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/geometry_utils.py
+-rw-rw-rw-   0        0        0   100673 2023-03-15 09:09:37.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/metadata.json
+-rw-rw-rw-   0        0        0     3028 2023-03-15 09:09:35.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-03-15 09:14:27.807585 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-03-15 09:14:27.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1802 2023-03-15 09:14:27.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-15 09:14:27.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-03-15 09:14:27.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-03-15 09:14:27.000000 feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3026 2023-03-15 09:12:47.000000 feffery_leaflet_components-0.0.1a9/package.json
+-rw-rw-rw-   0        0        0       42 2023-03-15 09:14:27.809751 feffery_leaflet_components-0.0.1a9/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-03-03 08:12:18.000000 feffery_leaflet_components-0.0.1a9/setup.py
```

### Comparing `feffery_leaflet_components-0.0.1a8/LICENSE` & `feffery_leaflet_components-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/README.md` & `feffery_leaflet_components-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletAntPath.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletAntPath.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletCircle.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletCircle.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletCircleMarker.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletCircleMarker.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletExport.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletExport.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletFeatureGroup.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletFeatureGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletFlowLayer.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletFlowLayer.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletFullscreenControl.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletFullscreenControl.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletGeoJSON.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletGeoJSON.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletHeatMap.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletHeatMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletLayerGroup.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletLayerGroup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 Keyword arguments:
 
 - children (a list of or a singular dash component, string or number; optional)
 
 - id (string; optional)
 
+- hidden (boolean; optional)
+
 - key (string; optional)
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
@@ -28,18 +30,18 @@
     - prop_name (string; optional):
         Holds which property is loading."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_leaflet_components'
     _type = 'LeafletLayerGroup'
     @_explicitize_args
-    def __init__(self, children=None, id=Component.UNDEFINED, key=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'key', 'loading_state']
+    def __init__(self, children=None, id=Component.UNDEFINED, key=Component.UNDEFINED, hidden=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'hidden', 'key', 'loading_state']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'key', 'loading_state']
+        self.available_properties = ['children', 'id', 'hidden', 'key', 'loading_state']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
         super(LeafletLayerGroup, self).__init__(children=children, **args)
```

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMap.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMapAction.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMapAction.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMapListener.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMapListener.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMarker.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMarker.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletMiniMap.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletMiniMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletPolygon.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletPolygon.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletPolyline.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletPolyline.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletPopup.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletPopup.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletRectangle.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletRectangle.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletStaticHeatMap.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletStaticHeatMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletSuperCluster.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletSuperCluster.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletTileLayer.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletTileLayer.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletTileSelect.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletTileSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/LeafletTooltip.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/LeafletTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/__init__.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/_imports_.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/coloring_utils.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/coloring_utils.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/feffery_leaflet_components.min.js` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/feffery_leaflet_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var e = function(t) {
                     return /\/_dash-component-suites\//.test(t.src)
                 }(i()),
                 n = o(t);
             if (!e) return n;
             var r = n.split("/"),
                 a = r.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_1-a8m1670680918"), r.splice(-1, 1, a.join(".")), r.join("/")
+            return a.splice(1, 0, "v0_0_1-a9m1678871367"), r.splice(-1, 1, a.join(".")), r.join("/")
         }
     }
     return n(n.s = 62)
 }([function(t, e) {
     t.exports = window.PropTypes
 }, function(t, e) {
     t.exports = window.React
@@ -27452,26 +27452,31 @@
                     layerContainer: r
                 })
             }
         })),
         Gn = function(t) {
             var e = t.id,
                 n = t.children,
-                o = t.loading_state,
-                a = (t.setProps, Object(r.useRef)(null));
-            return i.a.createElement(Fn, {
+                o = t.hidden,
+                a = t.loading_state,
+                s = (t.setProps, P()),
+                l = Object(r.useRef)(null);
+            return Object(r.useEffect)((function() {
+                l && s && !Object(S.isUndefined)(o) && (o ? s.removeLayer(l.current) : s.addLayer(l.current))
+            }), [o]), i.a.createElement(Fn, {
                 id: e,
-                ref: a,
-                "data-dash-is-loading": o && o.is_loading || void 0
+                ref: l,
+                "data-dash-is-loading": a && a.is_loading || void 0
             }, n)
         };
     Gn.propTypes = {
         id: a.a.string,
         key: a.a.string,
         children: a.a.node,
+        hidden: a.a.bool,
         loading_state: a.a.shape({
             is_loading: a.a.bool,
             prop_name: a.a.string,
             component_name: a.a.string
         }),
         setProps: a.a.func
     }, Gn.defaultProps = {};
```

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/geometry_utils.py` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/metadata.json` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222223%*

 * *Differences: {"'src/lib/components/LeafletLayerGroup.react.js'": "{'props': {'hidden': OrderedDict([('type', "*

 * *                                                    "OrderedDict([('name', 'bool')])), "*

 * *                                                    "('required', False), ('description', '')])}}"}*

```diff
@@ -1518,14 +1518,21 @@
             "children": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "node"
                 }
             },
+            "hidden": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
             "id": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
```

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components/package-info.json` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.1-a9'"}*

```diff
@@ -68,9 +68,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_leaflet_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.0.1-a8"
+    "version": "0.0.1-a9"
 }
```

### Comparing `feffery_leaflet_components-0.0.1a8/feffery_leaflet_components.egg-info/SOURCES.txt` & `feffery_leaflet_components-0.0.1a9/feffery_leaflet_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.0.1a8/package.json` & `feffery_leaflet_components-0.0.1a9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.1-a9'"}*

```diff
@@ -68,9 +68,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_leaflet_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.0.1-a8"
+    "version": "0.0.1-a9"
 }
```

### Comparing `feffery_leaflet_components-0.0.1a8/setup.py` & `feffery_leaflet_components-0.0.1a9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,14 @@
     version=package["version"],
     author=package['author'],
     packages=[package_name],
     include_package_data=True,
     license=package['license'],
     description=package.get('description', package_name),
     install_requires=[
-        'dm-tree>=0.1.7'
+        'dm-tree>=0.1.7',
+        'dash>=2.8.0'
     ],
     classifiers=[
         'Framework :: Dash',
     ],
 )
```

