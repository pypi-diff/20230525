# Comparing `tmp/napari-hdf5-netcdf-viewer-0.0.2.tar.gz` & `tmp/napari-hdf5-netcdf-viewer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-hdf5-netcdf-viewer-0.0.2.tar", last modified: Wed Apr 12 02:28:28 2023, max compression
+gzip compressed data, was "napari-hdf5-netcdf-viewer-0.1.0.tar", last modified: Thu May 25 14:03:49 2023, max compression
```

## Comparing `napari-hdf5-netcdf-viewer-0.0.2.tar` & `napari-hdf5-netcdf-viewer-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.505597 napari-hdf5-netcdf-viewer-0.0.2/
--rw-rw-r--   0 yunhalee   (501) staff       (20)     1517 2022-10-28 18:43:40.000000 napari-hdf5-netcdf-viewer-0.0.2/LICENSE
--rw-r--r--   0 yunhalee   (501) staff       (20)       96 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.0.2/MANIFEST.in
--rw-r--r--   0 yunhalee   (501) staff       (20)      817 2023-04-12 02:28:28.505804 napari-hdf5-netcdf-viewer-0.0.2/PKG-INFO
--rw-rw-r--   0 yunhalee   (501) staff       (20)       84 2022-10-29 03:05:16.000000 napari-hdf5-netcdf-viewer-0.0.2/README.md
--rw-r--r--   0 yunhalee   (501) staff       (20)       91 2022-10-11 15:38:42.000000 napari-hdf5-netcdf-viewer-0.0.2/pyproject.toml
--rw-r--r--   0 yunhalee   (501) staff       (20)     1290 2023-04-12 02:28:28.506796 napari-hdf5-netcdf-viewer-0.0.2/setup.cfg
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.498484 napari-hdf5-netcdf-viewer-0.0.2/src/
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.501664 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/
--rw-r--r--   0 yunhalee   (501) staff       (20)      106 2022-10-28 18:32:59.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/__init__.py
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.505178 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/_tests/
--rw-r--r--   0 yunhalee   (501) staff       (20)        0 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/_tests/__init__.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      407 2023-04-11 23:50:14.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/_tests/test_quick_hdf5_netcdf_viewer.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      574 2023-04-11 23:39:29.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/napari.yaml
--rw-r--r--   0 yunhalee   (501) staff       (20)     9072 2023-04-11 23:43:19.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.504268 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/
--rw-r--r--   0 yunhalee   (501) staff       (20)      817 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yunhalee   (501) staff       (20)      635 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       84 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       92 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/requires.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       26 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.458721 napari-hdf5-netcdf-viewer-0.1.0/
+-rw-rw-r--   0 yunhalee   (501) staff       (20)     1517 2022-10-28 18:43:40.000000 napari-hdf5-netcdf-viewer-0.1.0/LICENSE
+-rw-r--r--   0 yunhalee   (501) staff       (20)       96 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.1.0/MANIFEST.in
+-rw-r--r--   0 yunhalee   (501) staff       (20)     1262 2023-05-25 14:03:49.458938 napari-hdf5-netcdf-viewer-0.1.0/PKG-INFO
+-rw-rw-r--   0 yunhalee   (501) staff       (20)      529 2023-05-25 13:53:44.000000 napari-hdf5-netcdf-viewer-0.1.0/README.md
+-rw-r--r--   0 yunhalee   (501) staff       (20)       91 2022-10-11 15:38:42.000000 napari-hdf5-netcdf-viewer-0.1.0/pyproject.toml
+-rw-r--r--   0 yunhalee   (501) staff       (20)     1306 2023-05-25 14:03:49.460310 napari-hdf5-netcdf-viewer-0.1.0/setup.cfg
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.451593 napari-hdf5-netcdf-viewer-0.1.0/src/
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.454766 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/
+-rw-r--r--   0 yunhalee   (501) staff       (20)      106 2022-10-28 18:32:59.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/__init__.py
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.458301 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/_tests/
+-rw-r--r--   0 yunhalee   (501) staff       (20)        0 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/_tests/__init__.py
+-rw-r--r--   0 yunhalee   (501) staff       (20)      407 2023-04-11 23:50:14.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/_tests/test_quick_hdf5_netcdf_viewer.py
+-rw-r--r--   0 yunhalee   (501) staff       (20)      574 2023-04-11 23:39:29.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/napari.yaml
+-rw-r--r--   0 yunhalee   (501) staff       (20)    14965 2023-05-24 16:27:25.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.457349 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/
+-rw-r--r--   0 yunhalee   (501) staff       (20)     1262 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yunhalee   (501) staff       (20)      635 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       84 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)      107 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/requires.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       26 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/top_level.txt
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.2/LICENSE` & `napari-hdf5-netcdf-viewer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-hdf5-netcdf-viewer-0.0.2/setup.cfg` & `napari-hdf5-netcdf-viewer-0.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-hdf5-netcdf-viewer
-version = 0.0.2
+version = 0.1.0
 description = A napari plugin for quick-viewing HDF5 and NetCDF files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yunhal/napari-hdf5-netcdf-viewer
 author = Yunha Lee
 author_email = yunha.lee.00@gmail.com
 classifiers = 
