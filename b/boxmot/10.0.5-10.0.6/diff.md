# Comparing `tmp/boxmot-10.0.5.tar.gz` & `tmp/boxmot-10.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxmot-10.0.5.tar", last modified: Wed May 24 13:32:14 2023, max compression
+gzip compressed data, was "boxmot-10.0.6.tar", last modified: Thu May 25 17:01:56 2023, max compression
```

## Comparing `boxmot-10.0.5.tar` & `boxmot-10.0.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.973962 boxmot-10.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-24 13:30:30.000000 boxmot-10.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-05-24 13:32:14.973962 boxmot-10.0.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11100 2023-05-24 13:30:30.000000 boxmot-10.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.957962 boxmot-10.0.5/boxmot/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.961962 boxmot-10.0.5/boxmot/botsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/botsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/botsort/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/botsort/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/botsort/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/botsort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/botsort/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.961962 boxmot-10.0.5/boxmot/bytetrack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/bytetrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/bytetrack/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/bytetrack/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/bytetrack/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/bytetrack/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.961962 boxmot-10.0.5/boxmot/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.965962 boxmot-10.0.5/boxmot/deep/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/bnneck.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/hacnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/inceptionresnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/lmbn_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/mlfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/mudeep.py
--rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/osnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/osnet_ain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/pcb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/resnet_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/resnet_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/resnetmid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/shufflenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/models/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/reid_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/reid_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deep/reid_multibackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.969962 boxmot-10.0.5/boxmot/deepocsort/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/association.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/cmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/kalmanfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/deepocsort/ocsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.969962 boxmot-10.0.5/boxmot/ocsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/ocsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/ocsort/association.py
--rw-r--r--   0 runner    (1001) docker     (123)    59022 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/ocsort/kalmanfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/ocsort/ocsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.969962 boxmot-10.0.5/boxmot/strongsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.969962 boxmot-10.0.5/boxmot/strongsort/sort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/sort/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/strong_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.973962 boxmot-10.0.5/boxmot/strongsort/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/strongsort/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-24 13:30:30.000000 boxmot-10.0.5/boxmot/tracker_zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:32:14.961962 boxmot-10.0.5/boxmot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-05-24 13:32:14.000000 boxmot-10.0.5/boxmot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-24 13:32:14.000000 boxmot-10.0.5/boxmot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:32:14.000000 boxmot-10.0.5/boxmot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 13:32:14.000000 boxmot-10.0.5/boxmot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 13:32:14.000000 boxmot-10.0.5/boxmot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:32:14.973962 boxmot-10.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-24 13:30:30.000000 boxmot-10.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 17:00:33.000000 boxmot-10.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 17:01:56.605251 boxmot-10.0.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11421 2023-05-25 17:00:33.000000 boxmot-10.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/botsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/botsort/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/bytetrack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/bytetrack/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/deep/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/bnneck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/hacnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/inceptionresnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/inceptionv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/lmbn_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/mlfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/mudeep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/osnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/osnet_ain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/pcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnet_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnet_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/resnetmid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/shufflenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/models/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/reid_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/reid_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deep/reid_multibackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/deepocsort/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/cmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/kalmanfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/deepocsort/ocsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/ocsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59022 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/kalmanfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/ocsort/ocsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/strongsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/strongsort/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/sort/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/strong_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.605251 boxmot-10.0.6/boxmot/strongsort/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/strongsort/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-25 17:00:33.000000 boxmot-10.0.6/boxmot/tracker_zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:56.601251 boxmot-10.0.6/boxmot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:01:56.000000 boxmot-10.0.6/boxmot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:01:56.605251 boxmot-10.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-25 17:00:33.000000 boxmot-10.0.6/setup.py
```

### Comparing `boxmot-10.0.5/LICENSE` & `boxmot-10.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/PKG-INFO` & `boxmot-10.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxmot
-Version: 10.0.5
+Version: 10.0.6
 Summary: SOTA tracking methods for detection, segmentation and pose estimation models.
 Home-page: https://github.com/mikel-brostrom/yolov8_tracking
 Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues
 Project-URL: Source, https://github.com/mikel-brostrom/yolo_tracking
