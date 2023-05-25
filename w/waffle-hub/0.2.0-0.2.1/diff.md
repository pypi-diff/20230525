# Comparing `tmp/waffle_hub-0.2.0.tar.gz` & `tmp/waffle_hub-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.0.tar", last modified: Wed May  3 07:36:40 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.1.tar", last modified: Thu May 25 07:08:05 2023, max compression
```

## Comparing `waffle_hub-0.2.0.tar` & `waffle_hub-0.2.1.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.2.0/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.2.0/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      398 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8375 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10344 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3725 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      168 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2978 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4917 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/huggingface.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6352 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    36906 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10718 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7649 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3203 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9640 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13253 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35684 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9514 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      304 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    15174 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1680 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/conversion.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3218 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3706 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1919 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      319 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.2.1/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.2.1/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      398 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2670 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6092 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/tests/test_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8248 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10344 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3810 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      168 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3037 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4836 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/huggingface.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7268 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    40910 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2406 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10318 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8490 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2439 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/config.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3203 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8515 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4252 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12302 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    37106 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12854 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10134 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      304 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    15506 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/utils/conversion.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3218 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3706 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/utils/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2070 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       68 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      319 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.0/LICENSE` & `waffle_hub-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/PKG-INFO` & `waffle_hub-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.0
+Version: 0.2.1
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.0 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.1 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.0/README.md` & `waffle_hub-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/setup.py` & `waffle_hub-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,9 +62,9 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Operating System :: POSIX :: Linux",
         # 'Operating System :: MacOS',
         # 'Operating System :: Microsoft :: Windows',
     ],
     keywords="machine-learning, deep-learning, vision, ML, DL, AI, YOLO, Ultralytics, SNUAILAB",
-    entry_points={"console_scripts": ["wu = waffle_utils.run:app"]},
+    entry_points={"console_scripts": ["wu = waffle_utils.run:app", "wh = waffle_hub.run:app"]},
 )
```

### Comparing `waffle_hub-0.2.0/tests/test_dataset.py` & `waffle_hub-0.2.1/tests/test_dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     a = Annotation.semantic_segmentation(
         annotation_id=1,
         image_id=1,
         category_id=1,
         segmentation=segmentation,
         area=10000,
     )
+    assert a.bbox == [110, 110, 20, 20]
 
     # keypoint detection
     a = Annotation.keypoint_detection(
         annotation_id=1,
         image_id=1,
         category_id=1,
         keypoints=keypoints,
@@ -110,182 +111,155 @@
     dataset: Dataset = Dataset.new(name="test_new", task=TaskType.OBJECT_DETECTION, root_dir=tmpdir)
     assert Path(dataset.dataset_dir).exists()
 
     dataset.delete()
     assert not Path(dataset.dataset_dir).exists()
 
 
-def test_dataset_coco(coco_path, tmpdir):
+def _load(dataset_name, root_dir):
+    Dataset.load(dataset_name, root_dir=root_dir)
 
-    ds = Dataset.from_coco(
-        name="from_coco",
-        task=TaskType.OBJECT_DETECTION,
-        coco_file=coco_path / "coco.json",
-        coco_root_dir=coco_path / "images",
-        root_dir=tmpdir,
-    )
-    assert ds.dataset_info_file.exists()
-
-    ds = Dataset.from_coco(
-        name="import_train_val",
-        task=TaskType.OBJECT_DETECTION,
-        coco_file=[coco_path / "train.json", coco_path / "val.json"],
-        coco_root_dir=coco_path / "images",
-        root_dir=tmpdir,
-    )
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) == 60
-    assert len(val_ids) == 20
-    assert len(val_ids) == len(test_ids)
-    assert len(ds.images) == 80
 
-    ds = Dataset.from_coco(
-        name="import_train_val_test",
-        task=TaskType.OBJECT_DETECTION,
-        coco_file=[coco_path / "train.json", coco_path / "val.json", coco_path / "test.json"],
-        coco_root_dir=coco_path / "images",
-        root_dir=tmpdir,
+def _clone(dataset_name, root_dir):
+    Dataset.clone(
+        src_name=dataset_name,
+        name="clone_" + dataset_name,
+        src_root_dir=root_dir,
+        root_dir=root_dir,
     )
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) == 60
-    assert len(val_ids) == 20
-    assert len(test_ids) == 20
-    assert len(ds.images) == 100
 
-    ds = Dataset.load("from_coco", root_dir=tmpdir)
 
-    ds = Dataset.clone(
-        src_name="from_coco",
-        name="clone_coco",
-        src_root_dir=tmpdir,
-        root_dir=tmpdir,
-    )
+def _split(dataset_name, root_dir):
+    dataset = Dataset.load(dataset_name, root_dir=root_dir)
 
-    with pytest.raises(FileNotFoundError):
-        ds.export("coco")
+    dataset.split(0.8)
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) + len(val_ids) == len(dataset.images)
 
-    ds.split(0.8)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(ds.images)
+    dataset.split(0.445446, 0.554554)
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) + len(val_ids) == len(dataset.images)
 
-    ds.split(0.445446, 0.554554)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(ds.images)
+    dataset.split(0.4, 0.4, 0.2)
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) + len(val_ids) + len(test_ids) == len(dataset.images)
 
-    ds.split(0.4, 0.4, 0.2)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) + len(test_ids) == len(ds.images)
+    dataset.split(0.99999999999999, 0.0)
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 99 and len(val_ids) == 1 and len(test_ids) == 1
 
-    ds.split(0.99999999999999, 0.0)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(val_ids) == 1 and len(test_ids) == 1
+    dataset.split(0.00000000000001, 0.0)
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 1 and len(val_ids) == 99 and len(test_ids) == 99
 
     with pytest.raises(ValueError):
-        ds.split(0.0, 0.2)
+        dataset.split(0.0, 0.2)
 
     with pytest.raises(ValueError):
-        ds.split(0.9, 0.2)
-
-    ds.export("coco")
+        dataset.split(0.9, 0.2)
 
 
-def test_dataset_yolo(yolo_path, tmpdir):
+def _export(dataset_name, task: TaskType, root_dir):
+    dataset = Dataset.load(dataset_name, root_dir=root_dir)
 
-    ds = Dataset.from_yolo(
-        name="from_yolo",
-        task=TaskType.OBJECT_DETECTION,
-        yaml_path=yolo_path / "data.yaml",
-        root_dir=tmpdir,
-    )
-    assert ds.dataset_info_file.exists()
+    if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
+        dataset.export("coco")
+    if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
+        dataset.export("yolo")
+    if task in [TaskType.OBJECT_DETECTION, TaskType.CLASSIFICATION]:
+        dataset.export("huggingface")
 
-    ds = Dataset.load("from_yolo", root_dir=tmpdir)
 