@@ -17,16 +17,17 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	h5py
 	netCDF4
-	pathlib
 	magicgui
+	shapely
+	napari_geojson
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/napari.yaml` & `napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py` & `napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import napari
 import h5py
+import netCDF4 as nc
 import numpy as np
 import pathlib
 from pathlib import Path
-
+import xarray as xr
 from magicgui import magicgui, magic_factory
-import netCDF4 as nc
+import sys
+from napari_geojson import napari_get_reader
+
 
 # potential file extensions: 
 H5_FILENAME_LIST = ['h5', 'hdf5', 'hdf']
 NETCDF_FILENAME_LIST = ['nc', 'netcdf', 'ncf', 'nc4']  
 
-
 class FileReader:
 
     def __init__(self, viewer):
         self.data_list = []
         self.viewer = viewer
 
     def print_h5_objs(self, name, obj):
@@ -81,61 +83,60 @@
 
             print(" =======", fn, " file structure end============")
             print("                                               ")
 
             # For netcdf, print(f) will do the same thing as above but it is not pretty. 
 
 
-    def h5_to_napari(self, fn):
+    def all_h5_to_napari(self, fn, h5_varname):
 
         """
         Parameters
         ----------
         fn : netcdf file path 
+        h5_varname : variable name
         """
 
         label_name = 'label'
         point_name = 'annotation'
 
         with h5py.File(fn,'r') as f:
 
-            for d in self.data_list:
-
-                var_path = str(d)
-                data = f[var_path]
-                np_data = np.array(data)
-
-                if hasattr(data, 'shape'):
-
-                    if data.ndim >= 2: 
-
-                        if (label_name.casefold() in var_path.casefold() ):
-                            # read as labels
-                            print("WARNING: label layer is determined, based on matching {} in the data path".format(label_name))
-                            layer = self.viewer.add_labels(np_data, name= var_path)
-
-                        elif (point_name.casefold() in var_path.casefold() ):
-                            # read as points
-                            print("WARNING: point layer is determined, based on matching {} in the data path".format(point_name))
-                            layer = self.viewer.add_points(np_data, name= var_path)
-                        else: 
-                            # read as image
-                            for key, val in data.attrs.items():
-                                if (key == "_FillValue" ): 
-                                    print("_FillValue exits", len(np_data [np_data == data.attrs["_FillValue"][0]]))
-                                    np_data [np_data == data.attrs["_FillValue"][0]] = np.nan
-                                    
-                                elif (key == "MissingValue" ): 
-                                    print("MissingValue exits", len(np_data [np_data == data.attrs["MissingValue"][0]]))
-                                    np_data [np_data == data.attrs["MissingValue"][0]] = np.nan
+            var_path = str(h5_varname)
+            data = f[var_path]
+            np_data = np.array(data)
+
+            if hasattr(data, 'shape'):
+
+                if data.ndim >= 2: 
+
+                    if (label_name.casefold() in var_path.casefold() ):
+                        # read as labels
+                        print("WARNING: label layer is determined, based on matching {} in the data path".format(label_name))
+                        layer = self.viewer.add_labels(np_data, name= var_path)
+
+                    elif (point_name.casefold() in var_path.casefold() ):
+                        # read as points
+                        print("WARNING: point layer is determined, based on matching {} in the data path".format(point_name))
+                        layer = self.viewer.add_points(np_data, name= var_path)
+                    else: 
+                        # read as image
+                        for key, val in data.attrs.items():
+                            if (key == "_FillValue" ): 
+                                print("_FillValue exits", len(np_data [np_data == data.attrs["_FillValue"][0]]))
+                                np_data [np_data == data.attrs["_FillValue"][0]] = np.nan
+                                
+                            elif (key == "MissingValue" ): 
+                                print("MissingValue exits", len(np_data [np_data == data.attrs["MissingValue"][0]]))
+                                np_data [np_data == data.attrs["MissingValue"][0]] = np.nan
 