@@ -245,16 +245,24 @@
 ## Custom object detection model example
   
 <details>
 <summary>Click to exapand!</summary>
 
 ```python
 from boxmot import DeepOCSORT
+from pathlib import Path
 
-tracker = DeepOCSORT()
+
+tracker = DeepOCSORT(
+  model_weights=Path('mobilenetv2_x1_4_dukemtmcreid.pt'),  # which ReID model to use, when applicable
+  device='cuda:0',  # 'cpu', 'cuda:0', 'cuda:1', ... 'cuda:N'
+  fp16=True,  # wether to run the ReID model with half precision or not
+  det_thresh=0.2  # minimum valid detection confidence
+)
+  
 cap = cv.VideoCapture(0)
 while True:
     ret, im = cap.read()
     ...
     # dets: 
     #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
     # im:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boxmot Version: 10.0.5 Summary: SOTA tracking
+Metadata-Version: 2.1 Name: boxmot Version: 10.0.6 Summary: SOTA tracking
 methods for detection, segmentation and pose estimation models. Home-page:
 https://github.com/mikel-brostrom/yolov8_tracking Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues Project-
 URL: Source, https://github.com/mikel-brostrom/yolo_tracking Keywords: machine-
 learning,deep-learning,vision,ML,DL,AI,YOLO Platform: linux Platform: windows
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
@@ -123,16 +123,21 @@
 HOTA, MOTA, IDF1. Run it by ```bash $ python examples/evolve.py --tracking-
 method strongsort --benchmark MOT17 --n-trials 100 # tune strongsort for MOT17
 --tracking-method ocsort --benchmark  --objective HOTA # tune ocsort for
 maximizing HOTA on your custom tracking dataset ``` The set of hyperparameters
 leading to the best HOTA result are written to the tracker's config file.   ##
 Yolo-NAS tracking example  Click to expand! ```bash $ python examples/
 yolo_nas_track.py --source 0 ```  ## Custom object detection model example
-Click to exapand! ```python from boxmot import DeepOCSORT tracker = DeepOCSORT
-() cap = cv.VideoCapture(0) while True: ret, im = cap.read() ... # dets: # -
-your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls) # im: # - the
-original image (for better ReID results) # - the downscaled one fed to you
-model (faster) tracker_outputs = tracker.update(dets.cpu(), im) # --> (x, y, x,
-y, id, conf, cls) ... ```  ## Contact For Yolov8 tracking bugs and feature
-requests please visit [GitHub Issues](https://github.com/mikel-brostrom/
-Yolov5_StrongSORT_OSNet/issues). For business inquiries or professional support
-requests please send an email to: yolov5.deepsort.pytorch@gmail.com
+Click to exapand! ```python from boxmot import DeepOCSORT from pathlib import
+Path tracker = DeepOCSORT( model_weights=Path
+('mobilenetv2_x1_4_dukemtmcreid.pt'), # which ReID model to use, when
+applicable device='cuda:0', # 'cpu', 'cuda:0', 'cuda:1', ... 'cuda:N'
+fp16=True, # wether to run the ReID model with half precision or not
+det_thresh=0.2 # minimum valid detection confidence ) cap = cv.VideoCapture(0)
+while True: ret, im = cap.read() ... # dets: # - your model's nms:ed outputs of
+shape Nx6 (x, y, x, y, conf, cls) # im: # - the original image (for better ReID
+results) # - the downscaled one fed to you model (faster) tracker_outputs =
+tracker.update(dets.cpu(), im) # --> (x, y, x, y, id, conf, cls) ... ```  ##
+Contact For Yolov8 tracking bugs and feature requests please visit [GitHub
+Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). For
+business inquiries or professional support requests please send an email to:
+yolov5.deepsort.pytorch@gmail.com
```

### Comparing `boxmot-10.0.5/README.md` & `boxmot-10.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -212,16 +212,24 @@
 ## Custom object detection model example
   
 <details>
 <summary>Click to exapand!</summary>
 
 ```python
 from boxmot import DeepOCSORT
+from pathlib import Path
 
-tracker = DeepOCSORT()
+
+tracker = DeepOCSORT(
+  model_weights=Path('mobilenetv2_x1_4_dukemtmcreid.pt'),  # which ReID model to use, when applicable
+  device='cuda:0',  # 'cpu', 'cuda:0', 'cuda:1', ... 'cuda:N'
+  fp16=True,  # wether to run the ReID model with half precision or not
+  det_thresh=0.2  # minimum valid detection confidence
+)
+  
 cap = cv.VideoCapture(0)
 while True:
     ret, im = cap.read()
     ...
     # dets: 
     #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
     # im:
```

#### html2text {}

