# Comparing `tmp/tracebloc_package-dev-0.3.8.tar.gz` & `tmp/tracebloc_package-dev-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.3.8.tar", last modified: Thu May 18 06:24:20 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.3.9.tar", last modified: Thu May 25 07:52:03 2023, max compression
```

## Comparing `tracebloc_package-dev-0.3.8.tar` & `tracebloc_package-dev-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:24:20.633715 tracebloc_package-dev-0.3.8/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.8/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:24:20.633804 tracebloc_package-dev-0.3.8/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.8/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-18 06:24:20.634100 tracebloc_package-dev-0.3.8/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      859 2023-05-18 06:21:30.000000 tracebloc_package-dev-0.3.8/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:24:20.632388 tracebloc_package-dev-0.3.8/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5697 2023-03-23 06:34:00.000000 tracebloc_package-dev-0.3.8/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    16788 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    53410 2023-05-18 06:21:00.000000 tracebloc_package-dev-0.3.8/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.3.8/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7029 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10064 2023-05-18 06:23:40.000000 tracebloc_package-dev-0.3.8/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3832 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.3.8/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:24:20.633559 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)       73 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-25 07:52:03.570465 tracebloc_package-dev-0.3.9/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.9/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-25 07:52:03.570543 tracebloc_package-dev-0.3.9/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.9/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-25 07:52:03.570940 tracebloc_package-dev-0.3.9/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-05-25 07:51:03.000000 tracebloc_package-dev-0.3.9/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-25 07:52:03.569141 tracebloc_package-dev-0.3.9/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.3.9/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-05-19 09:01:53.000000 tracebloc_package-dev-0.3.9/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    20669 2023-05-25 06:32:21.000000 tracebloc_package-dev-0.3.9/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    59111 2023-05-24 09:14:21.000000 tracebloc_package-dev-0.3.9/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.3.9/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     8594 2023-05-25 06:18:17.000000 tracebloc_package-dev-0.3.9/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10152 2023-05-19 09:01:53.000000 tracebloc_package-dev-0.3.9/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5839 2023-05-23 18:03:05.000000 tracebloc_package-dev-0.3.9/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.3.9/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-25 07:52:03.570306 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.3.8/LICENSE.txt` & `tracebloc_package-dev-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.8/PKG-INFO` & `tracebloc_package-dev-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.3.8/setup.py` & `tracebloc_package-dev-0.3.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.3.8",
+    version="0.3.9",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
@@ -22,10 +22,14 @@
         "requests",
         "termcolor",
         "rich",
         "tqdm",
         "tensorflow_datasets",
         "dill",
         "silence_tensorflow",
+        "torch",
+        "torchvision",
+        "torchlightning",
+        "torchmetrics",
     ],
     zip_safe=False,
 )
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/check_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import tensorflow
 
 
 def get_optimizer(optimizer_name, learning_rate):
     """
-        Returns an optimizer based on the specified name and learning rate.
+    Returns an optimizer based on the specified name and learning rate.
 
-        Args:
-            optimizer_name (str): The name of the optimizer to use.
-            learning_rate (float or callable): The learning rate to use.
-            **kwargs: Additional keyword arguments for the optimizer.
+    Args:
+        optimizer_name (str): The name of the optimizer to use.
+        learning_rate (float or callable): The learning rate to use.
+        **kwargs: Additional keyword arguments for the optimizer.
 
-        Returns:
-            An instance of the specified optimizer class.
+    Returns:
+        An instance of the specified optimizer class.
     """
     type = learning_rate.pop("type")
     if type == "constant":
         learning_rate_func = get_learning_rate(learning_rate_name="constant")
     elif type == "custom":
         # Check if the learning_rate is a function (callable)
         if callable(learning_rate["value"]):
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/functional_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,128 @@
 import sys
 from silence_tensorflow import silence_tensorflow
+
 silence_tensorflow()
-import tensorflow_datasets as tfds
-from tensorflow.keras.applications.mobilenet import MobileNet
-from tensorflow.keras.layers import GlobalAveragePooling2D, Dense, Dropout, Flatten
-from tensorflow.keras import Sequential
-import tensorflow as tf
-import numpy as np
-from tensorflow_datasets.testing import mock_data
-import copy
 import os
-import dill
-import base64
 import dis
 import re
-import uuid
 import shutil
-import platform
-import subprocess
+from torch.utils.data import DataLoader
+import torch.optim as optim
+import torch.nn as nn
+import torchvision.datasets as datasets
 from inspect import getmembers, isfunction
-from importlib.machinery import SourceFileLoader
-from importlib.util import *
+from .utils import *
 
 
 # base class for checks on model file
 class CheckModel:
     MAX_MODEL_NAME_LENGTH = 64
     message = ""
     model = None
     tmp_file_path = ""
     file_name = "model.py"
     tmp_file = ""
     method_name = ""
+    class_name = ""
     input_shape = ""
     output_classes = ""