-                            layer = self.viewer.add_image(np_data, name= var_path)
+                        layer = self.viewer.add_image(np_data, name= var_path)
 
 
-    def netcdf_to_napari(self, fn):
+    def all_netcdf_to_napari(self, fn):
 
         """
         Parameters
         ----------
         fn : netcdf file path 
         """
 
@@ -160,15 +161,148 @@
                         if 'missing_value' in data.ncattrs() :
                             mvalue = getattr(data, 'missing_value')
                             print ("missing_value was {} and is replaced with np.nan".format(mvalue))
                             np_data [np_data == mvalue] = np.nan
 
                         # read as image
                         layer = self.viewer.add_image(np_data, name= var_path)
+    
+
+    def get_geo_dataset(self, fn, xr_data):
+
+        """
+        Parameters
+        ----------
+        fn : h5netcdf file path 
+        xr_data : data variable name you want to visualize (e.g., "O3", "PM25")
+        """
+
+        file =xr.open_dataset(fn, engine="h5netcdf")
+
+        df = file[xr_data]
+        print("data has the following coords : ", df.coords)
+        # boolean variables to check the dimensions for NAPARI
+        LONG_EXIST = False
+        LAT_EXIST = False
+        VERT_EXIST = False
+
+        # get longitude coords
+        long_list =['lon', 'longitude', 'long', 'x','LON','LONGITUDE', 'LONG', 'X','XLONG']
+
+        for x in long_list:
+            
+            if(x in df.coords):
+
+                LONG_EXIST=True
+                longitude = df.coords[x].values
+                lon_atrib = df.coords[x].attrs
+                longitude_scale = (np.amax(longitude) - np.amin(longitude))/len(longitude)
+
+                print('original long is ', longitude[:10])
+                print(np.amin(longitude),np.amax(longitude)) 
+
+                if(np.amin(longitude) >= 0 and np.amax(longitude) > 180):
+                    print("longitude is shifting to 0 to -180")
+                    # This condition won't work well for regional cases
+
+                    # longitude is shifting from 0~360 to -180~180
+                    df.coords[x] = (df.coords[x] + 180) % 360 - 180
+                    df = df.sortby(df.lon)
+                    df.coords[x].attrs = lon_atrib
+                
+                    # overwrite with shifted longitude
+                    longitude = df.coords[x].values
+                
+                    print('shifted long is ', longitude[:10])
+                
+        # Xarray converts 'missing_values' and '_FillValue' to NaN as a default. 
+        if hasattr(df.attrs, 'fmissing_value'): 
+            fvalue = df.attrs['fmissing_value']
+            print ("fmissing_value was {} and is replaced with np.nan".format(fvalue))
+            print(np_data.shape, fvalue.shape)
+            np_data [np_data == fvalue] = np.nan
+
+        # get latitude coords
+        lat_list =['lat', 'latitude', 'y', 'LAT', 'LATITUDE', 'Y','XLAT']
+
+        for x in lat_list:
+            if(x in df.coords):
+                LAT_EXIST=True
+                latitude = df.coords[x].values
+                latitude_scale = (np.amax(latitude) - np.amin(latitude))/len(latitude)
+        #print('lat is ', latitude[:10]) 
+
+        # get vertical coords
+        lev_list =['lev', 'levels', 'level','vertical', 'height','altitude', 'pressure','ver']
+
+        for x in lev_list:
+            if(x in df.coords):
+                VERT_EXIST=True
+                vertical = df.coords[x].values
+                #print('lev is ', df.coords[x].values[:10])
+
+                vertical_scale = 5 # hard-coded number  
+
+                # first vertical layer to be near the groun
+                if(vertical[0] < vertical[-1]):
+                    df = df.sortby(x, ascending=False)
+        
+        # for WRF or CMAQ, it may fail to get lat and long information, so try this
+        if (LONG_EXIST == False) or (LAT_EXIST == False):
+            print("Either Longitute or Latitude is available: LONG_EXIST {}; LAT_EXIST {}".format(LONG_EXIST, LAT_EXIST) )
+            print("Current version may not work for WRF, WRF-Chem, and CMAQ model outputs")
+            sys.exit("geo coords is not available")
+        
+
+        np_data = np.asarray(df.values)
+        print(xr_data, df.attrs)
+
+        from napari.layers import Shapes
+
+        my_shapes = [layer for layer in self.viewer.layers if isinstance(layer, Shapes)]
+        print(my_shapes)
+
+        if "Country borders" not in str(my_shapes): 
+            worldmap, world_shape_type = get_world_geojson()
+            shape_layer = self.viewer.add_shapes(worldmap, name = "Country borders", shape_type=world_shape_type, edge_width = 0)
+            if (LONG_EXIST == True) and (LAT_EXIST == True) and (VERT_EXIST == False ):
+                print("latitude array has been inversed for napari visualization")
+                set_scale_at_axis(shape_layer, axis=-2, value=-1)
+
+        if (LONG_EXIST == True) and (LAT_EXIST == True) and (VERT_EXIST == False ):
+            
+            print("latitude array has been inversed for napari visualization")
+
+            layer = self.viewer.add_image(np_data, name= xr_data)
+            
+            self.viewer.dims.axis_labels = ("lat", "lon") 
+            layer.colormap = 'hsv'
+            layer.opacity = 0.5
+            layer.scale = (1, latitude_scale*-1, longitude_scale)
+            layer.translate  = (0, 90, 0)
+            
+
+        if (LONG_EXIST == True) and (LAT_EXIST == True) and (VERT_EXIST == True ):
+            layer = self.viewer.add_image(np_data, name= xr_data)
+            self.viewer.dims.axis_labels = ("height", "lat", "lon") 
+            layer.colormap = 'hsv'
+            layer.opacity = 0.5
+            self.viewer.dims.ndisplay = 3
+            self.viewer.camera.angles = (-1.7571935971733401, -26.823353526707475, -77.73048528666025)
+            layer.translate  = (0, 0, -90, 0)
+            layer.scale = (1, vertical_scale, latitude_scale, longitude_scale)
+
+def get_world_geojson():
+
+    # Set the domain for defining the plot region.
+    fname= "/Users/yunhalee/Desktop/Napari/napari-geo-worldmap/world_0_360.geojson"
+    reader = napari_get_reader(fname)
+    layer_data = reader(fname)
 