```diff
@@ -103,16 +103,21 @@
 HOTA, MOTA, IDF1. Run it by ```bash $ python examples/evolve.py --tracking-
 method strongsort --benchmark MOT17 --n-trials 100 # tune strongsort for MOT17
 --tracking-method ocsort --benchmark  --objective HOTA # tune ocsort for
 maximizing HOTA on your custom tracking dataset ``` The set of hyperparameters
 leading to the best HOTA result are written to the tracker's config file.   ##
 Yolo-NAS tracking example  Click to expand! ```bash $ python examples/
 yolo_nas_track.py --source 0 ```  ## Custom object detection model example
-Click to exapand! ```python from boxmot import DeepOCSORT tracker = DeepOCSORT
-() cap = cv.VideoCapture(0) while True: ret, im = cap.read() ... # dets: # -
-your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls) # im: # - the
-original image (for better ReID results) # - the downscaled one fed to you
-model (faster) tracker_outputs = tracker.update(dets.cpu(), im) # --> (x, y, x,
-y, id, conf, cls) ... ```  ## Contact For Yolov8 tracking bugs and feature
-requests please visit [GitHub Issues](https://github.com/mikel-brostrom/
-Yolov5_StrongSORT_OSNet/issues). For business inquiries or professional support
-requests please send an email to: yolov5.deepsort.pytorch@gmail.com
+Click to exapand! ```python from boxmot import DeepOCSORT from pathlib import
+Path tracker = DeepOCSORT( model_weights=Path
+('mobilenetv2_x1_4_dukemtmcreid.pt'), # which ReID model to use, when
+applicable device='cuda:0', # 'cpu', 'cuda:0', 'cuda:1', ... 'cuda:N'
+fp16=True, # wether to run the ReID model with half precision or not
+det_thresh=0.2 # minimum valid detection confidence ) cap = cv.VideoCapture(0)
+while True: ret, im = cap.read() ... # dets: # - your model's nms:ed outputs of
+shape Nx6 (x, y, x, y, conf, cls) # im: # - the original image (for better ReID
+results) # - the downscaled one fed to you model (faster) tracker_outputs =
+tracker.update(dets.cpu(), im) # --> (x, y, x, y, id, conf, cls) ... ```  ##
+Contact For Yolov8 tracking bugs and feature requests please visit [GitHub
+Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). For
+business inquiries or professional support requests please send an email to:
+yolov5.deepsort.pytorch@gmail.com
```

### Comparing `boxmot-10.0.5/boxmot/__init__.py` & `boxmot-10.0.6/boxmot/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '10.0.5'
+__version__ = '10.0.6'
 
 from pathlib import Path
 
 from boxmot.strongsort.strong_sort import StrongSORT
 from boxmot.ocsort.ocsort import OCSort as OCSORT
 from boxmot.bytetrack.byte_tracker import BYTETracker
 from boxmot.botsort.bot_sort import BoTSORT