-    ds = Dataset.clone(
-        src_name="from_yolo",
-        name="clone_yolo",
-        src_root_dir=tmpdir,
-        root_dir=tmpdir,
+# test coco
+def _from_coco(dataset_name, task: TaskType, coco_path, root_dir):
+    dataset = Dataset.from_coco(
+        name=dataset_name,
+        task=task,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=root_dir,
     )
+    assert dataset.dataset_info_file.exists()
 
-    with pytest.raises(FileNotFoundError):
-        ds.export("yolo")
-
-    ds.split(0.8)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(ds.images)
-
-    ds.split(0.445446, 0.554554)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(ds.images)
-
-    ds.split(0.4, 0.4, 0.2)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) + len(test_ids) == len(ds.images)
+    dataset = Dataset.from_coco(
+        name=f"{task}_import_train_val",
+        task=task,
+        coco_file=[coco_path / "train.json", coco_path / "val.json"],
+        coco_root_dir=coco_path / "images",
+        root_dir=root_dir,
+    )
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 60
+    assert len(val_ids) == 20
+    assert len(val_ids) == len(test_ids)
+    assert len(dataset.images) == 80
 
-    ds.split(0.99999999999999, 0.0)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(val_ids) == 1 and len(test_ids) == 1
+    dataset = Dataset.from_coco(
+        name=f"{task}_import_train_val_test",
+        task=task,
+        coco_file=[coco_path / "train.json", coco_path / "val.json", coco_path / "test.json"],
+        coco_root_dir=coco_path / "images",
+        root_dir=root_dir,
+    )
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 60
+    assert len(val_ids) == 20
+    assert len(test_ids) == 20
+    assert len(dataset.images) == 100
 
-    with pytest.raises(ValueError):
-        ds.split(0.0, 0.2)
 
-    with pytest.raises(ValueError):
-        ds.split(0.9, 0.2)
+def _total_coco(dataset_name, task: TaskType, coco_path, root_dir):
+    _from_coco(dataset_name, task, coco_path, root_dir)
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, task, root_dir)
 
-    ds.export("yolo")
 
+def test_coco(coco_path, tmpdir):
+    for task in [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]:
+        _total_coco(f"coco_{task}", task, coco_path, tmpdir)
 
-def test_dataset_huggingface(huggingface_path, tmpdir):
 
-    ds = Dataset.from_huggingface(
-        name="from_huggingface",
-        task=TaskType.OBJECT_DETECTION,
+# test huggingface
+def _from_huggingface(dataset_name, task: TaskType, huggingface_path, root_dir):
+    dataset = Dataset.from_huggingface(
+        name=dataset_name,
+        task=task,
         dataset_dir=huggingface_path,
-        root_dir=tmpdir,
-    )
-    assert ds.dataset_info_file.exists()
-
-    ds = Dataset.load("from_huggingface", root_dir=tmpdir)
-
-    ds = Dataset.clone(
-        src_name="from_huggingface",
-        name="clone_huggingface",
-        src_root_dir=tmpdir,
-        root_dir=tmpdir,
+        root_dir=root_dir,
     )
+    assert dataset.dataset_info_file.exists()
 
-    with pytest.raises(FileNotFoundError):
-        ds.export("huggingface")
-
-    ds.split(0.8)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(ds.images)
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 80
+    assert len(dataset.images) == 100
 
-    ds.split(0.445446, 0.554554)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(ds.images)
 
-    ds.split(0.4, 0.4, 0.2)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(train_ids) + len(val_ids) + len(test_ids) == len(ds.images)
+def _total_huggingface(dataset_name, task: TaskType, huggingface_path, root_dir):
+    _from_huggingface(dataset_name, task, huggingface_path, root_dir)
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, task, root_dir)
 
-    ds.split(0.99999999999999, 0.0)
-    train_ids, val_ids, test_ids, unlabeled_ids = ds.get_split_ids()
-    assert len(val_ids) == 1 and len(test_ids) == 1
 
-    with pytest.raises(ValueError):
-        ds.split(0.0, 0.2)
-
-    with pytest.raises(ValueError):
-        ds.split(0.9, 0.2)
-
-    ds.export("huggingface")
+def test_huggingface(huggingface_detection_path, huggingface_classification_path, tmpdir):
+    _total_huggingface(
+        "huggingface_object_detection", TaskType.OBJECT_DETECTION, huggingface_detection_path, tmpdir
+    )
+    _total_huggingface(
+        "huggingface_classification",
+        TaskType.CLASSIFICATION,
+        huggingface_classification_path,
+        tmpdir,
+    )
 
 
+# dataloader
 def test_image_dataloader(coco_path, tmpdir):
 
     image_dataset = ImageDataset(coco_path / "images", 224)
     assert len(image_dataset) == 100
     image_dataloader = image_dataset.get_dataloader(batch_size=32, num_workers=0)
     assert len(image_dataloader) == 4
```

### Comparing `waffle_hub-0.2.0/tests/test_hub.py` & `waffle_hub-0.2.1/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/__init__.py` & `waffle_hub-0.2.1/waffle_hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 import enum
 import importlib
 import warnings
 from collections import OrderedDict
 
 from tabulate import tabulate
@@ -152,7 +152,12 @@
     CLASSIFICATION = enum.auto()
     OBJECT_DETECTION = enum.auto()
     SEMANTIC_SEGMENTATION = enum.auto()
     INSTANCE_SEGMENTATION = enum.auto()
     KEYPOINT_DETECTION = enum.auto()
     TEXT_RECOGNITION = enum.auto()
     REGRESSION = enum.auto()
+
+
+class SplitMethod(BaseEnum):
+    RANDOM = enum.auto()
+    STRATIFIED = enum.auto()
```

### Comparing `waffle_hub-0.2.0/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.1/waffle_hub/dataset/adapter/coco.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             image_id = d.pop("image_id")
             coco["images"].append({"id": image_id, **d})
 
             annotations = self.image_to_annotations[image_id]
             for annotation in annotations:
                 d = annotation.to_dict()
                 if d.get("segmentation", None):
-                    d["segmentation"] = convert_rle_to_polygon(d["segmentation"])
+                    if isinstance(d["segmentation"], dict):
+                        d["segmentation"] = convert_rle_to_polygon(d["segmentation"])
                 annotation_id = d.pop("annotation_id")
                 coco["annotations"].append({"id": annotation_id, **d})
 
         io.save_json(coco, export_dir / f"{split}.json", create_directory=True)
 
 
 def export_coco(self, export_dir: Union[str, Path]) -> str:
@@ -85,10 +86,10 @@
     if self.task == TaskType.CLASSIFICATION:
         _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     elif self.task == TaskType.OBJECT_DETECTION:
         _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     elif self.task == TaskType.INSTANCE_SEGMENTATION:
         _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     else:
