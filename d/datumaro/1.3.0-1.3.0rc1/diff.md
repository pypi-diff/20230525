# Comparing `tmp/datumaro-1.3.0.tar.gz` & `tmp/datumaro-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.3.0.tar", last modified: Thu May 25 07:09:31 2023, max compression
+gzip compressed data, was "datumaro-1.3.0rc1.tar", last modified: Mon May 22 06:25:28 2023, max compression
```

## Comparing `datumaro-1.3.0.tar` & `datumaro-1.3.0rc1.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.639011 datumaro-1.3.0/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)   375078 2023-05-25 07:07:57.000000 datumaro-1.3.0/3rd-party.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1090 2023-04-07 03:36:55.000000 datumaro-1.3.0/LICENSE
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      103 2023-04-07 03:36:55.000000 datumaro-1.3.0/MANIFEST.in
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      229 2023-04-07 03:36:55.000000 datumaro-1.3.0/NOTICE
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6116 2023-05-25 07:09:31.639011 datumaro-1.3.0/PKG-INFO
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5571 2023-05-25 07:07:57.000000 datumaro-1.3.0/README.md
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1715 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      178 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/__main__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/capi/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3379 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5686 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/__main__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/commands/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1317 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5187 2023-05-11 12:48:39.000000 datumaro-1.3.0/datumaro/cli/commands/convert.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3991 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9154 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/diff.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10146 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/download.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9340 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/explain.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5362 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/cli/commands/explore.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9046 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/filter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3073 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/generate.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4238 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/info.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10275 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/cli/commands/merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5979 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/patch.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/commands/require_project/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      985 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      124 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5227 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1957 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5906 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5892 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1677 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      123 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2946 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2150 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2758 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1132 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1412 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3116 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/stats.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8363 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/transform.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4837 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/contexts/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      121 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9089 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/contexts/project/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4501 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2553 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/contexts/source.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4097 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro/cli/util/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4007 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/cli/util/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    13328 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/util/diff.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      391 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/cli/util/errors.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5640 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/cli/util/project.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/abstracts/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       95 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1077 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/abstracts/merger.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/algorithms/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      135 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      111 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8837 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8073 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/algorithms/rise.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    29940 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/components/annotation.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/annotations/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      118 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/annotations/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8965 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/annotations/matcher.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5242 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/annotations/merger.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2146 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/cli_plugin.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8101 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/config.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3570 2023-05-12 05:40:06.000000 datumaro-1.3.0/datumaro/components/config_model.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2240 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/crypter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    48306 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/components/dataset.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10965 2023-04-19 06:22:49.000000 datumaro-1.3.0/datumaro/components/dataset_base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6034 2023-04-19 06:22:49.000000 datumaro-1.3.0/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10510 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/components/environment.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    18012 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/components/errors.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6306 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/components/explorer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    14287 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/components/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    19651 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/extractor_tfds.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10063 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/filter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    19989 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/components/format_detection.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      534 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/generator.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/hl_ops/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8684 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8679 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/components/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2901 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/launcher.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    36004 2023-05-04 01:31:37.000000 datumaro-1.3.0/datumaro/components/media.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2450 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/media_manager.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/components/merge/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3694 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/merge/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4103 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/merge/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12216 2023-04-19 06:22:49.000000 datumaro-1.3.0/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    24147 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4453 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/merge/union_merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    23487 2023-04-19 06:22:49.000000 datumaro-1.3.0/datumaro/components/operations.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5221 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/components/progress_reporting.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    89679 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/components/project.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9352 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/shift_analyzer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1830 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/components/transformer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2198 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/components/validator.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    22776 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/components/visualizer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      164 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/errors.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      172 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/ops.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/plugins/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1148 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.627010 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4038 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2217 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6576 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8600 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      232 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5963 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2636 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15043 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1514 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2129 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      232 2023-04-19 06:22:49.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2607 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10224 2023-05-11 12:48:39.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1625 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8758 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5585 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3626 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3875 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    17692 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      183 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7823 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10759 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12453 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    21517 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    20916 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    28664 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      552 2023-04-27 03:40:22.000000 datumaro-1.3.0/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7192 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6517 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3317 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    14327 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    20633 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      214 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       72 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11437 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15603 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      317 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1236 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      286 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6839 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11135 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      828 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1921 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      694 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11105 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2236 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1563 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5235 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12137 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6522 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      311 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1995 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4122 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7773 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8357 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5877 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.631010 datumaro-1.3.0/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6210 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11401 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3970 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3752 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11401 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    17893 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      711 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    20302 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15150 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11577 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12609 2023-04-27 03:40:22.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4274 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6508 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5109 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9234 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7220 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10932 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6660 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      556 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5407 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5151 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4262 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4819 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      563 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1873 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1814 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    38725 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      292 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6087 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6062 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1792 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7083 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    16304 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      420 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-05-11 12:48:39.000000 datumaro-1.3.0/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6671 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2943 2023-05-11 12:48:39.000000 datumaro-1.3.0/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1262 2023-05-11 12:48:39.000000 datumaro-1.3.0/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7790 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8885 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      308 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15663 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6453 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    16029 2023-05-18 12:50:18.000000 datumaro-1.3.0/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    31323 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10660 2023-05-18 12:50:18.000000 datumaro-1.3.0/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3217 2023-05-18 12:50:18.000000 datumaro-1.3.0/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3066 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4107 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10301 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12632 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12129 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      457 2023-05-02 23:15:41.000000 datumaro-1.3.0/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5573 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2879 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/explorer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    16787 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/ndr.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9757 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      411 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1133 2023-05-12 01:14:45.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1697 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1288 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2629 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2864 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2631 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2700 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2632 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/sampler/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       72 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7786 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8772 2023-04-19 06:22:49.000000 datumaro-1.3.0/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1213 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    32124 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/splitter.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/synthetic_data/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      155 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11335 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11577 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6194 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.635011 datumaro-1.3.0/datumaro/plugins/tiling/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      116 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9398 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9834 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1141 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/plugins/tiling/util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    48788 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/plugins/transforms.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    44207 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/plugins/validators.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      376 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/project.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.639011 datumaro-1.3.0/datumaro/util/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4809 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8553 2023-05-24 23:41:35.000000 datumaro-1.3.0/datumaro/util/annotation_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1198 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/attrs_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      262 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/definitions.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      882 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/util/file_utils.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11657 2023-04-27 05:10:33.000000 datumaro-1.3.0/datumaro/util/image.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      968 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/image_cache.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      795 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/log_utils.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11601 2023-05-11 12:48:39.000000 datumaro-1.3.0/datumaro/util/mask_tools.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3976 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/util/meta_file_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8479 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/os_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      758 2023-04-18 01:04:20.000000 datumaro-1.3.0/datumaro/util/pickle_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      246 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/samples.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4702 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/scope.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      616 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/telemetry_stub.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6073 2023-04-21 06:03:53.000000 datumaro-1.3.0/datumaro/util/telemetry_utils.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2579 2023-04-07 03:36:55.000000 datumaro-1.3.0/datumaro/util/tf_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       22 2023-05-25 07:07:57.000000 datumaro-1.3.0/datumaro/version.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-25 07:09:31.623010 datumaro-1.3.0/datumaro.egg-info/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6116 2023-05-25 07:09:31.000000 datumaro-1.3.0/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11871 2023-05-25 07:09:31.000000 datumaro-1.3.0/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        1 2023-05-25 07:09:31.000000 datumaro-1.3.0/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       53 2023-05-25 07:09:31.000000 datumaro-1.3.0/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      730 2023-05-25 07:09:31.000000 datumaro-1.3.0/datumaro.egg-info/requires.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        9 2023-05-25 07:09:31.000000 datumaro-1.3.0/datumaro.egg-info/top_level.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2488 2023-04-07 03:36:55.000000 datumaro-1.3.0/pyproject.toml
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      720 2023-05-11 12:48:39.000000 datumaro-1.3.0/requirements-core.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      266 2023-04-07 03:36:55.000000 datumaro-1.3.0/requirements-default.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       38 2023-05-25 07:09:31.639011 datumaro-1.3.0/setup.cfg
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3159 2023-05-11 12:48:39.000000 datumaro-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)   373252 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.332166 datumaro-1.3.0rc1/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.332166 datumaro-1.3.0rc1/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/abstracts/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48204 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89679 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38719 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47320 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44207 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/setup.py
```

### Comparing `datumaro-1.3.0/3rd-party.txt` & `datumaro-1.3.0rc1/3rd-party.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6936,46 +6936,9 @@
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 -------------------------------------------------------------
-Protocol Buffers
-
-BSD-3-Clause
-
-Copyright 2008 Google Inc.  All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
-
-    * Redistributions of source code must retain the above copyright
-notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above
-copyright notice, this list of conditions and the following disclaimer
-in the documentation and/or other materials provided with the
-distribution.
-    * Neither the name of Google Inc. nor the names of its
-contributors may be used to endorse or promote products derived from
-this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-Code generated by the Protocol Buffer compiler is owned by the owner
-of the input file used when generating it.  This code is not
-standalone and requires a support library to be linked with it.  This
-support library is itself covered by the above license.
--------------------------------------------------------------
 
 * Other names and brands may be claimed as the property of others.
