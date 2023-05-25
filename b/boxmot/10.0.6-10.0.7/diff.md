# Comparing `tmp/boxmot-10.0.6.tar.gz` & `tmp/boxmot-10.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxmot-10.0.6.tar", last modified: Thu May 25 17:01:56 2023, max compression
+gzip compressed data, was "boxmot-10.0.7.tar", last modified: Thu May 25 20:51:04 2023, max compression
```

## Comparing `boxmot-10.0.6.tar` & `boxmot-10.0.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 17:00:33.000000 boxmot-10.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 17:01:56.605251 boxmot-10.0.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11421 2023-05-25 17:00:33.000000 boxmot-10.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/botsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/bytetrack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/deep/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/bnneck.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/hacnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/inceptionresnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/lmbn_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/mlfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/mudeep.py
--rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/osnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/osnet_ain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/pcb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnet_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnet_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnetmid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/shufflenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/reid_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/reid_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/reid_multibackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/deepocsort/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/association.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/cmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/kalmanfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/ocsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/ocsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/association.py
--rw-r--r--   0 runner    (1001) docker     (123)    59022 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/kalmanfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/ocsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/strongsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/strongsort/sort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/strong_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/strongsort/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/tracker_zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:01:56.605251 boxmot-10.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-25 17:00:33.000000 boxmot-10.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.740467 boxmot-10.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 20:49:17.000000 boxmot-10.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 20:51:04.740467 boxmot-10.0.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11421 2023-05-25 20:49:17.000000 boxmot-10.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.728467 boxmot-10.0.7/boxmot/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-25 20:51:03.000000 boxmot-10.0.7/boxmot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.728467 boxmot-10.0.7/boxmot/botsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/botsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/botsort/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/botsort/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/botsort/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/botsort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/botsort/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.728467 boxmot-10.0.7/boxmot/bytetrack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/bytetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/bytetrack/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/bytetrack/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/bytetrack/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/bytetrack/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.732468 boxmot-10.0.7/boxmot/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.736467 boxmot-10.0.7/boxmot/deep/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/bnneck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/hacnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/inceptionresnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/inceptionv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/lmbn_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/mlfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/mudeep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/osnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/osnet_ain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/pcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/resnet_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/resnet_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/resnetmid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/shufflenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/models/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/reid_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/reid_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deep/reid_multibackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.736467 boxmot-10.0.7/boxmot/deepocsort/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/cmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/kalmanfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/deepocsort/ocsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.736467 boxmot-10.0.7/boxmot/ocsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/ocsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/ocsort/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59022 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/ocsort/kalmanfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/ocsort/ocsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.736467 boxmot-10.0.7/boxmot/strongsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.740467 boxmot-10.0.7/boxmot/strongsort/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/sort/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/strong_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.740467 boxmot-10.0.7/boxmot/strongsort/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/strongsort/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-25 20:49:17.000000 boxmot-10.0.7/boxmot/tracker_zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:51:04.728467 boxmot-10.0.7/boxmot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 20:51:04.000000 boxmot-10.0.7/boxmot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 20:51:04.000000 boxmot-10.0.7/boxmot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:51:04.000000 boxmot-10.0.7/boxmot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:51:04.000000 boxmot-10.0.7/boxmot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 20:51:04.000000 boxmot-10.0.7/boxmot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:51:04.740467 boxmot-10.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-25 20:49:17.000000 boxmot-10.0.7/setup.py
```

### Comparing `boxmot-10.0.6/LICENSE` & `boxmot-10.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/PKG-INFO` & `boxmot-10.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxmot
-Version: 10.0.6
+Version: 10.0.7
 Summary: SOTA tracking methods for detection, segmentation and pose estimation models.
 Home-page: https://github.com/mikel-brostrom/yolov8_tracking
 Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues
 Project-URL: Source, https://github.com/mikel-brostrom/yolo_tracking
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boxmot Version: 10.0.6 Summary: SOTA tracking
+Metadata-Version: 2.1 Name: boxmot Version: 10.0.7 Summary: SOTA tracking
 methods for detection, segmentation and pose estimation models. Home-page:
 https://github.com/mikel-brostrom/yolov8_tracking Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues Project-
 URL: Source, https://github.com/mikel-brostrom/yolo_tracking Keywords: machine-
 learning,deep-learning,vision,ML,DL,AI,YOLO Platform: linux Platform: windows
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
```

### Comparing `boxmot-10.0.6/README.md` & `boxmot-10.0.7/README.md`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/__init__.py` & `boxmot-10.0.7/boxmot/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '10.0.6'
+__version__ = '10.0.7'
 
 from pathlib import Path
 
 from boxmot.strongsort.strong_sort import StrongSORT
 from boxmot.ocsort.ocsort import OCSort as OCSORT
 from boxmot.bytetrack.byte_tracker import BYTETracker
 from boxmot.botsort.bot_sort import BoTSORT
```

