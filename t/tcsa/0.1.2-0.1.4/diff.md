# Comparing `tmp/tcsa-0.1.2.tar.gz` & `tmp/tcsa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcsa-0.1.2.tar", last modified: Thu Nov  3 15:06:47 2022, max compression
+gzip compressed data, was "/mnt/c/Users/radvi/Downloads/tcsa-0.1.4/dist/.tmp-tiovlifs/tcsa-0.1.4.tar", last modified: Thu May 25 11:14:53 2023, max compression
```

## Comparing `tcsa-0.1.2.tar` & `tcsa-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)        0 2022-11-03 15:06:46.000000 tcsa-0.1.2/
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)    35159 2022-10-27 09:36:51.000000 tcsa-0.1.2/LICENSE
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)       29 2022-07-18 17:33:57.000000 tcsa-0.1.2/MANIFEST.in
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     3173 2022-11-03 15:06:46.000000 tcsa-0.1.2/PKG-INFO
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     2517 2022-10-27 10:55:27.000000 tcsa-0.1.2/README.md
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     1037 2022-11-03 15:04:11.000000 tcsa-0.1.2/pyproject.toml
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)      213 2022-11-03 15:06:46.000000 tcsa-0.1.2/setup.cfg
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)       93 2022-07-18 17:43:33.000000 tcsa-0.1.2/setup.py
-drwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)        0 2022-11-03 15:06:45.000000 tcsa-0.1.2/src/
-drwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)        0 2022-11-03 15:06:46.000000 tcsa-0.1.2/src/tcsa/
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     6497 2022-11-03 15:03:13.000000 tcsa-0.1.2/src/tcsa/__init__.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     1582 2022-10-27 10:30:55.000000 tcsa-0.1.2/src/tcsa/cli.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)      310 2022-07-08 21:49:00.000000 tcsa-0.1.2/src/tcsa/config.json
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     3371 2022-10-27 10:28:39.000000 tcsa-0.1.2/src/tcsa/data.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     8720 2022-10-27 10:27:26.000000 tcsa-0.1.2/src/tcsa/data_preparation.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     3881 2022-10-27 10:27:19.000000 tcsa-0.1.2/src/tcsa/manual.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     7123 2022-10-27 10:27:38.000000 tcsa-0.1.2/src/tcsa/model.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     5925 2022-10-27 10:29:59.000000 tcsa-0.1.2/src/tcsa/pipeline.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     6732 2022-10-27 10:30:24.000000 tcsa-0.1.2/src/tcsa/prequisite.py
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     6775 2022-10-27 10:30:37.000000 tcsa-0.1.2/src/tcsa/thresholding.py
-drwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)        0 2022-11-03 15:06:46.000000 tcsa-0.1.2/src/tcsa.egg-info/
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)     3173 2022-11-03 15:06:42.000000 tcsa-0.1.2/src/tcsa.egg-info/PKG-INFO
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)      467 2022-11-03 15:06:44.000000 tcsa-0.1.2/src/tcsa.egg-info/SOURCES.txt
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)        1 2022-11-03 15:06:42.000000 tcsa-0.1.2/src/tcsa.egg-info/dependency_links.txt
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)       39 2022-11-03 15:06:42.000000 tcsa-0.1.2/src/tcsa.egg-info/entry_points.txt
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)      208 2022-11-03 15:06:42.000000 tcsa-0.1.2/src/tcsa.egg-info/requires.txt
--rwxrwxrwx   0 radvilemaur  (1000) radvilemaur  (1000)        5 2022-11-03 15:06:42.000000 tcsa-0.1.2/src/tcsa.egg-info/top_level.txt
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 11:14:52.000000 tcsa-0.1.4/
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)    35159 2022-10-27 09:36:51.000000 tcsa-0.1.4/LICENSE
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       29 2022-07-18 17:33:57.000000 tcsa-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2866 2023-05-25 11:14:52.000000 tcsa-0.1.4/PKG-INFO
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2210 2023-05-25 11:09:05.000000 tcsa-0.1.4/README.md
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     1044 2023-05-25 11:13:33.000000 tcsa-0.1.4/pyproject.toml
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      213 2023-05-25 11:14:53.000000 tcsa-0.1.4/setup.cfg
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       93 2022-07-18 17:43:33.000000 tcsa-0.1.4/setup.py
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa/
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6497 2023-05-25 11:14:02.000000 tcsa-0.1.4/src/tcsa/__init__.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     1582 2022-10-27 10:30:55.000000 tcsa-0.1.4/src/tcsa/cli.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      310 2022-07-08 21:49:00.000000 tcsa-0.1.4/src/tcsa/config.json
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     3371 2022-10-27 10:28:39.000000 tcsa-0.1.4/src/tcsa/data.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     8868 2023-05-25 09:06:16.000000 tcsa-0.1.4/src/tcsa/data_preparation.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     3881 2022-10-27 10:27:19.000000 tcsa-0.1.4/src/tcsa/manual.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     7123 2022-10-27 10:27:38.000000 tcsa-0.1.4/src/tcsa/model.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     5920 2023-05-24 14:47:01.000000 tcsa-0.1.4/src/tcsa/pipeline.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6731 2023-05-24 14:47:40.000000 tcsa-0.1.4/src/tcsa/prequisite.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6775 2022-10-27 10:30:37.000000 tcsa-0.1.4/src/tcsa/thresholding.py
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2866 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/PKG-INFO
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      467 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        1 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       39 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/entry_points.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      215 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/requires.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        5 2023-05-25 11:14:52.000000 tcsa-0.1.4/src/tcsa.egg-info/top_level.txt
```

### Comparing `tcsa-0.1.2/LICENSE` & `tcsa-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.2/PKG-INFO` & `tcsa-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcsa
-Version: 0.1.2
+Version: 0.1.4
 Summary: temporalis segmentation pipeline to assess CSA of temporalis muscle
 Author: Computational Oncology
 Project-URL: Homepage, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline
 Project-URL: Bug Tracker, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 
 # temporalis Cross Sectional Area (tCSA)
 
 The temporalis Cross Sectional Area (tCSA) is a Python package for the segmentation of the temporalis muscle in T1-weighted contrast enhanced MRI and returns the cross-sectional area of the muscle.
 
 Preferred input type is NIfTI files (.nii or .nii.gz), however, it is possible to work with DICOM files (.dcm) with the included converter in the package.
 
