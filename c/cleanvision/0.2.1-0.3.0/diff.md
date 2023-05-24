# Comparing `tmp/cleanvision-0.2.1.tar.gz` & `tmp/cleanvision-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanvision-0.2.1.tar", last modified: Sat Apr 22 00:33:32 2023, max compression
+gzip compressed data, was "cleanvision-0.3.0.tar", last modified: Wed May 24 22:27:52 2023, max compression
```

## Comparing `cleanvision-0.2.1.tar` & `cleanvision-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.783344 cleanvision-0.2.1/
--rw-r--r--   0 sanjana    (501) staff       (20)     5373 2023-04-10 14:40:45.000000 cleanvision-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 sanjana    (501) staff       (20)     2989 2023-04-11 02:44:57.000000 cleanvision-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 sanjana    (501) staff       (20)     3901 2023-04-10 14:40:45.000000 cleanvision-0.2.1/DEVELOPMENT.md
--rw-r--r--   0 sanjana    (501) staff       (20)    34523 2023-04-10 14:40:45.000000 cleanvision-0.2.1/LICENSE
--rw-r--r--   0 sanjana    (501) staff       (20)       58 2023-04-10 14:40:45.000000 cleanvision-0.2.1/MANIFEST.in
--rw-r--r--   0 sanjana    (501) staff       (20)    49948 2023-04-22 00:33:32.782331 cleanvision-0.2.1/PKG-INFO
--rw-r--r--   0 sanjana    (501) staff       (20)     8732 2023-04-21 23:53:01.000000 cleanvision-0.2.1/README.md
--rw-r--r--   0 sanjana    (501) staff       (20)     1747 2023-04-17 23:09:29.000000 cleanvision-0.2.1/pyproject.toml
--rw-r--r--   0 sanjana    (501) staff       (20)       38 2023-04-22 00:33:32.783490 cleanvision-0.2.1/setup.cfg
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.756636 cleanvision-0.2.1/src/
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.763038 cleanvision-0.2.1/src/cleanvision/
--rw-r--r--   0 sanjana    (501) staff       (20)      166 2023-04-19 16:30:00.000000 cleanvision-0.2.1/src/cleanvision/__init__.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.769802 cleanvision-0.2.1/src/cleanvision/dataset/
--rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/__init__.py
--rw-r--r--   0 sanjana    (501) staff       (20)      978 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/base_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1044 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/folder_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1076 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/hf_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1019 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/torch_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1184 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/utils.py
--rw-r--r--   0 sanjana    (501) staff       (20)    27295 2023-04-13 20:37:40.000000 cleanvision-0.2.1/src/cleanvision/imagelab.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.773065 cleanvision-0.2.1/src/cleanvision/issue_managers/
--rw-r--r--   0 sanjana    (501) staff       (20)     2069 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/__init__.py
--rw-r--r--   0 sanjana    (501) staff       (20)     8399 2023-04-13 20:37:40.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/duplicate_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)    10509 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/image_property.py
--rw-r--r--   0 sanjana    (501) staff       (20)    12286 2023-04-13 20:37:40.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/image_property_issue_manager.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.776538 cleanvision-0.2.1/src/cleanvision/utils/
--rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/utils/__init__.py
--rw-r--r--   0 sanjana    (501) staff       (20)     2155 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/utils/base_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)      668 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/utils/constants.py
--rw-r--r--   0 sanjana    (501) staff       (20)     3349 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/utils/utils.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1955 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/utils/viz_manager.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.765972 cleanvision-0.2.1/src/cleanvision.egg-info/
--rw-r--r--   0 sanjana    (501) staff       (20)    49948 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/PKG-INFO
--rw-r--r--   0 sanjana    (501) staff       (20)     1172 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/SOURCES.txt
--rw-r--r--   0 sanjana    (501) staff       (20)        1 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/dependency_links.txt
--rw-r--r--   0 sanjana    (501) staff       (20)      164 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/requires.txt
--rw-r--r--   0 sanjana    (501) staff       (20)       12 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/top_level.txt
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.781672 cleanvision-0.2.1/tests/
--rw-r--r--   0 sanjana    (501) staff       (20)     1969 2023-04-11 02:44:57.000000 cleanvision-0.2.1/tests/test_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     8473 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_duplicate_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)     4297 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_image_property_helpers.py
--rw-r--r--   0 sanjana    (501) staff       (20)     3594 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_image_property_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)     7541 2023-04-21 23:53:01.000000 cleanvision-0.2.1/tests/test_run.py
--rw-r--r--   0 sanjana    (501) staff       (20)      529 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_utils.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1064 2023-04-11 02:44:57.000000 cleanvision-0.2.1/tests/test_viz_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-24 22:27:43.000000 cleanvision-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-24 22:27:43.000000 cleanvision-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-24 22:27:43.000000 cleanvision-0.3.0/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-24 22:27:43.000000 cleanvision-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 22:27:43.000000 cleanvision-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    49939 2023-05-24 22:27:52.661222 cleanvision-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-24 22:27:43.000000 cleanvision-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-24 22:27:43.000000 cleanvision-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:27:52.661222 cleanvision-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/cleanvision/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/cleanvision/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/folder_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/imagelab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/src/cleanvision/issue_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/duplicate_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/image_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/image_property_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/src/cleanvision/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/base_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/viz_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/cleanvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49939 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_duplicate_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_image_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_image_property_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_viz_manager.py
```

### Comparing `cleanvision-0.2.1/CODE_OF_CONDUCT.md` & `cleanvision-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/CONTRIBUTING.md` & `cleanvision-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/DEVELOPMENT.md` & `cleanvision-0.3.0/DEVELOPMENT.md`

 * *Files 11% similar despite different names*

```diff
@@ -105,11 +105,17 @@
 This repo uses [EditorConfig](https://editorconfig.org/) to keep code style
 consistent across editors and IDEs. You can install a plugin for your editor,
 and then your editor will automatically ensure that indentation and line
 endings match the project style.
 
 ## Merging PRs to the codebase
 
-The docs for this repo are hosted by readthedocs.io and can be found [here](https://cleanvision.readthedocs.io/en/latest/). 
-Currently, merged PRs *will not* update the docs -- you **need** to do this manually after merging a PR.
-To update docs, go to the [readthedocs project page](https://readthedocs.org/projects/cleanvision/) and `build` latest version.
-If you want to see how a specific branch output looks, activate the branch in `version` tab and then `build` that branch.
+The docs for this repo are hosted by readthedocs.io and can be found [here](https://cleanvision.readthedocs.io/en/latest/).
+
+
+## Publishing Release
+- Ensure all **Checks** are successful for your release related PR after getting approvals from other code maintainers.
+- Merge all release related PRs.
+- Go to the Releases in the Github repo and draft a new release.
+- Create a new tag in the format `v{version}` corresponding to the version being released and click *Generate  release notes*.
+- Before publishing the release, ensure all checks are satisfied as the release on TestPypi and Pypi is automated and an error will result in publishing a new version.
+- Publish release
```

### Comparing `cleanvision-0.2.1/LICENSE` & `cleanvision-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/PKG-INFO` & `cleanvision-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.2.1
+Version: 0.3.0
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -720,15 +720,15 @@
 ```shell
 wget -nc 'https://cleanlab-public.s3.amazonaws.com/CleanVision/image_files.zip'
 ```
 
 1. Run CleanVision to audit the images.
 
 ```python
-from cleanvision.imagelab import Imagelab
+from cleanvision import Imagelab
 
 # Specify path to folder containing the image files in your dataset
 imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
 
 # Automatically check for a predefined list of issues within your dataset
 imagelab.find_issues()
```

### Comparing `cleanvision-0.2.1/README.md` & `cleanvision-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ```shell
 wget -nc 'https://cleanlab-public.s3.amazonaws.com/CleanVision/image_files.zip'
 ```
 
 1. Run CleanVision to audit the images.
 
 ```python
-from cleanvision.imagelab import Imagelab
+from cleanvision import Imagelab
 
 # Specify path to folder containing the image files in your dataset
 imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
 
 # Automatically check for a predefined list of issues within your dataset
 imagelab.find_issues()
```

### Comparing `cleanvision-0.2.1/pyproject.toml` & `cleanvision-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cleanvision"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     { name = "Cleanlab Inc.", email = "team@cleanlab.ai" },
 ]
 description = "Find issues in image datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["computer_vision", "cv", "image_data", "issue_detection", "data_quality", "image_quality", "machine_learning", "data_cleaning", "image_deduplication"]
```

### Comparing `cleanvision-0.2.1/src/cleanvision/dataset/base_dataset.py` & `cleanvision-0.3.0/src/cleanvision/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision/dataset/folder_dataset.py` & `cleanvision-0.3.0/src/cleanvision/dataset/folder_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision/dataset/hf_dataset.py` & `cleanvision-0.3.0/src/cleanvision/dataset/torch_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 from typing import TYPE_CHECKING, Union
 
 from PIL import Image
 
 from cleanvision.dataset.base_dataset import Dataset
 
 if TYPE_CHECKING:  # pragma: no cover
-    import datasets
+    from torchvision.datasets.vision import VisionDataset
 
 
-class HFDataset(Dataset):
-    """Wrapper class to handle datasets loaded from Huggingface."""
+class TorchDataset(Dataset):
+    """Wrapper class to handle datasets loaded from torchvision."""
 
-    def __init__(self, hf_dataset: "datasets.Dataset", image_key: str):
+    def __init__(self, torch_dataset: "VisionDataset") -> None:
         super().__init__()
-        self._data = hf_dataset
-        if image_key in hf_dataset.features:
-            self._image_key = image_key
-        else:
-            raise ValueError(
-                "Please specify the right image_key for this dataset. It can be found in dataset.features dict."
-            )
+        self._data = torch_dataset
+        # todo: catch errors
+        for i, obj in enumerate(torch_dataset[0]):
+            if isinstance(obj, Image.Image):
+                self._image_idx = i
         self._set_index()
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __getitem__(self, item: Union[int, str]) -> Image.Image:
-        return self._data[item][self._image_key]
+        return self._data[item][self._image_idx]
+
+    def get_name(self, index: Union[int, str]) -> str:
+        return f"idx: {index}"
 
     def _set_index(self) -> None:
         self.index = [i for i in range(len(self._data))]
-
-    def get_name(self, item: Union[int, str]) -> str:
-        return f"idx: {item}"
```

### Comparing `cleanvision-0.2.1/src/cleanvision/dataset/torch_dataset.py` & `cleanvision-0.3.0/src/cleanvision/dataset/hf_dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, Optional
 
 from PIL import Image
 
 from cleanvision.dataset.base_dataset import Dataset
 
 if TYPE_CHECKING:  # pragma: no cover
-    from torchvision.datasets.vision import VisionDataset
+    import datasets
 
 
-class TorchDataset(Dataset):
-    """Wrapper class to handle datasets loaded from torchvision."""
+class HFDataset(Dataset):
+    """Wrapper class to handle datasets loaded from Huggingface."""
 
-    def __init__(self, torch_dataset: "VisionDataset") -> None:
+    def __init__(self, hf_dataset: "datasets.Dataset", image_key: str):
         super().__init__()
-        self._data = torch_dataset
-        # todo: catch errors
-        for i, obj in enumerate(torch_dataset[0]):
-            if isinstance(obj, Image.Image):
-                self._image_idx = i
+        self._data = hf_dataset
+        if image_key in hf_dataset.features:
+            self._image_key = image_key
+        else:
+            raise ValueError(
+                "Please specify the right image_key for this dataset. It can be found in dataset.features dict."
+            )
         self._set_index()
 
     def __len__(self) -> int:
         return len(self._data)
 
-    def __getitem__(self, item: Union[int, str]) -> Image.Image:
-        return self._data[item][self._image_idx]
-
-    def get_name(self, index: Union[int, str]) -> str:
-        return f"idx: {index}"
+    def __getitem__(self, item: Union[int, str]) -> Optional[Image.Image]:
+        try:
+            image = self._data[item][self._image_key]
+            return image
+        except Exception as e:
+            print(f"Could not load image at index: {item}", e)
+            return None
 
     def _set_index(self) -> None:
         self.index = [i for i in range(len(self._data))]
+
+    def get_name(self, item: Union[int, str]) -> str:
+        return f"idx: {item}"
```

### Comparing `cleanvision-0.2.1/src/cleanvision/dataset/utils.py` & `cleanvision-0.3.0/src/cleanvision/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision/imagelab.py` & `cleanvision-0.3.0/src/cleanvision/imagelab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Imagelab is the core class in CleanVision for finding all types of issues in an image dataset.
 The methods in this module should suffice for most use-cases,
 but advanced users can get extra flexibility via the code in other CleanVision modules.
 """
+from __future__ import annotations
 
-import os
-import pickle
-from typing import List, Dict, Any, Optional, Tuple, TypeVar, Type
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, TypeVar, List, Dict, Any, Optional, Tuple, Type
 
 import numpy as np
 import pandas as pd
 from PIL import Image
 
+import cleanvision
 from cleanvision.dataset.torch_dataset import TorchDataset
 from cleanvision.dataset.utils import build_dataset
 from cleanvision.issue_managers import (
     IssueType,
     IssueManagerFactory,
     ISSUE_MANAGER_REGISTRY,
 )
@@ -24,30 +23,29 @@
 from cleanvision.utils.constants import (
     IMAGE_PROPERTY,
     DUPLICATE,
     IMAGE_PROPERTY_ISSUE_TYPES_LIST,
     DUPLICATE_ISSUE_TYPES_LIST,
     SETS,
 )
+from cleanvision.utils.serialize import Serializer
 from cleanvision.utils.utils import (
     deep_update_dict,
     get_is_issue_colname,
     get_score_colname,
     update_df,
     get_max_n_jobs,
 )
 from cleanvision.utils.viz_manager import VizManager
 
 if TYPE_CHECKING:  # pragma: no cover
     import datasets
     from torchvision.datasets.vision import VisionDataset
 
 __all__ = ["Imagelab"]
-
-OBJECT_FILENAME = "imagelab.pkl"
 TImagelab = TypeVar("TImagelab", bound="Imagelab")
 
 
 class Imagelab:
     """A single class to find all types of issues in image datasets.
     Imagelab detects issues in any image dataset and thus can be useful in most computer vision tasks including
     supervised and unsupervised training.
@@ -104,15 +102,15 @@
     Examples
     --------
 
     Basic usage of Imagelab class
 
     .. code-block:: python
 
-        from cleanvision.imagelab import Imagelab
+        from cleanvision import Imagelab
         imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
         imagelab.find_issues()
         imagelab.report()
 
     """
 
     def __init__(
@@ -127,23 +125,23 @@
             data_path, filepaths, hf_dataset, image_key, torchvision_dataset
         )
         if len(self._dataset) == 0:
             raise ValueError("No images found in the dataset specified")
         self.info: Dict[str, Any] = {"statistics": {}}
         self.issue_summary: pd.DataFrame = pd.DataFrame(
             columns=["issue_type", "num_images"]
-        )
+        ).astype({"issue_type": str, "num_images": np.int64})
 
         self.issues: pd.DataFrame = pd.DataFrame(index=self._dataset.index)
         self._issue_types: List[str] = []
         self._issue_managers: Dict[str, IssueManager] = {}
 
         # can be loaded from a file later
         self._config: Dict[str, Any] = self._set_default_config()
-        self._path = ""
+        self.cleanvision_version: str = cleanvision.__version__
 
     def _set_default_config(self) -> Dict[str, Any]:
         """Sets default values for various config variables used in Imagelab class
         The naming convention for methods is {method_name}_{config_variable_name}
 
         Returns
         -------
@@ -496,45 +494,50 @@
                     images=images,
                     titles=titles,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
                 )
 
         elif viz_name == "image_sets":
-            image_set_indices = list(self.info[issue_type][SETS][:num_images])
+            image_sets_indices = sorted(
+                self.info[issue_type][SETS], key=len, reverse=True
+            )
+            image_sets_indices = image_sets_indices[:num_images]
             image_sets = []
-            for indices in image_set_indices:
+            for indices in image_sets_indices:
                 image_sets.append([self._dataset[index] for index in indices])
 
             sets_str = "sets" if len(image_sets) > 1 else "set"
             if len(image_sets) < num_images:
                 print(
                     f"Found {len(image_sets)} {sets_str} of images with {issue_type} issue in the dataset."
                 )
             else:
                 print(
                     f"\nTop {num_images} {sets_str} of images with {issue_type} issue"
                 )
 
             title_sets = [
                 [self._dataset.get_name(index) for index in s]
-                for s in image_set_indices
+                for s in image_sets_indices
             ]
 
             if image_sets:
                 VizManager.image_sets(
                     image_sets,
                     title_sets,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
                 )
 
+    # todo: compress this code
     def visualize(
         self,
         image_files: Optional[List[str]] = None,
+        indices: Optional[List[str | int]] = None,
         issue_types: Optional[List[str]] = None,
         num_images: int = 4,
         cell_size: Tuple[int, int] = (2, 2),
     ) -> None:
         """Show specific images.
 
         Can be used for visualizing either:
@@ -546,14 +549,20 @@
 
         Parameters
         ----------
 
         image_files : List[str], optional
             List of filepaths for images to visualize.
 
+        indices: List[str|int], optional
+            List of indices of images in the dataset to visualize.
+            If the dataset is a local data_path, the indices are filepaths, which is also the index in `imagelab.issues` dataframe.
+            If the dataset is a huggingface or torchvision dataset, indices are of type int and corresponding to the indices in the dataset object.
+
+
         issue_types: List[str], optional
             List of issue types to visualize. For each type of issue, will show a few images representing the top-most severe instances of this issue in the dataset.
 
         num_images : int, optional
             Number of images to visualize from the dataset.
             These images are randomly selected if `issue_types` is ``None``.
             If `issue_types` is given, then this is the number of images for each issue type to visualize
@@ -604,14 +613,23 @@
             titles = [path.split("/")[-1] for path in image_files]
             VizManager.individual_images(
                 images,
                 titles,
                 ncols=self._config["visualize_num_images_per_row"],
                 cell_size=cell_size,
             )
+        elif indices:
+            images = [self._dataset[i] for i in indices]
+            titles = [self._dataset.get_name(i) for i in indices]
+            VizManager.individual_images(
+                images,
+                titles,
+                ncols=self._config["visualize_num_images_per_row"],
+                cell_size=cell_size,
+            )
         else:
             # todo: write test
             print("Sample images from the dataset")
             if image_files is None:
                 image_indices = list(
                     np.random.choice(
                         self._dataset.index,
@@ -634,82 +652,43 @@
     def get_stats(self) -> Any:
         """Returns dict of statistics computed from images when auditing the data such as: brightness, color space, aspect ratio, etc.
         If statistics have not been computed yet, then returns ``None``.
         """
         return self.info["statistics"]
 
     def save(self, path: str, force: bool = False) -> None:
-        """Saves this ImageLab instance into a folder at the given path.
-        Your saved Imagelab should be loaded from the same version of the CleanVision package.
+        """Saves this Imagelab instance, :py:attr:`issues` and :py:attr:`issue_summary` into a folder at the given path.
+        Your saved Imagelab should be loaded from the same version of the CleanVision package to avoid inconsistencies.
         This method does not save your image files.
 
         Parameters
         ----------
         path : str
             Path to folder where this Imagelab instance will be saved on disk.
 
         force: bool, default=False
             If set to True, any existing files at `path` will be overwritten.
-
-        Raises
-        ------
-        ValueError
-            If `allow_overwrite` is set to False, and an existing path is specified for saving Imagelab instance.
         """
-        path_exists = os.path.exists(path)
-        if not path_exists:
-            os.mkdir(path)
-        else:
-            if force:
-                print(
-                    f"WARNING: Existing files will be overwritten by newly saved files at: {path}"
-                )
-            else:
-                raise FileExistsError("Please specify a new path or set force=True")
-
-        self._path = path
-        object_file = os.path.join(self._path, OBJECT_FILENAME)
-        with open(object_file, "wb") as f:
-            pickle.dump(self, f)
-
-        print(f"Saved Imagelab to folder: {path}")
-        print(
-            "The data path and dataset must be not be changed to maintain consistent state when loading this Imagelab"
-        )
+        Serializer.serialize(path=path, imagelab=self, force=force)
 
     @classmethod
     def load(
         cls: Type[TImagelab], path: str, data_path: Optional[str] = None
-    ) -> TImagelab:
+    ) -> Imagelab:
         """Loads Imagelab from given path.
 
-
         Parameters
         ----------
         path : str
             Path to the saved Imagelab folder previously specified in :py:meth:`Imagelab.save` (not the individual pickle file).
         data_path : str
-            Path to image dataset previously used in Imagelab.
-            If the `data_path` is changed, Imagelab will not be loaded as some of its functionalities depend on it.
-            You should be using the same version of the CleanVision package previously used when saving the Imagelab.
+            Path to image dataset previously used in Imagelab, if your data exists locally as images in a folder.
+            If the `data_path` is changed, the code will break as Imagelab functionalities are dependent on it.
+            You should be using the same version of the CleanVision package previously used when saving Imagelab.
 
         Returns
         -------
         Imagelab
             Returns a saved instance of Imagelab
         """
-        if not os.path.exists(path):
-            raise ValueError(f"No folder found at specified path: {path}")
-
-        object_file = os.path.join(path, OBJECT_FILENAME)
-        with open(object_file, "rb") as f:
-            imagelab: TImagelab = pickle.load(f)
-
-        # todo: use hash for validating
-        # if data_path is not None:
-        #     filepaths = get_filepaths(data_path)
-        #     if set(filepaths) != set(imagelab._filepaths):
-        #         raise ValueError(
-        #             "Absolute path of image(s) has changed in the dataset. Cannot load Imagelab."
-        #         )
-        print("Successfully loaded Imagelab")
+        imagelab = Serializer.deserialize(path)
         return imagelab
```

### Comparing `cleanvision-0.2.1/src/cleanvision/issue_managers/__init__.py` & `cleanvision-0.3.0/src/cleanvision/issue_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision/issue_managers/duplicate_issue_manager.py` & `cleanvision-0.3.0/src/cleanvision/issue_managers/duplicate_issue_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import multiprocessing
 from typing import Any, Dict, List, Optional, Union
 
 import imagehash
 import numpy as np
 import pandas as pd
 from PIL import Image
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from cleanvision.dataset.base_dataset import Dataset
 from cleanvision.issue_managers import register_issue_manager, IssueType
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import SETS, DUPLICATE, MAX_PROCS
-from cleanvision.utils.utils import get_is_issue_colname
+from cleanvision.utils.utils import get_is_issue_colname, get_score_colname
 
 
-def get_hash(image: Image, params: Dict[str, Any]) -> str:
+def get_hash(image: Image.Image, params: Dict[str, Any]) -> str:
     hash_type, hash_size = params["hash_type"], params.get("hash_size", None)
     if hash_type == "md5":
         pixels = np.asarray(image)
         return hashlib.md5(pixels.tobytes()).hexdigest()
     elif hash_type == "whash":
         return str(imagehash.whash(image, hash_size=hash_size))
     elif hash_type == "phash":
@@ -32,16 +32,17 @@
     index: int,
     dataset: Dataset,
     to_compute: List[str],
     params: Dict[str, Any],
 ) -> Dict[str, Union[str, int]]:
     image = dataset[index]
     result: Dict[str, Union[str, int]] = {"index": index}