-        raise ValueError(f"Unsupported task type: {self.task_type}")
+        raise ValueError(f"Unsupported task type: {self.task}")
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.2.0/waffle_hub/dataset/adapter/huggingface.py` & `waffle_hub-0.2.1/waffle_hub/dataset/adapter/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,15 @@
             annotations = self.get_annotations(image.image_id)
             objects = []
             for annotation in annotations:
                 objects.append(
                     {
                         "id": annotation.annotation_id,
                         "area": annotation.area,
-                        "category": self.category_names[
-                            annotation.category_id - 1
-                        ],
+                        "category": self.category_names[annotation.category_id - 1],
                         "bbox": annotation.bbox,
                     }
                 )
 
             # image
             image_path = self.raw_image_dir / image.file_name
             pil_image = PIL.Image.open(image_path).convert("RGB")
@@ -157,14 +155,12 @@
     train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
         _export_huggingface_classification(
             self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
         )
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_huggingface_detection(
-            self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
-        )
+        _export_huggingface_detection(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     else:
-        raise ValueError(f"Unsupported task type: {self.task_type}")
+        raise ValueError(f"Unsupported task type: {self.task}")
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.2.0/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.1/waffle_hub/dataset/adapter/yolo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,42 @@
 import warnings
 from pathlib import Path
 from typing import Union
 
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
+from waffle_hub.schema.fields.image import Image
 from waffle_hub.utils.conversion import merge_multi_segment
 
 
+def _check_valid_file_paths(images: list[Image]) -> bool:
+    """Check file paths are valid
+    If the file name includes the words "images" or "labels," an error occurs during training
+
+    Args:
+        images (list[Image]): List of Image
+
+    Returns:
+        bool: True if valid
+    """
+    for image in images.values():
+        file_path = Path(image.file_name)
+        if "images" in file_path.parts:
+            raise ValueError(
+                f"The file path '{file_path}' is not allowed. Please choose a file path that does not contain the word 'images'"
+            )
+        if "labels" in file_path.parts:
+            raise ValueError(
+                f"The file path '{file_path}' is not allowed. Please choose a file path that does not contain the word 'labels'"
+            )
+    else:
+        return True
+
+
 def _export_yolo_classification(
     self,
     export_dir: Path,
     train_ids: list,
     val_ids: list,
     test_ids: list,
     unlabeled_ids: list,
@@ -167,14 +192,16 @@
 
     Args:
         export_dir (Union[str, Path]): Path to export directory
 
     Returns:
         str: Path to export directory
     """
+    _check_valid_file_paths(self.images)
+
     export_dir = Path(export_dir)
 
     train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
         _export_yolo_classification(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     elif self.task == TaskType.OBJECT_DETECTION:
```

### Comparing `waffle_hub-0.2.0/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.1/waffle_hub/dataset/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import logging
 import random
 import warnings
-from collections import OrderedDict
+from collections import OrderedDict, defaultdict
 from functools import cached_property
+from itertools import combinations
+from math import ceil, floor
 from pathlib import Path
 from typing import Union
 
 import cv2
 import PIL.Image
 import tqdm
 from pycocotools.coco import COCO
 from waffle_utils.file import io
 from waffle_utils.file.search import get_files, get_image_files
 from waffle_utils.log import datetime_now
 from waffle_utils.utils import type_validator
 
 from datasets import Dataset as HFDataset
 from datasets import DatasetDict, load_from_disk
-from waffle_hub import DataType, TaskType
+from waffle_hub import DataType, SplitMethod, TaskType
 from waffle_hub.dataset.adapter import (
     export_coco,
     export_huggingface,
     export_yolo,
 )
 from waffle_hub.schema import Annotation, Category, DatasetInfo, Image
 
@@ -184,25 +186,22 @@
     @cached_property
     def category_names(self) -> list[str]:
         categories: dict[int, Category] = self.categories
         return [c.name for c in sorted(categories.values(), key=lambda c: c.category_id)]
 
     @cached_property
     def image_to_annotations(self) -> dict[int, list[Annotation]]:
-        return OrderedDict(
-            {
-                image_id: list(
-                    filter(
-                        lambda a: a.image_id == image_id,
-                        self.annotations.values(),
-                    )
-                )
-                for image_id in self.images.keys()
-            }
-        )
+        if not hasattr(self, "_image_to_annotations"):
+            image_to_annotations = defaultdict(list)
+            for annotation in tqdm.tqdm(
+                self.annotations.values(), desc="Building image to annotation index"
+            ):
+                image_to_annotations[annotation.image_id].append(annotation)
+            self._image_to_annotations = dict(image_to_annotations)
+        return self._image_to_annotations
 
     # factories
     @classmethod
     def new(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
         """
         Create New Dataset.
         This method creates a new dataset directory and initialize dataset info file.
@@ -269,16 +268,16 @@
             Dataset: Dataset Class
         """
         src_ds = Dataset.load(src_name, src_root_dir)
         if not src_ds.initialized():
             raise FileNotFoundError(f"{src_ds.dataset_dir} has not been created by Waffle.")
 
         ds = Dataset.new(name, src_ds.task, root_dir)
-        ds.initialize()
         io.copy_files_to_directory(src_ds.dataset_dir, ds.dataset_dir, create_directory=True)
+        ds.initialize()
 
         return ds
 
     @classmethod
     def load(cls, name: str, root_dir: str = None) -> "Dataset":
         """
         Load Dataset.
@@ -547,15 +546,14 @@
                         Category.object_detection(
                             category_id=category_id + 1,
                             name=category_name,
                         )
                     ]
                 )
 
-            annotation_num = 0
             for image_id, image_path, label_path in zip(
                 image_ids,
                 get_image_files(image_dir),
                 get_files(label_dir, "txt"),
             ):
                 # image
                 img = cv2.imread(str(image_path))
@@ -567,35 +565,36 @@
                     height=height,
                 )
                 ds.add_images([image])
 
                 # annotation
                 with open(label_path) as f:  # TODO: use load_txt of waffle_utils after implementing
                     txt = f.readlines()
+
+                current_annotation_id = len(ds.get_annotations())
                 for i, t in enumerate(txt, start=1):
                     category_id, x, y, w, h = list(map(float, t.split()))
                     category_id = int(category_id) + 1
                     x *= width
                     y *= height
                     w *= width
                     h *= height
 
                     x -= w / 2
                     y -= h / 2
 
                     x, y, w, h = int(x), int(y), int(w), int(h)
                     annotation = Annotation.object_detection(
-                        annotation_id=annotation_num + i,
+                        annotation_id=current_annotation_id + i,
                         image_id=image_id,
                         category_id=category_id,
                         bbox=[x, y, w, h],
                         area=w * h,
                     )
                     ds.add_annotations([annotation])
-                annotation_num += len(txt)
 
                 # raw
                 dst = ds.raw_image_dir / f"{image_id}{image_path.suffix}"
                 io.copy_file(image_path, dst)
 
         if task == "object_detection":
             _import = _import_object_detection
