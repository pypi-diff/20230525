# Comparing `tmp/onnx-predict-yolov8-1.0.4.tar.gz` & `tmp/onnx-predict-yolov8-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-predict-yolov8-1.0.4.tar", last modified: Wed May 24 13:20:11 2023, max compression
+gzip compressed data, was "onnx-predict-yolov8-1.0.5.tar", last modified: Thu May 25 08:18:31 2023, max compression
```

## Comparing `onnx-predict-yolov8-1.0.4.tar` & `onnx-predict-yolov8-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 13:20:11.658432 onnx-predict-yolov8-1.0.4/
--rw-rw-rw-   0        0        0     1096 2023-05-23 12:24:50.000000 onnx-predict-yolov8-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2467 2023-05-24 13:20:11.657436 onnx-predict-yolov8-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-05-24 08:47:57.000000 onnx-predict-yolov8-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 13:20:11.633282 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/
--rw-rw-rw-   0        0        0     2467 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 13:20:11.655423 onnx-predict-yolov8-1.0.4/opyv8/
--rw-rw-rw-   0        0        0       61 2023-05-23 09:27:35.000000 onnx-predict-yolov8-1.0.4/opyv8/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-05-24 09:41:37.000000 onnx-predict-yolov8-1.0.4/opyv8/model.py
--rw-rw-rw-   0        0        0     2501 2023-05-24 09:57:12.000000 onnx-predict-yolov8-1.0.4/opyv8/predictor.py
--rw-rw-rw-   0        0        0     2362 2023-05-24 09:57:28.000000 onnx-predict-yolov8-1.0.4/opyv8/utils.py
--rw-rw-rw-   0        0        0      629 2023-05-24 09:46:17.000000 onnx-predict-yolov8-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 13:20:11.658432 onnx-predict-yolov8-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 08:18:31.970624 onnx-predict-yolov8-1.0.5/
+-rw-rw-rw-   0        0        0     1096 2023-05-23 12:24:50.000000 onnx-predict-yolov8-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2467 2023-05-25 08:18:31.969594 onnx-predict-yolov8-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-05-24 08:47:57.000000 onnx-predict-yolov8-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 08:18:31.965144 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/
+-rw-rw-rw-   0        0        0     2467 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 08:18:31.968652 onnx-predict-yolov8-1.0.5/opyv8/
+-rw-rw-rw-   0        0        0       61 2023-05-23 09:27:35.000000 onnx-predict-yolov8-1.0.5/opyv8/__init__.py
+-rw-rw-rw-   0        0        0     1185 2023-05-24 09:41:37.000000 onnx-predict-yolov8-1.0.5/opyv8/model.py
+-rw-rw-rw-   0        0        0     2501 2023-05-24 09:57:12.000000 onnx-predict-yolov8-1.0.5/opyv8/predictor.py
+-rw-rw-rw-   0        0        0     2362 2023-05-24 09:57:28.000000 onnx-predict-yolov8-1.0.5/opyv8/utils.py
+-rw-rw-rw-   0        0        0      629 2023-05-25 08:17:31.000000 onnx-predict-yolov8-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 08:18:31.970624 onnx-predict-yolov8-1.0.5/setup.cfg
```

### Comparing `onnx-predict-yolov8-1.0.4/LICENSE` & `onnx-predict-yolov8-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.4/PKG-INFO` & `onnx-predict-yolov8-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-predict-yolov8
-Version: 1.0.4
+Version: 1.0.5
 Author-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>, Kristian Torp <torp@cs.aau.dk>
 Maintainer-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT License
         
         Copyright (c) 2023 Aalborg University
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://www.cs.aau.dk/
 Project-URL: repository, https://github.com/fromm1990/onnx-predict-yolov8
 Keywords: ONNX,YOLOv8,onnxruntime,vision
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ONNX-PREDICT-YOLOV8
 This repository is a light weight library to ease the use of ONNX models exported by the Ultralytics YOLOv8 framework.
 
 ## Example Usage
```

### Comparing `onnx-predict-yolov8-1.0.4/README.md` & `onnx-predict-yolov8-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/PKG-INFO` & `onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-predict-yolov8
-Version: 1.0.4
+Version: 1.0.5
 Author-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>, Kristian Torp <torp@cs.aau.dk>
 Maintainer-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT License
         
         Copyright (c) 2023 Aalborg University
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://www.cs.aau.dk/
 Project-URL: repository, https://github.com/fromm1990/onnx-predict-yolov8
 Keywords: ONNX,YOLOv8,onnxruntime,vision
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ONNX-PREDICT-YOLOV8
 This repository is a light weight library to ease the use of ONNX models exported by the Ultralytics YOLOv8 framework.
 
 ## Example Usage
```

### Comparing `onnx-predict-yolov8-1.0.4/opyv8/model.py` & `onnx-predict-yolov8-1.0.5/opyv8/model.py`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.4/opyv8/predictor.py` & `onnx-predict-yolov8-1.0.5/opyv8/predictor.py`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.4/opyv8/utils.py` & `onnx-predict-yolov8-1.0.5/opyv8/utils.py`

 * *Files identical despite different names*