+    return layer_data[0][0], layer_data[0][1]["shape_type"]
 
 def set_scale_at_axis(layer, axis=0, value=1):
 
     """
     Parameters
     ----------
     layer : napari image layer 
@@ -177,84 +311,87 @@
     value : value assigned to the axis (e.g., -1 for flipping along the axis; 2 to increase the axis' physical scale)
     """
 
     curr_scale = layer.scale
     curr_scale[axis] = value
     layer.scale = curr_scale
 
+def load_path(viewer, path: str):
 
-'''
-need to update in future
-
-def geo_view_enabled (data):
-
-    if (data.ndim == 2):
-        print("latitude array has been inversed for napari visualization")
-        set_scale_at_axis(layer, axis = -2, value = -1)
-
-    if (data.ndim >= 3):
-        set_scale_at_axis(layer, axis = -2, value = -1)
-        viewer.dims.axis_labels = ("height", "lat", "lon") 
-        viewer.dims.ndisplay = 3
-        viewer.camera.angles = (-1.7571935971733401, -26.823353526707475, -77.73048528666025)
-
-'''
-
-def load_path(path: str):
-
-    """read file structure and open the images with napari if the path file format is hdf or netcdf.
+    """print the file structure and create a list of data to pass to the napari.
     Parameters
     ----------