```

### Comparing `datumaro-1.3.0/LICENSE` & `datumaro-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/PKG-INFO` & `datumaro-1.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,27 +34,27 @@
 ```
 <!--lint enable fenced-code-flag-->
 
 - [Getting started](https://openvinotoolkit.github.io/datumaro/latest/docs/get-started/quick-start-guide)
 - [Level Up](https://openvinotoolkit.github.io/datumaro/latest/docs/level-up/basic_skills)
 - [Features](#features)
 - [User manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
-- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro_module)
+- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro/datumaro)
 - [Contributing](#contributing)
 
 ## Features
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 - Dataset reading, writing, conversion in any direction.
   - [CIFAR-10/100](https://www.cs.toronto.edu/~kriz/cifar.html) (`classification`)
   - [Cityscapes](https://www.cityscapes-dataset.com/)
   - [COCO](http://cocodataset.org/#format-data) (`image_info`, `instances`, `person_keypoints`,
     `captions`, `labels`, `panoptic`, `stuff`)
-  - [CVAT](https://opencv.github.io/cvat/docs/manual/advanced/xml_format/)
+  - [CVAT](https://openvinotoolkit.github.io/cvat/docs/manual/advanced/xml_format)
   - [ImageNet](http://image-net.org/)
   - [Kitti](http://www.cvlibs.net/datasets/kitti/index.php) (`segmentation`, `detection`,
     `3D raw` / `velodyne points`)
   - [LabelMe](http://labelme.csail.mit.edu/Release3.0)
   - [LFW](http://vis-www.cs.umass.edu/lfw/) (`classification`, `person re-identification`,
     `landmarks`)
   - [MNIST](http://yann.lecun.com/exdb/mnist/) (`classification`)
```