### Comparing `boxmot-10.0.6/boxmot/botsort/basetrack.py` & `boxmot-10.0.7/boxmot/botsort/basetrack.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/botsort/bot_sort.py` & `boxmot-10.0.7/boxmot/botsort/bot_sort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/botsort/gmc.py` & `boxmot-10.0.7/boxmot/botsort/gmc.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/botsort/kalman_filter.py` & `boxmot-10.0.7/boxmot/botsort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/botsort/matching.py` & `boxmot-10.0.7/boxmot/botsort/matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/bytetrack/basetrack.py` & `boxmot-10.0.7/boxmot/bytetrack/basetrack.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/bytetrack/byte_tracker.py` & `boxmot-10.0.7/boxmot/bytetrack/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/bytetrack/kalman_filter.py` & `boxmot-10.0.7/boxmot/bytetrack/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/bytetrack/matching.py` & `boxmot-10.0.7/boxmot/bytetrack/matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/__init__.py` & `boxmot-10.0.7/boxmot/deep/models/__init__.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/attention.py` & `boxmot-10.0.7/boxmot/deep/models/attention.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/bnneck.py` & `boxmot-10.0.7/boxmot/deep/models/bnneck.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/densenet.py` & `boxmot-10.0.7/boxmot/deep/models/densenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/hacnn.py` & `boxmot-10.0.7/boxmot/deep/models/hacnn.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/inceptionresnetv2.py` & `boxmot-10.0.7/boxmot/deep/models/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/inceptionv4.py` & `boxmot-10.0.7/boxmot/deep/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/lmbn_n.py` & `boxmot-10.0.7/boxmot/deep/models/lmbn_n.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/mlfn.py` & `boxmot-10.0.7/boxmot/deep/models/mlfn.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/mobilenetv2.py` & `boxmot-10.0.7/boxmot/deep/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/mudeep.py` & `boxmot-10.0.7/boxmot/deep/models/mudeep.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/nasnet.py` & `boxmot-10.0.7/boxmot/deep/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/osnet.py` & `boxmot-10.0.7/boxmot/deep/models/osnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/osnet_ain.py` & `boxmot-10.0.7/boxmot/deep/models/osnet_ain.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/pcb.py` & `boxmot-10.0.7/boxmot/deep/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/resnet.py` & `boxmot-10.0.7/boxmot/deep/models/resnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/resnet_ibn_a.py` & `boxmot-10.0.7/boxmot/deep/models/resnet_ibn_a.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/resnet_ibn_b.py` & `boxmot-10.0.7/boxmot/deep/models/resnet_ibn_b.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/resnetmid.py` & `boxmot-10.0.7/boxmot/deep/models/resnetmid.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/senet.py` & `boxmot-10.0.7/boxmot/deep/models/senet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/shufflenet.py` & `boxmot-10.0.7/boxmot/deep/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/shufflenetv2.py` & `boxmot-10.0.7/boxmot/deep/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/squeezenet.py` & `boxmot-10.0.7/boxmot/deep/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/models/xception.py` & `boxmot-10.0.7/boxmot/deep/models/xception.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/reid_export.py` & `boxmot-10.0.7/boxmot/deep/reid_export.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/reid_model_factory.py` & `boxmot-10.0.7/boxmot/deep/reid_model_factory.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deep/reid_multibackend.py` & `boxmot-10.0.7/boxmot/deep/reid_multibackend.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deepocsort/args.py` & `boxmot-10.0.7/boxmot/deepocsort/args.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deepocsort/association.py` & `boxmot-10.0.7/boxmot/deepocsort/association.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deepocsort/cmc.py` & `boxmot-10.0.7/boxmot/deepocsort/cmc.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deepocsort/embedding.py` & `boxmot-10.0.7/boxmot/deepocsort/embedding.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deepocsort/kalmanfilter.py` & `boxmot-10.0.7/boxmot/deepocsort/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/deepocsort/ocsort.py` & `boxmot-10.0.7/boxmot/deepocsort/ocsort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/ocsort/association.py` & `boxmot-10.0.7/boxmot/ocsort/association.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/ocsort/kalmanfilter.py` & `boxmot-10.0.7/boxmot/ocsort/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/ocsort/ocsort.py` & `boxmot-10.0.7/boxmot/ocsort/ocsort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/detection.py` & `boxmot-10.0.7/boxmot/strongsort/sort/detection.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/iou_matching.py` & `boxmot-10.0.7/boxmot/strongsort/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/kalman_filter.py` & `boxmot-10.0.7/boxmot/strongsort/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/linear_assignment.py` & `boxmot-10.0.7/boxmot/strongsort/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/nn_matching.py` & `boxmot-10.0.7/boxmot/strongsort/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/preprocessing.py` & `boxmot-10.0.7/boxmot/strongsort/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/track.py` & `boxmot-10.0.7/boxmot/strongsort/sort/track.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/sort/tracker.py` & `boxmot-10.0.7/boxmot/strongsort/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/strong_sort.py` & `boxmot-10.0.7/boxmot/strongsort/strong_sort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/utils/draw.py` & `boxmot-10.0.7/boxmot/strongsort/utils/draw.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/utils/evaluation.py` & `boxmot-10.0.7/boxmot/strongsort/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/utils/io.py` & `boxmot-10.0.7/boxmot/strongsort/utils/io.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/utils/json_logger.py` & `boxmot-10.0.7/boxmot/strongsort/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/utils/parser.py` & `boxmot-10.0.7/boxmot/strongsort/utils/parser.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/strongsort/utils/tools.py` & `boxmot-10.0.7/boxmot/strongsort/utils/tools.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot/tracker_zoo.py` & `boxmot-10.0.7/boxmot/tracker_zoo.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/boxmot.egg-info/PKG-INFO` & `boxmot-10.0.7/boxmot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxmot
-Version: 10.0.6
+Version: 10.0.7
 Summary: SOTA tracking methods for detection, segmentation and pose estimation models.
 Home-page: https://github.com/mikel-brostrom/yolov8_tracking
 Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues
 Project-URL: Source, https://github.com/mikel-brostrom/yolo_tracking
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boxmot Version: 10.0.6 Summary: SOTA tracking
+Metadata-Version: 2.1 Name: boxmot Version: 10.0.7 Summary: SOTA tracking
 methods for detection, segmentation and pose estimation models. Home-page:
 https://github.com/mikel-brostrom/yolov8_tracking Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues Project-
 URL: Source, https://github.com/mikel-brostrom/yolo_tracking Keywords: machine-
 learning,deep-learning,vision,ML,DL,AI,YOLO Platform: linux Platform: windows
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
```

### Comparing `boxmot-10.0.6/boxmot.egg-info/SOURCES.txt` & `boxmot-10.0.7/boxmot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.6/setup.py` & `boxmot-10.0.7/setup.py`

 * *Files identical despite different names*

