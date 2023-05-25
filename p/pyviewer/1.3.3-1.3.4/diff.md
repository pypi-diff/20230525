# Comparing `tmp/pyviewer-1.3.3.tar.gz` & `tmp/pyviewer-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.3.3.tar", last modified: Tue Apr 25 04:55:05 2023, max compression
+gzip compressed data, was "pyviewer-1.3.4.tar", last modified: Thu May 25 01:59:06 2023, max compression
```

## Comparing `pyviewer-1.3.3.tar` & `pyviewer-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:55:05.646079 pyviewer-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-04-25 04:54:54.000000 pyviewer-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 04:55:05.646079 pyviewer-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-25 04:54:54.000000 pyviewer-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:55:05.646079 pyviewer-1.3.3/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (123)  3423528 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/MPLUSRounded1c-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    71936 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/roboto_mono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:55:05.646079 pyviewer-1.3.3/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:55:05.646079 pyviewer-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-25 04:54:54.000000 pyviewer-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:59:06.920392 pyviewer-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-25 01:58:57.000000 pyviewer-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 01:59:06.920392 pyviewer-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 01:58:57.000000 pyviewer-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:59:06.920392 pyviewer-1.3.4/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)  3423528 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/MPLUSRounded1c-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71936 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/roboto_mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-25 01:58:57.000000 pyviewer-1.3.4/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:59:06.920392 pyviewer-1.3.4/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 01:59:06.000000 pyviewer-1.3.4/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 01:59:06.000000 pyviewer-1.3.4/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:59:06.000000 pyviewer-1.3.4/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 01:59:06.000000 pyviewer-1.3.4/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 01:59:06.000000 pyviewer-1.3.4/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:59:06.920392 pyviewer-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 01:58:57.000000 pyviewer-1.3.4/setup.py
```

### Comparing `pyviewer-1.3.3/LICENSE` & `pyviewer-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.3/PKG-INFO` & `pyviewer-1.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.3
+Version: 1.3.4
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,9 +25,12 @@
 A viewer that shows ImGui UI elemets on the left, and a large image on the right. Runs in the main process, but supports visualizing torch tensors directly from GPU memory (unlike single_image_viewer).
 
 ## Other features
 * Bundles a custom build of PyImGui with plotting support (via ImPlot)
 * Dynamically rescalable user interface
 * Window resizing to integer multiple of content resolution
 
+## Installation
+`pip install pyviewer`
+
 ## Usage
 See `examples/demo.py` for a usage example.
```

### Comparing `pyviewer-1.3.3/README.md` & `pyviewer-1.3.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,9 +14,12 @@
 A viewer that shows ImGui UI elemets on the left, and a large image on the right. Runs in the main process, but supports visualizing torch tensors directly from GPU memory (unlike single_image_viewer).
 
 ## Other features
 * Bundles a custom build of PyImGui with plotting support (via ImPlot)
 * Dynamically rescalable user interface
 * Window resizing to integer multiple of content resolution
 
+## Installation
+`pip install pyviewer`
+
 ## Usage
-See `examples/demo.py` for a usage example.
+See `examples/demo.py` for a usage example.
```

### Comparing `pyviewer-1.3.3/pyviewer/MPLUSRounded1c-Medium.ttf` & `pyviewer-1.3.4/pyviewer/MPLUSRounded1c-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.3/pyviewer/gl_viewer.py` & `pyviewer-1.3.4/pyviewer/gl_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.3/pyviewer/imgui_themes.py` & `pyviewer-1.3.4/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.3/pyviewer/params.py` & `pyviewer-1.3.4/pyviewer/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import imgui
-from pyviewer.utils import enum_slider, combo_box_vals, slider_range_int, strict_dataclass
+from pyviewer.utils import enum_slider, combo_box_vals, slider_range_int, slider_range_float, strict_dataclass
 
 """ Small param wrappers for automatically creating UI widgets """
 
 class Param:
     def __init__(self, type, label: str, default_val, tooltip: str = None) -> None:
         self.type = type
         self.label = label
@@ -21,21 +21,21 @@
     def reset(self):
         self.value = self.default
 
     def draw(self):
         _, self.value = self.draw_widget()
         self.draw_tooltip()
 
-class RangeParam(Param):
+class _RangeParam(Param):
     def __init__(self, type, label, default_val, minval, maxval, tooltip: str = None) -> None:
         super().__init__(type, label, default_val, tooltip)
         self.min = minval
         self.max = maxval
 
