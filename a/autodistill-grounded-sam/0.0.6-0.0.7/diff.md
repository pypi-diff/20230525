# Comparing `tmp/autodistill_grounded_sam-0.0.6.tar.gz` & `tmp/autodistill_grounded_sam-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_grounded_sam-0.0.6.tar", last modified: Thu May 18 20:24:13 2023, max compression
+gzip compressed data, was "autodistill_grounded_sam-0.0.7.tar", last modified: Thu May 25 17:56:31 2023, max compression
```

## Comparing `autodistill_grounded_sam-0.0.6.tar` & `autodistill_grounded_sam-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 20:24:13.346884 autodistill_grounded_sam-0.0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      646 2023-05-18 20:24:13.346884 autodistill_grounded_sam-0.0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-05-18 16:28:39.000000 autodistill_grounded_sam-0.0.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 20:24:13.346884 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2023-05-18 20:23:46.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3607 2023-05-18 20:23:39.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam/grounded_sam.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9556 2023-05-18 18:04:53.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 20:24:13.346884 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      646 2023-05-18 20:24:13.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-18 20:24:13.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-18 20:24:13.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-05-18 20:24:13.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-05-18 20:24:13.000000 autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-18 20:24:13.346884 autodistill_grounded_sam-0.0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1319 2023-05-18 20:18:00.000000 autodistill_grounded_sam-0.0.6/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 20:24:13.346884 autodistill_grounded_sam-0.0.6/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-05-18 16:28:39.000000 autodistill_grounded_sam-0.0.6/test/test_hello.py
+drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.517629 autodistill_grounded_sam-0.0.7/
+-rw-r--r--   0 yeldarb    (501) staff       (20)      599 2023-05-25 17:56:31.517483 autodistill_grounded_sam-0.0.7/PKG-INFO
+-rw-r--r--   0 yeldarb    (501) staff       (20)     3157 2023-05-24 22:17:32.000000 autodistill_grounded_sam-0.0.7/README.md
+drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.516106 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/
+-rw-r--r--   0 yeldarb    (501) staff       (20)       85 2023-05-25 16:48:41.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/__init__.py
+-rw-r--r--   0 yeldarb    (501) staff       (20)     3522 2023-05-25 17:25:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/grounded_sam.py
+-rw-r--r--   0 yeldarb    (501) staff       (20)     7893 2023-05-25 17:25:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/helpers.py
+drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.516987 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/
+-rw-r--r--   0 yeldarb    (501) staff       (20)      599 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/PKG-INFO
+-rw-r--r--   0 yeldarb    (501) staff       (20)      390 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 yeldarb    (501) staff       (20)        1 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 yeldarb    (501) staff       (20)      134 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/requires.txt
+-rw-r--r--   0 yeldarb    (501) staff       (20)       25 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/top_level.txt
+-rw-r--r--   0 yeldarb    (501) staff       (20)       38 2023-05-25 17:56:31.517671 autodistill_grounded_sam-0.0.7/setup.cfg
+-rw-r--r--   0 yeldarb    (501) staff       (20)     1592 2023-05-25 17:25:31.000000 autodistill_grounded_sam-0.0.7/setup.py
+drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.517132 autodistill_grounded_sam-0.0.7/test/
+-rw-r--r--   0 yeldarb    (501) staff       (20)       41 2023-05-24 22:17:32.000000 autodistill_grounded_sam-0.0.7/test/test_hello.py
```

### Comparing `autodistill_grounded_sam-0.0.6/PKG-INFO` & `autodistill_grounded_sam-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: autodistill_grounded_sam
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
-License: UNKNOWN
-Description: Automatically distill large foundational models into smaller, in-domain models for deployment
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+
+Automatically distill large foundational models into smaller, in-domain models for deployment
```

### Comparing `autodistill_grounded_sam-0.0.6/README.md` & `autodistill_grounded_sam-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_grounded_sam-0.0.6/autodistill_grounded_sam/grounded_sam.py` & `autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/grounded_sam.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 
 import torch
 
 torch.use_deterministic_algorithms(False)
 
 import glob
 import subprocess
-import sys
-import urllib.request
 
 import cv2
 import numpy as np
-import supervision as sv
 import torch
 from autodistill.base_models import BaseModel
 from autodistill.ontology import ClassDescriptionOntology
-from supervision import DetectionDataset, Detections
+from supervision import DetectionDataset
 from tqdm import tqdm
 
 from autodistill_grounded_sam.helpers import (
     combine_detections,
     load_grounding_dino,
     load_SAM,
     split_data,
@@ -62,29 +59,29 @@
             )
 
             detections_list.append(detections)
 
         detections = combine_detections(
             detections_list, overwrite_class_ids=range(len(detections_list))
         )
-        
-        #SAM Predictions
+
+        # SAM Predictions
         xyxy = detections.xyxy
 
         self.sam_predictor.set_image(image)
         result_masks = []
         for box in xyxy:
             masks, scores, logits = self.sam_predictor.predict(
                 box=box, multimask_output=False
             )
             index = np.argmax(scores)
             result_masks.append(masks[index])
 
         detections.mask = np.array(result_masks)
-        
+
         # separate in supervison to combine detections and override class_ids
         return detections
 
     def label(self, context_folder, extension=".jpg", output_folder=None):
         if output_folder is None:
             output_folder = context_folder + "_labeled"
         os.makedirs(output_folder, exist_ok=True)
```

### Comparing `autodistill_grounded_sam-0.0.6/autodistill_grounded_sam.egg-info/PKG-INFO` & `autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: autodistill-grounded-sam
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
-License: UNKNOWN
-Description: Automatically distill large foundational models into smaller, in-domain models for deployment
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+
+Automatically distill large foundational models into smaller, in-domain models for deployment
```

### Comparing `autodistill_grounded_sam-0.0.6/setup.py` & `autodistill_grounded_sam-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 import setuptools
 from setuptools import find_packages
+import subprocess
+import sys
 import re
 
+# groundingdino needs torch to be installed before it can be installed
+# this is a hack but couldn't find any other way to make it work
+try:
+    import torch
+except:
+    subprocess.check_call([sys.executable, "-m", "pip", "install", 'torch'])
+
 with open("./autodistill_grounded_sam/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