-    for issue_type in to_compute:
-        result[issue_type] = get_hash(image, params[issue_type])
+    if image:
+        for issue_type in to_compute:
+            result[issue_type] = get_hash(image, params[issue_type])
     return result
 
 
 def compute_hash_wrapper(args: Dict[str, Any]) -> Dict[str, Union[str, int]]:
     return compute_hash(**args)
 
 
@@ -141,15 +142,15 @@
                     )
                 )
 
             results = sorted(results, key=lambda r: r["index"])
 
         for result in results:
             for issue_type in to_compute:
-                hash_str = result[issue_type]
+                hash_str = result.get(issue_type, None)
                 if hash_str in issue_type_hash_mapping[issue_type]:
                     issue_type_hash_mapping[issue_type][hash_str].append(
                         result["index"]
                     )
                 else:
                     issue_type_hash_mapping[issue_type][hash_str] = [result["index"]]
 
@@ -168,23 +169,34 @@
             )
         summary_df = pd.DataFrame.from_dict(summary_dict, orient="index")
         self.summary = summary_df.reset_index()
         self.summary = self.summary.rename(columns={"index": "issue_type"})
         self.summary = self.summary.astype({"issue_type": str})
 
     def _update_issues(self) -> None:
+        score_df = pd.DataFrame(index=self.issues.index)
+        score_df[get_score_colname(IssueType.EXACT_DUPLICATES.value)] = np.ones(
+            len(score_df)
+        )
+        score_df[get_score_colname(IssueType.NEAR_DUPLICATES.value)] = np.ones(
+            len(score_df)
+        )
+
         for issue_type in self.issue_types:
-            duplicated_images = []
+            score_col = get_score_colname(issue_type)
             for s in self.info[issue_type][SETS]:
-                duplicated_images.extend(s)
-            self.issues[
-                get_is_issue_colname(issue_type)
-            ] = self.issues.index.to_series().apply(
-                lambda x: True if x in duplicated_images else False
-            )
+                score = 1.0 / len(
+                    s
+                )  # will never be 0 because all images in this set are duplicated
+                score_df.loc[s, score_col] = score
+
+            self.issues = self.issues.join(score_df[[score_col]])
+            self.issues[get_is_issue_colname(issue_type)] = [
+                False if x == 1 else True for x in self.issues[score_col]
+            ]
 
     def _update_info(
         self,
         issue_types: List[str],
         issue_type_hash_mapping: Dict[str, Any],
         imagelab_info: Dict[str, Any],
     ) -> None:
```

### Comparing `cleanvision-0.2.1/src/cleanvision/issue_managers/image_property.py` & `cleanvision-0.3.0/src/cleanvision/issue_managers/image_property.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import List, Dict, Any, Union, overload, Optional
+from typing import List, Dict, Any, Union, overload
 
 import numpy as np
 import pandas as pd
 from PIL import ImageStat, ImageFilter
 from PIL.Image import Image
 
 from cleanvision.issue_managers import IssueType
