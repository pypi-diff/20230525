# Comparing `tmp/wise-pizza-0.1.4.tar.gz` & `tmp/wise-pizza-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.4.tar", last modified: Wed May 24 22:00:14 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.5.tar", last modified: Wed May 24 22:44:07 2023, max compression
```

## Comparing `wise-pizza-0.1.4.tar` & `wise-pizza-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:00:14.561309 wise-pizza-0.1.4/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-24 22:00:14.560954 wise-pizza-0.1.4/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/README.md
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-24 22:00:14.561385 wise-pizza-0.1.4/setup.cfg
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-24 21:49:13.000000 wise-pizza-0.1.4/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:00:14.549753 wise-pizza-0.1.4/wise_pizza/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11188 2023-05-24 21:35:26.000000 wise-pizza-0.1.4/wise_pizza/explain.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/find_alpha.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/make_matrix.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7499 2023-05-24 21:55:22.000000 wise-pizza-0.1.4/wise_pizza/plotting.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/segment_data.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/slicer.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/solver.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-24 21:09:58.000000 wise-pizza-0.1.4/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:00:14.560426 wise-pizza-0.1.4/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-24 22:00:14.000000 wise-pizza-0.1.4/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-24 22:00:14.000000 wise-pizza-0.1.4/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-24 22:00:14.000000 wise-pizza-0.1.4/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-24 22:00:14.000000 wise-pizza-0.1.4/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-24 22:00:14.000000 wise-pizza-0.1.4/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:44:07.935153 wise-pizza-0.1.5/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-24 22:44:07.934251 wise-pizza-0.1.5/PKG-INFO
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/README.md
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-24 22:44:07.935428 wise-pizza-0.1.5/setup.cfg
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-24 22:43:01.000000 wise-pizza-0.1.5/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:44:07.918951 wise-pizza-0.1.5/wise_pizza/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/__init__.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11404 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/explain.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/find_alpha.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/make_matrix.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/plotting.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/segment_data.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/slicer.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/solver.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:44:07.932758 wise-pizza-0.1.5/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.4/LICENSE` & `wise-pizza-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/PKG-INFO` & `wise-pizza-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.1.4/README.md` & `wise-pizza-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/setup.py` & `wise-pizza-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.4",
+    version="0.1.5",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.1.4/wise_pizza/explain.py` & `wise-pizza-0.1.5/wise_pizza/explain.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,19 +196,22 @@
             constrain_signs=constrain_signs,
             verbose=verbose,
         )
 
         sf_size.final_size = final_size
         sf_avg.final_size = final_size
         sp = SlicerPair(sf_size, sf_avg)