```

### Comparing `boxmot-10.0.5/boxmot/botsort/basetrack.py` & `boxmot-10.0.6/boxmot/botsort/basetrack.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/botsort/bot_sort.py` & `boxmot-10.0.6/boxmot/botsort/bot_sort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/botsort/gmc.py` & `boxmot-10.0.6/boxmot/botsort/gmc.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/botsort/kalman_filter.py` & `boxmot-10.0.6/boxmot/botsort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/botsort/matching.py` & `boxmot-10.0.6/boxmot/botsort/matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/bytetrack/basetrack.py` & `boxmot-10.0.6/boxmot/bytetrack/basetrack.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/bytetrack/byte_tracker.py` & `boxmot-10.0.6/boxmot/bytetrack/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/bytetrack/kalman_filter.py` & `boxmot-10.0.6/boxmot/bytetrack/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/bytetrack/matching.py` & `boxmot-10.0.6/boxmot/bytetrack/matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/__init__.py` & `boxmot-10.0.6/boxmot/deep/models/__init__.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/attention.py` & `boxmot-10.0.6/boxmot/deep/models/attention.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/bnneck.py` & `boxmot-10.0.6/boxmot/deep/models/bnneck.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/densenet.py` & `boxmot-10.0.6/boxmot/deep/models/densenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/hacnn.py` & `boxmot-10.0.6/boxmot/deep/models/hacnn.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/inceptionresnetv2.py` & `boxmot-10.0.6/boxmot/deep/models/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/inceptionv4.py` & `boxmot-10.0.6/boxmot/deep/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/lmbn_n.py` & `boxmot-10.0.6/boxmot/deep/models/lmbn_n.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/mlfn.py` & `boxmot-10.0.6/boxmot/deep/models/mlfn.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/mobilenetv2.py` & `boxmot-10.0.6/boxmot/deep/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/mudeep.py` & `boxmot-10.0.6/boxmot/deep/models/mudeep.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/nasnet.py` & `boxmot-10.0.6/boxmot/deep/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/osnet.py` & `boxmot-10.0.6/boxmot/deep/models/osnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/osnet_ain.py` & `boxmot-10.0.6/boxmot/deep/models/osnet_ain.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/pcb.py` & `boxmot-10.0.6/boxmot/deep/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/resnet.py` & `boxmot-10.0.6/boxmot/deep/models/resnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/resnet_ibn_a.py` & `boxmot-10.0.6/boxmot/deep/models/resnet_ibn_a.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/resnet_ibn_b.py` & `boxmot-10.0.6/boxmot/deep/models/resnet_ibn_b.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/resnetmid.py` & `boxmot-10.0.6/boxmot/deep/models/resnetmid.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/senet.py` & `boxmot-10.0.6/boxmot/deep/models/senet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/shufflenet.py` & `boxmot-10.0.6/boxmot/deep/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/shufflenetv2.py` & `boxmot-10.0.6/boxmot/deep/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/squeezenet.py` & `boxmot-10.0.6/boxmot/deep/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/models/xception.py` & `boxmot-10.0.6/boxmot/deep/models/xception.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/reid_export.py` & `boxmot-10.0.6/boxmot/deep/reid_export.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/reid_model_factory.py` & `boxmot-10.0.6/boxmot/deep/reid_model_factory.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deep/reid_multibackend.py` & `boxmot-10.0.6/boxmot/deep/reid_multibackend.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deepocsort/args.py` & `boxmot-10.0.6/boxmot/deepocsort/args.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deepocsort/association.py` & `boxmot-10.0.6/boxmot/deepocsort/association.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deepocsort/cmc.py` & `boxmot-10.0.6/boxmot/deepocsort/cmc.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deepocsort/embedding.py` & `boxmot-10.0.6/boxmot/deepocsort/embedding.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deepocsort/kalmanfilter.py` & `boxmot-10.0.6/boxmot/deepocsort/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/deepocsort/ocsort.py` & `boxmot-10.0.6/boxmot/deepocsort/ocsort.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         """
         # define constant velocity model
         if not orig:
             from .kalmanfilter import KalmanFilterNew as KalmanFilter
         else:
             from filterpy.kalman import KalmanFilter
         self.cls = cls
+        
         self.conf = bbox[-1]
         self.new_kf = new_kf
         if new_kf:
             self.kf = KalmanFilter(dim_x=8, dim_z=4)
             self.kf.F = np.array(
                 [
                     # x y w h x' y' w' h'
@@ -196,14 +197,15 @@
     def update(self, bbox, cls):
         """
         Updates the state vector with observed bbox.
         """
         if bbox is not None:
             self.frozen = False
             self.cls = cls
+            self.conf = bbox[-1]
             if self.last_observation.sum() >= 0:  # no previous observation
                 previous_box = None
                 for dt in range(self.delta_t, 0, -1):
                     if self.age - dt in self.observations:
                         previous_box = self.observations[self.age - dt]
                         break
                 if previous_box is None:
```

### Comparing `boxmot-10.0.5/boxmot/ocsort/association.py` & `boxmot-10.0.6/boxmot/ocsort/association.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/ocsort/kalmanfilter.py` & `boxmot-10.0.6/boxmot/ocsort/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/ocsort/ocsort.py` & `boxmot-10.0.6/boxmot/ocsort/ocsort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/detection.py` & `boxmot-10.0.6/boxmot/strongsort/sort/detection.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/iou_matching.py` & `boxmot-10.0.6/boxmot/strongsort/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/kalman_filter.py` & `boxmot-10.0.6/boxmot/strongsort/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/linear_assignment.py` & `boxmot-10.0.6/boxmot/strongsort/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/nn_matching.py` & `boxmot-10.0.6/boxmot/strongsort/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/preprocessing.py` & `boxmot-10.0.6/boxmot/strongsort/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/track.py` & `boxmot-10.0.6/boxmot/strongsort/sort/track.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/sort/tracker.py` & `boxmot-10.0.6/boxmot/strongsort/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/strong_sort.py` & `boxmot-10.0.6/boxmot/strongsort/strong_sort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/utils/draw.py` & `boxmot-10.0.6/boxmot/strongsort/utils/draw.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/utils/evaluation.py` & `boxmot-10.0.6/boxmot/strongsort/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/utils/io.py` & `boxmot-10.0.6/boxmot/strongsort/utils/io.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/utils/json_logger.py` & `boxmot-10.0.6/boxmot/strongsort/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/utils/parser.py` & `boxmot-10.0.6/boxmot/strongsort/utils/parser.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/strongsort/utils/tools.py` & `boxmot-10.0.6/boxmot/strongsort/utils/tools.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot/tracker_zoo.py` & `boxmot-10.0.6/boxmot/tracker_zoo.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/boxmot.egg-info/PKG-INFO` & `boxmot-10.0.6/boxmot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxmot
-Version: 10.0.5
+Version: 10.0.6
 Summary: SOTA tracking methods for detection, segmentation and pose estimation models.
 Home-page: https://github.com/mikel-brostrom/yolov8_tracking
 Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues
 Project-URL: Source, https://github.com/mikel-brostrom/yolo_tracking
@@ -245,16 +245,24 @@
 ## Custom object detection model example
   
 <details>
 <summary>Click to exapand!</summary>
 
 ```python
 from boxmot import DeepOCSORT
+from pathlib import Path
 
-tracker = DeepOCSORT()
+
+tracker = DeepOCSORT(
+  model_weights=Path('mobilenetv2_x1_4_dukemtmcreid.pt'),  # which ReID model to use, when applicable
+  device='cuda:0',  # 'cpu', 'cuda:0', 'cuda:1', ... 'cuda:N'
+  fp16=True,  # wether to run the ReID model with half precision or not
+  det_thresh=0.2  # minimum valid detection confidence
+)
+  
 cap = cv.VideoCapture(0)
 while True:
     ret, im = cap.read()
     ...
     # dets: 
     #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
     # im:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boxmot Version: 10.0.5 Summary: SOTA tracking
+Metadata-Version: 2.1 Name: boxmot Version: 10.0.6 Summary: SOTA tracking
 methods for detection, segmentation and pose estimation models. Home-page:
 https://github.com/mikel-brostrom/yolov8_tracking Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/mikel-brostrom/yolo_tracking/issues Project-
 URL: Source, https://github.com/mikel-brostrom/yolo_tracking Keywords: machine-
 learning,deep-learning,vision,ML,DL,AI,YOLO Platform: linux Platform: windows
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
@@ -123,16 +123,21 @@
 HOTA, MOTA, IDF1. Run it by ```bash $ python examples/evolve.py --tracking-
 method strongsort --benchmark MOT17 --n-trials 100 # tune strongsort for MOT17
 --tracking-method ocsort --benchmark  --objective HOTA # tune ocsort for
 maximizing HOTA on your custom tracking dataset ``` The set of hyperparameters
 leading to the best HOTA result are written to the tracker's config file.   ##
 Yolo-NAS tracking example  Click to expand! ```bash $ python examples/
 yolo_nas_track.py --source 0 ```  ## Custom object detection model example
-Click to exapand! ```python from boxmot import DeepOCSORT tracker = DeepOCSORT
-() cap = cv.VideoCapture(0) while True: ret, im = cap.read() ... # dets: # -
-your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls) # im: # - the
-original image (for better ReID results) # - the downscaled one fed to you
-model (faster) tracker_outputs = tracker.update(dets.cpu(), im) # --> (x, y, x,
-y, id, conf, cls) ... ```  ## Contact For Yolov8 tracking bugs and feature
-requests please visit [GitHub Issues](https://github.com/mikel-brostrom/
-Yolov5_StrongSORT_OSNet/issues). For business inquiries or professional support
-requests please send an email to: yolov5.deepsort.pytorch@gmail.com
+Click to exapand! ```python from boxmot import DeepOCSORT from pathlib import
+Path tracker = DeepOCSORT( model_weights=Path
+('mobilenetv2_x1_4_dukemtmcreid.pt'), # which ReID model to use, when
+applicable device='cuda:0', # 'cpu', 'cuda:0', 'cuda:1', ... 'cuda:N'
+fp16=True, # wether to run the ReID model with half precision or not
+det_thresh=0.2 # minimum valid detection confidence ) cap = cv.VideoCapture(0)
+while True: ret, im = cap.read() ... # dets: # - your model's nms:ed outputs of
+shape Nx6 (x, y, x, y, conf, cls) # im: # - the original image (for better ReID
+results) # - the downscaled one fed to you model (faster) tracker_outputs =
+tracker.update(dets.cpu(), im) # --> (x, y, x, y, id, conf, cls) ... ```  ##
+Contact For Yolov8 tracking bugs and feature requests please visit [GitHub
+Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). For
+business inquiries or professional support requests please send an email to:
+yolov5.deepsort.pytorch@gmail.com
```

### Comparing `boxmot-10.0.5/boxmot.egg-info/SOURCES.txt` & `boxmot-10.0.6/boxmot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.5/setup.py` & `boxmot-10.0.6/setup.py`

 * *Files identical despite different names*