@@ -224,65 +224,70 @@
         scores = pd.DataFrame(index=raw_scores.index)
         scores_data = normalizing_factor * raw_scores[self.score_columns[0]]
         scores_data[scores_data > 1] = 1
         scores[get_score_colname(issue_type)] = scores_data
         return scores
 
 
-def calc_blurriness(image: Image, max_resolution: int) -> float:
-    ratio = max(image.width, image.height) / max_resolution
-    if ratio > 1:
-        low_rs = image.resize((int(image.width // ratio), int(image.height // ratio)))
-    else:
-        low_rs = image
-    edges = get_edges(low_rs)
+def calc_blurriness(gray_image: Image) -> float:
+    edges = get_edges(gray_image)
     blurriness = ImageStat.Stat(edges).var[0]
-    assert isinstance(
-        blurriness, float
-    )  # ImageStat.Stat returns float but no typestub for package
     return np.sqrt(blurriness)  # type:ignore
 
 
+def calc_std_grayscale(gray_image: Image) -> float:
+    return np.std(gray_image.histogram())  # type: ignore
+
+
 class BlurrinessProperty(ImageProperty):
     name = "blurriness"
 
     @property
     def score_columns(self) -> List[str]:
         return self._score_columns
 
     def __init__(self) -> None:
-        self._score_columns = [self.name]
+        self._score_columns = [self.name, "blurriness_grayscale_std"]
         self.max_resolution = MAX_RESOLUTION_FOR_BLURRY_DETECTION
 
     def calculate(self, image: Image) -> Dict[str, Union[float, str]]:
-        return {self.name: calc_blurriness(image, self.max_resolution)}
+        ratio = max(image.width, image.height) / self.max_resolution
+        if ratio > 1:
+            resized_image = image.resize(
+                (int(image.width // ratio), int(image.height // ratio))
+            )
+        else:
+            resized_image = image.copy()
+        gray_image = resized_image.convert("L")
+        return {
+            self.name: calc_blurriness(gray_image),
+            "blurriness_grayscale_std": calc_std_grayscale(gray_image),
+        }
 
     def get_scores(
         self,
         raw_scores: pd.DataFrame,
         issue_type: str,
-        dark_issue_data: Optional[pd.DataFrame] = None,
         normalizing_factor: float = 1.0,
+        color_threshold: float = 1.0,
         **kwargs: Any,
     ) -> pd.DataFrame:
         super().get_scores(raw_scores, issue_type, **kwargs)
-        assert dark_issue_data is not None
-        only_blur_scores = 1 - np.exp(-1 * raw_scores[self.name] * normalizing_factor)
-        is_dark = dark_issue_data[get_is_issue_colname(IssueType.DARK.value)].astype(
-            "int"
+        blur_scores = 1 - np.exp(-1 * raw_scores[self.name] * normalizing_factor)
+        std_scores = 1 - np.exp(
+            -1 * raw_scores["blurriness_grayscale_std"] * normalizing_factor
         )
-        dark_score = dark_issue_data[get_score_colname(IssueType.DARK.value)]
-        blur_scores = np.minimum(only_blur_scores + is_dark * (1 - dark_score), 1)
+        std_scores[std_scores <= color_threshold] = 0
+
         scores = pd.DataFrame(index=raw_scores.index)
-        scores[get_score_colname(issue_type)] = blur_scores
+        scores[get_score_colname(issue_type)] = np.minimum(blur_scores + std_scores, 1)
         return scores
 
 
-def get_edges(image: Image) -> Image:
-    gray_image = image.convert("L")
+def get_edges(gray_image: Image) -> Image:
     edges = gray_image.filter(ImageFilter.FIND_EDGES)
     return edges
 
 
 def calc_color_space(image: Image) -> str:
     return get_image_mode(image)
```

### Comparing `cleanvision-0.2.1/src/cleanvision/issue_managers/image_property_issue_manager.py` & `cleanvision-0.3.0/src/cleanvision/issue_managers/image_property_issue_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import multiprocessing
 from typing import Dict, Any, List, Set, Optional, Union
 
 import pandas as pd
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from cleanvision.dataset.base_dataset import Dataset
 from cleanvision.issue_managers import register_issue_manager, IssueType
 from cleanvision.issue_managers.image_property import (
     BrightnessProperty,
     AspectRatioProperty,
     EntropyProperty,
@@ -19,28 +19,28 @@
     IMAGE_PROPERTY,
     MAX_PROCS,
     IMAGE_PROPERTY_ISSUE_TYPES_LIST,
 )
 from cleanvision.utils.utils import (
     get_is_issue_colname,
     update_df,
-    get_score_colname,
 )
 
 
 def compute_scores(
     index: int,
     dataset: Dataset,
     to_compute: List[str],
     image_properties: Dict[str, ImageProperty],
 ) -> Dict[str, Union[str, int, float]]:
-    image = dataset[index]
     result: Dict[str, Union[int, str, float]] = {"index": index}
-    for issue_type in to_compute:
-        result = {**result, **image_properties[issue_type].calculate(image)}
+    image = dataset[index]
+    if image:
+        for issue_type in to_compute:
+            result = {**result, **image_properties[issue_type].calculate(image)}
     return result
 
 
 def compute_scores_wrapper(args: Dict[str, Any]) -> Dict[str, Union[float, str, int]]:
     return compute_scores(**args)
 
 
@@ -54,22 +54,26 @@
         super().__init__()
         self.issue_types: List[str] = []
         self.params = self.get_default_params()
         self.image_properties = self._get_image_properties()
 
     def get_default_params(self) -> Dict[str, Any]:
         return {
-            IssueType.DARK.value: {"threshold": 0.37},
+            IssueType.DARK.value: {"threshold": 0.32},
             IssueType.LIGHT.value: {"threshold": 0.05},
             IssueType.ODD_ASPECT_RATIO.value: {"threshold": 0.35},
             IssueType.LOW_INFORMATION.value: {
                 "threshold": 0.3,
                 "normalizing_factor": 0.1,
             },
-            IssueType.BLURRY.value: {"threshold": 0.17, "normalizing_factor": 0.01},
+            IssueType.BLURRY.value: {
+                "threshold": 0.29,
+                "normalizing_factor": 0.01,
+                "color_threshold": 0.18,
+            },
             IssueType.GRAYSCALE.value: {},
         }
 
     def update_params(self, params: Dict[str, Any]) -> None:
         for issue_type in self.params:
             non_none_params = {
                 k: v for k, v in params.get(issue_type, {}).items() if v is not None
@@ -99,23 +103,14 @@
 
         # Add issues using same property
         if {IssueType.LIGHT.value, IssueType.DARK.value}.issubset(set(issue_types)):
             defer_set.add(IssueType.LIGHT.value)
 
         return defer_set
 
-    def _get_additional_to_compute_set(self, issue_types: List[str]) -> List[str]:
-        additional_set = []
-        if (
-            IssueType.BLURRY.value in issue_types
-            and IssueType.DARK.value not in issue_types
-        ):
-            additional_set.append(IssueType.DARK.value)
-        return additional_set
-
     def find_issues(
         self,
         *,
         params: Optional[Dict[str, Any]] = None,
         dataset: Optional[Dataset] = None,
         imagelab_info: Optional[Dict[str, Any]] = None,
         n_jobs: Optional[int] = None,
@@ -125,16 +120,14 @@
         assert params is not None
         assert imagelab_info is not None
         assert dataset is not None
         assert n_jobs is not None
 
         self.issue_types = list(params.keys())
         self.issues = pd.DataFrame(index=dataset.index)
-        additional_set = self._get_additional_to_compute_set(self.issue_types)
-        self.issue_types = self.issue_types + additional_set
 
         self.update_params(params)
 
         agg_computations = pd.DataFrame(index=dataset.index)
         agg_computations = self._add_prev_computations(agg_computations, imagelab_info)
 
         defer_set = self._get_defer_set(self.issue_types, agg_computations)
@@ -202,54 +195,17 @@
         issue_types: List[str]
             List of issue types for which to update `self.issues`
         """
         for issue_type in issue_types:
             score_column_names = self.image_properties[issue_type].score_columns
             score_columns = agg_computations[score_column_names]
 
-            # todo: this is hacky
-            # Only blurry issue is dependent on another issue (in this case dark) for computing scores.
-            # This if else block handles this special case.
-            if issue_type == IssueType.BLURRY.value:
-                # In the case when blurry scores need to be computed
-                # dark_score and is_dark_issue can be retrieved from one of these two places
-                # 1. self.issues
-                # 2. recomputed using brightness_perc_99 info present in agg_computations.
-                dark_issue = IssueType.DARK.value
-                if not {
-                    get_is_issue_colname(dark_issue),
-                    get_score_colname(dark_issue),
-                }.issubset(self.issues):
-                    dark_score_columns = agg_computations[
-                        self.image_properties[dark_issue].score_columns
-                    ]
-                    dark_property = self.image_properties[dark_issue]
-
-                    dark_issue_scores = dark_property.get_scores(
-                        dark_score_columns, dark_issue, **self.params[dark_issue]
-                    )
-                    is_dark_issue = dark_property.mark_issue(
-                        dark_issue_scores,
-                        self.params[dark_issue].get("threshold"),
-                        dark_issue,
-                    )
-                else:
-                    dark_issue_scores = self.issues[[get_score_colname(dark_issue)]]
-                    is_dark_issue = self.issues[[get_is_issue_colname(dark_issue)]]
-
-                issue_scores = self.image_properties[issue_type].get_scores(
-                    score_columns,
-                    issue_type,
-                    **self.params[issue_type],
-                    dark_issue_data=dark_issue_scores.join(is_dark_issue),
-                )
-            else:
-                issue_scores = self.image_properties[issue_type].get_scores(
-                    score_columns, issue_type, **self.params[issue_type]
-                )
+            issue_scores = self.image_properties[issue_type].get_scores(
+                score_columns, issue_type, **self.params[issue_type]
+            )
 
             is_issue = self.image_properties[issue_type].mark_issue(
                 issue_scores, self.params[issue_type].get("threshold"), issue_type
             )
             self.issues = self.issues.join(issue_scores)
             self.issues = self.issues.join(is_issue)
```

### Comparing `cleanvision-0.2.1/src/cleanvision/utils/base_issue_manager.py` & `cleanvision-0.3.0/src/cleanvision/utils/base_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision/utils/constants.py` & `cleanvision-0.3.0/src/cleanvision/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "grayscale",
 ]
 DUPLICATE_ISSUE_TYPES_LIST: List[str] = ["exact_duplicates", "near_duplicates"]
 SETS: str = "sets"
 
 # max number of processes that can be forked/spawned for multiprocessing
 MAX_PROCS = 5000
-MAX_RESOLUTION_FOR_BLURRY_DETECTION = 256
+MAX_RESOLUTION_FOR_BLURRY_DETECTION = 64
 
 IMAGE_FILE_EXTENSIONS: List[str] = [
     "*.jpg",
     "*.jpeg",
     "*.gif",
     "*.jp2",
     "*.TIFF",
```

### Comparing `cleanvision-0.2.1/src/cleanvision/utils/utils.py` & `cleanvision-0.3.0/src/cleanvision/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision/utils/viz_manager.py` & `cleanvision-0.3.0/src/cleanvision/utils/viz_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/src/cleanvision.egg-info/PKG-INFO` & `cleanvision-0.3.0/src/cleanvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.2.1
+Version: 0.3.0
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -720,15 +720,15 @@
 ```shell
 wget -nc 'https://cleanlab-public.s3.amazonaws.com/CleanVision/image_files.zip'
 ```
 
 1. Run CleanVision to audit the images.
 
 ```python
-from cleanvision.imagelab import Imagelab
+from cleanvision import Imagelab
 
 # Specify path to folder containing the image files in your dataset
 imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
 
 # Automatically check for a predefined list of issues within your dataset
 imagelab.find_issues()
```

### Comparing `cleanvision-0.2.1/src/cleanvision.egg-info/SOURCES.txt` & `cleanvision-0.3.0/src/cleanvision.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 DEVELOPMENT.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/cleanvision/__init__.py
 src/cleanvision/imagelab.py
+src/cleanvision/py.typed
 src/cleanvision.egg-info/PKG-INFO
 src/cleanvision.egg-info/SOURCES.txt
 src/cleanvision.egg-info/dependency_links.txt
 src/cleanvision.egg-info/requires.txt
 src/cleanvision.egg-info/top_level.txt
 src/cleanvision/dataset/__init__.py
 src/cleanvision/dataset/base_dataset.py
@@ -21,16 +22,18 @@
 src/cleanvision/issue_managers/__init__.py
 src/cleanvision/issue_managers/duplicate_issue_manager.py
 src/cleanvision/issue_managers/image_property.py
 src/cleanvision/issue_managers/image_property_issue_manager.py
 src/cleanvision/utils/__init__.py
 src/cleanvision/utils/base_issue_manager.py
 src/cleanvision/utils/constants.py
+src/cleanvision/utils/serialize.py
 src/cleanvision/utils/utils.py
 src/cleanvision/utils/viz_manager.py
 tests/test_dataset.py
 tests/test_duplicate_issue_manager.py
 tests/test_image_property_helpers.py
 tests/test_image_property_issue_manager.py
 tests/test_run.py
+tests/test_save_load.py
 tests/test_utils.py
 tests/test_viz_manager.py
```

### Comparing `cleanvision-0.2.1/tests/test_dataset.py` & `cleanvision-0.3.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/tests/test_duplicate_issue_manager.py` & `cleanvision-0.3.0/tests/test_duplicate_issue_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import numpy as np
+import pandas as pd
 import pytest
 from PIL import Image
 
 from cleanvision.issue_managers import IssueType
 from cleanvision.issue_managers.duplicate_issue_manager import (
     DuplicateIssueManager,
     get_hash,
 )
+from cleanvision.utils.utils import get_is_issue_colname, get_score_colname
+
 
 EXACT = IssueType.EXACT_DUPLICATES.value
 NEAR = IssueType.NEAR_DUPLICATES.value
 
 
 class TestDuplicateIssueManager:
     @pytest.fixture
@@ -199,14 +203,43 @@
         duplicate_sets = issue_manager._get_duplicate_sets(hash_image_mapping)
         assert len(duplicate_sets) == len(expected_duplicate_sets)
         duplicate_sets.sort()
         expected_duplicate_sets.sort()
         for s1, s2 in zip(duplicate_sets, expected_duplicate_sets):
             assert set(s1) == set(s2)
 
+    def test_update_issues(self, issue_manager, monkeypatch):
+        info = {
+            EXACT: {"sets": [[0, 1], [2, 3, 4]]},
+            NEAR: {"sets": [[5, 6], [7, 8, 9]]},
+        }
+        monkeypatch.setattr(issue_manager, "info", info)
+        monkeypatch.setattr(issue_manager, "issues", pd.DataFrame(index=range(11)))
+        monkeypatch.setattr(issue_manager, "issue_types", [EXACT, NEAR])
+
+        issue_manager._update_issues()
+
+        issues_df = issue_manager.issues
+        assert issues_df[get_is_issue_colname(EXACT)].sum() == 5
+        assert issues_df[get_is_issue_colname(NEAR)].sum() == 5
+
+        score_col = get_score_colname(EXACT)
+        assert (issues_df.loc[[0, 1], score_col] == 0.5).all()
+        assert np.isclose(
+            issues_df.loc[[2, 3, 4], score_col], np.array([0.33] * 3), rtol=0.1
+        ).all()
+        assert issues_df.loc[10, score_col] == 1
+
+        score_col = get_score_colname(NEAR)
+        assert (issues_df.loc[[5, 6], score_col] == 0.5).all()
+        assert np.isclose(
+            issues_df.loc[[7, 8, 9], score_col], np.array([0.33] * 3), rtol=0.1
+        ).all()
+        assert issues_df.loc[10, score_col] == 1
+
 
 def test_get_hash():
     img = Image.new("RGB", (200, 200), (255, 0, 0))
     hash = get_hash(img, {"hash_type": "md5"})
     assert hash is not None
 
     hash = get_hash(img, {"hash_type": "whash", "hash_size": 2})
```

### Comparing `cleanvision-0.2.1/tests/test_image_property_helpers.py` & `cleanvision-0.3.0/tests/test_image_property_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from cleanvision.issue_managers.image_property import (
     BrightnessProperty,
     calculate_brightness,
     get_image_mode,
     calc_aspect_ratio,
     calc_entropy,
     calc_blurriness,
-    get_edges,
 )
 from cleanvision.utils.utils import get_is_issue_colname, get_score_colname
 
 
 @pytest.mark.parametrize(
     "rgb,expected_brightness",
     [
@@ -42,19 +41,17 @@
 def test_calc_entropy():
     img = Image.new("RGB", (200, 200), (255, 0, 0))
     entropy_score = calc_entropy(img)  # min(width/height,height/width)
     assert entropy_score == img.entropy()
 
 
 def test_calc_bluriness():
-    img = Image.new("RGB", (200, 200), (255, 0, 0))
-    edges = get_edges(img)
-    blurriness = calc_blurriness(img, 512)
-    assert isinstance(edges, Image.Image)
-    assert isinstance(blurriness, float)
+    gray_img = Image.new("RGB", (200, 200), (0, 0, 0)).convert("L")
+    blurriness = calc_blurriness(gray_img)
+    assert blurriness == 0
 
 
 @pytest.mark.parametrize(
     "image,expected_mode",
     [
         [Image.new("RGB", (164, 164), (255, 255, 255)), "RGB"],
         [Image.new("RGB", (164, 164)), "RGB"],
```

### Comparing `cleanvision-0.2.1/tests/test_image_property_issue_manager.py` & `cleanvision-0.3.0/tests/test_image_property_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.1/tests/test_run.py` & `cleanvision-0.3.0/tests/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import pytest
 import torchvision
 from datasets import load_dataset
 
 from cleanvision.dataset.folder_dataset import FolderDataset
-from cleanvision.imagelab import Imagelab
+from cleanvision import Imagelab
 from cleanvision.issue_managers.image_property import BrightnessProperty
 from cleanvision.issue_managers.image_property_issue_manager import (
     compute_scores_wrapper,
 )
 from docs.source.tutorials.custom_issue_manager import CustomIssueManager
 
 
@@ -167,25 +167,25 @@
 def test_hf_dataset_run(generate_local_dataset, n_classes, images_per_class):
     hf_dataset = load_dataset(
         "imagefolder", data_dir=generate_local_dataset, split="train"
     )
     imagelab = Imagelab(hf_dataset=hf_dataset, image_key="image")
     imagelab.find_issues()
     imagelab.report()
-    assert len(imagelab.issues.columns) == 14
+    assert len(imagelab.issues.columns) == 16
     assert len(imagelab.issues) == n_classes * images_per_class
 
 
 @pytest.mark.usefixtures("set_plt_show")
 def test_torch_dataset_run(generate_local_dataset, n_classes, images_per_class):
     torch_ds = torchvision.datasets.ImageFolder(root=generate_local_dataset)
     imagelab = Imagelab(torchvision_dataset=torch_ds)
     imagelab.find_issues()
     imagelab.report()
-    assert len(imagelab.issues.columns) == 14
+    assert len(imagelab.issues.columns) == 16
     assert len(imagelab.issues) == n_classes * images_per_class
 
 
 @pytest.mark.usefixtures("set_plt_show")
 def test_visualize_sample_images(generate_local_dataset):
     imagelab = Imagelab(data_path=generate_local_dataset)
     imagelab.visualize()
@@ -202,9 +202,9 @@
 @pytest.mark.usefixtures("set_plt_show")
 def test_filepath_dataset_run(generate_local_dataset, images_per_class):
     files = os.listdir(generate_local_dataset / "class_0")
     filepaths = [os.path.join(generate_local_dataset / "class_0", f) for f in files]
     imagelab = Imagelab(filepaths=filepaths)
     imagelab.find_issues()
     imagelab.report()
-    assert len(imagelab.issues.columns) == 14
+    assert len(imagelab.issues.columns) == 16
     assert len(imagelab.issues) == images_per_class
```

### Comparing `cleanvision-0.2.1/tests/test_viz_manager.py` & `cleanvision-0.3.0/tests/test_viz_manager.py`

 * *Files identical despite different names*