@@ -619,14 +618,17 @@
 
             io.save_json(image_ids, ds.set_dir / f"{set_type}.json", True)
             current_image_id += image_num
 
             # import other field
             _import(set_dir, image_ids)
 
+        # TODO: add unlabeled set
+        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+
         return ds
 
     @classmethod
     def from_huggingface(
         cls,
         name: str,
         task: str,
@@ -742,14 +744,17 @@
                 start_num += set.num_rows
                 io.save_json(image_ids, ds.set_dir / f"{set_type}.json", True)
                 _import(set, task, image_ids)
         else:
             image_ids = list(range(1, dataset.num_rows + 1))
             _import(dataset, task, image_ids)
 
+        # TODO: add unlabeled set
+        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+
         return ds
 
     def initialize(self):
         """Initialize Dataset.
         It creates necessary directories under {dataset_root_dir}/{dataset_name}.
         """
         io.make_directory(self.raw_image_dir)
@@ -901,23 +906,25 @@
 
     # functions
     def split(
         self,
         train_ratio: float,
         val_ratio: float = 0.0,
         test_ratio: float = 0.0,
+        method: Union[str, SplitMethod] = SplitMethod.RANDOM,
         seed: int = 0,
     ):
         """
         Split Dataset to train, validation, test, (unlabeled) sets.
 
         Args:
             train_ratio (float): train num ratio (0 ~ 1).
             val_ratio (float, optional): val num ratio (0 ~ 1).
             test_ratio (float, optional): test num ratio (0 ~ 1).
+            method (Union[str, SplitMethod], optional): split method. Defaults to SplitMethod.RANDOM.
             seed (int, optional): random seed. Defaults to 0.
 
         Raises:
             ValueError: if train_ratio is not between 0.0 and 1.0.
             ValueError: if train_ratio + val_ratio + test_ratio is not 1.0.
 
         Examples:
@@ -938,32 +945,102 @@
         if train_ratio + val_ratio + test_ratio != 1.0:
             raise ValueError(
                 "train_ratio + val_ratio + test_ratio must be 1.0\n"
                 f"given train_ratio: {train_ratio}, val_ratio: {val_ratio}, test_ratio: {test_ratio}"
             )
 
         image_ids = list(self.images.keys())
-        random.seed(seed)
-        random.shuffle(image_ids)
-
         image_num = len(image_ids)
         if image_num <= 2:
             raise ValueError("image_num must be greater than 2\n" f"given image_num: {image_num}")
 
-        train_num = int(image_num * train_ratio)
-        val_num = int(image_num * val_ratio)
+        if method == SplitMethod.RANDOM:
+            train_num = max(int(image_num * train_ratio), 1)
+            val_num = max(int(image_num * val_ratio), 1)
+
+            random.seed(seed)
+            random.shuffle(image_ids)
+
+            if test_ratio == 0.0:
+                train_ids = image_ids[:train_num]
+                val_ids = image_ids[train_num:]
+                test_ids = val_ids
+            else:
+                train_ids = image_ids[:train_num]
+                val_ids = image_ids[train_num : train_num + val_num]
+                test_ids = image_ids[train_num + val_num :]
+
+        elif method == SplitMethod.STRATIFIED:
+            # """
+            # Given a dataset of image annotations, find the set of categories associated with each image and stratify them by categories.
+            # For example, if the dataset has annotations with the following image and category IDs:
+
+            # datasets: [
+            #     {"annotation_id": 1, "image_id": 1, "category_id": 1},
+            #     {"annotation_id": 2, "image_id": 1, "category_id": 2},
+            #     {"annotation_id": 3, "image_id": 2, "category_id": 1},
+            #     {"annotation_id": 4, "image_id": 2, "category_id": 2},
+            #     {"annotation_id": 5, "image_id": 3, "category_id": 1},
+            #     {"annotation_id": 6, "image_id": 4, "category_id": 1},
+            #     {"annotation_id": 7, "image_id": 5, "category_id": 2},
+            #     {"annotation_id": 8, "image_id": 6, "category_id": 2},
+            # ],
+
+            # the output should be stratified by categories:
+
+            # Categories 1 and 2 are associated with images 1, 2, 3, and 4.
+            # Category 1 is associated with images 3 and 4.
+            # Category 2 is associated with images 5 and 6.
+            # If the train_ratio : val_ratio is 0.5 : 0.5, a valid output would be:
+
+            # The training set consists of images 1, 3, and 5.
+            # The test set consists of images 2, 4, and 6.
+            # """
+
+            # train_ids = []
+            # val_ids = []
+            # test_ids = []
+
+            # # find set of categories
+            # num_category = len(self.categories)
+            # category_combinations = []
+            # for comb in [combinations(self.categories, num) for num in range(1, num_category + 1)]:
+            #     category_combinations.extend(comb)
+
+            # # for round error handling
+            # train_round_method = floor
+            # val_round_method = ceil
+
+            # # split by categories
+            # for comb in category_combinations:
+            #     image_ids_by_categories = list(
+            #         filter(
+            #             lambda image_id: set(comb)
+            #             == {ann.category_id for ann in self.image_to_annotations[image_id]},
+            #             image_ids,
+            #         )
+            #     )
+
+            #     num_images = len(image_ids_by_categories)
+            #     train_num = train_round_method(num_images * train_ratio)
+            #     val_num = val_round_method(num_images * val_ratio)
+            #     train_round_method, val_round_method = val_round_method, train_round_method
+
+            #     if test_ratio == 0.0:
+            #         train_ids += image_ids_by_categories[:train_num]
+            #         val_ids += image_ids_by_categories[train_num:]
+            #         test_ids += image_ids_by_categories[train_num:]
+            #     else:
+            #         train_ids += image_ids_by_categories[:train_num]
+            #         val_ids += image_ids_by_categories[train_num : train_num + val_num]
+            #         test_ids += image_ids_by_categories[train_num + val_num :]
+            raise NotImplementedError("(TODO) This feature will be updated soon.")
 
-        if test_ratio == 0.0:
-            train_ids = image_ids[:train_num]
-            val_ids = image_ids[train_num:]
-            test_ids = val_ids
         else:
-            train_ids = image_ids[:train_num]
-            val_ids = image_ids[train_num : train_num + val_num]
-            test_ids = image_ids[train_num + val_num :]
+            raise ValueError(f"Unknown split method: {method}")
 
         logger.info(
             f"train num: {len(train_ids)}  val num: {len(val_ids)}  test num: {len(test_ids)}"
         )
 
         io.save_json(
             train_ids,
@@ -1051,14 +1128,15 @@
                 warnings.warn(f"{export_dir} already exists. Removing exist export and override.")
 
             export_dir = export_function(self, export_dir)
 
             return export_dir
 
         except Exception as e:
-            io.remove_directory(export_dir)
+            if export_dir.exists():
+                io.remove_directory(export_dir)
             raise e
 
     def delete(self):
         """Delete Dataset"""
         io.remove_directory(self.dataset_dir)
         del self
```

### Comparing `waffle_hub-0.2.0/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.1/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.1/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py` & `waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,23 +25,27 @@
     TrainerCallback,
     TrainingArguments,
 )
 from transformers.utils import ModelOutput
 from waffle_utils.file import io
 
 from datasets import load_from_disk
+
+from waffle_hub import TaskType
 from waffle_hub.hub.adapter.hugging_face.train_input_helper import (
     ClassifierInputHelper,
     ObjectDetectionInputHelper,
 )
 from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
+from .config import DEFAULT_PARAMAS, MODEL_TYPES
+
 
 class CustomCallback(TrainerCallback):
     """
     This class is necessary to obtain logs for the training.
     """
 
     def __init__(self, trainer) -> None:
@@ -61,51 +65,16 @@
 class HuggingFaceHub(BaseHub):
 
     # Override
     LAST_CKPT_FILE = "weights/last_ckpt"
     BEST_CKPT_FILE = "weights/best_ckpt"
 
     # Common
-    MODEL_TYPES = {
-        "object_detection": {
-            "DETA": {
-                "base": "jozhang97/deta-resnet-50",
-            },
-            "DETR": {
-                "base": "facebook/detr-resnet-50",
-                "large": "facebook/detr-resnet-101",
-            },
-            "YOLOS": {
-                "tiny": "hustvl/yolos-tiny",
-            },
-        },
-        "classification": {
-            "ViT": {
-                "tiny": "WinKawaks/vit-tiny-patch16-224",
-                "base": "google/vit-base-patch16-224",
-            }
-        },
-    }
-
-    DEFAULT_PARAMAS = {
-        "object_detection": {
-            "epochs": 50,
-            "image_size": [800, 800],
-            "learning_rate": 5e-05,
-            "letter_box": True,  # TODO: implement letter_box
-            "batch_size": 16,
-        },
-        "classification": {
-            "epochs": 50,
-            "image_size": [224, 224],
-            "learning_rate": 5e-05,
-            "letter_box": False,
-            "batch_size": 16,
-        },
-    }
+    MODEL_TYPES = MODEL_TYPES
+    DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     def __init__(
         self,
         name: str,
         task: str,
         model_type: str,
         model_size: str,
@@ -213,18 +182,22 @@
             output_dir=str(self.artifact_dir),
             per_device_train_batch_size=cfg.batch_size,
             num_train_epochs=cfg.epochs,
             remove_unused_columns=False,
             push_to_hub=False,
             logging_strategy="epoch" if cfg.verbose else "no",
             evaluation_strategy="epoch",
+            save_strategy="epoch",
             learning_rate=cfg.learning_rate,
             dataloader_num_workers=cfg.workers,
             seed=cfg.seed,
-            greater_is_better=True,
+            metric_for_best_model="eval_loss",
+            greater_is_better=False,
+            save_total_limit=1,
+            load_best_model_at_end=False,
         )
 
     def training(self, cfg: TrainConfig, callback: TrainCallback):
 
         trainer = Trainer(
             model=cfg.train_input.model,
             args=cfg.train_input.training_args,
@@ -232,15 +205,18 @@
             train_dataset=cfg.train_input.dataset["train"],
             eval_dataset=cfg.train_input.dataset["val"],
             tokenizer=cfg.train_input.image_processor,
             compute_metrics=cfg.train_input.compute_metrics,
         )
         trainer.add_callback(CustomCallback(trainer))
         trainer.train()
-        trainer.save_model(str(self.artifact_dir / "weights"))
+        trainer.save_model(str(self.artifact_dir / "weights" / "last_ckpt"))
+        trainer._load_best_model()
+        trainer.save_model(str(self.artifact_dir / "weights" / "best_ckpt"))
+
         self.train_log = trainer.state.log_history
 
     def get_metrics(self) -> list[list[dict]]:
         metrics = []
 
         for epoch in range(0, len(self.train_log) - 1, 3):  # last is runtime info
 
@@ -254,73 +230,78 @@
                 epoch_metrics.append({"tag": key, "value": value})
             metrics.append(epoch_metrics)
 
         return metrics
 
     def on_train_end(self, cfg: TrainConfig):
         io.copy_files_to_directory(
-            self.artifact_dir / "weights",
+            self.artifact_dir / "weights" / "best_ckpt",
             self.best_ckpt_file,
             create_directory=True,
         )
+        io.copy_files_to_directory(
+            self.artifact_dir / "weights" / "last_ckpt",
+            self.last_ckpt_file,
+            create_directory=True,
+        )
         io.save_json(self.get_metrics(), self.metric_file)
 
-    def get_preprocess(self, task, pretrained_model: str = None) -> Callable:
+    def get_preprocess(self, pretrained_model: str = None) -> Callable:
         if pretrained_model is None:
             pretrained_model = self.best_ckpt_file
         image_processer = AutoImageProcessor.from_pretrained(pretrained_model)
 
         normalize = T.Normalize(image_processer.image_mean, image_processer.image_std, inplace=True)
 
         def preprocess(x, *args, **kwargs):
             return normalize(x)
 
         return preprocess
 
-    def get_postprocess(self, task: str, pretrained_model: str = None) -> Callable:
+    def get_postprocess(self: str, pretrained_model: str = None) -> Callable:
         if pretrained_model is None:
             pretrained_model = self.best_ckpt_file
         image_processer = AutoImageProcessor.from_pretrained(pretrained_model)
 
-        if task == "classification":
+        if self.task == TaskType.CLASSIFICATION:
 
             def inner(x: ModelOutput, *args, **kwargs) -> torch.Tensor:
                 return [x.logits]
 
-        elif task == "object_detection":
+        elif self.task == TaskType.OBJECT_DETECTION:
             post_process = image_processer.post_process_object_detection
 
             def inner(x: ModelOutput, *args, **kwargs) -> torch.Tensor:
 
                 x = post_process(x, threshold=-1)
 
                 xyxy = list(map(lambda x: x["boxes"], x))
                 confidences = list(map(lambda x: x["scores"], x))
                 category_ids = list(map(lambda x: x["labels"], x))
 
                 return xyxy, confidences, category_ids
 
         else:
-            raise NotImplementedError(f"Task {task} is not implemented.")
+            raise NotImplementedError(f"Task {self.task} is not implemented.")
 
         return inner
 
     def get_model(self) -> ModelWrapper:
         self.check_train_sanity()
 
         # get adapt functions
-        preprocess = self.get_preprocess(self.task)
-        postprocess = self.get_postprocess(self.task)
+        preprocess = self.get_preprocess()
+        postprocess = self.get_postprocess()
 
         # get model
-        if self.task == "object_detection":
+        if self.task == TaskType.OBJECT_DETECTION:
             model = AutoModelForObjectDetection.from_pretrained(
                 str(self.best_ckpt_file),
             )
-        elif self.task == "classification":
+        elif self.task == TaskType.CLASSIFICATION:
             model = AutoModelForImageClassification.from_pretrained(
                 str(self.best_ckpt_file),
             )
 
         model = ModelWrapper(
             model=model.eval(),
             preprocess=preprocess,
```

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/train_input_helper.py` & `waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/train_input_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,15 +128,17 @@
             )
         )
         if tuple(size) != tuple(self.image_size):
             raise ValueError(
                 f"pretrained model's image size is {size}, but you set {self.image_size}."
             )
 
-        _transforms = T.Compose([T.RandomResizedCrop(size[::-1]), T.ToTensor(), normalize])
+        _transforms = T.Compose(
+            [T.RandomResizedCrop(self.image_size[::-1]), T.ToTensor(), normalize]
+        )
 
         def transforms(examples: dict) -> dict:
             examples["pixel_values"] = [_transforms(img.convert("RGB")) for img in examples["image"]]
             del examples["image"]
             return examples
 
         return transforms
@@ -156,29 +158,40 @@
 
 
 class ObjectDetectionInputHelper(TrainInputHelper):
     def __init__(self, pretrained_model: str, image_size: Union[int, list[int]]) -> None:
         super().__init__(pretrained_model, image_size)
 
     def get_transforms(self) -> Callable:
-        size = (
-            (self.image_processor.size["shortest_edge"],) * 2
-            if "shortest_edge" in self.image_processor.size
-            else (
-                self.image_processor.size["width"],
-                self.image_processor.size["height"],
-            )
-        )
-
-        if tuple(size) != tuple(self.image_size):
-            warnings.warn(f"pretrained model's image size is {size}, but you set {self.image_size}.")
+        if "shortest_edge" in self.image_processor.size:
+            shortest_size = self.image_processor.size["shortest_edge"]
+            longest_size = self.image_processor.size["longest_edge"]
+            if min(self.image_size) < shortest_size:
+                warnings.warn(
+                    f"pretrained model's shortest edge is {shortest_size}, but you set {self.image_size}."
+                )
+                self.image_processor.size["shortest_edge"] = min(self.image_size)
+            if max(self.image_size) > longest_size:
+                warnings.warn(
+                    f"pretrained model's longest edge is {longest_size}, but you set {self.image_size}."
+                )
+                self.image_processor.size["longest_edge"] = max(self.image_size)
+        else:
+            size = (self.image_processor.size["width"], self.image_processor.size["height"])
+
+            if tuple(size) != tuple(self.image_size):
+                warnings.warn(
+                    f"pretrained model's image size is {size}, but you set {self.image_size}."
+                )
+                self.image_processor.size["width"] = self.image_size[0]
+                self.image_processor.size["height"] = self.image_size[1]
 
         _transforms = albumentations.Compose(
             [
-                albumentations.Resize(width=size[0], height=size[1]),
+                albumentations.Resize(width=self.image_size[0], height=self.image_size[1]),
                 albumentations.HorizontalFlip(p=0.5),
                 albumentations.RandomBrightnessContrast(p=0.5),
             ],
             bbox_params=albumentations.BboxParams(format="coco", label_fields=["category"]),
         )
 
         def formatted_anns(image_id: int, category: list, area: list, bbox: list) -> list[dict]:
```

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py` & `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/tx_model_hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,71 +16,32 @@
 import torch
 from attrdict import AttrDict
 from autocare_tx_model.core.model import build_model
 from autocare_tx_model.tools import train
 from torchvision import transforms as T
 from waffle_utils.file import io
 
+from waffle_hub import TaskType
 from waffle_hub.hub.adapter.tx_model.configs import (
     get_data_config,
     get_model_config,
 )
 from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
+from .config import DATA_TYPE_MAP, DEFAULT_PARAMAS, MODEL_TYPES, WEIGHT_PATH
 
-class TxModelHub(BaseHub):
 
-    # Common
-    MODEL_TYPES = {
-        "object_detection": {"YOLOv5": list("sml")},
-        "classification": {"Classifier": list("sml")},
-    }
-
-    # Backend Specifics
-    DATA_TYPE_MAP = {
-        "object_detection": "COCODetectionDataset",
-        "classification": "COCOClassificationDataset",
-    }
-
-    WEIGHT_PATH = {
-        "object_detection": {
-            "YOLOv5": {
-                "s": "temp/autocare_tx_model/detectors/small/model.pth",
-                "m": "temp/autocare_tx_model/detectors/medium/model.pth",
-                "l": "temp/autocare_tx_model/detectors/large/model.pth",
-            }
-        },
-        "classification": {
-            "Classifier": {
-                "s": "temp/autocare_tx_model/classifiers/small/model.pth",
-                "m": "temp/autocare_tx_model/classifiers/medium/model.pth",
-                "l": "temp/autocare_tx_model/classifiers/large/model.pth",
-            }
-        },
-    }
-
-    DEFAULT_PARAMAS = {
-        "object_detection": {
-            "epochs": 50,
-            "image_size": [640, 640],
-            "learning_rate": 0.01,
-            "letter_box": True,
-            "batch_size": 16,
-        },
-        "classification": {
-            "epochs": 50,
-            "image_size": [224, 224],
-            "learning_rate": 0.01,
-            "letter_box": False,
-            "batch_size": 16,
-        },
-    }
+class TxModelHub(BaseHub):
+    MODEL_TYPES = MODEL_TYPES
+    DATA_TYPE_MAP = DATA_TYPE_MAP
+    WEIGHT_PATH = WEIGHT_PATH
+    DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
@@ -137,42 +98,42 @@
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
     # Hub Utils
-    def get_preprocess(self, task: str, *args, **kwargs):
+    def get_preprocess(self, *args, **kwargs):
 
-        if task == "object_detection":
+        if self.task == TaskType.OBJECT_DETECTION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
-        elif task == "classification":
+        elif self.task == TaskType.CLASSIFICATION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
         return preprocess
 
-    def get_postprocess(self, task: str, *args, **kwargs):
+    def get_postprocess(self, *args, **kwargs):
 
-        if task == "object_detection":
+        if self.task == TaskType.OBJECT_DETECTION:
 
             def inner(x: torch.Tensor, *args, **kwargs):
                 xyxy = x[0]
                 scores = x[1]
                 class_ids = x[2]
 
                 return xyxy, scores, class_ids
 
-        elif task == "classification":
+        elif self.task == TaskType.CLASSIFICATION:
 
             def inner(x: torch.Tensor, *args, **kwargs):
                 x = [t.squeeze() for t in x]
                 return x
 
         return inner
 
@@ -281,16 +242,16 @@
         """Get model.
         Returns:
             ModelWrapper: Model wrapper
         """
         self.check_train_sanity()
 
         # get adapt functions
-        preprocess = self.get_preprocess(self.task)
-        postprocess = self.get_postprocess(self.task)
+        preprocess = self.get_preprocess()
+        postprocess = self.get_postprocess()
 
         # get model
         categories = [x["name"] for x in self.categories]
         cfg = io.load_json(self.artifact_dir / "model.json")
         cfg["ckpt"] = str(self.best_ckpt_file)
         cfg["model"]["head"]["num_classes"] = len(categories)
         cfg["num_classes"] = len(categories)
```

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,66 +13,28 @@
 from typing import Union
 
 import torch
 from torchvision import transforms as T
 from ultralytics import YOLO
 from waffle_utils.file import io
 
+from waffle_hub import TaskType
 from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
+from .config import DEFAULT_PARAMAS, MODEL_TYPES, TASK_MAP, TASK_SUFFIX
 
-class UltralyticsHub(BaseHub):
 
-    # Common
-    MODEL_TYPES = {
-        "object_detection": {"yolov8": list("nsmlx")},
-        "classification": {"yolov8": list("nsmlx")},
-        "instance_segmentation": {"yolov8": list("nsmlx")},
-        # "keypoint_detection": {"yolov8": list("nsmlx")},
-    }
-
-    # Backend Specifics
-    TASK_MAP = {
-        "object_detection": "detect",
-        "classification": "classify",
-        "instance_segmentation": "segment"
-        # "keypoint_detection": "pose"
-    }
-    TASK_SUFFIX = {
-        "detect": "",
-        "classify": "-cls",
-        "segment": "-seg",
-    }
-
-    DEFAULT_PARAMAS = {
-        "object_detection": {
-            "epochs": 50,
-            "image_size": [640, 640],
-            "learning_rate": 0.01,
-            "letter_box": True,
-            "batch_size": 16,
-        },
-        "classification": {
-            "epochs": 50,
-            "image_size": [224, 224],
-            "learning_rate": 0.01,
-            "letter_box": False,
-            "batch_size": 16,
-        },
-        "instance_segmentation": {
-            "epochs": 50,
-            "image_size": [640, 640],
-            "learning_rate": 0.01,
-            "letter_box": True,
-            "batch_size": 16,
-        },
-    }
+class UltralyticsHub(BaseHub):
+    MODEL_TYPES = MODEL_TYPES
+    TASK_MAP = TASK_MAP
+    TASK_SUFFIX = TASK_SUFFIX
+    DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
@@ -131,49 +93,49 @@
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
     # Hub Utils
-    def get_preprocess(self, task: str, *args, **kwargs):
+    def get_preprocess(self, *args, **kwargs):
 
-        if task == "classification":
+        if self.task == TaskType.CLASSIFICATION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
-        elif task == "object_detection":
+        elif self.task == TaskType.OBJECT_DETECTION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
-        elif task == "instance_segmentation":
+        elif self.task == TaskType.INSTANCE_SEGMENTATION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
         else:
-            raise NotImplementedError(f"Task {task} is not implemented.")
+            raise NotImplementedError(f"Task {self.task} is not implemented.")
 
         return preprocess
 
-    def get_postprocess(self, task: str, *args, **kwargs):
+    def get_postprocess(self, *args, **kwargs):
 
         id_mapper: list[int] = kwargs.get("id_mapper", [i for i in range(len(self.categories))])
 
-        if task == "classification":
+        if self.task == TaskType.CLASSIFICATION:
 
             def inner(x: torch.Tensor, *args, **kwargs):
                 return [x[:, id_mapper]]
 
-        elif task == "object_detection":
+        elif self.task == TaskType.OBJECT_DETECTION:
 
             def inner(x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs):
                 x = x[0]  # x[0]: prediction, x[1]: TODO: what is this...?
                 x = x.transpose(1, 2)
 
                 cxcywh = x[:, :, :4]
                 cx, cy, w, h = torch.unbind(cxcywh, dim=-1)
@@ -186,15 +148,15 @@
                 xyxy[:, :, ::2] /= image_size[0]
                 xyxy[:, :, 1::2] /= image_size[1]
                 probs = x[:, :, 4:][:, :, id_mapper]
                 confidences, class_ids = torch.max(probs, dim=-1)
 
                 return xyxy, confidences, class_ids
 
-        elif task == "instance_segmentation":
+        elif self.task == TaskType.INSTANCE_SEGMENTATION:
             num_category = len(self.categories)
 
             def inner(x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs):
                 preds = x[0]  # x[0]: prediction, x[1]: TODO: what is this...?
                 preds = preds.transpose(1, 2)
 
                 probs = preds[:, :, 4 : 4 + num_category]
@@ -227,15 +189,15 @@
 
                 masks = preds[:, :, 4 + num_category :]
                 masks = torch.bmm(masks, protos).sigmoid().view(masks.shape[0], -1, *mask_size)
 
                 return xyxy, confidences, class_ids, masks
 
         else:
-            raise NotImplementedError(f"Task {task} is not implemented.")
+            raise NotImplementedError(f"Task {self.task} is not implemented.")
 
         return inner
 
     def get_metrics(self) -> list[list[dict]]:
         # read csv file
         # epoch,         train/box_loss,         train/cls_loss,         train/dfl_loss,   metrics/precision(B),      metrics/recall(B),       metrics/mAP50(B),    metrics/mAP50-95(B),           val/box_loss,           val/cls_loss,           val/dfl_loss,                 lr/pg0,                 lr/pg1,                 lr/pg2
         #              0,                 2.0349,                 4.4739,                  1.214,                0.75962,                0.34442,                0.22858,                0.18438,                0.61141,                 2.8409,                0.78766,                 0.0919,                 0.0009,                 0.0009
@@ -352,18 +314,18 @@
 
         id_mapper: list[int] = [i for i in range(len(yolo_names))]
 
         yolo_names_inv = {v: k for k, v in yolo_names.items()}
         for i, name in enumerate(names):
             id_mapper[i] = yolo_names_inv[name]
 
-        preprocess = self.get_preprocess(self.task)
-        postprocess = self.get_postprocess(self.task, id_mapper=id_mapper)
+        preprocess = self.get_preprocess()
+        postprocess = self.get_postprocess(id_mapper=id_mapper)
 
         # wrap model
         model = ModelWrapper(
             model=model,
             preprocess=preprocess,
             postprocess=postprocess,
         )
 
-        return model
+        return model
```

### Comparing `waffle_hub-0.2.0/waffle_hub/hub/base_hub.py` & `waffle_hub-0.2.1/waffle_hub/hub/base_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from pathlib import Path
 from typing import Union
 
 import cpuinfo
 import cv2
 import torch
 import tqdm
+import numpy as np
+
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.hub.model.wrapper import get_parser
 from waffle_hub.schema.configs import (
@@ -34,21 +36,22 @@
 )
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
+from waffle_hub.schema.data import ImageInfo
 from waffle_hub.utils.callback import (
     EvaluateCallback,
     ExportCallback,
     InferenceCallback,
     TrainCallback,
 )
-from waffle_hub.utils.data import ImageDataset, LabeledDataset
+from waffle_hub.utils.data import ImageDataset, LabeledDataset, get_image_transform
 from waffle_hub.utils.draw import draw_results
 from waffle_hub.utils.evaluate import evaluate_function
 
 logger = logging.getLogger(__name__)
 
 
 class BaseHub:
@@ -260,14 +263,23 @@
     @categories.setter
     @type_validator(list)
     def categories(self, v):
         if isinstance(v[0], str):
             v = [{"supercategory": "object", "name": n} for n in v]
         self.__categories = v
 
+    @property
+    def default_params(self):
+        """Get default values from model.
+
+        Returns:
+            dict: default values
+        """
+        return self.DEFAULT_PARAMAS[self.task][self.model_type][self.model_size]
+
     @cached_property
     def hub_dir(self) -> Path:
         """Hub(Model) Directory"""
         return self.root_dir / self.name
 
     @cached_property
     def model_config_file(self) -> Path:
@@ -424,14 +436,42 @@
 
         Returns:
             list[dict]: inference result
         """
         if not self.inference_file.exists():
             return []
         return io.load_json(self.inference_file)
+    
+    # Hub Utils
+    def get_image_loader(self) -> tuple[torch.Tensor, ImageInfo]:
+        """Get image loader function.
+
+        Returns:
+            tuple[torch.Tensor, ImageInfo]: input transform function
+        
+        Example:
+            >>> transform = hub.get_image_loader()
+            >>> image, image_info = transform("path/to/image.jpg")
+            >>> model = hub.get_model()
+            >>> output = model(image.unsqueeze(0))
+        """
+        train_config: TrainConfig = self.get_train_config()
+        transform = get_image_transform(train_config.image_size, train_config.letter_box)
+        def inner(x: Union[np.ndarray, str]):
+            """Input Transform Function
+            
+            Args:
+                x (Union[np.ndarray, str]): opencv image or image path
+                
+            Returns:
+                tuple[torch.Tensor, ImageInfo]: image and image info
+            """
+            image, image_info = transform(x)
+            return image, image_info
+        return inner
 
     # Train Hook
     def before_train(self, cfg: TrainConfig):
         pass
 
     def on_train_start(self, cfg: TrainConfig):
         pass
@@ -542,16 +582,19 @@
             workers=workers,
             seed=seed,
             verbose=verbose,
         )
 
         # overwrite train config with default config
         for k, v in cfg.to_dict().items():
-            if v is None and k in self.DEFAULT_PARAMAS[self.task]:
-                setattr(cfg, k, self.DEFAULT_PARAMAS[self.task][k])
+            if v is None:
+                field_value = getattr(
+                    self.DEFAULT_PARAMAS[self.task][self.model_type][self.model_size], k
+                )
+                setattr(cfg, k, field_value)
 
         callback = TrainCallback(cfg.epochs + 1, self.get_metrics)
         result = TrainResult()
         result.callback = callback
 
         if hold:
             inner(callback, result)
```

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.1/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/configs.py` & `waffle_hub-0.2.1/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/data.py` & `waffle_hub-0.2.1/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.1/waffle_hub/schema/fields/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,24 @@
     def segmentation(self, v):
         if isinstance(v, dict):
             v: list = convert_rle_to_polygon(v)
         if v:
             for segment in v:
                 if len(segment) % 2 != 0:
                     raise ValueError("the length of segmentation should be divisible by 2.")
+
+            if self.bbox is None:
+                xs = [x for segment in v for x in segment[::2]]
+                ys = [y for segment in v for y in segment[1::2]]
+                x1 = min(xs)
+                y1 = min(ys)
+                w = max(xs) - x1
+                h = max(ys) - y1
+                self.bbox = [x1, y1, w, h]
+
         self.__segmentation = v
 
     @property
     def area(self):
         return self.__area
 
     @area.setter
```

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.1/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.1/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.1/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/utils/callback.py` & `waffle_hub-0.2.1/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.1/waffle_hub/utils/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def convert_rle_to_polygon(rle: dict) -> list:
     mask = convert_rle_to_mask(rle)
     return convert_mask_to_polygon(mask)
 
 
-def convert_mask_to_polygon(mask: np.ndarray) -> list:
+def convert_mask_to_polygon(mask: np.ndarray) -> list[list]:
     contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     polygon = []
 
     for contour in contours:
         # contour = np.flip(contour, axis=1)
         # polygon.append(contour.ravel().tolist())
```

### Comparing `waffle_hub-0.2.0/waffle_hub/utils/data.py` & `waffle_hub-0.2.1/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/utils/draw.py` & `waffle_hub-0.2.1/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.1/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.0/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.1/waffle_hub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.0
+Version: 0.2.1
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.0 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.1 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.0/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.1/waffle_hub.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+tests/test_cli.py
 tests/test_dataset.py
 tests/test_hub.py
 waffle_hub/__init__.py
 waffle_hub/run.py
 waffle_hub.egg-info/PKG-INFO
 waffle_hub.egg-info/SOURCES.txt
 waffle_hub.egg-info/dependency_links.txt
@@ -23,22 +24,25 @@
 waffle_hub/experimental/serve.py
 waffle_hub/experimental/auto_label/__init__.py
 waffle_hub/experimental/auto_label/grounding_dino.py
 waffle_hub/hub/__init__.py
 waffle_hub/hub/base_hub.py
 waffle_hub/hub/adapter/__init__.py
 waffle_hub/hub/adapter/hugging_face/__init__.py
+waffle_hub/hub/adapter/hugging_face/config.py
 waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
 waffle_hub/hub/adapter/hugging_face/train_input_helper.py
 waffle_hub/hub/adapter/tx_model/__init__.py
+waffle_hub/hub/adapter/tx_model/config.py
 waffle_hub/hub/adapter/tx_model/tx_model_hub.py
 waffle_hub/hub/adapter/tx_model/configs/__init__.py
 waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
 waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
 waffle_hub/hub/adapter/ultralytics/__init__.py
+waffle_hub/hub/adapter/ultralytics/config.py
 waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
 waffle_hub/hub/model/__init__.py
 waffle_hub/hub/model/wrapper.py
 waffle_hub/schema/__init__.py
 waffle_hub/schema/base_schema.py
 waffle_hub/schema/configs.py
 waffle_hub/schema/data.py
```

