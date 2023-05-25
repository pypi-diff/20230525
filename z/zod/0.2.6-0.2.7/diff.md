# Comparing `tmp/zod-0.2.6.tar.gz` & `tmp/zod-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.6.tar", max compression
+gzip compressed data, was "zod-0.2.7.tar", max compression
```

## Comparing `zod-0.2.6.tar` & `zod-0.2.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-05-23 09:30:48.888967 zod-0.2.6/LICENSE
--rw-r--r--   0        0        0     4809 2023-05-23 09:30:48.888967 zod-0.2.6/README.md
--rw-r--r--   0        0        0     1783 2023-05-23 09:30:48.888967 zod-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      982 2023-05-23 09:30:48.888967 zod-0.2.6/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-05-23 09:30:48.888967 zod-0.2.6/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-05-23 09:30:48.888967 zod-0.2.6/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-05-23 09:30:48.888967 zod-0.2.6/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14547 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7431 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/utils.py
--rw-r--r--   0        0        0     3682 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-05-23 09:30:48.892967 zod-0.2.6/zod/constants.py
--rw-r--r--   0        0        0      184 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-05-23 09:30:48.892967 zod-0.2.6/zod/zod_drives.py
--rw-r--r--   0        0        0      577 2023-05-23 09:30:48.892967 zod-0.2.6/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-05-23 09:30:48.892967 zod-0.2.6/zod/zod_sequences.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-25 12:01:49.078296 zod-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4809 2023-05-25 12:01:49.078296 zod-0.2.7/README.md
+-rw-r--r--   0        0        0     1783 2023-05-25 12:01:49.078296 zod-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-05-25 12:01:49.078296 zod-0.2.7/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-05-25 12:01:49.078296 zod-0.2.7/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-05-25 12:01:49.078296 zod-0.2.7/zod/anno/lane.py
+-rw-r--r--   0        0        0     4354 2023-05-25 12:01:49.078296 zod-0.2.7/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14496 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7431 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6049 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/utils.py
+-rw-r--r--   0        0        0     3682 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-05-25 12:01:49.082297 zod-0.2.7/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12061 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0     1016 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      123 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8031 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-05-25 12:01:49.082297 zod-0.2.7/zod/zod_drives.py
+-rw-r--r--   0        0        0      577 2023-05-25 12:01:49.082297 zod-0.2.7/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-05-25 12:01:49.082297 zod-0.2.7/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.7/PKG-INFO
```

### Comparing `zod-0.2.6/LICENSE` & `zod-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/README.md` & `zod-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/pyproject.toml` & `zod-0.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.6"
+version = "0.2.7"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.2.6/zod/__init__.py` & `zod-0.2.7/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/_zod_dataset.py` & `zod-0.2.7/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/anno/lane.py` & `zod-0.2.7/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/anno/object.py` & `zod-0.2.7/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/anno/parser.py` & `zod-0.2.7/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/anno/tsr/class_map.py` & `zod-0.2.7/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/anno/tsr/traffic_sign.py` & `zod-0.2.7/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/cli/download_zod.py` & `zod-0.2.7/zod/cli/download_zod.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,18 +232,17 @@
     if not settings.vehicle_data and "vehicle_data" in entry.name:
         return False
     if "lidar" in entry.name:
         if not settings.lidar:
             return False
         if "after" in entry.name or "before" in entry.name:
             # this is only the case for frames, where we have surrounding frames
-            distance = entry.name.split("_")[2][:2]
-            if "after" in entry.name and (int(distance) > settings.num_scans_after):
-                return False
-            if "before" in entry.name and (int(distance) > settings.num_scans_before):
+            distance = int(entry.name.split("_")[2][:2])
+            tgt = settings.num_scans_before if "before" in entry.name else settings.num_scans_after
+            if tgt != -1 and distance > tgt:
                 return False
     return True
 
 
 def _download_dataset(dl_settings: DownloadSettings, filter_settings: FilterSettings, dirname: str):
     dbx = ResumableDropbox(app_key=APP_KEY, oauth2_refresh_token=REFRESH_TOKEN, timeout=TIMEOUT)
     url, entries = _list_folder(dl_settings.url, dbx, dirname)
```

### Comparing `zod-0.2.6/zod/cli/extract_tsr_patches.py` & `zod-0.2.7/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/cli/generate_coco_json.py` & `zod-0.2.7/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/cli/main.py` & `zod-0.2.7/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/cli/utils.py` & `zod-0.2.7/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/cli/visualize_lidar.py` & `zod-0.2.7/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/constants.py` & `zod-0.2.7/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/box.py` & `zod-0.2.7/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/calibration.py` & `zod-0.2.7/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/ego_motion.py` & `zod-0.2.7/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/frame.py` & `zod-0.2.7/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/geometry.py` & `zod-0.2.7/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/info.py` & `zod-0.2.7/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/metadata.py` & `zod-0.2.7/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/sensor.py` & `zod-0.2.7/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/sequence.py` & `zod-0.2.7/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/data_classes/vehicle_data.py` & `zod-0.2.7/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_experimental/eval.py` & `zod-0.2.7/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_experimental/matching.py` & `zod-0.2.7/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_experimental/utils.py` & `zod-0.2.7/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/constants.py` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.7/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/utils/compensation.py` & `zod-0.2.7/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/utils/geometry.py` & `zod-0.2.7/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/utils/polygon_transformations.py` & `zod-0.2.7/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/utils/utils.py` & `zod-0.2.7/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/utils/visualization.py` & `zod-0.2.7/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/bev_utils.py` & `zod-0.2.7/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/colorlabeler.py` & `zod-0.2.7/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/lidar_3d.py` & `zod-0.2.7/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/lidar_bev.py` & `zod-0.2.7/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/lidar_on_image.py` & `zod-0.2.7/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/object_visualization.py` & `zod-0.2.7/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/oxts_on_image.py` & `zod-0.2.7/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/oxts_visualization.py` & `zod-0.2.7/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/visualization/polygon_utils.py` & `zod-0.2.7/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/zod_drives.py` & `zod-0.2.7/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/zod_frames.py` & `zod-0.2.7/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/zod/zod_sequences.py` & `zod-0.2.7/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.6/PKG-INFO` & `zod-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.2.6
+Version: 0.2.7
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

