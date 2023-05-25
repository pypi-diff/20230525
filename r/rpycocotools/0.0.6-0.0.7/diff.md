# Comparing `tmp/rpycocotools-0.0.6.tar.gz` & `tmp/rpycocotools-0.0.7.tar.gz`

## Comparing `rpycocotools-0.0.6.tar` & `rpycocotools-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,59 @@
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.toml
--rw-r--r--   0     1001      123       30 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/.gitignore
--rw-r--r--   0     1001      123    55307 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.lock
--rw-r--r--   0     1001      123     1088 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/README.md
--rw-r--r--   0     1001      123     1186 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/argparse.rs
--rw-r--r--   0     1001      123    19128 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/object_detection.rs
--rw-r--r--   0     1001      123     8344 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/pyo3.rs
--rw-r--r--   0     1001      123      181 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/coco.rs
--rw-r--r--   0     1001      123     3017 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/errors.rs
--rw-r--r--   0     1001      123     1901 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/lib.rs
--rw-r--r--   0     1001      123     1510 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/main.rs
--rw-r--r--   0     1001      123    23262 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/conversions.rs
--rw-r--r--   0     1001      123     6222 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/utils.rs
--rw-r--r--   0     1001      123      230 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/mask.rs
--rw-r--r--   0     1001      123      724 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/utils.rs
--rw-r--r--   0     1001      123     2296 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/display.rs
--rw-r--r--   0     1001      123     6037 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/draw.rs
--rw-r--r--   0     1001      123      141 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize.rs
--rw-r--r--   0     1001      123      610 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/tests/load_coco.rs
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.6/Cargo.toml
--rw-r--r--   0     1001      123      173 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/.gitignore
--rw-r--r--   0     1001      123       58 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/.rustfmt.toml
--rw-r--r--   0     1001      123    45992 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/Cargo.lock
--rw-r--r--   0     1001      123     2289 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/README.md
--rw-r--r--   0     1001      123       10 2023-05-17 13:28:34.000000 rpycocotools-0.0.6/dist/rpycocotools-0.0.6.tar.gz
--rw-r--r--   0     1001      123      634 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/Makefile
--rw-r--r--   0     1001      123        0 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/_static/.gitkeep
--rw-r--r--   0     1001      123     1572 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/conf.py
--rw-r--r--   0     1001      123     9389 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/dataset.rst
--rw-r--r--   0     1001      123      623 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/examples.rst
--rw-r--r--   0     1001      123      731 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/index.rst
--rw-r--r--   0     1001      123      800 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/make.bat
--rw-r--r--   0     1001      123      101 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/quickstart.rst
--rw-r--r--   0     1001      123     2943 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/segmentation_masks.rst
--rw-r--r--   0     1001      123     4234 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/pyproject.toml
--rw-r--r--   0     1001      123      171 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/python/rpycocotools/__init__.py
--rw-r--r--   0     1001      123      266 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/python/rpycocotools/anns.py
--rw-r--r--   0     1001      123     3402 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/python/rpycocotools/mask.py
--rw-r--r--   0     1001      123      872 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/README.md
--rw-r--r--   0     1001      123     4323 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-build.txt
--rw-r--r--   0     1001      123     6529 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-dev.txt
--rw-r--r--   0     1001      123    19383 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-doc.txt
--rw-r--r--   0     1001      123     7535 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-flake8.txt
--rw-r--r--   0     1001      123     4641 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-test.txt
--rw-r--r--   0     1001      123     3142 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements.txt
--rw-r--r--   0     1001      123     6021 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/coco.rs
--rw-r--r--   0     1001      123     1179 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/errors.rs
--rw-r--r--   0     1001      123     1524 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/lib.rs
--rw-r--r--   0     1001      123       31 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/main.rs
--rw-r--r--   0     1001      123     6476 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/mask.rs
--rw-r--r--   0     1001      123      205 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/tests/conftest.py
--rw-r--r--   0     1001      123     4055 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/tests/test_coco.py
--rw-r--r--   0     1001      123     5096 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/tests/test_mask.py
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 rpycocotools-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 rpycocotools-0.0.7/local_dependencies/cocotools/Cargo.toml
+-rw-r--r--   0     1001      123       30 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/.gitignore
+-rw-r--r--   0     1001      123    55307 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/Cargo.lock
+-rw-r--r--   0     1001      123     1693 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/README.md
+-rw-r--r--   0     1001      123     1186 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/argparse.rs
+-rw-r--r--   0     1001      123    19765 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/coco/object_detection.rs
+-rw-r--r--   0     1001      123     8377 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/coco/pyo3.rs
+-rw-r--r--   0     1001      123      181 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/coco.rs
+-rw-r--r--   0     1001      123     3017 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/errors.rs
+-rw-r--r--   0     1001      123     1901 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/lib.rs
+-rw-r--r--   0     1001      123     1510 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/main.rs
+-rw-r--r--   0     1001      123    23318 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/mask/conversions.rs
+-rw-r--r--   0     1001      123     6222 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/mask/utils.rs
+-rw-r--r--   0     1001      123      230 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/mask.rs
+-rw-r--r--   0     1001      123      724 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/utils.rs
+-rw-r--r--   0     1001      123     2296 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/visualize/display.rs
+-rw-r--r--   0     1001      123     6037 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/visualize/draw.rs
+-rw-r--r--   0     1001      123      141 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/src/visualize.rs
+-rw-r--r--   0     1001      123      610 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/local_dependencies/cocotools/tests/load_coco.rs
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.7/Cargo.toml
+-rw-r--r--   0     1001      123      173 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/.gitignore
+-rw-r--r--   0     1001      123       58 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/.rustfmt.toml
+-rw-r--r--   0     1001      123    45992 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/Cargo.lock
+-rw-r--r--   0     1001      123     4421 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/README.md
+-rw-r--r--   0     1001      123     2542 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/benchmarks/area.py
+-rw-r--r--   0     1001      123     2694 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/benchmarks/conftest.py
+-rw-r--r--   0     1001      123     2775 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/benchmarks/decode.py
+-rw-r--r--   0     1001      123      935 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/benchmarks/load.py
+-rw-r--r--   0     1001      123    48331 2023-05-25 15:48:38.000000 rpycocotools-0.0.7/dist/rpycocotools-0.0.7.tar.gz
+-rw-r--r--   0     1001      123      634 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/Makefile
+-rw-r--r--   0     1001      123        0 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/_static/.gitkeep
+-rw-r--r--   0     1001      123     1572 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/conf.py
+-rw-r--r--   0     1001      123    10951 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/dataset.rst
+-rw-r--r--   0     1001      123      623 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/examples.rst
+-rw-r--r--   0     1001      123      731 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/index.rst
+-rw-r--r--   0     1001      123      800 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/make.bat
+-rw-r--r--   0     1001      123      101 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/quickstart.rst
+-rw-r--r--   0     1001      123     2943 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/docs/segmentation_masks.rst
+-rw-r--r--   0     1001      123     4414 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/pyproject.toml
+-rw-r--r--   0     1001      123      171 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/python/rpycocotools/__init__.py
+-rw-r--r--   0     1001      123      349 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/python/rpycocotools/anns.py
+-rw-r--r--   0     1001      123     3402 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/python/rpycocotools/mask.py
+-rw-r--r--   0     1001      123     1015 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/README.md
+-rw-r--r--   0     1001      123    25684 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements-benchmarks.txt
+-rw-r--r--   0     1001      123     4323 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements-build.txt
+-rw-r--r--   0     1001      123     6529 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements-dev.txt
+-rw-r--r--   0     1001      123    19383 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements-doc.txt
+-rw-r--r--   0     1001      123     7535 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements-flake8.txt
+-rw-r--r--   0     1001      123     4641 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements-test.txt
+-rw-r--r--   0     1001      123     3142 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/requirements/requirements.txt
+-rw-r--r--   0     1001      123     6050 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/src/coco.rs
+-rw-r--r--   0     1001      123     1179 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/src/errors.rs
+-rw-r--r--   0     1001      123     1524 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/src/lib.rs
+-rw-r--r--   0     1001      123       31 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/src/main.rs
+-rw-r--r--   0     1001      123     6476 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/src/mask.rs
+-rw-r--r--   0     1001      123      205 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/tests/conftest.py
+-rw-r--r--   0     1001      123     3938 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/tests/test_coco.py
+-rw-r--r--   0     1001      123     5096 2023-05-25 15:46:56.000000 rpycocotools-0.0.7/tests/test_mask.py
+-rw-r--r--   0        0        0     6936 1970-01-01 00:00:00.000000 rpycocotools-0.0.7/PKG-INFO
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.toml` & `rpycocotools-0.0.7/local_dependencies/cocotools/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cocotools"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 rust-version = "1.64.0"
 description = "Package providing functionalities to work with COCO format datasets."
 readme = "README.md"
 categories = ["command-line-utilities"]
 authors = ["Hoel Bagard"]
 license = "MIT OR Apache-2.0"
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.lock` & `rpycocotools-0.0.7/local_dependencies/cocotools/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "cocotools"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "anyhow",
  "clap 4.1.8",
  "criterion",
  "image",
  "imageproc",
  "minifb",
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/argparse.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/argparse.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Visualize {
         /// Path to the COCO json annotation file.
         annotations_file: PathBuf,
         /// Path to the folder with the images.
         image_folder: PathBuf,
         /// The id of the image to visualize. It is often the same as the filename, but not necessarily.
         #[arg(short, long)]
-        sample_id: Option<u32>,
+        sample_id: Option<u64>,
     },
 
     /// Convert the segmentation format of the labels in a COCO annotation file.
     ConvertSegmentation {
         /// Path to the COCO json annotation file.
         annotations_path: PathBuf,
         target_segmentation: Segmentation,
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/object_detection.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/coco/object_detection.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,52 +10,77 @@
 use serde::{Deserialize, Serialize};
 
 use crate::errors::{self, LoadingError, MissingIdError};
 use crate::utils::load_img;
 use crate::visualize::draw;
 
 /// COCO dataset as-is, without additionnal functionalities.
-#[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
+#[derive(Clone, Debug, Default, PartialEq, Deserialize, Serialize)]
 pub struct Dataset {
+    #[serde(default)]
+    pub info: Info,
     pub images: Vec<Image>,
     pub annotations: Vec<Annotation>,
     pub categories: Vec<Category>,
+    #[serde(default)]
+    pub licenses: Vec<License>,
+}
+
+#[derive(Clone, Debug, Default, PartialEq, Eq, Deserialize, Serialize)]
+pub struct Info {
+    pub year: u32,
+    pub version: String,
+    pub description: String,
+    pub contributor: String,
+    pub url: String,
+    pub date_created: String,
+}
+
+#[derive(Clone, Debug, Default, PartialEq, Eq, Deserialize, Serialize)]
+pub struct License {
+    pub id: u32,
+    pub name: String,
+    pub url: String,
 }
 
 /// Stores information relating to one image.
 #[cfg_attr(
     feature = "pyo3",
     pyclass(get_all, set_all, module = "rpycocotools.anns")
 )]