+    framework = ""
     notallowed = ["__MACOSX", "__pycache__"]
     input_shape_patt = re.compile("(^input_shape\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     out_classes_patt = re.compile("(^output_classes\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_method_patt = re.compile("(^main_method\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
+    main_class_patt = re.compile("(^main_class\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
+    framework_patt = re.compile("(^framework\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
+
 
-    def __init__(self, progress_bar, model_name=None, model_path=None):  # pragma: no cover
+    def __init__(
+        self, progress_bar, model_name=None, model_path=None
+    ):  # pragma: no cover
         self.model_name = model_name
         self.model_path = model_path
         self.progress_bar = progress_bar
 
     def prepare_file(self, temp_file):
-        main_file, remove_lines, filelines = self.get_variables(temp_file)
-        if main_file:
-            self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
-            self.load_model(temp_file)
-            if self.method_name == "":
-                self.add_method(temp_file, remove_lines)
-            else:
+        try:
+            main_file, remove_lines, filelines = self.get_variables(temp_file)
+            if main_file and self.framework == TENSORFLOW_FRAMEWORK:
+                self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
+                if self.method_name == "":
+                    self.load_model(temp_file)
+                    self.add_method(temp_file, remove_lines)
+                else:
+                    self.edit_file(temp_file, filelines, remove_lines)
+            elif self.framework == PYTORCH_FRAMEWORK:
+                self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
                 self.edit_file(temp_file, filelines, remove_lines)
+            else:
+                raise Exception("Framework argument missing in file")
+        except Exception as e:
+            raise e
 
     def get_variables(self, temp_file):
         main_file = False
         remove_lines = []
         with open(temp_file, "r") as tmp_fp:
             filedata = tmp_fp.read()
         filelines = filedata.split("\n")
         for linenum, fileline in enumerate(filelines):
-            if (
-                self.input_shape_patt.match(fileline)
-                or self.out_classes_patt.match(fileline)
-                or self.main_method_patt.match(fileline)
-            ):
-                if self.input_shape_patt.match(fileline):
-                    self.input_shape = re.sub(
-                        "(input_shape\s{0,}[=]\s{0,})",
-                        "",
-                        fileline.replace("'", "").replace('"', ""),
-                    )
-                elif self.out_classes_patt.match(fileline):
-                    self.output_classes = re.sub(
-                        "(output_classes\s{0,}[=]\s{0,})",
-                        "",
-                        fileline.replace("'", "").replace('"', ""),
-                    )
-                elif self.main_method_patt.match(fileline):
-                    self.method_name = re.sub(
-                        "(main_method\s{0,}[=]\s{0,})",
-                        "",
-                        fileline.replace("'", "").replace('"', ""),
-                    )
+            if self.framework_patt.match(fileline):
+                self.framework = re.sub(
+                    "(framework\s{0,}[=]\s{0,})",
+                    "",
+                    fileline.replace("'", "").replace('"', ""),
+                )
                 remove_lines.append(linenum)
                 if not main_file:
                     self.file_name = os.path.split(temp_file)[1]
                     main_file = True
+            if self.framework == TENSORFLOW_FRAMEWORK:
+                if (
+                    self.input_shape_patt.match(fileline)
+                    or self.out_classes_patt.match(fileline)
+                    or self.main_method_patt.match(fileline)
+                ):
+                    if self.input_shape_patt.match(fileline):
+                        self.input_shape = re.sub(
+                            "(input_shape\s{0,}[=]\s{0,})",
+                            "",
+                            fileline.replace("'", "").replace('"', ""),
+                        )
+                    elif self.out_classes_patt.match(fileline):
+                        self.output_classes = re.sub(
+                            "(output_classes\s{0,}[=]\s{0,})",
+                            "",
+                            fileline.replace("'", "").replace('"', ""),
+                        )
+                    elif self.main_method_patt.match(fileline):
+                        self.method_name = re.sub(
+                            "(main_method\s{0,}[=]\s{0,})",
+                            "",
+                            fileline.replace("'", "").replace('"', ""),
+                        )
+                    remove_lines.append(linenum)
+                    if not main_file:
+                        self.file_name = os.path.split(temp_file)[1]
+                        main_file = True
+            elif self.framework == PYTORCH_FRAMEWORK:
+                if self.main_class_patt.match(fileline):
+                    self.class_name = re.sub(
+                        "(main_class\s{0,}[=]\s{0,})",
+                        "",
+                        fileline.replace("'", "").replace('"', ""),
+                    )
+                    remove_lines.append(linenum)
+                    if not main_file:
+                        self.file_name = os.path.split(temp_file)[1]
+                        main_file = True
+        if self.framework == "":
+            print("Framework parameter missing from file")
+            return False, [], []
         tmp_fp.close()
         return main_file, remove_lines, filelines
 
     def replace_vars(self, code):
         if re.search(
             f"[^a-zA-Z_\-0-9]{self.input_shape}[^a-zA-Z_\-0-9]", code
         ) or re.search(f"{self.input_shape}[^a-zA-Z_\-0-9]", code):
@@ -119,17 +150,18 @@
     def edit_file(self, temp_file, filelines, remove_lines=[]):
         edited_data = []
         with open(temp_file, "w") as tmp_fp:
             for linenum, fileline in enumerate(filelines):
                 if linenum in remove_lines:
                     continue
                 else:
-                    if re.search(f"def {self.method_name}\(.*\)", fileline):
-                        fileline = fileline.replace(str(self.method_name), "MyModel")
-                    fileline = self.replace_vars(fileline)
+                    if self.framework == TENSORFLOW_FRAMEWORK:
+                        if re.search(f"def {self.method_name}\(.*\)", fileline):
+                            fileline = fileline.replace(str(self.method_name), "MyModel")
+                        fileline = self.replace_vars(fileline)
                     edited_data.append(fileline)
             tmp_fp.writelines("\n".join(edited_data))
         tmp_fp.close()
 
     def get_imports(self, codelines):
         instructions = dis.get_instructions(codelines)
         instructions = [__ for __ in instructions]
@@ -210,71 +242,73 @@
 
     def check_MyModel(self):
         """
         Check if model is MyModel is present in model file
         """
         try:
             getmembers(self.model.MyModel, isfunction)
+            self.progress_bar.update(1)
         except Exception:  # pragma: no cover
             self.message = "Please upload file as per docs"
             raise
 
-    def load_model(self, filename):
+    def load_model(self, filename, update_progress_bar=False):
         try:
             sys.path.append(self.tmp_file_path)
             self.model = SourceFileLoader(
                 f"{filename}", f"{self.tmp_file}"
             ).load_module()
+            if self.framework == PYTORCH_FRAMEWORK:
+                class_ = getattr(self.model, self.class_name)
+                self.model = class_()
+            if update_progress_bar:
+                self.progress_bar.update(1)
         except Exception as e:
             if self.message == "":
                 self.message = f"Error loading the model file, {str(e)}"
             raise
 
     def extract_multiple_file(self):
         import zipfile
 
         with open(self.model_path, "rb") as file:
             with zipfile.ZipFile(file, "r") as zip_ref:
                 zip_ref.extractall(self.tmp_file_path)
         return False
 
     def load_model_file(self):
+        self.tmp_file_path = os.path.join(
+            self.model_path.rsplit("/", 1)[0],
+            f"tmpmodel_{self.model_name[: self.MAX_MODEL_NAME_LENGTH]}",
+        )
+        if not os.path.isdir(self.tmp_file_path):
+            os.mkdir(self.tmp_file_path)
         # check if file contains the MyModel function
         try:
             file = self.model_path.rsplit("/", 1)[1]
             if os.path.splitext(str(file))[1] == ".zip":
                 self.extract_multiple_file()
             else:
                 self.tmp_file = os.path.join(self.tmp_file_path, str(file))
                 self.file_name = str(file)
                 shutil.copy2(self.model_path, self.tmp_file_path)
             for tmp_f in os.listdir(self.tmp_file_path):
                 if not (os.path.isdir(tmp_f) or tmp_f in self.notallowed):
                     self.prepare_file(os.path.join(self.tmp_file_path, tmp_f))
-            self.load_model(self.file_name)
-            self.check_MyModel()
-            self.progress_bar.update(1)
+            self.load_model(self.file_name, update_progress_bar=True)
+            if self.framework == TENSORFLOW_FRAMEWORK:
+                self.check_MyModel()
+                self.check_model_arguments()
+            else:
+                self.progress_bar.update(2)
         except Exception as e:  # pragma: no cover
             if os.path.exists(self.tmp_file_path):
                 shutil.rmtree(self.tmp_file_path)
             if self.message == "":
-                self.message = f"\nError loading the model file, {str(e)}"
-            raise
-
-    def check_model_layers(self):
-        """
-        Check layers in model
-        """
-        try:
-            self.model.MyModel()
-            self.progress_bar.update(1)
-        except Exception:  # pragma: no cover
-            self.message = (
-                "\nNot able to load model from file, please refer to Tracebloc Docs"
-            )
+                self.message = f"\nError loading the model file"
             raise
 
     def check_model_arguments(self):
         """
         Check if MyModel contains:
             - input_shape
             - classes
@@ -282,97 +316,115 @@
         try:
             self.model = self.model.MyModel(input_shape=(256, 256, 3), output_classes=1)
             self.progress_bar.update(1)
         except Exception:  # pragma: no cover
             self.message = "\nModel file not provided as per docs: MyModel function receives no arguments"
             raise
 
+    def remove_tmp_file(self, update_progress_bar=False):
+        """
+        remove temporary model file
+        """
+        if os.path.exists(self.tmp_file_path):  # pragma: no cover
+            shutil.rmtree(self.tmp_file_path)
+        if update_progress_bar:
+            self.progress_bar.update(1)
+
+    def model_func_checks(self):
+        # check if model is eligible
+        try:
+            self.load_model_file()
+            self.message = "all check passed"
+            eligible = True
+        except Exception as e:  # pragma: no cover
+            if self.message == "":
+                self.message = f"Model checks failed with error as {e}"
+            eligible = False
+        if not eligible:
+            return eligible, self.message, None, self.progress_bar  # pragma: no cover
+        return True, self.message, self.model_name, self.progress_bar
+
+class TensorflowChecks:
+    def __init__(self, model, model_name, progress_bar):
+        self.message = None
+        self.model = model
+        self.model_name = model_name
+        self.progress_bar = progress_bar
+
+    def progress_bar_update(self):
+        if self.progress_bar is not None:
+            self.progress_bar.update(1)
+
     def is_model_supported(self):
         """
         Check if model contains:
             - input_shape
             - classes
         """
         tensorflow_supported_apis = (tf.keras.models.Sequential, tf.keras.Model)
-        model = self.model.MyModel()
+        model = self.model
         supported = isinstance(model, tensorflow_supported_apis)
         if supported:  # pragma: no cover
             # check if it is of model subclassing api
             if not hasattr(model, "input_shape"):
                 self.message = "\nModel file not provided as per docs: unsupported API used for Model"  # pragma: no cover
                 raise Exception("input shape missing")  # pragma: no cover
-        self.progress_bar.update(1)
+        self.progress_bar_update()
 
     def layer_instance_check(self):
         """
         If model layers are of type keras layers
         """
         for layer in self.model.layers:
             if not isinstance(layer, tf.keras.layers.Layer):
                 self.message = "\nLayers in Model are not supported by Tensorflow"  # pragma: no cover
                 raise Exception("invalid layer")  # pragma: no cover
-        self.progress_bar.update(1)
+        self.progress_bar_update()
 
     def small_training_loop(self, custom_loss=None):
         try:
             # mock dataset for small training
             classes = 1  # get output classes from model
             training_dataset = mock_dataset(classes)
             if custom_loss:
                 # check for custom loss
                 loss = custom_loss["value"]
 
             else:
                 loss = tf.keras.losses.CategoricalCrossentropy()
             self.model.compile(
-                optimizer=tf.keras.optimizers.Adam(), loss=loss,
+                optimizer=tf.keras.optimizers.Adam(),
+                loss=loss,
             )
             self.model.fit(training_dataset, epochs=1, verbose=0)
-            self.progress_bar.update(1)
+            self.progress_bar_update()
         except Exception as e:  # pragma: no cover
-            self.message = "\nModel not support training on image classification dataset."
+            self.message = (
+                "\nModel not support training on image classification dataset."
+            )
             raise
 
     def check_original_model_channels(self):
         """
         check for model channels to be 3
         """
-        model_channel = self.model.MyModel()
+        model_channel = self.model
         if model_channel.input_shape[3] != 3:
             self.message = (
                 "\nPlease provide model input shape with 3 channels"  # pragma: no cover
             )
             raise Exception("invalid input shape")  # pragma: no cover
-        self.progress_bar.update(1)
-
-    def remove_tmp_file(self):
-        """
-        remove temporary model file
-        """
-        if os.path.exists(self.tmp_file_path):  # pragma: no cover
-            shutil.rmtree(self.tmp_file_path)
-        self.progress_bar.update(1)
+        self.progress_bar_update()
 
     def is_model_eligible(self):
-
-        self.tmp_file_path = os.path.join(
-            self.model_path.rsplit("/", 1)[0],
-            f"tmpmodel_{self.model_name[: self.MAX_MODEL_NAME_LENGTH]}",
-        )
-        if not os.path.isdir(self.tmp_file_path):
-            os.mkdir(self.tmp_file_path)
         try:
-            self.load_model_file()
-            self.check_model_layers()
             self.is_model_supported()
             self.check_original_model_channels()
-            self.check_model_arguments()
             self.layer_instance_check()
             self.small_training_loop()
-            self.remove_tmp_file()
             self.message = "all check passed"
         except Exception as e:  # pragma: no cover
             if self.message == "":
                 self.message = f"Model checks failed with error as {e}"
             return False, self.message
         return True, self.message
 
@@ -380,59 +432,85 @@
         # check if model is eligible
         eligible, message = self.is_model_eligible()
         if not eligible:
             return eligible, message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
-def mock_dataset(classes):
-    num_examples = 3
-
-    def as_dataset(self, *args, **kwargs):
-        return tf.data.Dataset.from_generator(  # pragma: no cover
-            lambda: (
-                {
-                    "image": np.ones(shape=(256, 256, 3), dtype=np.uint8),
-                    "label": classes,
-                }
-                for i in range(num_examples)
-            ),
-            output_types=self.info.features.tf_dtype,
-            output_shapes=self.info.features.shape,
-        )
-
-    with mock_data(as_dataset_fn=as_dataset):
-        (ds_train, ds_test), ds_info = tfds.load(
-            "deep_weeds",
-            split=["train", "test"],
-            shuffle_files=True,
-            as_supervised=True,
-            with_info=True,
-        )
-
-    ds_train = ds_train.map(normalize_img, num_parallel_calls=tf.data.AUTOTUNE)
-    ds_train = ds_train.batch(8)
-    ds_train = ds_train.prefetch(tf.data.AUTOTUNE)
-    return ds_train
+class TorchChecks:
+    def __init__(self, model, model_name, progress_bar):
+        self.message = None
+        self.model = model
+        self.model_name = model_name
+        self.progress_bar = progress_bar
 
+    def is_model_supported(self):
+        """
+        Check if model contains:
+            - forward function
+        """
+        model = self.model
+        if not hasattr(model, "forward"):
+            self.message = "\nModel file not provided as per docs: forward function not found in  Model"
+            raise Exception("forward func missing")
+        self.progress_bar.update(1)
 
-def normalize_img(image, label):
-    """Normalizes images: `uint8` -> `float32`."""
-    return tf.cast(image, tf.float32) / 255.0, label  # pragma: no cover
+    def small_training_loop(self, custom_loss=None):
+        try:
+            # Define the number of fake images and other properties
+            num_images = 100
+            image_size = 32
+            num_channels = 3
+            num_classes = 10
+            # Create fake image data
+            train_dataset = datasets.FakeData(
+                size=num_images,
+                image_size=(num_channels, image_size, image_size),
+                num_classes=num_classes,
+                transform=transforms.ToTensor(),
+            )
 
-def test_code():
-    main_method = "MyModel"
-    input_shape = "input_shape"
-    output_classes = "output_classes"
+            train_loader = DataLoader(train_dataset, batch_size=16, shuffle=True)
 
+            # train_loader, classes = mock_torch_data(self.tmp_path)
+            criterion = nn.CrossEntropyLoss()
+            optimizer = optim.SGD(self.model.parameters(), lr=0.001, momentum=0.9)
+            for epoch in range(1):  # loop over the dataset multiple times
+
+                running_loss = 0.0
+                for i, data in enumerate(train_loader, 0):
+                    # get the inputs; data is a list of [inputs, labels]
+                    inputs, labels = data
+                    labels = torch.tensor(labels, dtype=torch.long)
+                    # zero the parameter gradients
+                    optimizer.zero_grad()
+
+                    # forward + backward + optimize
+                    outputs = self.model(inputs)
+                    loss = criterion(outputs, labels)
+                    loss.backward()
+                    optimizer.step()
 
-    def MyModel(input_shape=(224, 224, 3), output_classes=3):
+                    # print statistics
+                    running_loss += loss.item()
+            self.progress_bar.update(1)
+        except Exception as e:  # pragma: no cover
+            self.message = (
+                "\nModel not support training on image classification dataset."
+            )
+            raise
 
-        base_mobilenet_model = MobileNet(
-            input_shape=input_shape, include_top=False, weights=None
-        )
-        multi_disease_model = Sequential()
-        multi_disease_model.add(base_mobilenet_model)
-        multi_disease_model.add(GlobalAveragePooling2D())
-        multi_disease_model.add(Dropout(0.5))
-        multi_disease_model.add(Dense(output_classes, activation="sigmoid"))
-        return multi_disease_model
+    def model_func_checks(self):
+        # check if model is eligible
+        try:
+            self.is_model_supported()
+            self.progress_bar.update(2)
+            self.small_training_loop()
+            self.message = "all check passed"
+            eligible = True
+        except Exception as e:  # pragma: no cover
+            if self.message == "":
+                self.message = f"Model checks failed with error as {e}"
+            eligible = False
+        if not eligible:
+            return eligible, self.message, None, self.progress_bar  # pragma: no cover
+        return eligible, self.message, self.model_name, self.progress_bar
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/linkModelDataSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import inspect
 import requests, json
 import dill
 import base64
 from termcolor import colored
 from tracebloc_package import check_parameters
 from .utils import *
-from .functional_test import CheckModel, test_code
+from .functional_test import CheckModel, TensorflowChecks, TorchChecks
 
-CONSTANT = "constant"
-STANDARD = "standard"
-ADAPTIVE = "adaptive"
-CUSTOM = "custom"
-TYPE = "type"
-FUNCTION = "function"
-VALUE = "value"
 
 
 class LinkModelDataSet:
     """
     creating a training plan and assign data set
     parameters: modelId, datasetId, token
 
@@ -34,14 +27,15 @@
         weights,
         totalDatasetSize,
         total_images,
         num_classes,
         class_names,
         url="",
         environment="production",
+        framework=TENSORFLOW_FRAMEWORK,
     ):
         self.__url = url
         # self.__url = 'http://127.0.0.1:8000/'
         self.__token = token
         self.__earlystopCallback = {}
         self.__reducelrCallback = {}
         self.__modelCheckpointCallback = {}
@@ -98,14 +92,15 @@
         self.__upperboundTime = 0
         self.__weights = weights
         self.__images_per_class = json.dumps(self.__class_names)
         self.__eligibility_passed = True
         self.__error_method = []
         self.__reform_model = False
         self._environment = environment
+        self.__framework = framework
         self.__experiment_url = "https://ai.tracebloc.io/experiments/"
         if environment == "development" or environment == "ds":
             self.__experimenturl = "https://dev.tracebloc.io/experiments/"
         elif environment == "staging":
             self.__experimenturl = "https://stg.tracebloc.io/experiments/"
 
     def resetTrainingPlan(self):
@@ -157,18 +152,28 @@
         self.__eligibility_passed = True
         self.__reform_model = False
         print("Training Plan Parameters reset")
 
     def __print_error(self, error):
         self.__eligibility_passed = False
         method = inspect.currentframe().f_back.f_code.co_name
-        text = colored(error, "red",)
+        text = colored(
+            error,
+            "red",
+        )
         print(text, "\n")
         self.__error_method.append(method)
 
+    def __not_supported_parameters(self, parameter):
+        text = colored(
+            f"The parameter {parameter} is not supported till now on pytorch",
+            "red",
+        )
+        print(text, "\n")
+
     def __remove_error_method(self):
         method = inspect.currentframe().f_back.f_code.co_name
         if method in self.__error_method:
             self.__error_method.remove(method)
         if len(self.__error_method) == 0:
             self.__eligibility_passed = True
 
@@ -196,25 +201,34 @@
             else:
                 checkeligible = False
                 error_msg = "trainingDatasetSize dictionary must contain all classes that are present in the dataset. Customisation in terms of classes is not allowed."
                 self.__print_error(error_msg)
         if checkeligible:
             self.__trainingClasses = training_dataset
             self.__trainingDatasetSize = getImagesCount(training_dataset)
-            self.__subdataset = json.dumps({"trainingDatasetSize": self.__trainingDatasetSize, "trainingClasses": self.__trainingClasses})
+            self.__subdataset = json.dumps(
+                {
+                    "trainingDatasetSize": self.__trainingDatasetSize,
+                    "trainingClasses": self.__trainingClasses,
+                }
+            )
             self.__remove_error_method()
             # recalculate the validation split
             header = {"Authorization": f"Token {self.__token}"}
             data = {
                 "edges_involved": json.dumps(list(self.__total_images.keys())),
                 "images_per_class": json.dumps(training_dataset),
                 "type": "recalculate_image_count_per_edge",
                 "datasetId": self.__datasetId,
             }
-            re = requests.post(f"{self.__url}check-model/", headers=header, data=data,)
+            re = requests.post(
+                f"{self.__url}check-model/",
+                headers=header,
+                data=data,
+            )
             body_unicode = re.content.decode("utf-8")
             content = json.loads(body_unicode)
             if re.status_code == 200:
                 self.__total_images = content["total_images_per_edge"]
                 self.__validation_split = self.__default_validation_split()
             # else:
             #     self.__print_error(content['message'])
@@ -226,15 +240,19 @@
         header = {"Authorization": f"Token {self.__token}"}
         data = {
             "model_name": self.__modelId,
             "image_shape": self.__image_shape,
             "image_type": self.__image_type,
             "type": "reform_model",
         }
-        re = requests.post(f"{self.__url}check-model/", headers=header, data=data,)
+        re = requests.post(
+            f"{self.__url}check-model/",
+            headers=header,
+            data=data,
+        )
         if re.status_code == 202:
             body_unicode = re.content.decode("utf-8")
             content = json.loads(body_unicode)
             self.__modelId = content["model_name"]
         if re.status_code == 400:
             body_unicode = re.content.decode("utf-8")
             content = json.loads(body_unicode)
@@ -260,16 +278,14 @@
     def imageType(self, image_type: str):
         """
         Set image type to be used for training
         parameters: string type values.
         supported type: ['rgb', 'gray']
         example: trainingObject.imageType('rgb')
         default: rgb
-
-
         """
         allowed_types = ["rgb", "grayscale"]
         try:
             if type(image_type) is str:
                 allowed_types.index(image_type.lower())
                 self.__image_type = image_type.lower()
                 self.__update_image_model()
@@ -296,48 +312,20 @@
         """
         String.
         Name of the experiment
         example:trainingObject.experimentName('Classifying manufacturing defects')
         """
         self.__name = str(name)
 
-    # def category(self, category: str):
-    #     """
-    #     String.
-    #     Category of experiment, like classification
-    #     example:trainingObject.category('classification')
-    #     default_value: 'Classification'
-    #
-    #     """
-    #     if type(category) == str:
-    #         self.__category = category
-    #     else:
-    #         print("Invalid input type given for category\n\n")
-    #
-    # def modelType(self, modelType: str):
-    #     """
-    #     String.
-    #     Type of model used in the experiment, like VGGNET
-    #     example:trainingObject.modelType('VGGNET')
-    #
-    #
-    #     """
-    #     if type(modelType) == str:
-    #         self.__modelType = modelType
-    #     else:
-    #         print("Invalid input type given for modelType\n\n")
-
     def objective(self, objective: str):
         """
         String.
         Objective of the experiment
         example:trainingObject.objective('Classify images using Convolutional Neural Networks (specifically, VGG16)
         pre-trained on the ImageNet dataset with Keras deep learning library.')
-
-
         """
         if type(objective) == str:
             self.__objective = objective
             self.__remove_error_method()
         else:
             error_msg = "Please enter a string in objective\n"
             self.__print_error(error_msg)
@@ -348,32 +336,28 @@
         Number of epochs to train the model.
         An epoch is an iteration over the entire data provided.
         Note that in conjunction with initial_epoch, epochs is to be understood as "final epoch".
         The model is not trained for a number of iterations given by epochs,
         but merely until the epoch of index epochs is reached.
         example: trainingObject.epochs(100)
         default: 10
-
-
         """
         if type(epochs) == int and epochs != 0:
             self.__epochs = epochs
             self.__remove_error_method()
         else:
             error_msg = "Invalid input type or value '0' given for epochs\n"
             self.__print_error(error_msg)
 
     def cycles(self, cycles: int):
         """
         Set number of cycles
         parameters: integer type values.
         example: trainingObject.cycles(10)
         default: 1
-
-
         """
         if type(cycles) == int and cycles != 0:
             self.__cycles = cycles
             self.__remove_error_method()
         else:
             self.__eligibility_passed = False
             error_msg = "Invalid input type or value '0' given for cycles\n"
@@ -400,16 +384,14 @@
             return batch
 
     def batchSize(self, batchSize: int):
         """
         Integer or None. Number of samples per gradient update. If unspecified, batch_size will default to 32.
         example: trainingObject.batchSize(16)
         default: 32
-
-
         """
         # get edge with lowest images
         edge_min = min(self.__total_images, key=self.__total_images.get)
         # get images count for selected edge
         images = int(self.__total_images[edge_min])
         # check for no of batches
         if type(batchSize) == int:
@@ -436,16 +418,14 @@
         return minimum
 
     def validation_split(self, validation_split: float):
         """
         Float. Fraction of images reserved for validation (strictly between 0 and 1).
         example: trainingObject.validation_split(0.2)
         default: 0.1
-
-
         """
         # calculate minimum validation split using the following equation
         # minimum = number of classes / total images
         # get edge with lowest images
         edge_min = min(self.__total_images, key=self.__total_images.get)
         images = int(self.__total_images[edge_min])
         minimum = round(self.__num_classes / images, 2)
@@ -459,37 +439,45 @@
 
     def optimizer(self, optimizer: str):
         """
         String (name of optimizer)
         example: trainingObject.optimizer('rmsprop')
         supported optimizers: ['adam','rmsprop','sgd','adadelta', 'adagrad', 'adamax','nadam', 'ftrl']
         default: 'sgd'
-
-
         """
-        o = ["adam", "rmsprop", "sgd", "adadelta", "adagrad", "adamax", "nadam", "ftrl"]
-        optlrrateflag = True
-        error = None
-        optimizer = optimizer.lower()
-        try:
-            o.index(optimizer)
-            if self.__learningRateSet:
-                optlrrateflag, error = check_parameters.get_optimizer(
-                    optimizer, self.__learningRate.copy()
-                )
-            if not optlrrateflag and error is not None:
-                error_msg = f"While setting optimiser error Occured as {error}"
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            o = ["adam", "rmsprop", "sgd", "adadelta", "adagrad", "adamax", "nadam", "ftrl"]
+            optlrrateflag = True
+            error = None
+            optimizer = optimizer.lower()
+            try:
+                o.index(optimizer)
+                if self.__learningRateSet:
+                    optlrrateflag, error = check_parameters.get_optimizer(
+                        optimizer, self.__learningRate.copy()
+                    )
+                if not optlrrateflag and error is not None:
+                    error_msg = f"While setting optimiser error Occurred as {error}"
+                    self.__print_error(error_msg)
+                else:
+                    self.__optimizer = optimizer
+                    self.__optimizerSet = True
+                    self.__remove_error_method()
+            except Exception as e:
+                error_msg = f"Please provide supported optimizers: {o}\n"
                 self.__print_error(error_msg)
-            else:
+        else:
+            o = ["adam", "rmsprop", "sgd", "adadelta", "adagrad", "adamax", "nadam", "ftrl"]
+            try:
+                o.index(optimizer)
                 self.__optimizer = optimizer
-                self.__optimizerSet = True
                 self.__remove_error_method()
-        except Exception as e:
-            error_msg = f"Please provide supported optimizers: {o}\n"
-            self.__print_error(error_msg)
+            except:
+                error_msg = f"Please provide supported optimizers: {o}\n"
+                self.__print_error(error_msg)
 
     def learningRate(self, learningRate: dict):
         """
         Set learning rate by passing a dictionary
         There are three different type of learningrate : constant, adaptive, custom
         default: {'type': 'constant', 'value': 0.0001}
         Set constant type learning rate for optimization.
@@ -505,51 +493,56 @@
         example:
         def custom_LearningRate_schedular(epoch):
             if epoch < 5:
                 return 0.01
             else:
                 return 0.01 * tf.math.exp(0.1 * (10 - epoch))
         trainingObject.learningRateCustom({'type': 'constant', 'value': custom_LearningRate_schedular, 'epoch': 4})
-
-
-
         """
-        optlrrateflag = True
-        error = None
-        if TYPE in learningRate.keys():
-            if self.__optimizerSet:
-                optlrrateflag, error = check_parameters.get_optimizer(
-                    self.__optimizer, learningRate.copy()
-                )
-            if not optlrrateflag:
-                error_msg = f"While setting Learning Rate error Occured as {error}"
-                self.__print_error(error_msg)
-            else:
-                if learningRate[TYPE] == CUSTOM and callable(learningRate[VALUE]):
-                    try:
-                        # Serialize the loss function
-                        serialized_data = learningRate
-                        # Encode the binary data as text
-                        encoded_data = base64.b64encode(serialized_data).decode("utf-8")
-                        self.__learningRate = {TYPE: CUSTOM, VALUE: encoded_data}
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            optlrrateflag = True
+            error = None
+            if TYPE in learningRate.keys():
+                if self.__optimizerSet:
+                    optlrrateflag, error = check_parameters.get_optimizer(
+                        self.__optimizer, learningRate.copy()
+                    )
+                if not optlrrateflag:
+                    error_msg = f"While setting Learning Rate error Occured as {error}"
+                    self.__print_error(error_msg)
+                else:
+                    if learningRate[TYPE] == CUSTOM and callable(learningRate[VALUE]):
+                        try:
+                            # Serialize the loss function
+                            serialized_data = learningRate
+                            # Encode the binary data as text
+                            encoded_data = base64.b64encode(serialized_data).decode("utf-8")
+                            self.__learningRate = {TYPE: CUSTOM, VALUE: encoded_data}
+                            self.__learningRateSet = True
+                            self.__remove_error_method()
+                        except Exception as e:
+                            error_msg = f"Error while setting custom learning rate : {e}\n"
+                            self.__print_error(error_msg)
+                    elif learningRate[TYPE] == CONSTANT or learningRate[TYPE] == ADAPTIVE:
+                        self.__learningRate = learningRate
                         self.__learningRateSet = True
                         self.__remove_error_method()
-                    except Exception as e:
-                        error_msg = f"Error while setting custom learning rate : {e}\n"
+                    else:
+                        error_msg = "Input not as per given convention for learningRate\n"
                         self.__print_error(error_msg)
-                elif learningRate[TYPE] == CONSTANT or learningRate[TYPE] == ADAPTIVE:
-                    self.__learningRate = learningRate
-                    self.__learningRateSet = True
-                    self.__remove_error_method()
-                else:
-                    error_msg = "Input not as per given convention for learningRate\n"
-                    self.__print_error(error_msg)
+            else:
+                error_msg = "Input not as per given convention for learningRate\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Input not as per given convention for learningRate\n"
-            self.__print_error(error_msg)
+            if learningRate[TYPE] == CONSTANT:
+                self.__learningRate = learningRate
+                self.__remove_error_method()
+            else:
+                error_msg = "Adaptive and Custom learning rate"
+                self.__not_supported_parameters(error_msg)
 
     def lossFunction(self, lossFunction: dict):
         """
         Set loss function
         parameters: string type values or custom loss function.
         default: {'type': 'standard', 'value':'categorical_crossentropy'}
 
@@ -569,179 +562,200 @@
 
             # summing both loss values along batch dimension
             loss = K.sum(loss, axis=1)        # (batch_size,)
 
             return loss
         trainingObject.lossFunctionCustom({'type': 'custom', 'value':custom_mse})
         """
-        l = ["binary_crossentropy", "categorical_crossentropy", "mse"]
-        if TYPE in lossFunction.keys() and VALUE in lossFunction.keys():
-            if lossFunction[TYPE] == STANDARD:
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            l = ["binary_crossentropy", "categorical_crossentropy", "mse"]
+            if TYPE in lossFunction.keys() and VALUE in lossFunction.keys():
+                if lossFunction[TYPE] == STANDARD:
+                    try:
+                        l.index(lossFunction[VALUE].lower())
+                        self.__lossFunction = lossFunction
+                        self.__remove_error_method()
+                    except:
+                        error_msg = f"Please provide tensorflow supported default loss functions losses: {l}\n"
+                        self.__print_error(error_msg)
+                elif lossFunction[TYPE] == CUSTOM:
+                    if callable(lossFunction[VALUE]):
+                        try:
+                            # Serialize the loss function
+                            serialized_data = dill.dumps(lossFunction[VALUE])
+                            # Encode the binary data as text
+                            encoded_data = base64.b64encode(serialized_data).decode("utf-8")
+
+                            try:
+                                # TODO: change the check model class according to framework used
+                                model_checks = TensorflowChecks(model=self.__model, model_name=self.__modelName, progress_bar=None)
+                                model_checks.small_training_loop(custom_loss=lossFunction)
+
+                                lossFunction[VALUE] = encoded_data
+                                self.__lossFunction = lossFunction
+                                self.__remove_error_method()
+                            except Exception as e:
+                                error_msg = f"custom loss provided give error as {e}\n"
+                                self.__print_error(error_msg)
+                                return
+                        except Exception as e:
+                            error_msg = (
+                                f"Please provide supported loss functions or custom loss build with tensorflow "
+                                f"supported default losses: {lossFunction}\n"
+                            )
+                            self.__print_error(error_msg)
+                else:
+                    error_msg = "Invalid input function given for loss function\n"
+                    self.__print_error(error_msg)
+            else:
+                error_msg = "type missing in lossfunction"
+                self.__print_error(error_msg)
+        else:
+            l = ["binary_crossentropy", "categorical_crossentropy", "mse"]
+            if TYPE in lossFunction.keys() and VALUE in lossFunction.keys() and lossFunction[TYPE] == STANDARD:
                 try:
                     l.index(lossFunction[VALUE].lower())
                     self.__lossFunction = lossFunction
                     self.__remove_error_method()
                 except:
                     error_msg = f"Please provide tensorflow supported default loss functions losses: {l}\n"
                     self.__print_error(error_msg)
-            elif lossFunction[TYPE] == CUSTOM:
-                if callable(lossFunction[VALUE]):
-                    try:
-                        # Serialize the loss function
-                        serialized_data = dill.dumps(lossFunction[VALUE])
-                        # Encode the binary data as text
-                        encoded_data = base64.b64encode(serialized_data).decode("utf-8")
-
-                        try:
-                            model_checks = CheckModel()
-                            model_checks.model = self.__model
-                            model_checks.small_training_loop(custom_loss=lossFunction)
-
-                            lossFunction[VALUE] = encoded_data
-                            self.__lossFunction = lossFunction
-                            self.__remove_error_method()
-                        except Exception as e:
-                            error_msg = f"custom loss provided give error as {e}\n"
-                            self.__print_error(error_msg)
-                            return
-                    except Exception as e:
-                        error_msg = (
-                            f"Please provide supported loss functions or custom loss build with tensorflow "
-                            f"supported default losses: {lossFunction}\n"
-                        )
-                        self.__print_error(error_msg)
             else:
-                error_msg = "Invalid input function given for loss function\n"
-                self.__print_error(error_msg)
-        else:
-            error_msg = "type missing in lossfunction"
-            self.__print_error(error_msg)
+                error_msg = "Custom loss function"
+                self.__not_supported_parameters(error_msg)
 
     def __getlayers(self):
         """
         load model and get all layers avaiable in model
         """
         isvalidlayers, model_layers = layer_instance_check(self.__model)
         return model_layers
 
     def layersFreeze(self, layersFreeze: list):
         """
         Provide name of layers in a list to be frozen before training a model.
         Get layers name in a model provided with the summary shown above.
         example: trainingObject.layersFreeze(['layer_name','layer_name', ...])
         default: None
-
-
         """
-        all_layers = self.__getlayers()
-        if type(layersFreeze) == list and all(
-            isinstance(sub, str) for sub in layersFreeze
-        ):
-            layers_eligible = True
-            for layer in layersFreeze:
-                if layer not in all_layers:
-                    layers_eligible = False
-            if layers_eligible:
-                layersFreeze = str(layersFreeze)
-                self.__layers_non_trainable = layersFreeze
-                self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            all_layers = self.__getlayers()
+            if type(layersFreeze) == list and all(
+                isinstance(sub, str) for sub in layersFreeze
+            ):
+                layers_eligible = True
+                for layer in layersFreeze:
+                    if layer not in all_layers:
+                        layers_eligible = False
+                if layers_eligible:
+                    layersFreeze = str(layersFreeze)
+                    self.__layers_non_trainable = layersFreeze
+                    self.__remove_error_method()
+                else:
+                    error_msg = f"Provide layers only which model contains for layersFreeze : {all_layers}\n"
+                    self.__print_error(error_msg)
             else:
-                error_msg = f"Provide layers only which model contains for layersFreeze : {all_layers}\n"
+                error_msg = "Provide values as list of strings for layersFreeze\n"
                 self.__print_error(error_msg)
         else:
-            error_msg = "Provide values as list of strings for layersFreeze\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("layersFreeze")
 
     def terminateOnNaNCallback(self):
         """
         Callback that terminates training when a NaN loss is encountered.
         example: trainingObject.terminateOnNaNCallback()
-
-
         """
-        c = [""]
-        self.__terminateOnNaNCallback["terminateOnNaN"] = c
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            c = [""]
+            self.__terminateOnNaNCallback["terminateOnNaN"] = c
+        else:
+            self.__not_supported_parameters("terminateOnNaNCallback")
 
     def modelCheckpointCallback(self, monitor: str, save_best_only: bool):
         """
         Callback to save the model weights. parameters: monitor: Quantity to be monitored, save_best_only:  if
         save_best_only=True, it only saves when the model is considered the "best" and the latest best model
         according to the quantity monitored will not be overwritten. example: trainingObject.modelCheckpointCallback(
         'val_loss', True)
-
-
         """
-        f = ["accuracy", "loss", "val_loss", "val_accuracy"]
-        try:
-            f.index(monitor.lower())
-            if type(save_best_only) == bool:
-                c = [monitor, save_best_only]
-                self.__modelCheckpointCallback["modelCheckpoint"] = c
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid datatype for arguments given for save_best_only\n"
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            f = ["accuracy", "loss", "val_loss", "val_accuracy"]
+            try:
+                f.index(monitor.lower())
+                if type(save_best_only) == bool:
+                    c = [monitor, save_best_only]
+                    self.__modelCheckpointCallback["modelCheckpoint"] = c
+                    self.__remove_error_method()
+                else:
+                    error_msg = "Invalid datatype for arguments given for save_best_only\n"
+                    self.__print_error(error_msg)
+            except:
+                error_msg = f"Please provide supported monitor values: {f}\n"
                 self.__print_error(error_msg)
-        except:
-            error_msg = f"Please provide supported monitor values: {f}\n"
-            self.__print_error(error_msg)
+        else:
+            self.__not_supported_parameters("modelCheckpointCallback")
 
     def earlystopCallback(self, monitor: str, patience: int):
         """
         Stop training when a monitored metric has stopped improving.
         parameters: monitor: Quantity to be monitored,
                                 patience: Number of epochs with no improvement after which training will be stopped.
         example: trainingObject.earlystopCallback('loss', 10)
 
 
         """
-        f = ["accuracy", "loss", "val_loss", "val_accuracy"]
-        try:
-            f.index(monitor.lower())
-            if type(patience) == int:
-                c = [monitor, patience]
-                self.__earlystopCallback["earlystopping"] = c
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid datatype for arguments given for patience\n"
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            f = ["accuracy", "loss", "val_loss", "val_accuracy"]
+            try:
+                f.index(monitor.lower())
+                if type(patience) == int:
+                    c = [monitor, patience]
+                    self.__earlystopCallback["earlystopping"] = c
+                    self.__remove_error_method()
+                else:
+                    error_msg = "Invalid datatype for arguments given for patience\n"
+                    self.__print_error(error_msg)
+            except:
+                error_msg = f"Please provide supported monitor values: {f}\n"
                 self.__print_error(error_msg)
-        except:
-            error_msg = f"Please provide supported monitor values: {f}\n"
-            self.__print_error(error_msg)
+        else:
+            self.__not_supported_parameters("earlystopCallback")
 
     def reducelrCallback(
         self, monitor: str, factor: float, patience: int, min_delta: float
     ):
         """
         Reduce learning rate when a metric has stopped improving. parameters: monitor: Quantity to be monitored,
         factor: factor by which the learning rate will be reduced. new_lr = lr * factor. patience: number of epochs
         with no improvement after which learning rate will be reduced. min_delta: threshold for measuring the new
         optimum, to only focus on significant changes.
         example: trainingObject.reducelrCallback('loss', 0.1, 10, 0.0001)
-
-
         """
-        f = ["accuracy", "loss", "val_loss", "val_accuracy"]
-        try:
-            f.index(monitor.lower())
-            if (
-                type(factor) == float
-                and type(patience) == int
-                and type(min_delta) == float
-            ):
-                c = [monitor, factor, patience, min_delta]
-                self.__reducelrCallback["reducelr"] = c
-                self.__remove_error_method()
-            else:
-                error_msg = (
-                    "Invalid datatype for arguments given for reducelrCallback\n"
-                )
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            f = ["accuracy", "loss", "val_loss", "val_accuracy"]
+            try:
+                f.index(monitor.lower())
+                if (
+                    type(factor) == float
+                    and type(patience) == int
+                    and type(min_delta) == float
+                ):
+                    c = [monitor, factor, patience, min_delta]
+                    self.__reducelrCallback["reducelr"] = c
+                    self.__remove_error_method()
+                else:
+                    error_msg = (
+                        "Invalid datatype for arguments given for reducelrCallback\n"
+                    )
+                    self.__print_error(error_msg)
+            except:
+                error_msg = f"Please provide supported monitor values: {f}\n"
                 self.__print_error(error_msg)
-        except:
-            error_msg = f"Please provide supported monitor values: {f}\n"
-            self.__print_error(error_msg)
+        else:
+            self.__not_supported_parameters("reducelrCallback")
 
     def __setCallbacks(self):
         """
         List of dictionaries.
         List of tensorflow callbacks for training.
         default: []
         """
@@ -753,331 +767,386 @@
         if len(self.__modelCheckpointCallback) != 0:
             c.append(self.__modelCheckpointCallback)
         if len(self.__terminateOnNaNCallback) != 0:
             c.append(self.__terminateOnNaNCallback)
 
         self.__callbacks = str(c)
 
-    # def stepsPerEpoch(self, stepsPerEpoch: int):
-    #     """
-    #     Integer.
-    #     Total number of steps (batches of samples) before declaring
-    #     one epoch finished and starting the next epoch.
-    #     example: setStepsPerEpoch(5)
-    #     default: None
-    #     """
-    #     if type(stepsPerEpoch) == int and stepsPerEpoch >= 15:
-    #         self.__stepsPerEpoch = stepsPerEpoch
-    #     else:
-    #         print(
-    #             "Invalid input type or value less than 15 given for stepsPerEpoch\n\n"
-    #         )
-
-    # def initialEpoch(self, initialEpoch: int):
-    #     """
-    #     Integer. Epoch at which to start training
-    #     (useful for resuming a previous training run).
-    #     example: setInitialEpoch(2)
-    #     default: 0
-    #     """
-    #     if type(initialEpoch) == int:
-    #         self.__initialEpoch = initialEpoch
-    #     else:
-    #         print("Invalid input type given for initialEpoch\n\n")
-
-    # def validationSteps(self, validationSteps: int):
-    #     """
-    #     Integer. Total number of steps (batches of samples) to draw before stopping
-    #     when performing validation at the end of every epoch.
-    #     example: setValidationSteps(20)
-    #     default: None
-    #     """
-    #     if type(validationSteps) == int and validationSteps >= 15:
-    #         self.__validationSteps = validationSteps
-    #     else:
-    #         print(
-    #             "Invalid input type or value less than 15 given for validationSteps\n\n"
-    #         )
-    # def featurewise_center(self, featurewise_center: bool):
-    #     """
-    #     Boolean. Set input mean to 0 over the dataset, feature-wise.
-    #     example: trainingObject.featurewise_center(True)
-    #     default: False
-    #
-    #
-    #     """
-    #     if type(featurewise_center) == bool:
-    #         self.__featurewise_center = featurewise_center
-    #     else:
-    #         print("Invalid input type given for featurewise_center\n\n")
-
     def samplewise_center(self, samplewise_center: bool):
         """
         Boolean. Set each sample mean to 0.
         example: trainingObject.samplewise_center(True)
         default: False
-
-
         """
-        if type(samplewise_center) == bool:
-            self.__samplewise_center = samplewise_center
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(samplewise_center) == bool:
+                self.__samplewise_center = samplewise_center
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for samplewise_center\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for samplewise_center\n"
-            self.__print_error(error_msg)
-
-    # def featurewise_std_normalization(self, featurewise_std_normalization: bool):
-    #     """
-    #     Boolean. Divide inputs by std of the dataset, feature-wise.
-    #     example: trainingObject.featurewise_std_normalization(True)
-    #     default: False
-    #
-    #
-    #     """
-    #     if type(featurewise_std_normalization) == bool:
-    #         self.__featurewise_std_normalization = featurewise_std_normalization
-    #     else:
-    #         print("Invalid input type given for featurewise_std_normalization\n\n")
+            self.__not_supported_parameters("samplewise_center")
 
     def samplewise_std_normalization(self, samplewise_std_normalization: bool):
         """
         Boolean. Divide each input by its std.
         example: trainingObject.samplewise_std_normalization(True)
         default: False
-
-
         """
-        if type(samplewise_std_normalization) == bool:
-            self.__samplewise_std_normalization = samplewise_std_normalization
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(samplewise_std_normalization) == bool:
+                self.__samplewise_std_normalization = samplewise_std_normalization
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for samplewise_std_normalization\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for samplewise_std_normalization\n"
-            self.__print_error(error_msg)
-
-    # def zca_whitening(self, zca_whitening: bool):
-    #     """
-    #     Boolean. Apply ZCA whitening.
-    #     example: trainingObject.zca_whitening(True)
-    #     default: False
-    #
-    #
-    #     """
-    #     if type(zca_whitening) == bool:
-    #         self.__zca_whitening = zca_whitening
-    #     else:
-    #         print("Invalid input type given for zca_whitening\n\n")
+            self.__not_supported_parameters("samplewise_std_normalization")
 
     def rotation_range(self, rotation_range: int):
         """
         Int. Degree range for random rotations.
         example: trainingObject.rotation_range(2)
         default: 0
-
-
         """
-        if type(rotation_range) == int:
-            self.__rotation_range = rotation_range
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(rotation_range) == int:
+                self.__rotation_range = rotation_range
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for rotation_range\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for rotation_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("rotation_range")
 
     def width_shift_range(self, width_shift_range):
         """
         Float or int
         float: fraction of total width, if < 1, or pixels if >= 1.
         int: integer number of pixels from interval (-width_shift_range, +width_shift_range)
         With width_shift_range=2 possible values are integers [-1, 0, +1], same as with width_shift_range=[-1, 0, +1],
         while with width_shift_range=1.0 possible values are floats in the interval [-1.0, +1.0).
         example: trainingObject.width_shift_range(0.1)
         default: 0.0
-
-
         """
-        if type(width_shift_range) == float or type(width_shift_range) == int:
-            self.__width_shift_range = width_shift_range
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(width_shift_range) == float or type(width_shift_range) == int:
+                self.__width_shift_range = width_shift_range
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for width_shift_range\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for width_shift_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("width_shift_range")
 
     def height_shift_range(self, height_shift_range):
         """
         Float or int
         float: fraction of total height, if < 1, or pixels if >= 1.
         int: integer number of pixels from interval (-height_shift_range, +height_shift_range)
         With height_shift_range=2 possible values are integers [-1, 0, +1], same as with height_shift_range=[-1, 0, +1],
         while with height_shift_range=1.0 possible values are floats in the interval [-1.0, +1.0).
         example: trainingObject.height_shift_range(0.1)
         default: 0.0
-
-
         """
-        if type(height_shift_range) == float or type(height_shift_range) == int:
-            self.__height_shift_range = height_shift_range
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(height_shift_range) == float or type(height_shift_range) == int:
+                self.__height_shift_range = height_shift_range
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for height_shift_range\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for height_shift_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("height_shift_range")
 
     def brightness_range(self, brightness_range):
         """
         Tuple or list of two floats. Range for picking a brightness shift value from.
         example: trainingObject.brightness_range((0.1,0.4))
         default: None
-
-
         """
-        if (type(brightness_range) == tuple and len(brightness_range) == 2) or (
-            type(brightness_range) == list and len(brightness_range)
-        ) == 2:
-
-            if (
-                type(brightness_range[0]) == float
-                and type(brightness_range[1]) == float
-            ):
-                brightness_range = str(brightness_range)
-                self.__brightness_range = brightness_range
-                self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if (type(brightness_range) == tuple and len(brightness_range) == 2) or (
+                type(brightness_range) == list and len(brightness_range)
+            ) == 2:
+
+                if (
+                    type(brightness_range[0]) == float
+                    and type(brightness_range[1]) == float
+                ):
+                    brightness_range = str(brightness_range)
+                    self.__brightness_range = brightness_range
+                    self.__remove_error_method()
+                else:
+                    error_msg = "provide float values for brightness_range\n"
+                    self.__print_error(error_msg)
             else:
-                error_msg = "provide float values for brightness_range\n"
+                error_msg = "Please provide tuple of two floats for brightness_range\n"
                 self.__print_error(error_msg)
         else:
-            error_msg = "Please provide tuple of two floats for brightness_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("brightness_range")
 
     def shear_range(self, shear_range: float):
         """
         Float. Shear Intensity (Shear angle in counter-clockwise direction in degrees)
         example: trainingObject.shear_range(0.2)
         default: 0.0
-
-
         """
-        if type(shear_range) == float:
-            self.__shear_range = shear_range
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(shear_range) == float:
+                self.__shear_range = shear_range
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for shear_range\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for shear_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("shear_range")
 
     def zoom_range(self, zoom_range):
         """
         Float or [lower, upper]. Range for random zoom. If a float, [lower, upper] = [1-zoom_range, 1+zoom_range].
         example: trainingObject.zoom_range(0.2)
         default: 0.0
-
-
         """
-        if type(zoom_range) == float or type(zoom_range) == list:
-            self.__zoom_range = zoom_range
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(zoom_range) == float or type(zoom_range) == list:
+                self.__zoom_range = zoom_range
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for zoom_range\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for zoom_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("zoom_range")
 
     def channel_shift_range(self, channel_shift_range: float):
         """
         Float. Range for random channel shifts.
         example: trainingObject.channel_shift_range(0.4)
         default: 0.0
-
-
         """
-        if type(channel_shift_range) == float:
-            self.__channel_shift_range = channel_shift_range
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(channel_shift_range) == float:
+                self.__channel_shift_range = channel_shift_range
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for channel_shift_range\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for channel_shift_range\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("channel_shift_range")
 
     def fill_mode(self, fill_mode: str):
         """
         One of {"constant", "nearest", "reflect" or "wrap"}. Default is 'nearest'.
         Points outside the boundaries of the input are filled according to the given mode:
         'constant': kkkkkkkk|abcd|kkkkkkkk (cval=k)
         'nearest': aaaaaaaa|abcd|dddddddd
         'reflect': abcddcba|abcd|dcbaabcd
         'wrap': abcdabcd|abcd|abcdabcd
         example: trainingObject.fill_mode("nearest")
         default: "nearest"
-
-
         """
-        f = ["constant", "nearest", "reflect", "wrap"]
-        try:
-            f.index(fill_mode.lower())
-            self.__fill_mode = fill_mode.lower()
-            self.__remove_error_method()
-        except:
-            error_msg = f"Please provide supported fill modes: {f}\n"
-            self.__print_error(error_msg)
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            f = ["constant", "nearest", "reflect", "wrap"]
+            try:
+                f.index(fill_mode.lower())
+                self.__fill_mode = fill_mode.lower()
+                self.__remove_error_method()
+            except:
+                error_msg = f"Please provide supported fill modes: {f}\n"
+                self.__print_error(error_msg)
+        else:
+            self.__not_supported_parameters("fill_mode")
 
     def cval(self, cval: float):
         """
         Float or Int. Value used for points outside the boundaries when fill_mode = "constant".
         example: trainingObject.cval(0.3)
         default: 0.0
-
-
         """
-        if type(cval) == float:
-            self.__cval = cval
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(cval) == float:
+                self.__cval = cval
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for cval\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for cval\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("cval")
 
     def horizontal_flip(self, horizontal_flip: bool):
         """
         Boolean. Randomly flip inputs horizontally.
         example: trainingObject.horizontal_flip(True)
         default: False
-
-
         """
-        if type(horizontal_flip) == bool:
-            self.__horizontal_flip = horizontal_flip
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(horizontal_flip) == bool:
+                self.__horizontal_flip = horizontal_flip
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for horizontal_flip\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for horizontal_flip\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("horizontal_flip")
 
     def vertical_flip(self, vertical_flip: bool):
         """
         Boolean. Randomly flip inputs vertically.
         example: trainingObject.vertical_flip(True)
         default: False
-
-
         """
-        if type(vertical_flip) == bool:
-            self.__vertical_flip = vertical_flip
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(vertical_flip) == bool:
+                self.__vertical_flip = vertical_flip
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for vertical_flip\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for vertical_flip\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("vertical_flip")
 
     def rescale(self, rescale: float):
         """
         rescaling factor. Defaults to None. If None, no rescaling is applied,
         otherwise we multiply the data by the value provided (after applying all other transformations).
         example: trainingObject.rescale(0.003921568627)
         default: None
+        """
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(rescale) == float:
+                self.__rescale = rescale
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for rescale\n"
+                self.__print_error(error_msg)
+        else:
+            self.__not_supported_parameters("rescale")
 
-
+    def shuffle(self, shuffle: bool):
         """
-        print("\n")
-        if type(rescale) == float:
-            self.__rescale = rescale
-            self.__remove_error_method()
+        whether to shuffle the data (default: True)
+        example: trainingObject.shuffle(False)
+        default: True
+        """
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(shuffle) == bool:
+                self.__shuffle = shuffle
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type given for shuffle\n"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type given for rescale\n"
-            self.__print_error(error_msg)
+            self.__not_supported_parameters("shuffle")
 
+    # def category(self, category: str):
+    #     """
+    #     String.
+    #     Category of experiment, like classification
+    #     example:trainingObject.category('classification')
+    #     default_value: 'Classification'
+    #
+    #     """
+    #     if type(category) == str:
+    #         self.__category = category
+    #     else:
+    #         print("Invalid input type given for category\n\n")
+    #
+    # def modelType(self, modelType: str):
+    #     """
+    #     String.
+    #     Type of model used in the experiment, like VGGNET
+    #     example:trainingObject.modelType('VGGNET')
+    #
+    #
+    #     """
+    #     if type(modelType) == str:
+    #         self.__modelType = modelType
+    #     else:
+    #         print("Invalid input type given for modelType\n\n")
+    #
+    # def stepsPerEpoch(self, stepsPerEpoch: int):
+    #     """
+    #     Integer.
+    #     Total number of steps (batches of samples) before declaring
+    #     one epoch finished and starting the next epoch.
+    #     example: setStepsPerEpoch(5)
+    #     default: None
+    #     """
+    #     if type(stepsPerEpoch) == int and stepsPerEpoch >= 15:
+    #         self.__stepsPerEpoch = stepsPerEpoch
+    #     else:
+    #         print(
+    #             "Invalid input type or value less than 15 given for stepsPerEpoch\n\n"
+    #         )
+    #
+    # def initialEpoch(self, initialEpoch: int):
+    #     """
+    #     Integer. Epoch at which to start training
+    #     (useful for resuming a previous training run).
+    #     example: setInitialEpoch(2)
+    #     default: 0
+    #     """
+    #     if type(initialEpoch) == int:
+    #         self.__initialEpoch = initialEpoch
+    #     else:
+    #         print("Invalid input type given for initialEpoch\n\n")
+    #
+    # def validationSteps(self, validationSteps: int):
+    #     """
+    #     Integer. Total number of steps (batches of samples) to draw before stopping
+    #     when performing validation at the end of every epoch.
+    #     example: setValidationSteps(20)
+    #     default: None
+    #     """
+    #     if type(validationSteps) == int and validationSteps >= 15:
+    #         self.__validationSteps = validationSteps
+    #     else:
+    #         print(
+    #             "Invalid input type or value less than 15 given for validationSteps\n\n"
+    #         )
+    # def featurewise_center(self, featurewise_center: bool):
+    #     """
+    #     Boolean. Set input mean to 0 over the dataset, feature-wise.
+    #     example: trainingObject.featurewise_center(True)
+    #     default: False
+    #
+    #
+    #     """
+    #     if type(featurewise_center) == bool:
+    #         self.__featurewise_center = featurewise_center
+    #     else:
+    #         print("Invalid input type given for featurewise_center\n\n")
+    #
+    # def featurewise_std_normalization(self, featurewise_std_normalization: bool):
+    #     """
+    #     Boolean. Divide inputs by std of the dataset, feature-wise.
+    #     example: trainingObject.featurewise_std_normalization(True)
+    #     default: False
+    #
+    #
+    #     """
+    #     if type(featurewise_std_normalization) == bool:
+    #         self.__featurewise_std_normalization = featurewise_std_normalization
+    #     else:
+    #         print("Invalid input type given for featurewise_std_normalization\n\n")
+    #
+    # def zca_whitening(self, zca_whitening: bool):
+    #     """
+    #     Boolean. Apply ZCA whitening.
+    #     example: trainingObject.zca_whitening(True)
+    #     default: False
+    #
+    #
+    #     """
+    #     if type(zca_whitening) == bool:
+    #         self.__zca_whitening = zca_whitening
+    #     else:
+    #         print("Invalid input type given for zca_whitening\n\n")
+    #
     # def data_format(self, data_format: str):
     #     """
     #     String.
     #     Image data format, either "channels_first" or "channels_last".
     #     "channels_last" mode means that the images should have shape
     #     (samples, height, width, channels),
     #     "channels_first" mode means that the images should have shape
@@ -1087,57 +1156,43 @@
     #     """
     #     d = ["channels_last"]
     #     try:
     #         d.index(data_format.lower())
     #         self.__data_format = data_format.lower()
     #     except:
     #         print(f"Please provide supported fill modes: {d}\n\n")
+    #
     # def dtype(self, dtype: str):
     #     """
     #     String.
     #     Dtype to use for the generated arrays.
     #     example: dtype('float32')
     #     default: None
     #     """
     #     d = ["float32", "float64"]
     #     try:
     #         d.index(dtype.lower())
     #         self.__dtype = dtype.lower()
     #     except:
     #         print(f"Please provide supported fill modes: {d}\n\n")
-
-    def shuffle(self, shuffle: bool):
-        """
-        whether to shuffle the data (default: True)
-        example: trainingObject.shuffle(False)
-        default: True
-
-
-        """
-        if type(shuffle) == bool:
-            self.__shuffle = shuffle
-            self.__remove_error_method()
-        else:
-            error_msg = "Invalid input type given for shuffle\n"
-            self.__print_error(error_msg)
-
+    #
     # def metrics(self,metrics:list):
     # 	'''
     # 	List of strings.
     # 	List of metrics to be evaluated by the model
     # 	during training and testing.
     # 	example: setMetrics(['accuracy','mse'])
     # 	default: ['accuracy']
     # 	'''
     # 	if type(metrics)== list and all(isinstance(sub, str) for sub in metrics):
     # 		metrics = str(metrics)
     # 		self.__metrics = metrics
     # 	else:
     # 		print("Provide values as list of strings")
-
+    #
     # 	def __display_time(self,seconds, granularity=5):
     # 		intervals = (
     # 		('weeks', 604800),  # 60 * 60 * 24 * 7
     # 		('days', 86400),    # 60 * 60 * 24
     # 		('hours', 3600),    # 60 * 60
     # 		('minutes', 60),
     # 		('seconds', 1),)
@@ -1147,15 +1202,15 @@
     # 			value = seconds // count
     # 			if value:
     # 				seconds -= value * count
     # 				if value == 1:
     # 					name = name.rstrip('s')
     # 				result.append("{} {}".format(value, name))
     # 		return ', '.join(result[:granularity])
-
+    #
     # 	def getEstimate(self):
     #
     # 		header = {'Authorization' : f"Token {self.__token}"}
     # 		re = requests.post(f"{self.__url}flops/",headers= header,data={'datasetId':self.__datasetId,
     # 			'batchSize':self.__batchSize,'noOfEpochs':self.__epochs,'modelName':self.__modelName})
     # # 		print(re.status_code)
     # 		if re.status_code == 200:
@@ -1294,14 +1349,15 @@
             "upperboundTime": self.__upperboundTime,
             "callbacks": self.__callbacks,
             "pre_trained_weights": self.__weights,
             "subdataset": self.__subdataset,
             "images_per_class": self.__images_per_class,
             "image_shape": self.__image_shape,
             "image_type": self.__image_type,
+            "framework": self.__framework,
         }
 
         return parameters
 
     def getTrainingPlan(self):
         if self.__eligibility_passed:
             print(
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/messages.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/upload.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
-
+import torch
 import requests, json, pickle
 from importlib.machinery import SourceFileLoader
 from termcolor import colored
 import os
 import rich
 from tqdm import tqdm
 from .utils import *
-from .functional_test import CheckModel
+from .functional_test import CheckModel, TensorflowChecks, TorchChecks
 
 # hide warnings from tensorflow
 import warnings
 
 warnings.filterwarnings("ignore")
 
 
@@ -24,14 +24,15 @@
 
     """
 
     def __init__(self, modelname, token, weights=False, url=""):
         self.__modelname = ""
         self.__model_path = ""
         self.__weights_path = ""
+        self.__framework = TENSORFLOW_FRAMEWORK
         self.__ext = ".py"
         self.model = None
         self.__get_paths(modelname)
         self.__token = token
         self.weights = weights
         self.__url = url + "upload/"
         self.__check_model_url = url + "check-model/"
@@ -70,59 +71,100 @@
     def getNewModelId(self):
         if self.__recievedModelname is not None:
             return (
                 self.__recievedModelname,
                 self.__modelname,
                 self.__ext,
                 self.__model_path,
+                self.__framework,
             )
 
     def upload(self):
         # load model from current directory
+        status = False
+        message = None
+        # create progress bar with total number of nested functions
+        self.progress_bar = tqdm(total=8, desc="Model Upload Progress")
         try:
-            status = False
-            message = None
-            # create progress bar with total number of nested functions
-            progress_bar = tqdm(total=9, desc='Model Upload Progress')
             # call check model class for model checks
-            model_checks = CheckModel(
-                progress_bar, model_name=self.__modelname, model_path=self.__model_path,
+            model_checks_generic = CheckModel(
+                self.progress_bar,
+                model_name=self.__modelname,
+                model_path=self.__model_path,
             )
-            status, message, model_name, progress_bar = model_checks.model_func_checks()
+            (
+                status,
+                message,
+                model_name,
+                progress_bar,
+            ) = model_checks_generic.model_func_checks()
             if not status:
-                text = colored(message, "red", )
+                model_checks_generic.remove_tmp_file()
+                text = colored(
+                    message,
+                    "red",
+                )
                 print(text, "\n")
-                progress_bar.close()
+                self.progress_bar.close()
                 return None
-            else:
-                self.model = model_checks.model
-                updated_model_name = self.__upload_model()
-                progress_bar.update(1)
-                progress_bar.close()
-                return updated_model_name
+            loaded_model = model_checks_generic.model
+            self.__framework = model_checks_generic.framework
+            model_check_class = TensorflowChecks
+            if self.__framework == PYTORCH_FRAMEWORK:
+                model_check_class = TorchChecks
+            elif self.__framework == TENSORFLOW_FRAMEWORK:
+                model_check_class = TensorflowChecks
+            model_checks = model_check_class(
+                model=loaded_model,
+                model_name=model_name,
+                progress_bar=self.progress_bar,
+            )
+            (
+                status,
+                message,
+                model_name,
+                progress_bar,
+            ) = model_checks.model_func_checks()
+            if not status:
+                model_checks_generic.remove_tmp_file()
+                text = colored(
+                    message,
+                    "red",
+                )
+                print(text, "\n")
+                self.progress_bar.close()
+                return None
+            self.progress_bar.update(1)
+            model_checks_generic.remove_tmp_file(update_progress_bar=True)
+            self.model = model_checks.model
+            updated_model_name = self.__upload_model()
+            self.progress_bar.close()
+            return updated_model_name
         except FileNotFoundError:
             text = colored(
                 f"\nUpload failed. There is no model with the name '{self.__modelname}' in your folder '{os.getcwd()}'.",
                 "red",
             )
             print(text, "\n")
             rich.print(
                 "For more information check the [link=https://docs.tracebloc.io/user-uploadModel]docs[/link]"
             )
-            progress_bar.close()
+            self.progress_bar.close()
             return None
         except Exception as e:
             text = colored(
                 f"\nUpload failed.",
                 "red",
             )
             print(text, "\n")
             if self.__url != "https://tracebloc.azurewebsites.net/":
-                print(f"Error in Upload is {e} at {sys.exc_info()[-1].tb_lineno} with message : {message}")
-            progress_bar.close()
+                print(
+                    f"Error in Upload is {e} at {sys.exc_info()[-1].tb_lineno} with message : {message}"
+                )
+            self.progress_bar.close()
             return None
 
     def __upload_model(self):
         model_file = open(self.__model_path, "rb")
         if self.weights:
             w = self.checkWeights()
             if not w:
@@ -148,17 +190,21 @@
         )
         model_file.close()
         body_unicode = r.content.decode("utf-8")
         content = json.loads(body_unicode)
         text = content["text"]
         check_status = content["check_status"]
         if not check_status:
-            tex = colored(text, "red", )
+            tex = colored(
+                text,
+                "red",
+            )
             print(tex, "\n")
             return None
+        self.progress_bar.update(1)
         return content["model_name"]
 
     def checkWeights(self):
         # load model weights from current directory
         try:
             weights_file = open(self.__weights_path, "rb")
         except FileNotFoundError:
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/user.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         if r.status_code == 200:
             print(f"\nLogged in as {self.__username}")
             token = json.loads(r.text)["token"]
             return token
         else:
             print("\n")
             text = colored(
-                "Login credentials are not correct. Please try again.", "red",
+                "Login credentials are not correct. Please try again.",
+                "red",
             )
             print(text, "\n")
             return ""
 
     def logout(self):
         """Call this to logout from current sesion"""
         try:
@@ -117,14 +118,15 @@
             self.__modelName = modelname
             modelobj = Model(self.__modelName, self.__token, self.__weights, self.__url)
             (
                 self.__modelId,
                 self.__modelName,
                 self.__ext,
                 path,
+                self.__framework,
             ) = modelobj.getNewModelId()
             self.__model = modelobj.model
             if self.__modelId == "" or self.__modelId is None:
                 text = colored(f"'{self.__modelName}' upload Failed.", "red")
                 print(text, "\n")
                 self.__weights = False
                 return
@@ -168,14 +170,15 @@
                     self.__weights,
                     self.__totalDatasetSize,
                     self.__total_images,
                     self.__num_classes,
                     self.__class_names,
                     self.__url,
                     self.__environment,
+                    self.__framework,
                 )
             else:
                 return None
         except:
             text = colored("Model Link Failed!", "red")
             print(text, "\n")
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/utils.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 import tensorflow_datasets as tfds
 import tensorflow as tf
+import torch
+import torchvision
+import torchvision.transforms as transforms
 import numpy as np
 from tensorflow_datasets.testing import mock_data
 from importlib.machinery import SourceFileLoader
 import base64
 import ast
 
 
+TENSORFLOW_FRAMEWORK = "tensorflow"
+PYTORCH_FRAMEWORK = "pytorch"
+CONSTANT = "constant"
+STANDARD = "standard"
+ADAPTIVE = "adaptive"
+CUSTOM = "custom"
+TYPE = "type"
+FUNCTION = "function"
+VALUE = "value"
+
 def check_MyModel(filename, path):
     try:
         # check if file contains the MyModel function
         model = SourceFileLoader(filename, f"{path}").load_module()
         model.MyModel(input_shape=(500, 500, 3), classes=10)
         return True, model
 
@@ -121,7 +134,60 @@
 
 
 def getImagesCount(images_count):
     count = 0
     for key in images_count.keys():
         count += images_count[key]
     return count
+
+
+def mock_dataset(classes):
+    num_examples = 3
+
+    def as_dataset(self, *args, **kwargs):
+        return tf.data.Dataset.from_generator(  # pragma: no cover
+            lambda: (
+                {
+                    "image": np.ones(shape=(256, 256, 3), dtype=np.uint8),
+                    "label": classes,
+                }
+                for i in range(num_examples)
+            ),
+            output_types=self.info.features.tf_dtype,
+            output_shapes=self.info.features.shape,
+        )
+
+    with mock_data(as_dataset_fn=as_dataset):
+        (ds_train, ds_test), ds_info = tfds.load(
+            "deep_weeds",
+            split=["train", "test"],
+            shuffle_files=True,
+            as_supervised=True,
+            with_info=True,
+        )
+
+    ds_train = ds_train.map(normalize_img, num_parallel_calls=tf.data.AUTOTUNE)
+    ds_train = ds_train.batch(8)
+    ds_train = ds_train.prefetch(tf.data.AUTOTUNE)
+    return ds_train
+
+
+def normalize_img(image, label):
+    """Normalizes images: `uint8` -> `float32`."""
+    return tf.cast(image, tf.float32) / 255.0, label  # pragma: no cover
+
+
+def test_code():
+    main_method = "MyModel"
+    input_shape = "input_shape"
+    output_classes = "output_classes"
+
+    def MyModel(input_shape=(224, 224, 3), output_classes=3):
+        base_mobilenet_model = MobileNet(
+            input_shape=input_shape, include_top=False, weights=None
+        )
+        multi_disease_model = Sequential()
+        multi_disease_model.add(base_mobilenet_model)
+        multi_disease_model.add(GlobalAveragePooling2D())
+        multi_disease_model.add(Dropout(0.5))
+        multi_disease_model.add(Dense(output_classes, activation="sigmoid"))
+        return multi_disease_model
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package/weights.py` & `tracebloc_package-dev-0.3.9/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