-For now tCSA is only available on POSIX systems (Linux, and macOS) and require python >= 3.7.
+For now tCSA is only available on POSIX systems (Linux, and macOS) and require python == 3.7.
 
 
 ## Table of Contents
 
 
 - [Installation](#installation)
 - [Quick start](#quick-start)
@@ -36,17 +36,14 @@
 
 To install the package, create a new virtual environment and run the following command:
 
 `python -m pip install tcsa`
 
 ## Quick start
 
-Download the pre-trained weights (https://drive.google.com/drive/folders/1shgt5S6WFO3BJAKJfI22JSzKPVA3uFOQ?fbclid=IwAR2icSJ2UnRfc721X_6WAF_A0kHQuBBUz-s5-rCHFgBe8bFVK1rXhV7ahfM) and store them in a folder titled `/trained_weights` in the project working directory where the images folder is also present. 
-
-
 Once installed, tCSA can be run in the command line interface with `tcsa`.
 
 
 `tcsa .path/to/images -o path/to/output/folder/temporalis.csv --both-sides --delete`
 
 
 - `../images`: is the path to where the MRI are stored, it can be a directory or a single image
```

### Comparing `tcsa-0.1.2/README.md` & `tcsa-0.1.4/src/tcsa.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: tcsa
+Version: 0.1.4
+Summary: temporalis segmentation pipeline to assess CSA of temporalis muscle
+Author: Computational Oncology
+Project-URL: Homepage, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline
+Project-URL: Bug Tracker, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline/-/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # temporalis Cross Sectional Area (tCSA)
 
 The temporalis Cross Sectional Area (tCSA) is a Python package for the segmentation of the temporalis muscle in T1-weighted contrast enhanced MRI and returns the cross-sectional area of the muscle.
 
 Preferred input type is NIfTI files (.nii or .nii.gz), however, it is possible to work with DICOM files (.dcm) with the included converter in the package.
 
-For now tCSA is only available on POSIX systems (Linux, and macOS) and require python >= 3.7.
+For now tCSA is only available on POSIX systems (Linux, and macOS) and require python == 3.7.
 
 
 ## Table of Contents
 
 
 - [Installation](#installation)
 - [Quick start](#quick-start)
@@ -21,17 +36,14 @@
 
 To install the package, create a new virtual environment and run the following command:
 
 `python -m pip install tcsa`
 
 ## Quick start
 
-Download the pre-trained weights (https://drive.google.com/drive/folders/1shgt5S6WFO3BJAKJfI22JSzKPVA3uFOQ?fbclid=IwAR2icSJ2UnRfc721X_6WAF_A0kHQuBBUz-s5-rCHFgBe8bFVK1rXhV7ahfM) and store them in a folder titled `/trained_weights` in the project working directory where the images folder is also present. 
-
-
 Once installed, tCSA can be run in the command line interface with `tcsa`.
 
 
 `tcsa .path/to/images -o path/to/output/folder/temporalis.csv --both-sides --delete`
 
 
 - `../images`: is the path to where the MRI are stored, it can be a directory or a single image
```

### Comparing `tcsa-0.1.2/pyproject.toml` & `tcsa-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tcsa"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   { name="Computational Oncology"},
 ]
 description = "temporalis segmentation pipeline to assess CSA of temporalis muscle"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,15 +22,15 @@
   'tensorflow==1.14.0',
   'segmentation-models==1.0.1',
   'protobuf==3.20.1',
   'h5py==2.10.0',
   'opencv-python',
   'antspyx',
   'nibabel',
-  'intensity-normalization',
+  'intensity-normalization==2.1.4',
   'scikit-image',
   'gdown',
   'tqdm',
   'simpleitk',
   'requests',
   'packaging',
   'dicom2nifti',
```

### Comparing `tcsa-0.1.2/src/tcsa/__init__.py` & `tcsa-0.1.4/src/tcsa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import logging
 
 __title__ = "tcsa"
 __description__ = "temporalis segmentation pipeline to assess CSA of temporalis"
 __url__ = "https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline"
 __author__ = """Computational Oncology"""
 # __email__ = ""
-__version__ = "0.1.2"
+__version__ = "0.1.4"
 __license__ = "GPL 3"
 __copyright__ = "Copyright 2022 Imperial College London"
 
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 import requests
```

### Comparing `tcsa-0.1.2/src/tcsa/cli.py` & `tcsa-0.1.4/src/tcsa/cli.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.2/src/tcsa/data.py` & `tcsa-0.1.4/src/tcsa/data.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.2/src/tcsa/data_preparation.py` & `tcsa-0.1.4/src/tcsa/data_preparation.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,8 +219,11 @@
         ):
             img = nib.load(slice).get_fdata()
             img = np.rot90(img[:,:], 3)
             filename = slice.name[: -len(''.join(slice.suffixes))]
             output_directory = path_to_test_folder / patient.name / 'original'
             output_directory.mkdir(parents=True, exist_ok=True)
             output_path = output_directory / f'{filename}.png'
-            imageio.imsave(str(output_path), img)
+            # additional line to work with new imageio version (2.29.0)
+            img_upd = img.astype('uint8')
+            # end of new code
+            imageio.imsave(str(output_path), img_upd)
```

### Comparing `tcsa-0.1.2/src/tcsa/manual.py` & `tcsa-0.1.4/src/tcsa/manual.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.2/src/tcsa/model.py` & `tcsa-0.1.4/src/tcsa/model.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.2/src/tcsa/pipeline.py` & `tcsa-0.1.4/src/tcsa/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see https://www.gnu.org/licenses/.
 
 
 from pathlib import Path
 
 from tcsa import PATHS
-from .prequisite import run_prequisite
-from .data_preparation import (slicing, preprocessing, converting_to_png)
+from prequisite import run_prequisite
+from data_preparation import (slicing, preprocessing, converting_to_png)
 
-from .model import unet
-from .data import (testGenerator, saveResult)
-from .thresholding import (select_slice, temporalis_csa)
+from model import unet
+from data import (testGenerator, saveResult)
+from thresholding import (select_slice, temporalis_csa)
 import cv2
 
 import logging
 FORMAT = "%(message)s"
 logging.basicConfig(level=logging.INFO, format=FORMAT)
 log = logging.getLogger(__name__)
```

### Comparing `tcsa-0.1.2/src/tcsa/prequisite.py` & `tcsa-0.1.4/src/tcsa/prequisite.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import logging
 import importlib.resources
 import dicom2nifti
 import sys
 import shutil
 
 from tcsa import PATHS
-from .data_preparation import is_nifti, is_dicom
+from data_preparation import is_nifti, is_dicom
 
 FORMAT = "%(message)s"
 logging.basicConfig(level=logging.INFO, format=FORMAT)
 log = logging.getLogger(__name__)
 
 log_conv = logging.getLogger('dicom2nifti')
 log_conv.setLevel(logging.ERROR)
```

### Comparing `tcsa-0.1.2/src/tcsa/thresholding.py` & `tcsa-0.1.4/src/tcsa/thresholding.py`

 * *Files identical despite different names*