-        sp.plot = lambda width=2000, height=500: plot_split_segments(
-            sp.s1,
-            sp.s2,
-            width=width,
-            height=height,
+        sp.plot = (
+            lambda plot_is_static=True, width=2000, height=500: plot_split_segments(
+                sp.s1,
+                sp.s2,
+                plot_is_static=plot_is_static,
+                width=width,
+                height=height,
+            )
         )
         return sp
 
     else:
         sf = SliceFinder()
 
         sf.fit(
@@ -225,16 +228,16 @@
             constrain_signs=constrain_signs,
             verbose=verbose,
         )
 
         sf.pre_total = df1[total_name].sum()
         sf.post_total = df2[total_name].sum()
 
-        sf.plot = lambda width=1000, height=1000: plot_waterfall(
-            sf, width=width, height=height
+        sf.plot = lambda plot_is_static=True, width=1000, height=1000: plot_waterfall(
+            sf, plot_is_static=plot_is_static, width=width, height=height
         )
         sf.task = "changes in totals"
         return sf
 
 
 def explain_levels(
     df: pd.DataFrame,
@@ -297,12 +300,12 @@
     )
 
     for s in sf.segments:
         s["naive_avg"] += average
         s["total"] += average * s["seg_size"]
     # print(average)
     sf.reg.intercept_ = average
-    sf.plot = lambda width=2000, height=500: plot_segments(
-        sf, width=width, height=height
+    sf.plot = lambda plot_is_static=True, width=2000, height=500: plot_segments(
+        sf, plot_is_static=plot_is_static, width=width, height=height
     )
     sf.task = "levels"
     return sf
```

### Comparing `wise-pizza-0.1.4/wise_pizza/find_alpha.py` & `wise-pizza-0.1.5/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/wise_pizza/make_matrix.py` & `wise-pizza-0.1.5/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/wise_pizza/plotting.py` & `wise-pizza-0.1.5/wise_pizza/plotting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+from typing import Optional
+
 import plotly.graph_objects as go
 import plotly.io as pio
+from plotly.io import to_image
 from plotly.subplots import make_subplots
 
 from wise_pizza.slicer import SliceFinder
 
 pio.templates.default = "plotly_white"
 
 import numpy as np
 import pandas as pd
+from IPython.display import Image
 
 
 def plot_split_segments(
     sf_size: SliceFinder,
     sf_avg: SliceFinder,
+    plot_is_static: bool = False,
     width: int = 2000,
     height: int = 500,
 ):
     """
     Plot split segments for explain_changes: split_fits
     @param sf_size: SliceFinder from sizes
     @param sf_avg: SliceFinder from averages
+    @param denominator: denominator of the value
+    @param plot_is_static: static (True) or dynamic (False) plotly result
     @param width: parameter to modify the final width of the plot
     @param height: parameter to modify the final height of the plot
     """
     size_data = pd.DataFrame(sf_size.segments, index=np.array(sf_size.segment_labels))
     avg_data = pd.DataFrame(sf_avg.segments, index=np.array(sf_avg.segment_labels))
 
     size_average = sf_size.reg.intercept_
@@ -101,25 +108,38 @@
         col=2,
         row=2,
         annotation_text="Global average",
     )
 
     for i in range(1, 3):
         fig.update_yaxes(autorange="reversed", row=i)
-    fig.show()
+    if plot_is_static:
+        # Convert the figure to a static image
+        image_bytes = to_image(fig, format="png", scale=2)
+
+        # Display the static image in the Jupyter notebook
+        return Image(
+            image_bytes,
+            height=height + len(size_data.index) * 30,
+            width=width + len(size_data.index) * 30,
+        )
+    else:
+        fig.show()
 
 
 def plot_segments(
     sf: SliceFinder,
+    plot_is_static: bool = False,
     width: int = 2000,
     height: int = 500,
 ):
     """
     Plot segments for explain_levels
     @param sf: SliceFinder
+    @param plot_is_static: static (True) or dynamic (False) plotly result
     @param width: parameter to modify the final width of the plot
     @param height: parameter to modify the final height of the plot
     """
 
     seg_data = pd.DataFrame(sf.segments)
     seg_data["avg"] = seg_data["coef"] + sf.reg.intercept_
     seg_data.index = np.array(sf.segment_labels)
@@ -174,15 +194,27 @@
         x=average,
         line_width=3,
         line_dash="dash",
         line_color="red",
         col=2,
         annotation_text="Global average",
     )
-    fig.show()
+
+    if plot_is_static:
+        # Convert the figure to a static image
+        image_bytes = to_image(fig, format="png", scale=2)
+
+        # Display the static image in the Jupyter notebook
+        return Image(
+            image_bytes,
+            height=height + len(sf.segment_labels) * 30,
+            width=width + len(sf.segment_labels) * 30,
+        )
+    else:
+        fig.show()
 
 
 def waterfall_args(sf: SliceFinder):
     """
     Waterfall plot arguments
     @param sf: SliceFinder
     """
@@ -233,18 +265,21 @@
             "tickfont": {"size": tickfront_size},  # set font size of x-axis tick labels
         },
         "width": width,
         "height": height,
     }
 
 
-def plot_waterfall(sf: SliceFinder, width: int = 1000, height: int = 1000):
+def plot_waterfall(
+    sf: SliceFinder, plot_is_static: bool = False, width: int = 1000, height: int = 1000
+):
     """
     Plot waterfall and Bar for explain_changes
     @param sf: SliceFinder
+    @param plot_is_static: static (True) or dynamic (False) plotly result
     @param width: parameter to modify the final width of the plot
     @param height: parameter to modify the final height of the plot
     """
     assert hasattr(sf, "pre_total"), "Please call fit_change first"
     data = pd.DataFrame(sf.segments, index=np.array(sf.segment_labels))
     trace1 = go.Waterfall(name="Segments waterfall", **waterfall_args(sf))
 
@@ -269,8 +304,15 @@
 
     fig.update_layout(
         title="Segments contributing most to the change",
         #         showlegend = True,
         **waterfall_layout_args(sf, width, height)
     )
 
-    fig.show()
+    if plot_is_static:
+        # Convert the figure to a static image
+        image_bytes = to_image(fig, format="png", scale=2)
+
+        # Display the static image in the Jupyter notebook
+        return Image(image_bytes, width=width, height=height)
+    else:
+        fig.show()
```

### Comparing `wise-pizza-0.1.4/wise_pizza/segment_data.py` & `wise-pizza-0.1.5/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/wise_pizza/slicer.py` & `wise-pizza-0.1.5/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/wise_pizza/solver.py` & `wise-pizza-0.1.5/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/wise_pizza/utils.py` & `wise-pizza-0.1.5/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.4/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.5/wise_pizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