-class Range2Param(Param):
+class _Range2Param(Param):
     def __init__(self, type, label, default_val, minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
         super().__init__(type, label, default_val, tooltip)
         self.min = minval
         self.max = maxval
         self.overlap = overlap  # allow v2 to go below v1?
 
 class EnumParam(Param):
@@ -57,15 +57,15 @@
 class BoolParam(Param):
     def __init__(self, label, default_val: bool, tooltip: str = None) -> None:
         super().__init__(bool, label, default_val, tooltip)
     
     def draw_widget(self):
         return imgui.checkbox(self.label, self.value)
 
-class IntParam(RangeParam):
+class IntParam(_RangeParam):
     def __init__(self, label, default_val: int, minval, maxval, buttons=False, tooltip: str = None) -> None:
         super().__init__(int, label, default_val, minval, maxval, tooltip)
         self.buttons = buttons
     
     def draw_widget(self):
         changed, val = imgui.slider_int(self.label, self.value, self.min, self.max)
         if self.buttons:
@@ -74,31 +74,41 @@
                 changed, val = (True, max(self.min, min(self.max, val - 1)))
             imgui.same_line()
             if imgui.button(f'>##{self.label}'):
                 changed, val = (True, max(self.min, min(self.max, val + 1)))
 
         return changed, val
 
-class Int2Param(Range2Param):
+class Int2Param(_Range2Param):
     def __init__(self, label, default_val: tuple[int], minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
         super().__init__(tuple[int], label, default_val, minval, maxval, overlap, tooltip)
     
     def draw_widget(self):
         if not self.overlap:
             return slider_range_int(*self.value, self.min, self.max, title=self.label)
         else:
             return imgui.slider_int2(self.label, *self.value, self.min, self.max)
 
-class FloatParam(RangeParam):
+class FloatParam(_RangeParam):
     def __init__(self, label, default_val: float, minval, maxval, tooltip: str = None) -> None:
         super().__init__(float, label, default_val, minval, maxval, tooltip)
     
     def draw_widget(self):
         return imgui.slider_float(self.label, self.value, self.min, self.max)
     
+class Float2Param(_Range2Param):
+    def __init__(self, label, default_val: tuple[float], minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
+        super().__init__(tuple[float], label, default_val, minval, maxval, overlap, tooltip)
+    
+    def draw_widget(self):
+        if not self.overlap:
+            return slider_range_float(*self.value, self.min, self.max, title=self.label)
+        else:
+            return imgui.slider_float2(self.label, *self.value, self.min, self.max)
+    
 ##########################################
 # Container that exposes raw values
 
 @strict_dataclass
 class ParamContainer:
     def __iter__(self):
         for attr, _ in self.__dataclass_fields__.items():
```

### Comparing `pyviewer-1.3.3/pyviewer/roboto_mono.ttf` & `pyviewer-1.3.4/pyviewer/roboto_mono.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.3/pyviewer/single_image_viewer.py` & `pyviewer-1.3.4/pyviewer/single_image_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 has_torch = False
 try:
     import torch
     has_torch = True
 except:
     pass
 
-from .gl_viewer import viewer
+from . import gl_viewer
 from .utils import begin_inline, normalize_image_data, PannableArea
 
 class ImgShape(ctypes.Structure):
     _fields_ = [('h', ctypes.c_uint), ('w', ctypes.c_uint), ('c', ctypes.c_uint)]
 class WindowSize(ctypes.Structure):
     _fields_ = [('w', ctypes.c_uint), ('h', ctypes.c_uint)]
 
@@ -111,15 +111,20 @@
         self._start()
 
     def close(self):
         self.should_quit.value = 1
         self.ui_process.join()
 
     def process_func(self):
-        v = viewer(self.title, swap_interval=int(self.vsync), hidden=self.hidden.value)
+        # Avoid double cuda init issues
+        # (single image viewer cannot use GPU memory anyway)
+        gl_viewer.has_pycuda = False
+        gl_viewer.cuda_synchronize = lambda : None
+        
+        v = gl_viewer.viewer(self.title, swap_interval=int(self.vsync), hidden=self.hidden.value)
         v._window_hidden = self.hidden.value
         v.set_interp_nearest()
         v.pan_handler = PannableArea()
         compute_thread = Thread(target=self.compute, args=[v])
 
         def set_glfw_callbacks(window):
             self.window_size_callback(window, *glfw.get_window_size(window)) # call once to set defaults
@@ -251,14 +256,15 @@
 # Single global instance
 # Removes need to pass variable around in code
 # Just call draw() (optionally call init first)
 inst: SingleImageViewer = None
 
 def init(*args, sync=True, **kwargs):
     global inst
+
     if inst is None:
         inst = SingleImageViewer(*args, **kwargs)
         if sync:
             inst.wait_for_startup() # if calling from debugger: need to give process time to start
 
 def draw(*, img_hwc=None, img_chw=None, ignore_pause=False):
     init('SIV') # no-op if init already performed
```

### Comparing `pyviewer-1.3.3/pyviewer/toolbar_viewer.py` & `pyviewer-1.3.4/pyviewer/toolbar_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.3/pyviewer/utils.py` & `pyviewer-1.3.4/pyviewer/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -399,14 +399,28 @@
         return ch, (min(s, e), max(s, e))
     elif s != v1:
         return ch, (min(s, e), e)
     elif e != v2:
         return ch, (s, max(s, e))
     else:
         return ch, (s, e)
+    
+# Float2 slider that prevents overlap
+def slider_range_float(v1, v2, vmin, vmax, push=False, title='', width=0.0):
+    with imgui_item_width(width):
+        ch, (s, e) = imgui.slider_float2(title, v1, v2, vmin, vmax)
+
+    if push:
+        return ch, (min(s, e), max(s, e))
+    elif s != v1:
+        return ch, (min(s, e), e)
+    elif e != v2:
+        return ch, (s, max(s, e))
+    else:
+        return ch, (s, e)
 
 # Shape batch as square if possible
 def get_grid_dims(B):
     if B == 0:
         return (0, 0)
     
     S = int(B**0.5 + 0.5)
```

### Comparing `pyviewer-1.3.3/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.3.4/pyviewer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.3
+Version: 1.3.4
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,9 +25,12 @@
 A viewer that shows ImGui UI elemets on the left, and a large image on the right. Runs in the main process, but supports visualizing torch tensors directly from GPU memory (unlike single_image_viewer).
 
 ## Other features
 * Bundles a custom build of PyImGui with plotting support (via ImPlot)
 * Dynamically rescalable user interface
 * Window resizing to integer multiple of content resolution
 
+## Installation
+`pip install pyviewer`
+
 ## Usage
 See `examples/demo.py` for a usage example.
```

### Comparing `pyviewer-1.3.3/setup.py` & `pyviewer-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import sys
 if 'develop' in sys.argv:
     print("WARNING: 'python setup.py develop' won't install \
         dependencies correctly, please use 'pip install -e .' instead.")
 
 setup(name='pyviewer',
-    version='1.3.3',
+    version='1.3.4',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
```