### Comparing `datumaro-1.3.0/README.md` & `datumaro-1.3.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 ```
 <!--lint enable fenced-code-flag-->
 
 - [Getting started](https://openvinotoolkit.github.io/datumaro/latest/docs/get-started/quick-start-guide)
 - [Level Up](https://openvinotoolkit.github.io/datumaro/latest/docs/level-up/basic_skills)
 - [Features](#features)
 - [User manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
-- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro_module)
+- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro/datumaro)
 - [Contributing](#contributing)
 
 ## Features
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 - Dataset reading, writing, conversion in any direction.
   - [CIFAR-10/100](https://www.cs.toronto.edu/~kriz/cifar.html) (`classification`)
   - [Cityscapes](https://www.cityscapes-dataset.com/)
   - [COCO](http://cocodataset.org/#format-data) (`image_info`, `instances`, `person_keypoints`,
     `captions`, `labels`, `panoptic`, `stuff`)
-  - [CVAT](https://opencv.github.io/cvat/docs/manual/advanced/xml_format/)
+  - [CVAT](https://openvinotoolkit.github.io/cvat/docs/manual/advanced/xml_format)
   - [ImageNet](http://image-net.org/)
   - [Kitti](http://www.cvlibs.net/datasets/kitti/index.php) (`segmentation`, `detection`,
     `3D raw` / `velodyne points`)
   - [LabelMe](http://labelme.csail.mit.edu/Release3.0)
   - [LFW](http://vis-www.cs.umass.edu/lfw/) (`classification`, `person re-identification`,
     `landmarks`)
   - [MNIST](http://yann.lecun.com/exdb/mnist/) (`classification`)
```

### Comparing `datumaro-1.3.0/datumaro/__init__.py` & `datumaro-1.3.0rc1/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/capi/pybind.cpp` & `datumaro-1.3.0rc1/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/__main__.py` & `datumaro-1.3.0rc1/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/convert.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/detect_format.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/diff.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/download.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/explain.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/explore.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/explore.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     build_tree = project.working_tree.clone()
     for target in targets:
         build_tree.build_targets.add_explore_stage(target, params=explorer_args)
 
     explorer = Explorer(*source_datasets)
     for dataset in source_datasets:
         dst_dir = dataset.data_path
-        dataset.save(dst_dir, save_media=True, save_hashkey_meta=True)
+        dataset.save(dst_dir, save_media=True)
 
     if args.stage:
         project.working_tree.config.update(build_tree.config)
         project.working_tree.save()
 
     # Get query datasetitem through query path
     if osp.exists(args.query):
```

### Comparing `datumaro-1.3.0/datumaro/cli/commands/filter.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/generate.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/info.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/merge.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/patch.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/stats.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/transform.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/commands/validate.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/contexts/model.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/contexts/source.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/contexts/util.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/util/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/util/diff.py` & `datumaro-1.3.0rc1/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/cli/util/project.py` & `datumaro-1.3.0rc1/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/abstracts/merger.py` & `datumaro-1.3.0rc1/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Sequence, Tuple
+from typing import Dict, List, Sequence, Tuple
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from matplotlib.figure import Figure
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset_base import IDataset
@@ -40,53 +40,36 @@
     allowing comparison of the dataset's overall average or averages grouped by labels.
 
     .. [1] Zhou, Tianyi, Shengjie Wang, and Jeff Bilmes.
     "Robust curriculum learning: from clean label detection to noisy label self-correction."
     International Conference on Learning Representations. 2021.
     """
 
-    allowed_task_names = {"OTX-MultiClassCls", "OTX-Det"}
-    allowed_tracking_loss_types = {"cls", "bbox", "centerness", "bbox_refine"}
+    allowed_task_names = {"OTX-MultiClassCls"}
 
-    def __init__(
-        self, dataset: IDataset, alpha: float = 0.001, tracking_loss_type: Optional[str] = None
-    ) -> None:
+    def __init__(self, dataset: IDataset, alpha: float = 0.001) -> None:
         purpose = dataset.infos().get("purpose")
         if purpose != "noisy_label_detection":
             raise DatasetError(
                 f'Dataset infos should have purpose="noisy_label_detection", but it has {purpose}.'
             )
 
         task = dataset.infos().get("task")
-        if task not in self.allowed_task_names:
+        if task != "OTX-MultiClassCls":
             raise DatasetError(
-                f"task={task} is not allowed. The allowed task names are {self.allowed_task_names}."
-            )
-        elif task == "OTX-Det" and tracking_loss_type is None:
-            raise DatasetError(
-                'If task="OTX-Det", tracking_loss_type should not be None. '
-                f"The allowed tracking loss types are {self.allowed_tracking_loss_types}."
-            )
-        elif (
-            tracking_loss_type is not None
-            and tracking_loss_type not in self.allowed_tracking_loss_types
-        ):
-            raise DatasetError(
-                f"tracking_loss_type={tracking_loss_type} "
-                f"but the allowed tracking loss types are {self.allowed_tracking_loss_types}."
+                f"{task} is not allowed. The allowed task names are {self.allowed_task_names}."
             )
 
         self._dataset = dataset
         self._alpha = alpha
-        self._df = self._parse_to_dataframe(dataset, alpha, tracking_loss_type)
+        self._df = self._parse_to_dataframe(dataset, alpha)
         self._mean_loss_dyns = self._df.mean(0)
         self._mean_loss_dyns_per_label = {
             label_id: df_sub.mean(0) for label_id, df_sub in self._df.groupby("ann_label")
         }
-        self._tracking_loss_type = tracking_loss_type
 
     @property
     def alpha(self) -> float:
         """A parameter to obtain EMA loss dynamics statistics.
 
         ema_loss_dyns(t) := (1 - alpha) * ema_loss_dyns(t - 1) + alpha * loss_dyns(t)"""
         return self._alpha
@@ -105,27 +88,22 @@
 
     @property
     def ema_dataframe(self) -> pd.DataFrame:
         """Pandas DataFrame including full EMA loss dynamics statistics."""
         return self._df
 
     @staticmethod
-    def _parse_to_dataframe(
-        dataset: IDataset, ema_alpha: float = 0.001, tracking_loss_type: Optional[str] = None
-    ) -> pd.DataFrame:
+    def _parse_to_dataframe(dataset: IDataset, ema_alpha: float = 0.001) -> pd.DataFrame:
         """Parse loss dynamics statistics from Datumaro dataset to Pandas DataFrame."""
-        key = (
-            "loss_dynamics" if tracking_loss_type is None else f"loss_dynamics_{tracking_loss_type}"
-        )
         ema_loss_dyns_list = []
         for item in dataset:
             for ann in item.annotations:
                 # The first value should be start from zero
                 loss_dyns = pd.Series(
-                    [0.0] + ann.attributes.get(key),
+                    [0.0] + ann.attributes.get("loss_dynamics"),
                     index=[-1] + ann.attributes.get("iters"),
                     name=(item.id, item.subset, ann.id, ann.label),
                 )
                 ema_loss_dyns = loss_dyns.ewm(alpha=ema_alpha, adjust=False).mean().iloc[1:]
                 ema_loss_dyns_list.append(ema_loss_dyns)
 
         df = pd.DataFrame(ema_loss_dyns_list).rename_axis(
@@ -188,19 +166,21 @@
                 self._mean_loss_dyns.iloc[1:]
                 if label_id is None
                 else self._mean_loss_dyns_per_label[label_id].iloc[1:]
             )
             plt.plot(mean_series, color=mean_plot_color, linestyle=mean_plot_style, label="mean")
 
             cands = cands_by_label_id[label_id]
-            for cand in cands:
-                row = self._df.loc[(cand.id, cand.subset, cand.ann_id, cand.label_id)]
+            ids = [cand.id for cand in cands]
+            target = self._df.query(f"item_id == {ids}")
+
+            for (item_id, subset_id, ann_id, label), row in target.iterrows():
                 plt.plot(
                     row.dropna().iloc[1:],
-                    label=f"id={cand.id}, subset={cand.subset}, ann_id={cand.ann_id}, label_id={cand.label_id}",
+                    label=f"id={item_id}, subset={subset_id}, ann_id={ann_id}, label_id={label}",
                     **kwargs,
                 )
 
             plt.ylabel("EMA training loss dynamics")
             plt.xlabel("Training iterations")
 
             plt.title(
```

### Comparing `datumaro-1.3.0/datumaro/components/algorithms/rise.py` & `datumaro-1.3.0rc1/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/annotation.py` & `datumaro-1.3.0rc1/datumaro/components/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,26 +208,19 @@
 
 @attrs(slots=True, order=False)
 class Label(Annotation):
     _type = AnnotationType.label
     label: int = field(converter=int)
 
 
-@attrs(slots=True, eq=False, order=False)
+@attrs(slots=True, order=False)
 class HashKey(Annotation):
     _type = AnnotationType.hash_key
     hash_key: np.ndarray = field(factory=lambda: np.zeros((1, 64), dtype=np.uint8))
 
-    def __eq__(self, other):
-        if not super().__eq__(other):
-            return False
-        if not isinstance(other, __class__):
-            return False
-        return np.array_equal(self.hash_key, other.hash_key)
-
 
 RgbColor = Tuple[int, int, int]
 
 Colormap = Dict[int, RgbColor]
 """Represents { index -> color } mapping for segmentation masks"""
```

### Comparing `datumaro-1.3.0/datumaro/components/annotations/matcher.py` & `datumaro-1.3.0rc1/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/annotations/merger.py` & `datumaro-1.3.0rc1/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/cli_plugin.py` & `datumaro-1.3.0rc1/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/config.py` & `datumaro-1.3.0rc1/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/config_model.py` & `datumaro-1.3.0rc1/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/crypter.py` & `datumaro-1.3.0rc1/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/dataset.py` & `datumaro-1.3.0rc1/datumaro/components/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 from datumaro.components.media import Image, MediaElement
 from datumaro.components.merge import DEFAULT_MERGE_POLICY
 from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
 from datumaro.components.transformer import ItemTransform, Transform
 from datumaro.plugins.transforms import ProjectLabels
 from datumaro.util import is_method_redefined
 from datumaro.util.log_utils import logging_disabled
-from datumaro.util.meta_file_util import load_hash_key
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scoped
 
 DEFAULT_FORMAT = "datumaro"
 
 
 class ItemStatus(Enum):
@@ -1278,15 +1277,14 @@
             raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from cause
         except Exception as e:
             raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from e
 
         dataset._source_path = path
         dataset._format = format
 
-        dataset = load_hash_key(path, dataset)
         return dataset
 
     @staticmethod
     def detect(path: str, *, env: Optional[Environment] = None, depth: int = 2) -> str:
         """
         Attempts to detect dataset format of a given directory.
```

### Comparing `datumaro-1.3.0/datumaro/components/dataset_base.py` & `datumaro-1.3.0rc1/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/dataset_item_storage.py` & `datumaro-1.3.0rc1/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/environment.py` & `datumaro-1.3.0rc1/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/errors.py` & `datumaro-1.3.0rc1/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/explorer.py` & `datumaro-1.3.0rc1/datumaro/components/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/exporter.py` & `datumaro-1.3.0rc1/datumaro/components/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# Copyright (C) 2019-2023 Intel Corporation
+# Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
 import shutil
 import warnings
 from tempfile import mkdtemp
 from typing import NoReturn, Optional, Tuple, TypeVar, Union
 
 import attr
 from attrs import define, field
 
-from datumaro.components.annotation import HashKey
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.dataset_base import DatasetItem, IDataset
 from datumaro.components.errors import (
     AnnotationExportError,
     DatasetExportError,
     DatumaroError,
@@ -159,20 +158,14 @@
 
         rmtree(save_dir)
         os.replace(tmpdir, save_dir)
 
         return retval
 
     def apply(self):
-        """Execute the data-format conversion"""
-        if self._save_hashkey_meta:
-            self._save_hashkey_file(self._save_dir)
-        return self._apply_impl()
-
-    def _apply_impl(self):
         raise NotImplementedError("Should be implemented in a subclass")
 
     def __init__(
         self,
         extractor: IDataset,
         save_dir: str,
         *,
@@ -286,22 +279,14 @@
 
     def _save_meta_file(self, path):
         save_meta_file(path, self._extractor.categories())
 
     def _save_hashkey_file(self, path):
         save_hashkey_file(path, self._extractor)
 
-    def _check_hash_key_existence(self, item):
-        if self._save_hashkey_meta:
-            return
-        for annotation in item.annotations:
-            if isinstance(annotation, HashKey):
-                self._save_hashkey_meta = True
-                return
-
 
 # TODO: Currently, ExportContextComponent is introduced only for Datumaro and DatumaroBinary format
 # for multi-processing. We need to propagate this to everywhere in Datumaro 1.2.0
 
 
 class ExportContextComponent:
     def __init__(
```

### Comparing `datumaro-1.3.0/datumaro/components/extractor_tfds.py` & `datumaro-1.3.0rc1/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/filter.py` & `datumaro-1.3.0rc1/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/format_detection.py` & `datumaro-1.3.0rc1/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/generator.py` & `datumaro-1.3.0rc1/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/hl_ops/__init__.py` & `datumaro-1.3.0rc1/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/importer.py` & `datumaro-1.3.0rc1/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/launcher.py` & `datumaro-1.3.0rc1/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/media.py` & `datumaro-1.3.0rc1/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/media_manager.py` & `datumaro-1.3.0rc1/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/merge/__init__.py` & `datumaro-1.3.0rc1/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/merge/base.py` & `datumaro-1.3.0rc1/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/merge/exact_merge.py` & `datumaro-1.3.0rc1/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/merge/intersect_merge.py` & `datumaro-1.3.0rc1/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/merge/union_merge.py` & `datumaro-1.3.0rc1/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/operations.py` & `datumaro-1.3.0rc1/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/progress_reporting.py` & `datumaro-1.3.0rc1/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/project.py` & `datumaro-1.3.0rc1/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/shift_analyzer.py` & `datumaro-1.3.0rc1/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/transformer.py` & `datumaro-1.3.0rc1/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/validator.py` & `datumaro-1.3.0rc1/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/components/visualizer.py` & `datumaro-1.3.0rc1/datumaro/components/visualizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -204,50 +204,15 @@
 
         return random.choices(self._items, k=n_samples)
 
     @overload
     def vis_gallery(
         self,
         ids: List[str],
-        ann_ids: List[int],
-        subsets: Union[str, List[str]],
-        *,
-        grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
-    ):
-        """Visualize several :class:`DatasetItem` as a gallery.
-
-        If `ann_ids` is given, only draw one annotation matching `ann_id` per item.
-        For example, if `ids = ["item_0", "item_1"]` and `ann_ids = [2, 3]`, The item with
-        `item.id` = "item_0" will only draw the annotation with `ann.id` = 2 and will not draw the others.
-
-        Parameters
-        ----------
-        ids
-            A list of :class:`DatasetItem`'s ID to visualize
-        ann_ids
-            A list of :class:`Annotation`'s ID to visualize
-        subsets
-            A list of :class:`DatasetItem`'s subset name to visualize.
-            If a string is given, it is automatically expanded into
-            a list up to the length of `ids`.
-        grid_size
-            Grid size of the gallery plot. If `None`, we automatically infer its size.
-
-        Return
-        ------
-            :class:`Figure` include visualization plots.
-        """
-        ...
-
-    @overload
-    def vis_gallery(
-        self,
-        ids: List[str],
-        subsets: Union[str, List[str]],
-        *,
+        subsets: Union[str, List[str]] = None,
         grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
     ):
         """Visualize several :class:`DatasetItem` as a gallery
 
         Parameters
         ----------
         ids
@@ -265,15 +230,14 @@
         """
         ...
 
     @overload
     def vis_gallery(
         self,
         items: List[DatasetItem],
-        *,
         grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
     ):
         """Visualize several :class:`DatasetItem` as a gallery
 
         Parameters
         ----------
         items
@@ -288,101 +252,98 @@
     def vis_gallery(
         self,
         *inputs,
         grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
     ) -> Figure:
         """Visualize several :class:`DatasetItem` as a gallery"""
         if len(inputs) == 1:
+            ids, subsets = None, None
             (items,) = inputs
-            ids = [item.id for item in items]
-            subsets = [item.subset for item in items]
-            ann_ids = [None for _ in items]
+
         elif len(inputs) == 2:
             ids, subsets = inputs
             items = None
-            ann_ids = [None for _ in ids]
-        elif len(inputs) == 3:
-            ids, ann_ids, subsets = inputs
+            if isinstance(subsets, str):
+                subsets = [subsets] * len(ids)  # expand it to have len(ids)
 
-        if isinstance(subsets, str):
-            subsets = [subsets] * len(ids)  # expand it to have len(ids)
+        def _parse_inputs(
+            ids: Optional[List[str]],
+            subsets: Optional[List[str]],
+            items: Optional[List[DatasetItem]],
+        ) -> Tuple[List[str], List[str]]:
+            if ids is not None and subsets is not None:
+                return ids, subsets
+            elif items is not None:
+                return [item.id for item in items], [item.subset for item in items]
+            raise ValueError(
+                f"ids={ids}, subsets={subsets}, and items={items} is an invalid input."
+            )
 
-        assert (
-            len(ids) == len(ann_ids) == len(subsets)
-        ), "ids, ann_ids, subset should have the same length"
+        ids, subsets = _parse_inputs(ids, subsets, items)
 
         nrows, ncols = _infer_grid_size(len(ids), grid_size)
         fig, axs = plt.subplots(nrows, ncols, figsize=self.figsize)
 
         assert len(ids) == len(
             subsets
         ), "If subset is a list, it should have the same length as ids."
 
-        for item_id, subset, ann_id, ax in zip(ids, subsets, ann_ids, axs.flatten()):
-            self.vis_one_sample(item_id, subset, ann_id=ann_id, ax=ax)
+        for item_id, subset, ax in zip(ids, subsets, axs.flatten()):
+            self.vis_one_sample(item_id, subset, ax=ax)
 
         return fig
 
     @overload
     def vis_one_sample(
         self,
-        item_id: str,
-        subset: str,
-        *,
-        ann_id: Optional[int] = None,
+        item_id: str = None,
+        subset: str = None,
         ax: Optional[Axes] = None,
     ) -> Figure:
         """Visualize one :class:`DatasetItem`
 
         Parameters
         ----------
         item_id
             ID of :class:`DatasetItem` to visualize
         subset
             Subset name of :class:`DatasetItem` to visualize
-        ann_id
-            If not `None`, only draw an annotation which has `id=ann_id`.
         ax
             If not `None`, draw on `ax` instead of creating a new one
 
         Return
         ------
             :class:`Figure` include visualization plot of the :class:`DatasetItem`.
         """
         ...
 
     @overload
     def vis_one_sample(
         self,
-        item: DatasetItem,
-        *,
-        ann_id: Optional[int] = None,
+        item: DatasetItem = None,
         ax: Optional[Axes] = None,
     ) -> Figure:
         """Visualize one :class:`DatasetItem`
 
         Parameters
         ----------
         item
             :class:`DatasetItem` to visualize
-        ann_id
-            If not `None`, only draw an annotation which has `id=ann_id`.
         ax
             If not `None`, draw on `ax` instead of creating a new one
 
         Return
         ------
             :class:`Figure` include visualization plot of the :class:`DatasetItem`.
         """
         ...
 
     def vis_one_sample(
         self,
         *inputs,
-        ann_id: Optional[int] = None,
         ax: Optional[Axes] = None,
     ) -> Figure:
         """Visualize one dataset item"""
         if len(inputs) == 1:
             item_id, subset = None, None
             (item,) = inputs
 
@@ -450,17 +411,15 @@
         context = defaultdict(list)
         for ann in annotations:
             if ann.type in self.ignored_types:
                 ignore_type = AnnotationType(ann.type).name
                 msg = f"{ignore_type} in self.ignored_types. Skip it."
                 warnings.warn(msg)
                 continue
-
-            if ann_id is None or ann_id == ann.id:
-                self._draw(ann, label_categories, fig, ax, context[ann.type])
+            self._draw(ann, label_categories, fig, ax, context[ann.type])
 
         return fig
 
     def _draw_label(
         self,
         ann: Label,
         label_categories: Optional[LabelCategories],
```

### Comparing `datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
             export_context=export_context,
             num_shards=self._num_shards,
             max_shard_size=self._max_shard_size,
             max_chunk_size=self._max_chunk_size,
             ctx=ctx,
         )
 
-    def _apply_impl(self, *args, **kwargs):
+    def apply(self, *args, **kwargs):
         if self._num_workers == 0:
             return self._apply()
 
         with Pool(processes=self._num_workers) as pool:
             return self._apply(pool)
 
     def _apply(self, pool: Optional[Pool] = None):
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         super().detect(context)
         return FormatDetectionConfidence.MEDIUM
 
 
 class AvaExporter(Exporter):
     DEFAULT_IMAGE_EXT = AvaPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         save_dir = self._save_dir
 
         ann_dir = osp.join(save_dir, AvaPath.ANNOTATION_DIR)
         os.makedirs(ann_dir, exist_ok=True)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/brats.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/camvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
         self._apply_colormap = apply_colormap
 
         if label_map is None:
             label_map = LabelmapType.source.name
         self._load_categories(label_map)
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         for subset_name, subset in self._extractor.subsets().items():
             segm_list = {}
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cifar.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,16 +198,15 @@
                 root_dir = osp.dirname(root["url"])
                 sources += cls._find_sources_recursive(
                     root_dir,
                     "",
                     "cifar",
                     # Subset files have no extension in the format, and
                     # should not be the meta file.
-                    file_filter=lambda p: not osp.isdir(p)
-                    and not osp.splitext(osp.basename(p))[1]
+                    file_filter=lambda p: not osp.splitext(osp.basename(p))[1]
                     and osp.basename(p) != meta_file_name,
                 )
 
             return sources
 
         sources = []
         sources += _find(path, CifarPath.META_10_FILE)
@@ -215,15 +214,15 @@
 
         return sources
 
 
 class CifarExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cityscapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 from collections import OrderedDict
 from enum import Enum, auto
 from typing import Optional
@@ -97,15 +96,15 @@
         ("licenseplate", (0, 0, 142)),
     ]
 )
 
 
 class CityscapesPath:
     GT_FINE_DIR = "gtFine"
-    IMGS_FINE_DIR = ""
+    IMGS_FINE_DIR = "imgsFine"
     ORIGINAL_IMAGE_DIR = "leftImg8bit"
     ORIGINAL_IMAGE = "_" + ORIGINAL_IMAGE_DIR
     INSTANCES_IMAGE = "_instanceIds.png"
     GT_INSTANCE_MASK_SUFFIX = "_" + GT_FINE_DIR + INSTANCES_IMAGE
     COLOR_IMAGE = "_color.png"
     LABELIDS_IMAGE = "_labelIds.png"
     LABEL_TRAIN_IDS_SUFFIX = "_" + GT_FINE_DIR + "_labelTrainIds.png"
@@ -206,18 +205,14 @@
             self._path = osp.dirname(osp.dirname(osp.dirname(path)))
             images_dir = path
             annotations_dir = osp.join(self._path, CityscapesPath.GT_FINE_DIR, subset)
 
         self._images_dir = images_dir
         self._gt_anns_dir = annotations_dir
 
-        for path in [self._images_dir, self._gt_anns_dir]:
-            if not osp.isdir(path):
-                raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
-
         super().__init__(subset=subset, ctx=ctx)
 
         self._items = list(self._load_items().values())
 
     def _load_categories(self, path, use_train_label_map=False):
         label_map = None
         if has_meta_file(path):
@@ -312,31 +307,22 @@
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
 
 class CityscapesImporter(Importer):
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annotation_patterns = [
+        patterns = [
             f"{CityscapesPath.GT_FINE_DIR}/**/*{CityscapesPath.GT_INSTANCE_MASK_SUFFIX}",
             f"{CityscapesPath.GT_FINE_DIR}/**/*{CityscapesPath.LABEL_TRAIN_IDS_SUFFIX}",
-        ]
-
-        media_patterns = [
             f"{CityscapesPath.IMGS_FINE_DIR}/{CityscapesPath.ORIGINAL_IMAGE_DIR}"
             f"/**/*{CityscapesPath.ORIGINAL_IMAGE}.*",
         ]
-
         with context.require_any():
-            for pattern in annotation_patterns:
-                with context.alternative():
-                    context.require_file(pattern)
-
-        with context.require_any():
-            for pattern in media_patterns:
+            for pattern in patterns:
                 with context.alternative():
                     context.require_file(pattern)
 
     @classmethod
     def find_sources(cls, path):
         sources = cls._find_sources_recursive(
             path, "", "cityscapes", dirname=CityscapesPath.GT_FINE_DIR, max_depth=1
@@ -390,35 +376,26 @@
 
         self._apply_colormap = apply_colormap
 
         if label_map is None:
             label_map = LabelmapType.source.name
         self._load_categories(label_map)
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         for subset_name, subset in self._extractor.subsets().items():
-            media_dir = osp.join(
-                self._save_dir,
-                CityscapesPath.IMGS_FINE_DIR,
-                CityscapesPath.ORIGINAL_IMAGE_DIR,
-                subset_name,
-            )
-            os.makedirs(media_dir, exist_ok=True)
-
-            mask_dir = osp.join(self._save_dir, CityscapesPath.GT_FINE_DIR, subset_name)
-            os.makedirs(mask_dir, exist_ok=True)
-
             for item in subset:
                 image_path = osp.join(
-                    media_dir,
+                    CityscapesPath.IMGS_FINE_DIR,
+                    CityscapesPath.ORIGINAL_IMAGE_DIR,
+                    subset_name,
                     item.id + CityscapesPath.ORIGINAL_IMAGE + self._find_image_ext(item),
                 )
                 if self._save_media:
                     self._save_image(item, osp.join(self._save_dir, image_path))
 
                 masks = [a for a in item.annotations if a.type == AnnotationType.mask]
                 if not masks:
@@ -433,14 +410,15 @@
                         if m.attributes.get("is_crowd", False)
                         else self._label_id_mapping(m.label) * 1000 + (m.id or (i + 1))
                         for i, m in enumerate(masks)
                     ],
                     instance_labels=[self._label_id_mapping(m.label) for m in masks],
                 )
 
+                mask_dir = osp.join(self._save_dir, CityscapesPath.GT_FINE_DIR, subset_name)
                 mask_name = item.id + "_" + CityscapesPath.GT_FINE_DIR
 
                 color_mask_path = osp.join(mask_dir, mask_name + CityscapesPath.COLOR_IMAGE)
                 self.save_mask(color_mask_path, compiled_mask.class_mask)
 
                 cls_mask_path = osp.join(mask_dir, mask_name + CityscapesPath.LABELIDS_IMAGE)
                 self.save_mask(
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,15 +709,15 @@
             if not self._reindex:
                 image_id = cast(item.attributes.get("id"), int, len(self._image_ids) + 1)
             else:
                 image_id = len(self._image_ids) + 1
             self._image_ids[item.id] = image_id
         return image_id
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         self._make_dirs()
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,15 @@
         for item in extractor:
             if item_hw is None:
                 item_hw = item.media.size
             elif item_hw != item.media.size:
                 return None
         return (item_hw[1], item_hw[0])
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         self._images_dir = osp.join(self._save_dir, CvatPath.IMAGES_DIR)
         os.makedirs(self._images_dir, exist_ok=True)
 
         for subset_name, subset in self._extractor.subsets().items():
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from typing import Optional
 
+import numpy as np
+
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Caption,
     Cuboid3d,
     Ellipse,
+    HashKey,
     Label,
     LabelCategories,
     MaskCategories,
     Points,
     PointsCategories,
     Polygon,
     PolyLine,
     RleMask,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError, MediaTypeError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util import parse_json_file
+from datumaro.util.meta_file_util import has_hashkey_file, parse_hashkey_file
 from datumaro.version import __version__
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 
 class DatumaroBase(SubsetBase):
     LEGACY_VERSION = "legacy"
@@ -95,15 +99,16 @@
         self._parsed_anns = parse_json_file(path)
         return self._parsed_anns.get("dm_format_version", self.LEGACY_VERSION)
 
     def _load_impl(self, path: str) -> None:
         """Actual implementation of loading Datumaro format."""
         self._infos = self._load_infos(self._parsed_anns)
         self._categories = self._load_categories(self._parsed_anns)
-        self._items = self._load_items(self._parsed_anns)
+        items = self._load_items(self._parsed_anns)
+        self._items = self._load_hash_key(items)
 
     @staticmethod
     def _load_infos(parsed):
         return parsed.get("infos", {})
 
     @staticmethod
     def _load_categories(parsed):
@@ -201,14 +206,24 @@
                 attributes=item_desc.get("attr"),
             )
 
             items.append(item)
 
         return items
 
+    def _load_hash_key(self, items):
+        if not has_hashkey_file(self._rootpath):
+            return items
+
+        hashkey_dict = parse_hashkey_file(self._rootpath)
+        for item in items:
+            hash_key = hashkey_dict[item.subset + "/" + item.id]
+            item.annotations.append(HashKey(hash_key=np.asarray(hash_key, dtype=np.uint8)))
+        return items
+
     @staticmethod
     def _load_annotations(item):
         parsed = item["annotations"]
         loaded = []
 
         for ann in parsed:
             ann_id = ann.get("id")
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
 
         return _SubsetWriter(
             context=self,
             ann_file=osp.join(self._annotations_dir, subset + self.PATH_CLS.ANNOTATION_EXT),
             export_context=export_context,
         )
 
-    def _apply_impl(self, pool: Optional[Pool] = None, *args, **kwargs):
+    def apply(self, pool: Optional[Pool] = None, *args, **kwargs):
         os.makedirs(self._save_dir, exist_ok=True)
 
         images_dir = osp.join(self._save_dir, self.PATH_CLS.IMAGES_DIR)
         os.makedirs(images_dir, exist_ok=True)
         self._images_dir = images_dir
 
         annotations_dir = osp.join(self._save_dir, self.PATH_CLS.ANNOTATIONS_DIR)
@@ -464,7 +464,15 @@
             )
             if osp.isfile(pcd_path):
                 os.unlink(pcd_path)
 
             related_images_path = osp.join(save_dir, cls.PATH_CLS.IMAGES_DIR, item.subset, item.id)
             if osp.isdir(related_images_path):
                 shutil.rmtree(related_images_path)
+
+    def _check_hash_key_existence(self, item):
+        if self._save_hashkey_meta:
+            return
+        for annotation in item.annotations:
+            if isinstance(annotation, HashKey):
+                self._save_hashkey_meta = True
+                return
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,13 +311,13 @@
             ann_file=osp.join(self._annotations_dir, subset + self.PATH_CLS.ANNOTATION_EXT),
             export_context=export_context,
             secret_key_file=osp.join(self._save_dir, self.PATH_CLS.SECRET_KEY_FILE),
             no_media_encryption=self._no_media_encryption,
             max_blob_size=self._max_blob_size,
         )
 
-    def _apply_impl(self, *args, **kwargs):
+    def apply(self, *args, **kwargs):
         if self._num_workers == 0:
-            return super()._apply_impl()
+            return super().apply()
 
         with Pool(processes=self._num_workers) as pool:
-            return super()._apply_impl(pool)
+            return super().apply(pool)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .format import IcdarPath
 
 
 class IcdarWordRecognitionExporter(Exporter):
     DEFAULT_IMAGE_EXT = IcdarPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         for subset_name, subset in self._extractor.subsets().items():
             annotation = ""
             for item in subset:
                 image_filename = self._make_image_filename(item)
@@ -45,15 +45,15 @@
                 with open(anno_file, "w", encoding="utf-8") as f:
                     f.write(annotation)
 
 
 class IcdarTextLocalizationExporter(Exporter):
     DEFAULT_IMAGE_EXT = IcdarPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         for subset_name, subset in self._extractor.subsets().items():
             for item in subset:
                 if self._save_media and item.media:
                     self._save_image(item, subdir=osp.join(subset_name, IcdarPath.IMAGES_DIR))
@@ -80,15 +80,15 @@
                 with open(anno_file, "w", encoding="utf-8") as f:
                     f.write(annotation)
 
 
 class IcdarTextSegmentationExporter(Exporter):
     DEFAULT_IMAGE_EXT = IcdarPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         for subset_name, subset in self._extractor.subsets().items():
             for item in subset:
                 self._save_item(subset_name, subset, item)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_dir.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 DatasetItem(id=item_id, subset=self._subset, media=Image.from_file(path=path))
             )
 
 
 class ImageDirExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
-    def _apply_impl(self):
+    def apply(self):
         os.makedirs(self._save_dir, exist_ok=True)
 
         for item in self._extractor:
             if item.media:
                 self._save_image(item)
             else:
                 log.debug("Item '%s' has no image info", item.id)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         compression = parse_str_enum_value(
             compression, Compression, default=ImageZipPath.DEFAULT_COMPRESSION
         )
 
         self._archive_name = name
         self._compression = compression.value
 
-    def _apply_impl(self):
+    def apply(self):
         os.makedirs(self._save_dir, exist_ok=True)
 
         archive_path = osp.join(self._save_dir, self._archive_name)
 
         if osp.exists(archive_path):
             raise FileExistsError(
                 "Zip file: %s, already exist, "
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     """
 
 
 class ImagenetExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
     USE_SUBSET_DIRS = False
 
-    def _apply_impl(self):
+    def apply(self):
         def _get_name(item: DatasetItem) -> str:
             id_parts = item.id.split(ImagenetPath.SEP_TOKEN)
 
             if len(id_parts) == 1:
                 # e.g. item.id = my_img_1
                 return item.id
             else:
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
         return cls._find_sources_recursive(path, ".txt", "imagenet_txt", file_filter=file_filter)
 
 
 class ImagenetTxtExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         subset_dir = self._save_dir
         os.makedirs(subset_dir, exist_ok=True)
 
         extractor = self._extractor
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         elif KittiTask.detection in self._tasks:
             self._categories = {
                 AnnotationType.label: self._extractor.categories().get(
                     AnnotationType.label, LabelCategories()
                 )
             }
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         for subset_name, subset in self._extractor.subsets().items():
             if KittiTask.segmentation in self._tasks:
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,15 +456,15 @@
                     )
 
         elif self._save_media and not item.media:
             log.debug("Item '%s' has no image info", item.id)
 
         return index
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and self._extractor.media_type() is not PointCloud:
             raise MediaTypeError("Media type is not a point cloud")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
             pass
         return subsets
 
 
 class LabelMeExporter(Exporter):
     DEFAULT_IMAGE_EXT = LabelMePath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/lfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             path, ext, "lfw", filename=base, dirname=LfwPath.ANNOTATION_DIR
         )
 
 
 class LfwExporter(Exporter):
     DEFAULT_IMAGE_EXT = LfwPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/market1501.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         query = item.attributes.get("query")
         if query is not None and isinstance(query, str):
             query = str_to_bool(query)
         if query:
             dirname = Market1501Path.QUERY_DIR
         return dirname
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         for subset_name, subset in self._extractor.subsets().items():
             annotation = ""
             used_frames = {}
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mars.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             and osp.basename(p).split("-")[1] == "labels",
         )
 
 
 class MnistExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             path, ".csv", "mnist_csv", file_filter=lambda p: not osp.basename(p).startswith("meta")
         )
 
 
 class MnistCsvExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mot.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mot.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             path, ".txt", "mot_seq", dirname="gt", filename=osp.splitext(MotPath.GT_FILENAME)[0]
         )
 
 
 class MotSeqGtExporter(Exporter):
     DEFAULT_IMAGE_EXT = MotPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         extractor = self._extractor
 
         if extractor.media_type() and not issubclass(extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         image_dir = osp.join(self._save_dir, MotPath.IMAGE_DIR)
         os.makedirs(image_dir, exist_ok=True)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mots.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mots.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 subsets.extend(detected)
         return subsets
 
 
 class MotsPngExporter(Exporter):
     DEFAULT_IMAGE_EXT = MotsPath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             tasks = set(MvtecTask)
         elif isinstance(tasks, MvtecTask):
             tasks = {tasks}
         else:
             tasks = set(parse_str_enum_value(t, MvtecTask) for t in tasks)
         self._tasks = tasks
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         for subset_name, subset in self._extractor.subsets().items():
             if MvtecTask.segmentation in self._tasks or MvtecTask.detection in self._tasks:
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/open_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,15 +707,15 @@
             ):
                 os.unlink(osp.join(self._annotations_dir, file_name))
 
 
 class OpenImagesExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         self._save(_AnnotationWriter(self._save_dir))
 
     @classmethod
     def patch(cls, dataset, patch, save_dir, **options):
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                     for ann in anns
                     for point_coord in ann.attributes.get("point_coords", [[]])
                 )
             ),
         }
         return annotation_data
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         subsets = self._extractor.subsets()
         pbars = self._ctx.progress_reporter.split(len(subsets))
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 
     def __init__(self, extractor, save_dir, reindex=False, allow_undeclared_attrs=False, **kwargs):
         super().__init__(extractor, save_dir, **kwargs)
 
         self._reindex = reindex
         self._allow_undeclared_attrs = allow_undeclared_attrs
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and self._extractor.media_type() is not PointCloud:
             raise MediaTypeError("Media type is not an image")
 
         if 1 < len(self._extractor.subsets()):
             log.warning(
                 "Supervisely pointcloud format supports only a single "
                 "subset. Subset information will be ignored on export."
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         return parser
 
     def __init__(self, extractor, save_dir, save_masks=False, **kwargs):
         super().__init__(extractor, save_dir, **kwargs)
 
         self._save_masks = save_masks
 
-    def _apply_impl(self):
+    def apply(self):
         os.makedirs(self._save_dir, exist_ok=True)
 
         label_categories = self._extractor.categories().get(AnnotationType.label, LabelCategories())
         get_label = (
             lambda label_id: label_categories.items[label_id].name if label_id is not None else ""
         )
         label_ids = OrderedDict(
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
                 ]
         return []
 
 
 class VggFace2Exporter(Exporter):
     DEFAULT_IMAGE_EXT = VggFace2Path.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         def _get_name_id(item_parts, label_name):
             if 1 < len(item_parts) and item_parts[0] == label_name:
                 return "/".join([label_name, *item_parts[1:]])
             else:
                 return "/".join([label_name, *item_parts])
 
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
@@ -264,15 +264,15 @@
         for subset_name, subset in self._extractor.subsets().items():
             bboxes_table = []
             landmarks_table = []
             for item in subset:
                 item_parts = item.id.split("/")
                 if item.media and self._save_media:
                     labels = set(
-                        p.label for p in item.annotations if (getattr(p, "label", None) is not None)
+                        p.label for p in item.annotations if getattr(p, "label") is not None
                     )
                     if labels:
                         for label in labels:
                             image_dir = label_categories[label].name
                             if 1 < len(item_parts) and image_dir == item_parts[0]:
                                 image_dir = ""
                             self._save_image(item, subdir=osp.join(subset_name, image_dir))
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/video.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         if label_map is None:
             label_map = LabelmapType.source.name
         assert isinstance(label_map, (str, dict)), label_map
         self._load_categories(label_map)
 
         self._patch = None
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         self.make_dirs()
         self.save_subsets()
         self.save_label_map()
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/widerface.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             path, ".txt", "wider_face", dirname=WiderFacePath.ANNOTATIONS_DIR
         )
 
 
 class WiderFaceExporter(Exporter):
     DEFAULT_IMAGE_EXT = WiderFacePath.IMAGE_EXT
 
-    def _apply_impl(self):
+    def apply(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         save_dir = self._save_dir
         os.makedirs(save_dir, exist_ok=True)
 
         label_categories = self._extractor.categories()[AnnotationType.label]
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def __init__(
         self, extractor: IDataset, save_dir: str, *, add_path_prefix: bool = True, **kwargs
     ) -> None:
         super().__init__(extractor, save_dir, **kwargs)
 
         self._prefix = "data" if add_path_prefix else ""
 
-    def _apply_impl(self):
+    def apply(self):
         extractor = self._extractor
         save_dir = self._save_dir
 
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
         os.makedirs(save_dir, exist_ok=True)
@@ -219,15 +219,15 @@
         for must_name in self.must_subset_names:
             if must_name not in subset_names:
                 raise DatasetExportError(
                     f'Subset "{must_name}" is not in {subset_names}, '
                     "but YoloUltralytics requires both of them."
                 )
 
-    def _apply_impl(self):
+    def apply(self):
         extractor = self._extractor
         save_dir = self._save_dir
 
         os.makedirs(save_dir, exist_ok=True)
 
         try:
             self._check_dataset()
```

### Comparing `datumaro-1.3.0/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/explorer.py` & `datumaro-1.3.0rc1/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/ndr.py` & `datumaro-1.3.0rc1/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.3.0rc1/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.3.0rc1/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/shift_analyzer.py` & `datumaro-1.3.0rc1/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/splitter.py` & `datumaro-1.3.0rc1/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.3.0rc1/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/tiling/tile.py` & `datumaro-1.3.0rc1/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/tiling/util.py` & `datumaro-1.3.0rc1/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/plugins/transforms.py` & `datumaro-1.3.0rc1/datumaro/plugins/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,61 +337,24 @@
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument("-s", "--start", type=int, default=1, help="Start value for item ids")
         return parser
 
-    def __init__(self, extractor, start: int = 1):
+    def __init__(self, extractor, start=1):
         super().__init__(extractor)
         self._length = "parent"
         self._start = start
 
     def __iter__(self):
         for i, item in enumerate(self._extractor):
             yield self.wrap_item(item, id=i + self._start)
 
 
-class ReindexAnnotations(ItemTransform, CliPlugin):
-    """
-    Replaces dataset items' annotations with sequential indices.
-    """
-
-    @classmethod
-    def build_cmdline_parser(cls, **kwargs):
-        parser = super().build_cmdline_parser(**kwargs)
-        parser.add_argument("-s", "--start", type=int, default=1, help="Start value for item ids")
-        parser.add_argument(
-            "-r",
-            "--reindex-each-item",
-            action="store_true",
-            help="If true, reindex for each item every timeReindex for each item. For example, "
-            "item_1 will have ann(id=1), ann(id=2), ..., ann(id=5) and item_2 will have ann_1(id=1), ..., "
-            "if reindex_each_item=true and start=1, otherwise, item_2 will have ann_1(id=6), ..., "
-            "because item_1 has ann_5(id=5).",
-        )
-        return parser
-
-    def __init__(self, extractor, start: int = 1, reindex_each_item: bool = False):
-        super().__init__(extractor)
-        self._length = "parent"
-        self._start = start
-        self._cur_idx = start
-        self._reindex_each_item = reindex_each_item
-
-    def transform_item(self, item: DatasetItem) -> DatasetItem:
-        annotations = [
-            ann.wrap(id=idx) for idx, ann in enumerate(item.annotations, start=self._cur_idx)
-        ]
-
-        self._cur_idx = self._start if self._reindex_each_item else self._cur_idx + len(annotations)
-
-        return item.wrap(annotations=annotations)
-
-
 class Sort(Transform, CliPlugin):
     """
     Sorts dataset items.
     """
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
```

### Comparing `datumaro-1.3.0/datumaro/plugins/validators.py` & `datumaro-1.3.0rc1/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/__init__.py` & `datumaro-1.3.0rc1/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/annotation_util.py` & `datumaro-1.3.0rc1/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/attrs_util.py` & `datumaro-1.3.0rc1/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/file_utils.py` & `datumaro-1.3.0rc1/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/image.py` & `datumaro-1.3.0rc1/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/image_cache.py` & `datumaro-1.3.0rc1/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/log_utils.py` & `datumaro-1.3.0rc1/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/mask_tools.py` & `datumaro-1.3.0rc1/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/meta_file_util.py` & `datumaro-1.3.0rc1/datumaro/util/meta_file_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
 from collections import OrderedDict
 
-import numpy as np
-
 from datumaro.components.annotation import AnnotationType, HashKey
 from datumaro.util import dump_json_file, find, parse_json_file
 
 DATASET_META_FILE = "dataset_meta.json"
 DATASET_HASHKEY_FILE = "hash_keys.json"
-DATASET_HASHKEY_FOLDER = "hash_key_meta"
 
 
 def is_meta_file(path):
     return osp.splitext(osp.basename(path))[1] == ".json"
 
 
 def has_meta_file(path):
@@ -29,15 +26,17 @@
 
 
 def get_meta_file(path):
     return osp.join(path, DATASET_META_FILE)
 
 
 def get_hashkey_file(path):
-    hashkey_folder_path = osp.join(path, DATASET_HASHKEY_FOLDER)
+    hashkey_folder_path = osp.join(path, "hash_key_meta")
+    if not osp.exists(hashkey_folder_path):
+        os.makedirs(hashkey_folder_path)
     return osp.join(hashkey_folder_path, DATASET_HASHKEY_FILE)
 
 
 def parse_meta_file(path):
     meta_file = path
     if osp.isdir(path):
         meta_file = get_meta_file(path)
@@ -106,17 +105,14 @@
 
 
 def save_hashkey_file(path, item_list):
     dataset_hashkey = {}
 
     if osp.isdir(path):
         meta_file = get_hashkey_file(path)
-    hashkey_folder_path = osp.join(path, DATASET_HASHKEY_FOLDER)
-    if not osp.exists(hashkey_folder_path):
-        os.makedirs(hashkey_folder_path)
 
     hashkey_dict = parse_hashkey_file(path)
     if not hashkey_dict:
         hashkey_dict = {}
 
     for item in item_list:
         item_id = item.id
@@ -126,18 +122,7 @@
                 hashkey = annotation.hash_key
                 break
         hashkey_dict.update({item_subset + "/" + item_id: hashkey.tolist()})
 
     dataset_hashkey["hashkey"] = hashkey_dict
 
     dump_json_file(meta_file, dataset_hashkey, indent=True)
-
-
-def load_hash_key(path, dataset):
-    if not os.path.isdir(path) or not has_hashkey_file(path):
-        return dataset
-
-    hashkey_dict = parse_hashkey_file(path)
-    for item in dataset:
-        hash_key = hashkey_dict[item.subset + "/" + item.id]
-        item.annotations.append(HashKey(hash_key=np.asarray(hash_key, dtype=np.uint8)))
-    return dataset
```

### Comparing `datumaro-1.3.0/datumaro/util/os_util.py` & `datumaro-1.3.0rc1/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/pickle_util.py` & `datumaro-1.3.0rc1/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/scope.py` & `datumaro-1.3.0rc1/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/telemetry_stub.py` & `datumaro-1.3.0rc1/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/telemetry_utils.py` & `datumaro-1.3.0rc1/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro/util/tf_util.py` & `datumaro-1.3.0rc1/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro.egg-info/PKG-INFO` & `datumaro-1.3.0rc1/datumaro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,27 +34,27 @@
 ```
 <!--lint enable fenced-code-flag-->
 
 - [Getting started](https://openvinotoolkit.github.io/datumaro/latest/docs/get-started/quick-start-guide)
 - [Level Up](https://openvinotoolkit.github.io/datumaro/latest/docs/level-up/basic_skills)
 - [Features](#features)
 - [User manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
-- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro_module)
+- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro/datumaro)
 - [Contributing](#contributing)
 
 ## Features
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 - Dataset reading, writing, conversion in any direction.
   - [CIFAR-10/100](https://www.cs.toronto.edu/~kriz/cifar.html) (`classification`)
   - [Cityscapes](https://www.cityscapes-dataset.com/)
   - [COCO](http://cocodataset.org/#format-data) (`image_info`, `instances`, `person_keypoints`,
     `captions`, `labels`, `panoptic`, `stuff`)
-  - [CVAT](https://opencv.github.io/cvat/docs/manual/advanced/xml_format/)
+  - [CVAT](https://openvinotoolkit.github.io/cvat/docs/manual/advanced/xml_format)
   - [ImageNet](http://image-net.org/)
   - [Kitti](http://www.cvlibs.net/datasets/kitti/index.php) (`segmentation`, `detection`,
     `3D raw` / `velodyne points`)
   - [LabelMe](http://labelme.csail.mit.edu/Release3.0)
   - [LFW](http://vis-www.cs.umass.edu/lfw/) (`classification`, `person re-identification`,
     `landmarks`)
   - [MNIST](http://yann.lecun.com/exdb/mnist/) (`classification`)
```

### Comparing `datumaro-1.3.0/datumaro.egg-info/SOURCES.txt` & `datumaro-1.3.0rc1/datumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/datumaro.egg-info/requires.txt` & `datumaro-1.3.0rc1/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/pyproject.toml` & `datumaro-1.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/requirements-core.txt` & `datumaro-1.3.0rc1/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.0/setup.py` & `datumaro-1.3.0rc1/setup.py`

 * *Files identical despite different names*