-#[derive(Clone, Debug, PartialEq, Eq, Deserialize, Serialize)]
+#[derive(Clone, Debug, Default, PartialEq, Eq, Deserialize, Serialize)]
 pub struct Image {
-    pub id: u32,
+    pub id: u64,
     pub width: u32,
     pub height: u32,
     pub file_name: String,
-    // "license": int,
-    // "flickr_url": str,
-    // "coco_url": str,
-    // "date_captured": datetime,
+    #[serde(default)]
+    pub license: u32,
+    #[serde(default)]
+    pub flickr_url: String,
+    #[serde(default)]
+    pub coco_url: String,
+    #[serde(default)]
+    pub date_captured: String,
 }
 
 /// Object instance annotation for object detection.\
 ///
 /// Each object instance annotation contains a series of fields, including the category id and segmentation mask of the object.\
 /// In [the original COCO dataset](https://cocodataset.org/#home), the segmentation format depends on whether the instance represents a single object (`iscrowd=0` in which case polygons are used) or a collection of objects (`iscrowd=1` in which case RLE is used). Note that a single object (iscrowd=0) may require multiple polygons, for example if occluded.\
 /// Crowd annotations (`iscrowd=1`) are used to label large groups of objects (e.g. a crowd of people). In addition, an enclosing bounding box is provided for each object (box coordinates are measured from the top left image corner and are 0-indexed).\
 /// Finally, the categories field of the annotation structure stores the mapping of category id to category and supercategory names.
 #[cfg_attr(
     feature = "pyo3",
     pyclass(subclass, get_all, set_all, module = "rpycocotools.anns")
 )]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 pub struct Annotation {
-    pub id: u32,
-    pub image_id: u32,
+    pub id: u64,
+    pub image_id: u64,
     pub category_id: u32,
     /// Segmentation in the annotation file can be a polygon, RLE or COCO RLE.\
     /// Examples of what each segmentation should look like in the JSON file:
     /// - [`Polygons`]: `"segmentation": [[510.66, 423.01, 511.72, 420.03, ..., 510.45, 423.01]]`
     /// - [`Rle`]: `"segmentation": {"size": [40, 40], "counts": [245, 5, 35, 5, ..., 5, 35, 5, 1190]}`
     /// - [`CocoRle`]: `"segmentation": {"size": [480, 640], "counts": "aUh2b0X...BgRU4"}`
     pub segmentation: Segmentation,
@@ -168,20 +193,20 @@
 }
 
 /// COCO dataset represented as a hashmap where the hashmap's keys are the ids.
 ///
 /// This struct provides methods to make working with the dataset easier and more efficient.
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 pub struct HashmapDataset {
-    pub(crate) anns: HashMap<u32, Annotation>,
+    pub(crate) anns: HashMap<u64, Annotation>,
     cats: HashMap<u32, Category>,
-    imgs: HashMap<u32, Image>,
+    imgs: HashMap<u64, Image>,
     /// Hashmap that links an image id to the image's annotations
     // Use Rc to reference the annotations directly ?
-    img_to_anns: HashMap<u32, HashSet<u32>>,
+    img_to_anns: HashMap<u64, HashSet<u64>>,
     pub image_folder: PathBuf,
 }
 
 impl HashmapDataset {
     /// Loads a COCO dataset from the annotation file and the image folder.
     ///
     /// # Errors
@@ -209,24 +234,24 @@
     ) -> Result<Self, LoadingError> {
         let cats = dataset
             .categories
             .into_iter()
             .map(|category| (category.id, category))
             .collect();
 
-        let imgs: HashMap<u32, Image> = dataset
+        let imgs: HashMap<u64, Image> = dataset
             .images
             .clone()
             .into_iter()
             .map(|image| (image.id, image))
             .collect();
 
-        let mut anns: HashMap<u32, Annotation> = HashMap::new();
+        let mut anns: HashMap<u64, Annotation> = HashMap::new();
         // Have (at least) an empty set for each image to avoid getting an error in the case where an image does not have any annotation.
-        let mut img_to_anns: HashMap<u32, HashSet<u32>> = dataset
+        let mut img_to_anns: HashMap<u64, HashSet<u64>> = dataset
             .images
             .into_iter()
             .map(|image| (image.id, HashSet::new()))
             .collect();
 
         for mut annotation in dataset.annotations {
             let ann_id = annotation.id;
@@ -262,15 +287,15 @@
     }
 
     /// Return the annotation corresponding to the given annotation id.
     ///
     /// # Errors
     ///
     /// Will return `Err` if there is no entry in the dataset corresponding to `ann_id`.
-    pub fn get_ann(&self, ann_id: u32) -> Result<&Annotation, MissingIdError> {
+    pub fn get_ann(&self, ann_id: u64) -> Result<&Annotation, MissingIdError> {
         self.anns
             .get(&ann_id)
             .ok_or(MissingIdError::Annotation(ann_id))
     }
 
     /// Returns all the annotations of the dataset.
     #[must_use]
@@ -296,45 +321,45 @@
     }
 
     /// Return the image entry corresponding to the given image id.
     ///
     /// # Errors
     ///
     /// Will return `Err` if there is no entry corresponding to `img_id`.
-    pub fn get_img(&self, img_id: u32) -> Result<&Image, MissingIdError> {
+    pub fn get_img(&self, img_id: u64) -> Result<&Image, MissingIdError> {
         self.imgs.get(&img_id).ok_or(MissingIdError::Image(img_id))
     }
 
     /// Returns all the images of the dataset.
     #[must_use]
     pub fn get_imgs(&self) -> Vec<&Image> {
         self.imgs.values().collect()
     }
 
     /// Return the annotations for the given image id.
     ///
     /// # Errors
     ///
     /// Will return `Err` if there is no entry corresponding to `img_id`.
-    pub fn get_img_anns(&self, img_id: u32) -> Result<Vec<&Annotation>, MissingIdError> {
+    pub fn get_img_anns(&self, img_id: u64) -> Result<Vec<&Annotation>, MissingIdError> {
         self.img_to_anns
             .get(&img_id)
             .map_or(Err(MissingIdError::Image(img_id)), |ann_ids| {
                 ann_ids.iter().map(|ann_id| self.get_ann(*ann_id)).collect()
             })
     }
 
     /// Draw the annotations for the given image id on the image and return it.
     ///
     /// # Errors
     ///
     /// Will return `Err` if there is no image or annotation entry for `img_id`. Or if the segmentation annotations could not be decompressed.
     pub fn draw_img_anns(
         &self,
-        img_id: u32,
+        img_id: u64,
         draw_bbox: bool,
     ) -> Result<image::ImageBuffer<image::Rgb<u8>, Vec<u8>>, errors::CocoError> {
         let img_path = self.image_folder.join(&self.get_img(img_id)?.file_name);
         let mut img = load_img(&img_path)?;
         draw::anns(&mut img, &self.get_img_anns(img_id)?, draw_bbox)?;
         Ok(img)
     }
@@ -385,14 +410,15 @@
 
 impl From<&HashmapDataset> for Dataset {
     fn from(dataset: &HashmapDataset) -> Self {
         Self {
             images: dataset.get_imgs().into_iter().cloned().collect(),
             annotations: dataset.get_anns().into_iter().cloned().collect(),
             categories: dataset.get_cats().into_iter().cloned().collect(),
+            ..Default::default()
         }
     }
 }
 
 impl PartialEq for PolygonsRS {
     // TODO: redo this function in a clearer way:
     // - Search for the first point of self in other. If it's not there, then return false.
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/pyo3.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/coco/pyo3.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 use crate::coco::object_detection::*;
 
 #[pymethods]
 impl Annotation {
     #[new]
     fn new(
-        id: u32,
-        image_id: u32,
+        id: u64,
+        image_id: u64,
         category_id: u32,
         segmentation: Segmentation,
         area: f64,
         bbox: Bbox,
         iscrowd: u32,
     ) -> Self {
         Self {
@@ -88,20 +88,21 @@
         }
     }
 }
 
 #[pymethods]
 impl Image {
     #[new]
-    fn new(id: u32, width: u32, height: u32, file_name: String) -> Self {
+    fn new(id: u64, width: u32, height: u32, file_name: String) -> Self {
         Self {
             id,
             width,
             height,
             file_name,
+            ..Default::default()
         }
     }
 
     fn __repr__(&self) -> String {
         format!(
             "Image(id={}, width='{}', height='{}', file_name='{}')",
             self.id, self.width, self.height, self.file_name
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/errors.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/errors.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 use thiserror::Error;
 
 /// Error returned when trying to access an element of the dataset that does not exist.
 #[derive(thiserror::Error)]
 pub enum MissingIdError {
     #[error("The following annotation id was not found in the dataset: `{0}`.")]
-    Annotation(u32),
+    Annotation(u64),
     #[error("The following category id was not found in the dataset: `{0}`.")]
     Category(u32),
     #[error("The following image id was not found in the dataset: `{0}`.")]
-    Image(u32),
+    Image(u64),
     // #[error(transparent)]
     // InvalidValue(#[from] anyhow::Error),
 }
 
 /// Error returned when a json annotations file cannot be loaded/parsed or when an image cannot be loaded.
 #[derive(Error)]
 pub enum LoadingError {
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/lib.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/main.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/main.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/conversions.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/mask/conversions.rs`

 * *Files 0% similar despite different names*

```diff
@@ -347,17 +347,20 @@
             let mut points_poly: Vec<imageproc::point::Point<i32>> = Vec::new();
             for i in (0..poly.len()).step_by(2) {
                 points_poly.push(imageproc::point::Point::new(
                     poly[i] as i32,
                     poly[i + 1] as i32,
                 ));
             }
-            if let Some(last_point) = points_poly.last() {
+
+            while let Some(last_point) = points_poly.last() {
                 if points_poly[0].x == last_point.x && points_poly[0].y == last_point.y {
                     points_poly.pop();
+                } else {
+                    break;
                 }
             }
 
             drawing::draw_polygon_mut(&mut mask, &points_poly, image::Luma([1u8]));
         }
 
         Self::from_shape_vec(
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/utils.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/mask/utils.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/utils.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/display.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/visualize/display.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 use crate::utils;
 
 /// Visualize the annotations for the given image id.
 ///
 /// # Errors
 ///
 /// Will return `Err` if `img_id` is not present in the dataset.
-pub fn img_anns(dataset: &HashmapDataset, img_id: u32) -> Result<(), Box<dyn std::error::Error>> {
+pub fn img_anns(dataset: &HashmapDataset, img_id: u64) -> Result<(), Box<dyn std::error::Error>> {
     let anns = dataset.get_img_anns(img_id)?;
     let img_name = &dataset.get_img(img_id)?.file_name;
     let img_path = dataset.image_folder.join(img_name);
 
     self::anns(&img_path, &anns, true)?;
 
     Ok(())
```

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/draw.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/src/visualize/draw.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/local_dependencies/cocotools/tests/load_coco.rs` & `rpycocotools-0.0.7/local_dependencies/cocotools/tests/load_coco.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/Cargo.lock` & `rpycocotools-0.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "cocotools"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "anyhow",
  "clap",
  "image",
  "imageproc",
  "minifb",
  "ndarray",
@@ -1245,15 +1245,15 @@
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "rpycocotools"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "anyhow",
  "cocotools",
  "ndarray",
  "nshare",
  "numpy",
  "pyo3",
```

### Comparing `rpycocotools-0.0.6/docs/Makefile` & `rpycocotools-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/docs/conf.py` & `rpycocotools-0.0.7/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "rpycocotools"
 copyright = "2023, Hoel Bagard"
 author = "Hoel Bagard"
-release = "0.0.3"
+release = "0.0.7"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 autodoc_typehints = "none"
 master_doc = "index"
```

### Comparing `rpycocotools-0.0.6/docs/dataset.rst` & `rpycocotools-0.0.7/docs/dataset.rst`

 * *Files 14% similar despite different names*

```diff
@@ -110,14 +110,56 @@
     :param int image_id: The id of the image corresponding to this annotation.
     :param int category_id: The id of the category corresponding to this annotation.
     :param Polygons | PolygonsRS | RLE | COCO_RLE segmentation: The segmentation data for the annotation, which can be of type Polygons, PolygonsRS, RLE or COCO_RLE.
     :param float area: The area of the annotation bounding box.
     :param BBox bbox: The bounding box of the annotation.
     :param int iscrowd: The iscrowd flag for the annotation, which indicates if the annotation represents a group of objects or not.
 
+    .. attribute:: id
+
+        The id of the category.
+
+        :type: int
+
+    .. attribute:: image_id
+
+        The id of the image corresponding to this annotation.
+
+        :type: int
+
+    .. attribute:: category_id
+
+        The id of the category corresponding to this annotation.
+
+        :type: int
+
+    .. attribute:: segmentation
+
+        The segmentation data for the annotation, which can be of type Polygons, PolygonsRS, RLE or COCO_RLE.
+
+        :type: Polygons | PolygonsRS | RLE | COCO_RLE
+
+    .. attribute:: area
+
+        The area of the annotation bounding box.
+
+        :type: float
+
+    .. attribute:: bbox
+
+        The bounding box of the annotation.
+
+        :type: BBox
+
+    .. attribute:: iscrowd
+
+        The iscrowd flag for the annotation, which indicates if the annotation represents a group of objects or not.
+
+        :type: int
+
 .. class:: rpycocotools.anns.Category(id: int, name: str, supercategory: str) -> None
 
     Creates a category used for COCO object detection tasks.
 
     :param int id: The id of the category.
     :param str name: The name of the category.
     :param str supercategory: The supercategory of the category.
@@ -261,7 +303,19 @@
         :type: list[int]
 
     .. attribute:: counts
 
         The COCO RLE representation of the mask.
 
         :type: str
+
+.. function:: from_dataset(images: Sequence[Image], annotations: Sequence[_AnnotationAny], categories: Sequence[Category], image_folder_path: str) -> COCO
+
+  Construct a COCO dataset from its components and the image folder.
+
+  :param Sequence[Image] images: The image entries composing the data.
+  :param Sequence[Annotation] annotations: The annotations entries composing the data.
+  :param Sequence[Category] categories: The categories entries composing the data.
+  :param str image_folder_path: Path to the folder with the images.
+  :raise ValueError: If there is an annotation with an image id X, but no image entry has this id.
+  :return: The constructed COCO dataset.
+  :rtype: :py:class:`COCO`
```

### Comparing `rpycocotools-0.0.6/docs/examples.rst` & `rpycocotools-0.0.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/docs/index.rst` & `rpycocotools-0.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/docs/make.bat` & `rpycocotools-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/docs/segmentation_masks.rst` & `rpycocotools-0.0.7/docs/segmentation_masks.rst`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/pyproject.toml` & `rpycocotools-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "rpycocotools"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{name="Bagard Hoel"}]
 description = "Package providing utilities to load, manipulate, convert and visualize COCO format datasets."
 keywords = ["COCO", "COCO dataset"]
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -35,14 +35,15 @@
 module-name = "rpycocotools._rpycocotools"
 # bindings = "cffi"
 # compatibility = "linux"
 
 [project.optional-dependencies]
 build = ["maturin"]
 test = ["pytest", "hypothesis"]
+benchmarks = ["pytest-benchmark", "pycocotools", "pycocotools-stubs"]
 dev = ["pip-tools", "ruff", "pyright"]
 doc = ["sphinx", "sphinx-rtd-theme", "sphinx-hoverxref", "sphinx-codeautolink"]
 flake8 = [
     "flake8>=5.0.4,<6.0",
     "flake8-bugbear>=23.3.12,<24.0",
     "flake8-builtins>=2.1.0,<3.0",
     "flake8-comprehensions>=3.12.0,<4.0",
@@ -58,14 +59,15 @@
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/7.1.x/explanation/goodpractices.html
 addopts = [
     "--import-mode=importlib",
     "--strict-markers",
 ]
+markers = ["coco2017"]
 
 [tool.ruff]
 select = ["ALL"]
 exclude = ["docs/conf.py"]
 line-length = 120
 
 [tool.ruff.isort]
@@ -79,16 +81,17 @@
 max-args = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
-"python/rpycocotools/anns.py" = ["D101", "F403", "F405"]
+"python/rpycocotools/anns.py" = ["D101", "F401", "F403", "F405"]
 "tests/**/*.py" = ["D1", "INP001", "PLR2004", "S101"]
+"benchmarks/**/*.py" = ["D1", "INP001", "S101"]
 
 [tool.pyright]
 include = ["tests"]
 ignore = ["python"]
 pythonVersion = "3.11"
 pythonPlatform = "Linux"
 
@@ -131,17 +134,18 @@
 import-order-style = "smarkets"
 inline-quotes = "double"
 # D1: Missing docstring
 # I100: Import statements are in the wrong order.
 # I201: Missing newline between import groups.
 # F401: imported but unused
 per-file-ignores = [
+    "benchmarks/*.py:D1",
     "tests/*.py:D1,I201,I100",
     "python/rpycocotools/__init__.py:F401,I100,NQA102",
-    "python/rpycocotools/anns.py:D101,F403,F405"
+    "python/rpycocotools/anns.py:D101,F401,F403,F405"
 ]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
     "import-error",
     "no-name-in-module",
```

### Comparing `rpycocotools-0.0.6/python/rpycocotools/mask.py` & `rpycocotools-0.0.7/python/rpycocotools/mask.py`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/requirements/README.md` & `rpycocotools-0.0.7/requirements/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ### Requirements generation
 
 The requirements can be re-generated with the following commands
 ```
 pip-compile --output-file=requirements/requirements.txt --resolver=backtracking pyproject.toml --generate-hashes
 pip-compile --extra=test --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml --generate-hashes
+pip-compile --extra=benchmarks --output-file=requirements/requirements-benchmarks.txt --resolver=backtracking pyproject.toml --generate-hashes
 pip-compile --extra=dev --output-file=requirements/requirements-dev.txt --resolver=backtracking pyproject.toml --generate-hashes
 pip-compile --extra=doc --output-file=requirements/requirements-doc.txt --resolver=backtracking pyproject.toml --generate-hashes
 pip-compile --extra=build --output-file=requirements/requirements-build.txt --resolver=backtracking pyproject.toml --generate-hashes
 pip-compile --extra=flake8 --output-file=requirements/requirements-flake8.txt --resolver=backtracking pyproject.toml --generate-hashes
 ```
```

### Comparing `rpycocotools-0.0.6/requirements/requirements-build.txt` & `rpycocotools-0.0.7/requirements/requirements-build.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=build --generate-hashes --output-file=requirements/requirements-build.txt --resolver=backtracking pyproject.toml
 #
-maturin==0.15.1 \
-    --hash=sha256:0e89a87549d671056f9358832c8aa1bb522abcf13eeca83327a58b091d4f5a98 \
-    --hash=sha256:229d7eb6e14455a3c69a10a4546f082c7bd5490b8ec7f50d5d10edcea600dc64 \
-    --hash=sha256:247bec13d82021972e5cb4eb38e7a7aea0e7a034beab60f0e0464ffe7423f24b \
-    --hash=sha256:37ddbc261db778c73829173f43624b6178dd4244fae8e4b278323e050e899a14 \
-    --hash=sha256:3b4c296b12736756d1d084c04b5a60281011e77b763eb9c69c39444d2421ad31 \
-    --hash=sha256:616220c8c875526b22605bbb0be189ff859956abad8fe6e49c9ad2caa761ebca \
-    --hash=sha256:61eda19c37394660c3b0b9c6dbfa7d411a5dca1a93c9dcf7baa718f3a03fda04 \
-    --hash=sha256:7a7e02f265c30bac9f16e65c9d14184b3228c26b03dbe83a15220ab09fceabd7 \
-    --hash=sha256:a40c96dc135e1571159155bdbd8c06509dea14a9317ca0e5b7cae4c8d2016b93 \
-    --hash=sha256:ab5f8d8858440f35d833bce8bbf8233e595afa23fe00c513f7b671183946ea02 \
-    --hash=sha256:b54421ae71e1e3dde92105d300187b9ac3b257a5b33c1d670ff9ee5266a1bd81 \
-    --hash=sha256:dabb8ff46461c6fb1d68e8972a172cf1dede3c9825a41e4a6caecc95c26ca3b4 \
-    --hash=sha256:f604b65fd9f0b94856e88cf8b345e21a27276297e6df4ad9305937887feda13b
+maturin==0.15.3 \
+    --hash=sha256:058f69ab91e8168559e97112eb0594a2a547e6c36aacdefe1f4e60536115dc07 \
+    --hash=sha256:0af91ab0faf1d6c0cc386c9751b2889c860bd228e4f0f5d15e9576ac3d8042a3 \
+    --hash=sha256:1415890346e07fa604d0c40fa31ec61b873326b2c9d57f15a474c98268b4f268 \
+    --hash=sha256:14c258e0595db830a2b4faa1d44ff1aaf651e925396c1da20c65d18f51e5ab6b \
+    --hash=sha256:2bcfd23c961fa1e449eb95984dc48487d83917a1d26aee39d26c297851ac5218 \
+    --hash=sha256:3e9eb8bf3698c2047e5172495869ac806e76dad37bf016d42056f5740c225a54 \
+    --hash=sha256:3fa0ec5f80a2fe13bc91a23a2aab4b2655950f0ac358c79ffad7d539dd8bbd15 \
+    --hash=sha256:6549802af70bc515ac21a7094234d824ffc95b517da970cf004d7a341dc6d370 \
+    --hash=sha256:6a66837319e423ed6945d1d965ca9195a856fc1fa9dc99b7f9a0e4f27fb558f4 \
+    --hash=sha256:9fd402d8492b3d9db23ef6c5d6254a4d9f77868cd17502005934a6ca2456fcf7 \
+    --hash=sha256:bbeb6442e5e6080a445604778de8665cb7c5b5fee7b0fedecf4d12968a062cca \
+    --hash=sha256:e903ab8031cc198711e4ad3f842746f163e31e3c91980345feabe984f0b5e0b0 \
+    --hash=sha256:ee8a7d0987e9d85818df54da20a858f4d35255b5efd302ee6160efe24520c7be
     # via rpycocotools (pyproject.toml)
 numpy==1.24.3 \
     --hash=sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187 \
     --hash=sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812 \
     --hash=sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7 \
     --hash=sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4 \
     --hash=sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6 \
@@ -47,15 +47,15 @@
     --hash=sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4 \
     --hash=sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02 \
     --hash=sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c \
     --hash=sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b
     # via
     #   rpycocotools (pyproject.toml)
     #   rpycocotools-stubs
-rpycocotools-stubs==0.0.5 \
-    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
-    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
+rpycocotools-stubs==0.0.7 \
+    --hash=sha256:841f94f413eba45304b61ed9dde833901ddb6ba7bc381feebdb2450a55185f19 \
+    --hash=sha256:fac9b6ba4aefc563e3e869c8321e49d5d5184b9f1616578d84f6fdd052b43a08
     # via rpycocotools (pyproject.toml)
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.6.0 \
+    --hash=sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223 \
+    --hash=sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768
     # via rpycocotools-stubs
```

### Comparing `rpycocotools-0.0.6/requirements/requirements-dev.txt` & `rpycocotools-0.0.7/requirements/requirements-dev.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
     --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
     # via pip-tools
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via pip-tools
-nodeenv==1.7.0 \
-    --hash=sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e \
-    --hash=sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b
+nodeenv==1.8.0 \
+    --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
+    --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
     # via pyright
 numpy==1.24.3 \
     --hash=sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187 \
     --hash=sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812 \
     --hash=sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7 \
     --hash=sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4 \
     --hash=sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6 \
@@ -56,44 +56,44 @@
     --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
     --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
     # via rpycocotools (pyproject.toml)
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via build
-pyright==1.1.306 \
-    --hash=sha256:008eb2a29584ae274a154d749cf81476a3073fb562a462eac8d43a753378b9db \
-    --hash=sha256:16d5d198be64de497d5f9002000a271176c381e21b977ca5566cf779b643c9ed
+pyright==1.1.309 \
+    --hash=sha256:1abcfa83814d792a5d70b38621cc6489acfade94ebb2279e55ba1f394d54296c \
+    --hash=sha256:a8b052c1997f7334e80074998ea0f93bd149550e8cf27ccb5481d3b2e1aad161
     # via rpycocotools (pyproject.toml)
-rpycocotools-stubs==0.0.5 \
-    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
-    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
+rpycocotools-stubs==0.0.7 \
+    --hash=sha256:841f94f413eba45304b61ed9dde833901ddb6ba7bc381feebdb2450a55185f19 \
+    --hash=sha256:fac9b6ba4aefc563e3e869c8321e49d5d5184b9f1616578d84f6fdd052b43a08
     # via rpycocotools (pyproject.toml)
-ruff==0.0.265 \
-    --hash=sha256:1d5a8de2fbaf91ea5699451a06f4074e7a312accfa774ad9327cde3e4fda2081 \
-    --hash=sha256:2a9b38bdb40a998cbc677db55b6225a6c4fadcf8819eb30695e1b8470942426b \
-    --hash=sha256:30ddfe22de6ce4eb1260408f4480bbbce998f954dbf470228a21a9b2c45955e4 \
-    --hash=sha256:4057eb539a1d88eb84e9f6a36e0a999e0f261ed850ae5d5817e68968e7b89ed9 \
-    --hash=sha256:5028950f7af9b119d43d91b215d5044976e43b96a0d1458d193ef0dd3c587bf8 \
-    --hash=sha256:53c17f0dab19ddc22b254b087d1381b601b155acfa8feed514f0d6a413d0ab3a \
-    --hash=sha256:62a9578b48cfd292c64ea3d28681dc16b1aa7445b7a7709a2884510fc0822118 \
-    --hash=sha256:9ac13b11d9ad3001de9d637974ec5402a67cefdf9fffc3929ab44c2fcbb850a1 \
-    --hash=sha256:9e9db5ccb810742d621f93272e3cc23b5f277d8d00c4a79668835d26ccbe48dd \
-    --hash=sha256:a11bd0889e88d3342e7bc514554bb4461bf6cc30ec115821c2425cfaac0b1b6a \
-    --hash=sha256:a8b44a245b60512403a6a03a5b5212da274d33862225c5eed3bcf12037eb19bb \
-    --hash=sha256:aa17b13cd3f29fc57d06bf34c31f21d043735cc9a681203d634549b0e41047d1 \
-    --hash=sha256:b279fa55ea175ef953208a6d8bfbcdcffac1c39b38cdb8c2bfafe9222add70bb \
-    --hash=sha256:c78470656e33d32ddc54e8482b1b0fc6de58f1195586731e5ff1405d74421499 \
-    --hash=sha256:d0f9967f84da42d28e3d9d9354cc1575f96ed69e6e40a7d4b780a7a0418d9409 \
-    --hash=sha256:d586e69ab5cbf521a1910b733412a5735936f6a610d805b89d35b6647e2a66aa \
-    --hash=sha256:f54facf286103006171a00ce20388d88ed1d6732db3b49c11feb9bf3d46f90e9
+ruff==0.0.269 \
+    --hash=sha256:03ff42bc91ceca58e0f0f072cb3f9286a9208f609812753474e799a997cdad1a \
+    --hash=sha256:11ddcfbab32cf5c420ea9dd5531170ace5a3e59c16d9251c7bd2581f7b16f602 \
+    --hash=sha256:1f19f59ca3c28742955241fb452f3346241ddbd34e72ac5cb3d84fadebcf6bc8 \
+    --hash=sha256:3569bcdee679045c09c0161fabc057599759c49219a08d9a4aad2cc3982ccba3 \
+    --hash=sha256:374b161753a247904aec7a32d45e165302b76b6e83d22d099bf3ff7c232c888f \
+    --hash=sha256:3f5dc7aac52c58e82510217e3c7efd80765c134c097c2815d59e40face0d1fe6 \
+    --hash=sha256:56347da63757a56cbce7d4b3d6044ca4f1941cd1bbff3714f7554360c3361f83 \
+    --hash=sha256:5a20658f0b97d207c7841c13d528f36d666bf445b00b01139f28a8ccb80093bb \
+    --hash=sha256:6da8ee25ef2f0cc6cc8e6e20942c1d44d25a36dce35070d7184655bc14f63f63 \
+    --hash=sha256:9ca0a1ddb1d835b5f742db9711c6cf59f213a1ad0088cb1e924a005fd399e7d8 \
+    --hash=sha256:a374434e588e06550df0f8dcb74777290f285678de991fda4e1063c367ab2eb2 \
+    --hash=sha256:bbeb857b1e508a4487bdb02ca1e6d41dd8d5ac5335a5246e25de8a3dff38c1ff \
+    --hash=sha256:bd81b8e681b9eaa6cf15484f3985bd8bd97c3d114e95bff3e8ea283bf8865062 \
+    --hash=sha256:cec2f4b84a14b87f1b121488649eb5b4eaa06467a2387373f750da74bdcb5679 \
+    --hash=sha256:e131b4dbe798c391090c6407641d6ab12c0fa1bb952379dde45e5000e208dabb \
+    --hash=sha256:f062059b8289a4fab7f6064601b811d447c2f9d3d432a17f689efe4d68988450 \
+    --hash=sha256:f3b59ccff57b21ef0967ea8021fd187ec14c528ec65507d8bcbe035912050776
     # via rpycocotools (pyproject.toml)
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.6.0 \
+    --hash=sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223 \
+    --hash=sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768
     # via rpycocotools-stubs
 wheel==0.40.0 \
     --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
     --hash=sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247
     # via pip-tools
 
 # WARNING: The following packages were not pinned, but pip requires them to be
```

### Comparing `rpycocotools-0.0.6/requirements/requirements-doc.txt` & `rpycocotools-0.0.7/requirements/requirements-doc.txt`

 * *Files 6% similar despite different names*

```diff
@@ -203,21 +203,21 @@
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via sphinx
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via sphinx
-requests==2.30.0 \
-    --hash=sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294 \
-    --hash=sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4
-    # via sphinx
-rpycocotools-stubs==0.0.5 \
-    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
-    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+    # via sphinx
+rpycocotools-stubs==0.0.7 \
+    --hash=sha256:841f94f413eba45304b61ed9dde833901ddb6ba7bc381feebdb2450a55185f19 \
+    --hash=sha256:fac9b6ba4aefc563e3e869c8321e49d5d5184b9f1616578d84f6fdd052b43a08
     # via rpycocotools (pyproject.toml)
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via sphinx
 soupsieve==2.4.1 \
     --hash=sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8 \
@@ -236,17 +236,17 @@
     --hash=sha256:02a5c768bc1de5f8f8248c02fadc7be0e23370b4c265a2495c0a7c3f337e5d71 \
     --hash=sha256:2db64a2012dbf1772f95638196ae4885a6849ddd3d44f594e4f8875bf7b73779
     # via rpycocotools (pyproject.toml)
 sphinx-hoverxref==1.3.0 \
     --hash=sha256:1064e4b1da49422873de555d79dc544da1556820fee05ab56f39d36cc86ba6ad \
     --hash=sha256:e517dab4cb8186da58d78c53781459ee1116ec9c8413580c7dc43e124c5f3177
     # via rpycocotools (pyproject.toml)
-sphinx-rtd-theme==1.2.0 \
-    --hash=sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8 \
-    --hash=sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2
+sphinx-rtd-theme==1.2.1 \
+    --hash=sha256:2cc9351176cbf91944ce44cefd4fab6c3b76ac53aa9e15d6db45a3229ad7f866 \
+    --hash=sha256:cf9a7dc0352cf179c538891cb28d6fad6391117d4e21c891776ab41dd6c8ff70
     # via rpycocotools (pyproject.toml)
 sphinxcontrib-applehelp==1.0.4 \
     --hash=sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228 \
     --hash=sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e
     # via sphinx
 sphinxcontrib-devhelp==1.0.2 \
     --hash=sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e \
@@ -270,15 +270,15 @@
     --hash=sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72 \
     --hash=sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5 \
     --hash=sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd \
     --hash=sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952
     # via sphinx
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.6.0 \
+    --hash=sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223 \
+    --hash=sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768
     # via rpycocotools-stubs
 urllib3==2.0.2 \
     --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
     --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
     # via requests
```

### Comparing `rpycocotools-0.0.6/requirements/requirements-flake8.txt` & `rpycocotools-0.0.7/requirements/requirements-flake8.txt`

 * *Files 3% similar despite different names*

```diff
@@ -111,25 +111,25 @@
     --hash=sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019 \
     --hash=sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1
     # via flake8-docstrings
 pyflakes==2.5.0 \
     --hash=sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2 \
     --hash=sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3
     # via flake8
-rpycocotools-stubs==0.0.5 \
-    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
-    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
+rpycocotools-stubs==0.0.7 \
+    --hash=sha256:841f94f413eba45304b61ed9dde833901ddb6ba7bc381feebdb2450a55185f19 \
+    --hash=sha256:fac9b6ba4aefc563e3e869c8321e49d5d5184b9f1616578d84f6fdd052b43a08
     # via rpycocotools (pyproject.toml)
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via pydocstyle
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.6.0 \
+    --hash=sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223 \
+    --hash=sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768
     # via
     #   flake8-noqa
     #   rpycocotools-stubs
 
 # WARNING: The following packages were not pinned, but pip requires them to be
 # pinned when the requirements file includes hashes. Consider using the --allow-unsafe flag.
 # setuptools
```

### Comparing `rpycocotools-0.0.6/requirements/requirements-test.txt` & `rpycocotools-0.0.7/requirements/requirements-test.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 #    pip-compile --extra=test --generate-hashes --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml
 #
 attrs==23.1.0 \
     --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
     --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
     # via hypothesis
-hypothesis==6.75.2 \
-    --hash=sha256:29fee1fabf764eb021665d20e633ef7ba931c5841de20f9ff3e01e8a512d6a4d \
-    --hash=sha256:50c270b38d724ce0fefa71b8e3511d123f7a31a9af9ea003447d4e1489292fbc
+hypothesis==6.75.3 \
+    --hash=sha256:15cdadb80a7ac59087581624d266a4fb585b5cce9b7f88f506c481a9f0e583f6 \
+    --hash=sha256:a12bf34c29bd22757d20edf93f95805978ed0ffb8d0b22dbadc890a79dc9baa8
     # via rpycocotools (pyproject.toml)
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 numpy==1.24.3 \
     --hash=sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187 \
@@ -56,19 +56,19 @@
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
     # via pytest
 pytest==7.3.1 \
     --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
     --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
     # via rpycocotools (pyproject.toml)
-rpycocotools-stubs==0.0.5 \
-    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
-    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
+rpycocotools-stubs==0.0.7 \
+    --hash=sha256:841f94f413eba45304b61ed9dde833901ddb6ba7bc381feebdb2450a55185f19 \
+    --hash=sha256:fac9b6ba4aefc563e3e869c8321e49d5d5184b9f1616578d84f6fdd052b43a08
     # via rpycocotools (pyproject.toml)
 sortedcontainers==2.4.0 \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
     # via hypothesis
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.6.0 \
+    --hash=sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223 \
+    --hash=sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768
     # via rpycocotools-stubs
```

### Comparing `rpycocotools-0.0.6/requirements/requirements.txt` & `rpycocotools-0.0.7/requirements/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     --hash=sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4 \
     --hash=sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02 \
     --hash=sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c \
     --hash=sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b
     # via
     #   rpycocotools (pyproject.toml)
     #   rpycocotools-stubs
-rpycocotools-stubs==0.0.5 \
-    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
-    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
+rpycocotools-stubs==0.0.7 \
+    --hash=sha256:841f94f413eba45304b61ed9dde833901ddb6ba7bc381feebdb2450a55185f19 \
+    --hash=sha256:fac9b6ba4aefc563e3e869c8321e49d5d5184b9f1616578d84f6fdd052b43a08
     # via rpycocotools (pyproject.toml)
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.6.0 \
+    --hash=sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223 \
+    --hash=sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768
     # via rpycocotools-stubs
```

### Comparing `rpycocotools-0.0.6/src/coco.rs` & `rpycocotools-0.0.7/src/coco.rs`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,25 @@
         Ok(Self(dataset))
     }
 
     fn __len__(&self) -> usize {
         self.0.get_imgs().len()
     }
 
-    fn get_img(&self, py: Python<'_>, img_id: u32) -> PyResult<Py<object_detection::Image>> {
+    fn get_img(&self, py: Python<'_>, img_id: u64) -> PyResult<Py<object_detection::Image>> {
         Py::new(
             py,
             self.0
                 .get_img(img_id)
                 .map_err(PyMissingIdError::from)?
                 .clone(),
         )
     }
 
-    fn get_ann(&self, py: Python<'_>, ann_id: u32) -> PyResult<Py<object_detection::Annotation>> {
+    fn get_ann(&self, py: Python<'_>, ann_id: u64) -> PyResult<Py<object_detection::Annotation>> {
         Py::new(
             py,
             self.0
                 .get_ann(ann_id)
                 .map_err(PyMissingIdError::from)?
                 .clone(),
         )
@@ -89,15 +89,15 @@
             .into_iter()
             .map(|cat| Py::new(py, cat.clone()))
             .collect()
     }
 
     fn get_img_anns(
         &self,
-        img_id: u32,
+        img_id: u64,
         py: Python<'_>,
     ) -> PyResult<Vec<Py<object_detection::Annotation>>> {
         self.0
             .get_img_anns(img_id)
             .map_err(PyMissingIdError::from)?
             .into_iter()
             .map(|ann| Py::new(py, ann.clone()))
@@ -105,15 +105,15 @@
     }
 
     /// Visualize an image and its annotations.
     ///
     /// ## Errors
     ///
     /// Will return `Err` if the image cannot be drawn (potentially due to it not being in the dataset) or cannot be displayed.
-    pub fn visualize_img(&self, img_id: u32) -> PyResult<()> {
+    pub fn visualize_img(&self, img_id: u64) -> PyResult<()> {
         let img = self
             .0
             .draw_img_anns(img_id, true)
             .map_err(|err| match err {
                 CocoError::MissingId(err) => PyKeyError::new_err(err.to_string()),
                 CocoError::Mask(err) => PyValueError::new_err(err.to_string()),
                 CocoError::Loading(err) => PyValueError::new_err(err.to_string()),
@@ -134,15 +134,15 @@
     ///
     /// ## Errors
     ///
     /// Will return `Err` if the image cannot be drawn (potentially due to it not being in the dataset).
     pub fn draw_anns<'a>(
         &self,
         py: Python<'a>,
-        img_id: u32,
+        img_id: u64,
         draw_bboxes: bool,
     ) -> PyResult<&'a PyArray3<u8>> {
         let img = self
             .0
             .draw_img_anns(img_id, draw_bboxes)
             .map_err(|err| match err {
                 CocoError::MissingId(err) => PyKeyError::new_err(err.to_string()),
@@ -177,14 +177,15 @@
     image_folder_path: &PyUnicode,
 ) -> PyResult<PyCOCO> {
     let image_folder_path = PathBuf::from(image_folder_path.to_str()?);
     let dataset = object_detection::Dataset {
         images,
         annotations,
         categories,
+        ..Default::default()
     };
     let dataset = COCO::from_dataset(dataset, image_folder_path).map_err(PyLoadingError::from)?;
     Ok(PyCOCO(dataset))
 }
 
 #[pyclass(name = "Polygons", module = "rpycocotools.anns")]
 #[derive(Debug)]
```

### Comparing `rpycocotools-0.0.6/src/errors.rs` & `rpycocotools-0.0.7/src/errors.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/src/lib.rs` & `rpycocotools-0.0.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/src/mask.rs` & `rpycocotools-0.0.7/src/mask.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.6/tests/test_coco.py` & `rpycocotools-0.0.7/tests/test_coco.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,21 +78,23 @@
 @given(u32_st, u32_st, u32_st, u32_st)
 def test_bbox_repr(left: int, top: int, width: int, height: int) -> None:
     bbox = rpycocotools.anns.BBox(left, top, width, height)
     assert str(bbox) == f"BBox(left={left}, top={top}, width={width}, height={height})"
 
 
 def test_dataset_from_components() -> None:
-    expected_ann = Annotation(id=1,
-                              image_id=1,
-                              category_id=1,
-                              segmentation=COCO_RLE(size=[380, 800], counts="a"),
-                              area=1,
-                              bbox=BBox(left=1, top=1, width=1, height=1),
-                              iscrowd=1)
+    expected_ann = Annotation(
+        id=1,
+        image_id=1,
+        category_id=1,
+        segmentation=COCO_RLE(size=[380, 800], counts="a"),
+        area=1,
+        bbox=BBox(left=1, top=1, width=1, height=1),
+        iscrowd=1,
+    )
     anns = [
         expected_ann,
         rpycocotools.anns.Annotation(2, 2, 1, COCO_RLE([1, 1], "b"), 1, rpycocotools.anns.BBox(1, 1, 1, 1), 1),
     ]
     imgs = [
         rpycocotools.anns.Image(1, 380, 800, "test1"),
         rpycocotools.anns.Image(2, 640, 480, "test2"),
```

### Comparing `rpycocotools-0.0.6/tests/test_mask.py` & `rpycocotools-0.0.7/tests/test_mask.py`

 * *Files identical despite different names*