+    viewer - napari viewer
     path: str
         hdf5 or netcdf file path
     -------
     """
 
-    viewer = napari.Viewer()
-    viewer.axes.visible = True
-
     plugin = FileReader(viewer)
 
+    # print the file structure and create the data list for napari
     if path.endswith(tuple(H5_FILENAME_LIST)) :
         with h5py.File(path,'r') as f:
             print("                                               ")
             print(" =======", path, " file structure start =========")
 
             f.visititems(plugin.print_h5_objs)
 
             print(" =======", path, " file structure end============")
             print("                                               ")
-        plugin.h5_to_napari(path)
-    
+        # turn off plugin.all_h5_to_napari(path)
     # check if a netcdf file
     elif path.endswith(tuple(NETCDF_FILENAME_LIST)) :
         print("                                               ")
         print(" =======", path, " file structure start =========")   
 
         plugin.print_netcdf(path)
 
         print(" =======", path, " file structure end============")
         print("                                               ")
-
-        plugin.netcdf_to_napari(path)
-    
+        # turn off plugin.all_netcdf_to_napari(path)
     # file is not either h5 or netcdf
     else:
         print("Failure: {} is recognized as neither hdf5 nor netcdf".format(path))
+        sys.exit("Not acceptable files")
 
-@magic_factory
-def make_widget(file_path: "pathlib.Path" = Path()):
-    filename = str(file_path)
-    load_path(filename)
+    return plugin.data_list
 
+def data_to_napari(viewer, path: str):
+    """read the data arrays and visualized with napari.
+    Parameters
+    ----------
+    viewer: napari viewer
+    path: str
+        hdf5 or netcdf file path
+    -------
+    """
+    plugin = FileReader(viewer)
 
-if __name__ == "__main__":
+    data_list = load_path(viewer, path)
+
+    @magic_factory (dropdown={"choices": data_list})
+    def make_widget_dropdown(dropdown=data_list[0]):
 
-    fpath = '/Users/yunhalee/nc_h5_files/OMI-Aura_L3-OMTO3e_2005m1214_v002-2006m0929t143855.h5'
+        varname = str(dropdown)
+        print(f"varname {varname}")
+
+        # HDF seems not to work well with Xarray (to get dimensions), so for now only simple visualization is used 
+        if path.endswith(tuple(H5_FILENAME_LIST)) :
+            plugin.all_h5_to_napari(path, varname)
+        else: 
+            plugin.get_geo_dataset(path, varname)
+
+    viewer.window.add_dock_widget(make_widget_dropdown(), area="right") 
+
+@magic_factory ()
+def make_widget(viewer: "napari.viewer.Viewer", file_path: "pathlib.Path" = Path()):
+    filename = str(file_path)
+    load_path(viewer, filename)
+    data_to_napari(viewer, filename)
+
+if __name__ == "__main__":
 
     viewer = napari.Viewer()
     viewer.window.add_dock_widget(make_widget(), area="right")  
 
     napari.run()
-
-    load_path(fpath)
-
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt` & `napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

