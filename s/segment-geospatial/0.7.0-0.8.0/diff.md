# Comparing `tmp/segment-geospatial-0.7.0.tar.gz` & `tmp/segment-geospatial-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.7.0.tar", last modified: Sun May 21 02:28:41 2023, max compression
+gzip compressed data, was "segment-geospatial-0.8.0.tar", last modified: Wed May 24 04:08:45 2023, max compression
```

## Comparing `segment-geospatial-0.7.0.tar` & `segment-geospatial-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71643 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/samgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/text_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-21 02:28:41.677598 segment-geospatial-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82805 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/setup.py
```

### Comparing `segment-geospatial-0.7.0/LICENSE` & `segment-geospatial-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.7.0/PKG-INFO` & `segment-geospatial-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.7.0
+Version: 0.8.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -38,26 +38,28 @@
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
--   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
--   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/input_prompts)
+-   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
@@ -69,16 +71,22 @@
 
 ![](https://i.imgur.com/Cb4ZaKY.gif)
 
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
+-   Automatic mask generation
+
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+-   Using SAM with ArcGIS Pro
+
+[![Alt text](https://img.youtube.com/vi/VvyInoQ6N8Q/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Using SAM with Desktop GIS
 
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
 
@@ -87,7 +95,9 @@
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
+-   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
+-   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.7.0/README.md` & `segment-geospatial-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
--   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
--   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/input_prompts)
+-   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
@@ -47,16 +49,22 @@
 
 ![](https://i.imgur.com/Cb4ZaKY.gif)
 
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
+-   Automatic mask generation
+
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+-   Using SAM with ArcGIS Pro
+
+[![Alt text](https://img.youtube.com/vi/VvyInoQ6N8Q/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Using SAM with Desktop GIS
 
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
 
@@ -65,7 +73,9 @@
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
+-   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
+-   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.7.0/samgeo/common.py` & `segment-geospatial-0.8.0/samgeo/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1915,15 +1915,15 @@
         except (TypeError, KeyError) as e:
             print(f"Error handling map interaction: {e}")
 
     m.on_interaction(handle_map_interaction)
 
     def segment_button_click(change):
         if change["new"]:
-            reset_button.value = False
+            segment_button.value = False
             with output:
                 output.clear_output()
                 if len(m.fg_markers) == 0:
                     print("Please add some foreground markers.")
                     segment_button.value = False
                     return
 
@@ -2181,7 +2181,346 @@
     # Wait for a key press to exit
     cv2.waitKey(0)
 
     # Destroy the window
     cv2.destroyAllWindows()
 
     return left_clicks, right_clicks
+
+
+def install_package(package):
+    """Install a Python package.
+
+    Args:
+        package (str | list): The package name or a GitHub URL or a list of package names or GitHub URLs.
+    """
+    import subprocess
+
+    if isinstance(package, str):
+        packages = [package]
+
+    for package in packages:
+        if package.startswith("https://github.com"):
+            package = f"git+{package}"
+
+        # Execute pip install command and show output in real-time
+        command = f"pip install {package}"
+        process = subprocess.Popen(command.split(), stdout=subprocess.PIPE)
+
+        # Print output in real-time
+        while True:
+            output = process.stdout.readline()
+            if output == b"" and process.poll() is not None:
+                break
+            if output:
+                print(output.decode("utf-8").strip())
+
+        # Wait for process to complete
+        process.wait()
+
+
+def text_sam_gui(sam, basemap="SATELLITE", out_dir=None, **kwargs):
+    """Display the SAM Map GUI.
+
+    Args:
+        sam (SamGeo):
+        basemap (str, optional): The basemap to use. Defaults to "SATELLITE".
+        out_dir (str, optional): The output directory. Defaults to None.
+
+    """
+    try:
+        import shutil
+        import tempfile
+        import leafmap
+        import ipyleaflet
+        import ipyevents
+        import ipywidgets as widgets
+        import leafmap.colormaps as cm
+        from ipyfilechooser import FileChooser
+    except ImportError:
+        raise ImportError(
+            "The sam_map function requires the leafmap package. Please install it first."
+        )
+
+    if out_dir is None:
+        out_dir = tempfile.gettempdir()
+
+    m = leafmap.Map(**kwargs)
+    m.default_style = {"cursor": "crosshair"}
+    m.add_basemap(basemap, show=False)
+
+    # Skip the image layer if localtileserver is not available
+    try:
+        m.add_raster(sam.source, layer_name="Image")
+    except:
+        pass
+
+    widget_width = "280px"
+    button_width = "90px"
+    padding = "0px 4px 0px 4px"  # upper, right, bottom, left
+    style = {"description_width": "initial"}
+
+    toolbar_button = widgets.ToggleButton(
+        value=True,
+        tooltip="Toolbar",
+        icon="gear",
+        layout=widgets.Layout(width="28px", height="28px", padding="0px 0px 0px 4px"),
+    )
+
+    close_button = widgets.ToggleButton(
+        value=False,
+        tooltip="Close the tool",
+        icon="times",
+        button_style="primary",
+        layout=widgets.Layout(height="28px", width="28px", padding="0px 0px 0px 4px"),
+    )
+
+    text_prompt = widgets.Text(
+        description="Text prompt:",
+        style=style,
+        layout=widgets.Layout(width=widget_width, padding=padding),
+    )
+
+    box_slider = widgets.FloatSlider(
+        description="Box threshold:",
+        min=0,
+        max=1,
+        value=0.5,
+        step=0.01,
+        readout=True,
+        continuous_update=True,
+        layout=widgets.Layout(width=widget_width, padding=padding),
+        style=style,
+    )
+
+    text_slider = widgets.FloatSlider(
+        description="Text threshold:",
+        min=0,
+        max=1,
+        step=0.01,
+        value=0.5,
+        readout=True,
+        continuous_update=True,
+        layout=widgets.Layout(width=widget_width, padding=padding),
+        style=style,
+    )
+
+    cmap_dropdown = widgets.Dropdown(
+        description="Palette:",
+        options=cm.list_colormaps(),
+        value="viridis",
+        style=style,
+        layout=widgets.Layout(width=widget_width, padding=padding),
+    )
+
+    opacity_slider = widgets.FloatSlider(
+        description="Opacity:",
+        min=0,
+        max=1,
+        value=0.5,
+        readout=True,
+        continuous_update=True,
+        layout=widgets.Layout(width=widget_width, padding=padding),
+        style=style,
+    )
+
+    def opacity_changed(change):
+        if change["new"]:
+            if hasattr(m, "layer_name"):
+                mask_layer = m.find_layer(m.layer_name)
+                if mask_layer is not None:
+                    mask_layer.interact(opacity=opacity_slider.value)
+
+    opacity_slider.observe(opacity_changed, "value")
+
+    segment_button = widgets.ToggleButton(
+        description="Segment",
+        value=False,
+        button_style="primary",
+        layout=widgets.Layout(padding=padding),
+    )
+
+    save_button = widgets.ToggleButton(
+        description="Save", value=False, button_style="primary"
+    )
+
+    reset_button = widgets.ToggleButton(
+        description="Reset", value=False, button_style="primary"
+    )
+    segment_button.layout.width = button_width
+    save_button.layout.width = button_width
+    reset_button.layout.width = button_width
+
+    output = widgets.Output(
+        layout=widgets.Layout(
+            width=widget_width, padding=padding, max_width=widget_width
+        )
+    )
+
+    toolbar_header = widgets.HBox()
+    toolbar_header.children = [close_button, toolbar_button]
+    toolbar_footer = widgets.VBox()
+    toolbar_footer.children = [
+        text_prompt,
+        box_slider,
+        text_slider,
+        cmap_dropdown,
+        opacity_slider,
+        widgets.HBox(
+            [segment_button, save_button, reset_button],
+            layout=widgets.Layout(padding="0px 4px 0px 4px"),
+        ),
+        output,
+    ]
+    toolbar_widget = widgets.VBox()
+    toolbar_widget.children = [toolbar_header, toolbar_footer]
+
+    toolbar_event = ipyevents.Event(
+        source=toolbar_widget, watched_events=["mouseenter", "mouseleave"]
+    )
+
+    def handle_toolbar_event(event):
+        if event["type"] == "mouseenter":
+            toolbar_widget.children = [toolbar_header, toolbar_footer]
+        elif event["type"] == "mouseleave":
+            if not toolbar_button.value:
+                toolbar_widget.children = [toolbar_button]
+                toolbar_button.value = False
+                close_button.value = False
+
+    toolbar_event.on_dom_event(handle_toolbar_event)
+
+    def toolbar_btn_click(change):
+        if change["new"]:
+            close_button.value = False
+            toolbar_widget.children = [toolbar_header, toolbar_footer]
+        else:
+            if not close_button.value:
+                toolbar_widget.children = [toolbar_button]
+
+    toolbar_button.observe(toolbar_btn_click, "value")
+
+    def close_btn_click(change):
+        if change["new"]:
+            toolbar_button.value = False
+            if m.toolbar_control in m.controls:
+                m.remove_control(m.toolbar_control)
+            toolbar_widget.close()
+
+    close_button.observe(close_btn_click, "value")
+
+    def segment_button_click(change):
+        if change["new"]:
+            segment_button.value = False
+            with output:
+                output.clear_output()
+                if len(text_prompt.value) == 0:
+                    print("Please enter a text prompt first.")
+                elif sam.source is None:
+                    print("Please run sam.set_image() first.")
+                else:
+                    print("Segmenting...")
+                    layer_name = text_prompt.value.replace(" ", "_")
+                    filename = os.path.join(
+                        out_dir, f"{layer_name}_{random_string()}.tif"
+                    )
+                    sam.predict(
+                        sam.source,
+                        text_prompt.value,
+                        box_slider.value,
+                        text_slider.value,
+                        output=filename,
+                    )
+                    sam.output = filename
+                    if m.find_layer(layer_name) is not None:
+                        m.remove_layer(m.find_layer(layer_name))
+                    if os.path.exists(filename):
+                        try:
+                            m.add_raster(
+                                filename,
+                                layer_name=layer_name,
+                                palette=cmap_dropdown.value,
+                                opacity=opacity_slider.value,
+                                nodata=0,
+                                zoom_to_layer=False,
+                            )
+                            m.layer_name = layer_name
+                            output.clear_output()
+                        except Exception as e:
+                            print(e)
+
+    segment_button.observe(segment_button_click, "value")
+
+    def filechooser_callback(chooser):
+        with output:
+            if chooser.selected is not None:
+                try:
+                    filename = chooser.selected
+                    shutil.copy(sam.output, filename)
+                    vector = filename.replace(".tif", ".shp")
+                    raster_to_vector(filename, vector)
+
+                except Exception as e:
+                    print(e)
+
+                if hasattr(m, "save_control") and m.save_control in m.controls:
+                    m.remove_control(m.save_control)
+                    delattr(m, "save_control")
+                save_button.value = False
+
+    def save_button_click(change):
+        if change["new"]:
+            with output:
+                output.clear_output()
+                if not hasattr(m, "layer_name"):
+                    print("Please click the Segment button first.")
+                else:
+                    sandbox_path = os.environ.get("SANDBOX_PATH")
+                    filechooser = FileChooser(
+                        path=os.getcwd(),
+                        filename=f"{m.layer_name}.tif",
+                        sandbox_path=sandbox_path,
+                        layout=widgets.Layout(width="454px"),
+                    )
+                    filechooser.use_dir_icons = True
+                    filechooser.filter_pattern = ["*.tif"]
+                    filechooser.register_callback(filechooser_callback)
+                    save_control = ipyleaflet.WidgetControl(
+                        widget=filechooser, position="topright"
+                    )
+                    m.add_control(save_control)
+                    m.save_control = save_control
+
+        else:
+            if hasattr(m, "save_control") and m.save_control in m.controls:
+                m.remove_control(m.save_control)
+                delattr(m, "save_control")
+
+    save_button.observe(save_button_click, "value")
+
+    def reset_button_click(change):
+        if change["new"]:
+            segment_button.value = False
+            save_button.value = False
+            reset_button.value = False
+            opacity_slider.value = 0.5
+            box_slider.value = 0.5
+            text_slider.value = 0.5
+            cmap_dropdown.value = "viridis"
+            text_prompt.value = ""
+            output.clear_output()
+            try:
+                if hasattr(m, "layer_name") and m.find_layer(m.layer_name) is not None:
+                    m.remove_layer(m.find_layer(m.layer_name))
+                m.clear_drawings()
+            except:
+                pass
+
+    reset_button.observe(reset_button_click, "value")
+
+    toolbar_control = ipyleaflet.WidgetControl(
+        widget=toolbar_widget, position="topright"
+    )
+    m.add_control(toolbar_control)
+    m.toolbar_control = toolbar_control
+
+    return m
```

### Comparing `segment-geospatial-0.7.0/samgeo/samgeo.py` & `segment-geospatial-0.8.0/samgeo/samgeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,24 @@
                 crop_n_points_downscale_factor: int = 1,
                 point_grids: Optional[List[np.ndarray]] = None,
                 min_mask_region_area: int = 0,
                 output_mode: str = "binary_mask",
 
         """
         # Download the checkpoint if it does not exist
+        CACHE_PATH = os.environ.get(
+            "TORCH_HOME", os.path.expanduser("~/.cache/torch/hub/checkpoints")
+        )
         if not os.path.exists(checkpoint):
-            print(f"Checkpoint {checkpoint} does not exist.")
-            download_checkpoint(output=checkpoint)
+            basename = os.path.basename(checkpoint)
+            checkpoint = os.path.join(CACHE_PATH, basename)
+            if not os.path.exists(checkpoint):
+                print(f"Checkpoint {checkpoint} does not exist.")
+                download_checkpoint(output=checkpoint)
+        self.checkpoint = checkpoint
 
         # Use cuda if available
         if device is None:
             device = "cuda" if torch.cuda.is_available() else "cpu"
             if device == "cuda":
                 torch.cuda.empty_cache()
 
@@ -593,14 +600,26 @@
     def image_to_image(self, image, **kwargs):
         return image_to_image(image, self, **kwargs)
 
     def download_tms_as_tiff(self, source, pt1, pt2, zoom, dist):
         image = draw_tile(source, pt1[0], pt1[1], pt2[0], pt2[1], zoom, dist)
         return image
 
+    def raster_to_vector(self, image, output, simplify_tolerance=None, **kwargs):
+        """Save the result to a vector file.
+
+        Args:
+            image (str): The path to the image file.
+            output (str): The path to the vector file.
+            simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+                The higher this value, the smaller the number of vertices in the resulting geometry.
+        """
+
+        raster_to_vector(image, output, simplify_tolerance=simplify_tolerance, **kwargs)
+
     def tiff_to_vector(self, tiff_path, output, simplify_tolerance=None, **kwargs):
         """Convert a tiff file to a gpkg file.
 
         Args:
             tiff_path (str): The path to the tiff file.
             output (str): The path to the vector file.
             simplify_tolerance (float, optional): The maximum allowed geometry displacement.
```

### Comparing `segment-geospatial-0.7.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.8.0/segment_geospatial.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.7.0
+Version: 0.8.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -38,26 +38,28 @@
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
--   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
--   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/input_prompts)
+-   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
@@ -69,16 +71,22 @@
 
 ![](https://i.imgur.com/Cb4ZaKY.gif)
 
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
+-   Automatic mask generation
+
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+-   Using SAM with ArcGIS Pro
+
+[![Alt text](https://img.youtube.com/vi/VvyInoQ6N8Q/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Using SAM with Desktop GIS
 
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
 
@@ -87,7 +95,9 @@
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
+-   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
+-   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.7.0/setup.py` & `segment-geospatial-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.7.0',
+    version='0.8.0',
     zip_safe=False,
 )
```

