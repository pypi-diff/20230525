# Comparing `tmp/molgraph-0.3.1.tar.gz` & `tmp/molgraph-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.3.1.tar", last modified: Mon Apr 17 15:00:07 2023, max compression
+gzip compressed data, was "molgraph-0.3.2.tar", last modified: Thu May 25 14:35:09 2023, max compression
```

## Comparing `molgraph-0.3.1.tar` & `molgraph-0.3.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.168252 molgraph-0.3.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-04-17 15:00:07.168252 molgraph-0.3.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2402 2022-09-20 11:35:03.000000 molgraph-0.3.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.160252 molgraph-0.3.1/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-04-17 14:59:55.000000 molgraph-0.3.1/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.160252 molgraph-0.3.1/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.1/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.1/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.1/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.1/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.1/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.1/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.1/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3345 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.1/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11266 2022-09-02 16:19:13.000000 molgraph-0.3.1/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9279 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11313 2023-04-17 14:48:25.000000 molgraph-0.3.1/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10527 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14948 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/attentional/gt_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12894 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/layers/base.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.1/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9916 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9754 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7748 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10599 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.1/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.1/molgraph/layers/geometric/_radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9441 2022-09-02 12:17:48.000000 molgraph-0.3.1/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10267 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/layers/geometric/gcf_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.1/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21742 2023-04-17 07:38:04.000000 molgraph-0.3.1/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15618 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/layers/message_passing/mpnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 14:58:28.000000 molgraph-0.3.1/molgraph/layers/ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.1/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.3.1/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.1/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1987 2022-08-18 17:05:36.000000 molgraph-0.3.1/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.1/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.1/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11055 2022-08-31 15:11:51.000000 molgraph-0.3.1/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9439 2022-09-14 10:36:59.000000 molgraph-0.3.1/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11842 2022-08-31 15:11:51.000000 molgraph-0.3.1/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2022-08-18 17:06:18.000000 molgraph-0.3.1/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20437 2022-08-31 15:11:51.000000 molgraph-0.3.1/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.1/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.1/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.1/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.1/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.1/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.1/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.164252 molgraph-0.3.1/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.1/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.1/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.1/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.168252 molgraph-0.3.1/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.1/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.168252 molgraph-0.3.1/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.1/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.1/molgraph/models/interpretability/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.1/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.1/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.168252 molgraph-0.3.1/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.1/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.1/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.1/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    35151 2023-04-17 08:33:09.000000 molgraph-0.3.1/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 15:00:07.160252 molgraph-0.3.1/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-04-17 15:00:07.000000 molgraph-0.3.1/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2966 2023-04-17 15:00:07.000000 molgraph-0.3.1/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 15:00:07.000000 molgraph-0.3.1/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-04-17 15:00:07.000000 molgraph-0.3.1/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-04-17 15:00:07.000000 molgraph-0.3.1/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-17 15:00:07.168252 molgraph-0.3.1/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.1/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.801055 molgraph-0.3.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-25 14:35:09.801055 molgraph-0.3.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2402 2022-09-20 11:35:03.000000 molgraph-0.3.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-25 14:18:24.000000 molgraph-0.3.2/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.2/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.2/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.2/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.2/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.2/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.2/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.2/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3345 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.2/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11266 2022-09-02 16:19:13.000000 molgraph-0.3.2/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9279 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11313 2023-04-18 12:14:45.000000 molgraph-0.3.2/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10527 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14948 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/attentional/gt_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12894 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/layers/base.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.2/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9916 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9754 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10703 2023-05-25 14:29:15.000000 molgraph-0.3.2/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10599 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.2/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.2/molgraph/layers/geometric/_radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9441 2022-09-02 12:17:48.000000 molgraph-0.3.2/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10267 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/layers/geometric/gcf_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.2/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21742 2023-04-17 07:38:04.000000 molgraph-0.3.2/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15618 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/layers/message_passing/mpnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.2/molgraph/layers/ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.2/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.3.2/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.2/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1987 2022-08-18 17:05:36.000000 molgraph-0.3.2/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.2/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.2/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11055 2022-08-31 15:11:51.000000 molgraph-0.3.2/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9439 2022-09-14 10:36:59.000000 molgraph-0.3.2/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11842 2022-08-31 15:11:51.000000 molgraph-0.3.2/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2022-08-18 17:06:18.000000 molgraph-0.3.2/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20437 2022-08-31 15:11:51.000000 molgraph-0.3.2/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.2/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.2/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.2/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.2/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.2/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.2/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.2/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.2/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.2/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.2/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.797055 molgraph-0.3.2/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.2/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.2/molgraph/models/interpretability/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.2/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.2/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.801055 molgraph-0.3.2/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.2/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.2/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.2/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35151 2023-04-21 13:12:30.000000 molgraph-0.3.2/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-25 14:35:09.793055 molgraph-0.3.2/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-25 14:35:09.000000 molgraph-0.3.2/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2966 2023-05-25 14:35:09.000000 molgraph-0.3.2/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-25 14:35:09.000000 molgraph-0.3.2/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-05-25 14:35:09.000000 molgraph-0.3.2/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-05-25 14:35:09.000000 molgraph-0.3.2/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-25 14:35:09.801055 molgraph-0.3.2/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.2/setup.py
```

### Comparing `molgraph-0.3.1/LICENSE` & `molgraph-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/PKG-INFO` & `molgraph-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.1
+Version: 0.3.2
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.1/README.md` & `molgraph-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/_filter_warnings.py` & `molgraph-0.3.2/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/__init__.py` & `molgraph-0.3.2/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.3.2/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.3.2/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.3.2/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.3.2/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/conformer_generator.py` & `molgraph-0.3.2/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/conformer_utils.py` & `molgraph-0.3.2/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/encoders.py` & `molgraph-0.3.2/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/features.py` & `molgraph-0.3.2/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.3.2/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/ops.py` & `molgraph-0.3.2/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/chemistry/vis.py` & `molgraph-0.3.2/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/__init__.py` & `molgraph-0.3.2/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.3.2/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.3.2/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.3.2/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.3.2/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.3.2/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/base.py` & `molgraph-0.3.2/molgraph/layers/base.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.3.2/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.3.2/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.3.2/molgraph/layers/geometric/dtnn_conv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras import initializers
 from tensorflow.keras import regularizers
 from tensorflow.keras import constraints
 from tensorflow.keras import activations
-from tensorflow.keras import layers
+
+import numpy as np
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
+from molgraph.layers.geometric import _radial_basis
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class GINConv(BaseLayer):
+class DTNNConv(BaseLayer):
 
-    '''Graph isomorphism convolution layer (GIN).
+    """Deep Tensor Neural Network (DTNN).
 
-    Implementation based on Dwivedi et al. (2022) [#]_ and Xu et al. (2019) [#]_.
+    Implementation is based on Schütt et al. (2017a) [#]_.
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
+    ...         # edge_feature encodes distances between edge_dst and edge_src
+    ...         'edge_feature': [[0.3, 0.3], [0.1, 0.2, 0.1, 0.4, 0.4, 0.2]],
     ...     }
     ... )
-    >>> # Build a model with GINConv
+    >>> # Build a model with DTNNConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GINConv(16, activation='relu'),
-    ...     molgraph.layers.GINConv(16, activation='relu')
+    ...     molgraph.layers.DTNNConv(16, activation='relu'),
+    ...     molgraph.layers.DTNNConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
@@ -58,43 +61,63 @@
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
+    ...         # edge_feature encodes distances between edge_dst and edge_src
+    ...         'edge_feature': [0.3, 0.3, 0.1, 0.2, 0.1, 0.4, 0.4, 0.2],
     ...     }
     ... )
-    >>> # Build a model with GINConv
+    >>> # Build a model with DTNNConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GINConv(16, activation='relu'),
-    ...     molgraph.layers.GINConv(16, activation='relu')
+    ...     molgraph.layers.DTNNConv(16, activation='relu'),
+    ...     molgraph.layers.DTNNConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
-            Number of output units.
+            The number of output units.
+        distance_min (float):
+            The smallest center (mean) to be used for the radial basis function.
+            I.e., it defines the minimum distance between atom pairs; or the
+            minimum electrostatic interaction between nuclei, in the case of
+            Coulomb values. Default to -1.0.
+        distance_max (float):
+            The largest center (mean) to be used for the radial basis function.
+            I.e., it defines the maximum distance between atom pairs; or the
+            maximum electrostatic interaction between nuclei, in the case of
+            Coulomb values. Default to 18.0.
+        distance_granularity (float):
+            The distance between each center (mean) of the radial basis function.
+            The smaller the granularity, the more centers will be used.
+            Default to 0.1.
+        rbf_stddev (float, str):
+            The standard deviation of the radial basis function. If 'auto',
+            'distance_granularity' will be used as standard deviation.
+            Default to 'auto'.
         self_projection (bool):
             Whether to apply self projection. Default to True.
         batch_norm: (bool):
             Whether to apply batch normalization to the output. Default to True.
         residual: (bool)
             Whether to add skip connection to the output. Default to True.
         dropout: (float, None):
             Dropout applied to the output of the layer. Default to None.
         activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the output of the layer. Default to 'relu'.
+            Activation function applied to the output of the layer. Default to None.
         use_bias (bool):
             Whether the layer should use biases. Default to True.
         kernel_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the kernels. Default to
-            tf.keras.initializers.TruncatedNormal(stddev=0.005).
+            tf.keras.initializers.GlorotUniform().
         bias_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the biases. Default to
             tf.keras.initializers.Constant(0.).
         kernel_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the kernels. Default to None.
         bias_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the biases. Default to None.
@@ -103,31 +126,34 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
-        .. [#] https://arxiv.org/pdf/2003.00982.pdf
-        .. [#] https://arxiv.org/pdf/1810.00826.pdf
+        .. [#] https://www.nature.com/articles/ncomms13890
+    """
 
-    '''
 
     def __init__(
         self,
         units: Optional[int] = None,
+        distance_min: float = -1.0,
+        distance_max: float = 18.0,
+        distance_granularity: float = 0.1,
+        rbf_stddev: Optional[Union[float, str]] = 'auto',
         self_projection: bool = True,
         batch_norm: bool = True,
         residual: bool = True,
         dropout: Optional[float] = None,
-        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
+        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = None,
         use_bias: bool = True,
         kernel_initializer: Union[
             str, initializers.Initializer
-        ] = initializers.TruncatedNormal(stddev=0.005),
+        ] = initializers.GlorotUniform(),
         bias_initializer: Union[
             str, initializers.Initializer
         ] = initializers.Constant(0.),
         kernel_regularizer: Optional[regularizers.Regularizer] = None,
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
@@ -146,65 +172,66 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
-        self.batch_norm = batch_norm
-        self.activation = activations.get('relu')
         self.apply_self_projection = self_projection
+        self.distance_min = distance_min
+        self.distance_max = distance_max
+        self.distance_granularity = distance_granularity
+        self.rbf_stddev = rbf_stddev
+
+        self.rbf = _radial_basis.RadialBasis(
+            self.distance_min,
+            self.distance_max,
+            self.distance_granularity,
+            self.rbf_stddev
+        )
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
-
-        self.projection_1 = self.get_dense(self.units)
-        self.projection_2 = self.get_dense(self.units)
-        self.epsilon = self.add_weight(
-            shape=(),
-            initializer='zeros',
-            regularizer=None,
-            trainable=True,
-            name='epsilon')
-
-        if self.batch_norm:
-            self.batch_norm = layers.BatchNormalization()
-        else:
-            self.batch_norm = None
-
+        self.edge_projection = self.get_dense(self.units)
+        self.node_projection_1 = self.get_dense(self.units)
+        self.node_projection_2 = self.get_dense(self.units)
+        self.node_projection_3 = self.get_dense(self.units)
         if self.apply_self_projection:
-           self.self_projection = self.get_dense(self.units)
+            self.self_projection = self.get_dense(self.units)
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
-        node_feature = propagate_node_features(
-            node_feature=tensor.node_feature,
-            edge_dst=tensor.edge_dst,
-            edge_src=tensor.edge_src)
+        num_segments = tf.shape(tensor.node_feature)[0]
 
-        node_feature = (
-            (1 + self.epsilon) * tensor.node_feature + node_feature)
+        node_feature = self.node_projection_1(tensor.node_feature)
+        node_feature = tf.gather(node_feature, tensor.edge_src)
 
-        node_feature = self.projection_1(node_feature)
+        edge_weight = self.rbf(tensor.edge_feature)
+        edge_weight = self.edge_projection(edge_weight)
 
-        if self.apply_self_projection:
-            node_feature += self.self_projection(tensor.node_feature)
+        node_feature *= edge_weight
+
+        node_feature = self.node_projection_2(node_feature)
 
-        if self.batch_norm is not None:
-            node_feature = self.batch_norm(node_feature)
+        node_feature = tf.nn.tanh(node_feature)
 
-        node_feature = self.activation(node_feature)
+        node_feature = tf.math.unsorted_segment_sum(
+            node_feature, tensor.edge_dst, num_segments)
 
-        node_feature = self.projection_2(node_feature)
+        if self.apply_self_projection:
+            node_feature += self.self_projection(tensor.node_feature)
 
         return tensor.update({'node_feature': node_feature})
 
     def get_config(self):
         base_config = super().get_config()
-        config = {
+        base_config.update({
             'self_projection': self.apply_self_projection,
-        }
-        base_config.update(config)
+            'distance_min': self.distance_min,
+            'distance_max': self.distance_max,
+            'distance_granularity': self.distance_granularity,
+            'rbf_stddev': self.rbf_stddev
+        })
         return base_config
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `molgraph-0.3.1/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.3.2/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/geometric/_radial_basis.py` & `molgraph-0.3.2/molgraph/layers/geometric/_radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.3.2/molgraph/layers/geometric/gcf_conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import propagate_node_features
 from molgraph.layers.geometric import _radial_basis
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class DTNNConv(BaseLayer):
+class GCFConv(BaseLayer):
 
-    """Deep Tensor Neural Network (DTNN).
+    """(Graph) continuous filter convolution layer ((G)CFConv).
 
-    Implementation is based on Schütt et al. (2017a) [#]_.
+    Implementation is based on Schütt et al. (2017b) [#]_.
+
+    Operates on 3D molecular graphs (encoding distance geometry).
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -38,19 +40,19 @@
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...         # edge_feature encodes distances between edge_dst and edge_src
     ...         'edge_feature': [[0.3, 0.3], [0.1, 0.2, 0.1, 0.4, 0.4, 0.2]],
     ...     }
     ... )
-    >>> # Build a model with DTNNConv
+    >>> # Build a model with GCFConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.DTNNConv(16, activation='relu'),
-    ...     molgraph.layers.DTNNConv(16, activation='relu')
+    ...     molgraph.layers.GCFConv(16, activation='relu'),
+    ...     molgraph.layers.GCFConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
@@ -65,19 +67,19 @@
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
     ...         # edge_feature encodes distances between edge_dst and edge_src
     ...         'edge_feature': [0.3, 0.3, 0.1, 0.2, 0.1, 0.4, 0.4, 0.2],
     ...     }
     ... )
-    >>> # Build a model with DTNNConv
+    >>> # Build a model with GCFConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.DTNNConv(16, activation='relu'),
-    ...     molgraph.layers.DTNNConv(16, activation='relu')
+    ...     molgraph.layers.GCFConv(16, activation='relu'),
+    ...     molgraph.layers.GCFConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
             The number of output units.
@@ -126,15 +128,15 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
-        .. [#] https://www.nature.com/articles/ncomms13890
+        .. [#] https://arxiv.org/pdf/1706.08566.pdf
     """
 
 
     def __init__(
         self,
         units: Optional[int] = None,
         distance_min: float = -1.0,
@@ -172,14 +174,15 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
+        self.activation = shifted_softplus
         self.apply_self_projection = self_projection
         self.distance_min = distance_min
         self.distance_max = distance_max
         self.distance_granularity = distance_granularity
         self.rbf_stddev = rbf_stddev
 
         self.rbf = _radial_basis.RadialBasis(
@@ -190,48 +193,69 @@
         )
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
-        self.edge_projection = self.get_dense(self.units)
+
+        self.filter_generator_1 = self.get_dense(self.units, self.activation)
+        self.filter_generator_2 = self.get_dense(self.units, self.activation)
+
         self.node_projection_1 = self.get_dense(self.units)
-        self.node_projection_2 = self.get_dense(self.units)
+        self.node_projection_2 = self.get_dense(self.units, self.activation)
         self.node_projection_3 = self.get_dense(self.units)
+
         if self.apply_self_projection:
             self.self_projection = self.get_dense(self.units)
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
-        num_segments = tf.shape(tensor.node_feature)[0]
+        cosine_weight = cosine_weight_from_distance(tensor.edge_feature),
+        rbf_feature = self.rbf(tensor.edge_feature)
+        rbf_weight = self.filter_generator_2(
+            self.filter_generator_1(rbf_feature))
 
         node_feature = self.node_projection_1(tensor.node_feature)
-        node_feature = tf.gather(node_feature, tensor.edge_src)
-
-        edge_weight = self.rbf(tensor.edge_feature)
-        edge_weight = self.edge_projection(edge_weight)
-
-        node_feature *= edge_weight
 
-        node_feature = self.node_projection_2(node_feature)
+        rbf_weight *= cosine_weight
 
-        node_feature = tf.nn.tanh(node_feature)
-
-        node_feature = tf.math.unsorted_segment_sum(
-            node_feature, tensor.edge_dst, num_segments)
+        node_feature = propagate_node_features(
+            node_feature=node_feature,
+            edge_dst=tensor.edge_dst,
+            edge_src=tensor.edge_src,
+            edge_weight=rbf_weight,
+            mode='mean')
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
+        node_feature = self.node_projection_3(
+            self.node_projection_2(node_feature))
+
         return tensor.update({'node_feature': node_feature})
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({
             'self_projection': self.apply_self_projection,
             'distance_min': self.distance_min,
             'distance_max': self.distance_max,
             'distance_granularity': self.distance_granularity,
             'rbf_stddev': self.rbf_stddev
         })
         return base_config
+
+
+def shifted_softplus(x):
+    return tf.math.log(0.5 * tf.math.exp(x) + 0.5)
+
+def cosine_weight_from_distance(
+    distance: tf.Tensor,
+    distance_cutoff: float = 10.,
+    dtype: tf.DType = tf.float32,
+) -> tf.Tensor:
+    """Passes distances (floating point values) to a cosine function to obtain
+    weights for associated source nodes. Outputted values (also floating point
+    values) are in range [0, 1].
+    """
+    return (0.5 * (tf.math.cos((distance / distance_cutoff) * np.pi) + 1))
```

### Comparing `molgraph-0.3.1/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.3.2/molgraph/layers/convolutional/gin_conv.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras import initializers
 from tensorflow.keras import regularizers
 from tensorflow.keras import constraints
 from tensorflow.keras import activations
-
-import numpy as np
+from tensorflow.keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
+from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
-from molgraph.layers.geometric import _radial_basis
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class GCFConv(BaseLayer):
-
-    """(Graph) continuous filter convolution layer ((G)CFConv).
+class GINConv(BaseLayer):
 
-    Implementation is based on Schütt et al. (2017b) [#]_.
+    '''Graph isomorphism convolution layer (GIN).
 
-    Operates on 3D molecular graphs (encoding distance geometry).
+    Implementation based on Dwivedi et al. (2022) [#]_, Xu et al. (2019) [#]_, 
+    and Hu et al. (2020) [#]_.
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
-    ...         # edge_feature encodes distances between edge_dst and edge_src
-    ...         'edge_feature': [[0.3, 0.3], [0.1, 0.2, 0.1, 0.4, 0.4, 0.2]],
     ...     }
     ... )
-    >>> # Build a model with GCFConv
+    >>> # Build a model with GINConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GCFConv(16, activation='relu'),
-    ...     molgraph.layers.GCFConv(16, activation='relu')
+    ...     molgraph.layers.GINConv(16, activation='relu'),
+    ...     molgraph.layers.GINConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
@@ -63,63 +59,85 @@
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
-    ...         # edge_feature encodes distances between edge_dst and edge_src
-    ...         'edge_feature': [0.3, 0.3, 0.1, 0.2, 0.1, 0.4, 0.4, 0.2],
     ...     }
     ... )
-    >>> # Build a model with GCFConv
+    >>> # Build a model with GINConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GCFConv(16, activation='relu'),
-    ...     molgraph.layers.GCFConv(16, activation='relu')
+    ...     molgraph.layers.GINConv(16, activation='relu'),
+    ...     molgraph.layers.GINConv(16, activation='relu')
+    ... ])
+    >>> gnn_model.output_shape
+    (None, 16)
+
+    With edge features ("GINEConv"):
+
+    >>> graph_tensor = molgraph.GraphTensor(
+    ...     data={
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
+    ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'node_feature': [
+    ...             [1.0, 0.0],
+    ...             [1.0, 0.0],
+    ...             [1.0, 0.0],
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0]
+    ...         ],
+    ...         'graph_indicator': [0, 0, 1, 1, 1],
+    ...         'edge_feature': [
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0],
+    ...             [0.0, 1.0],
+    ...             [0.0, 1.0],
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0],
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0]
+    ...         ],
+    ...     }
+    ... )
+    >>> # Build a model with GINConv
+    >>> gnn_model = tf.keras.Sequential([
+    ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
+    ...     molgraph.layers.GINConv(
+    ...         16, activation='relu', use_edge_features=True), # need to be explicit
+    ...     molgraph.layers.GINConv(
+    ...         16, activation='relu', use_edge_features=True)  # need to be explicit
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
-            The number of output units.
-        distance_min (float):
-            The smallest center (mean) to be used for the radial basis function.
-            I.e., it defines the minimum distance between atom pairs; or the
-            minimum electrostatic interaction between nuclei, in the case of
-            Coulomb values. Default to -1.0.
-        distance_max (float):
-            The largest center (mean) to be used for the radial basis function.
-            I.e., it defines the maximum distance between atom pairs; or the
-            maximum electrostatic interaction between nuclei, in the case of
-            Coulomb values. Default to 18.0.
-        distance_granularity (float):
-            The distance between each center (mean) of the radial basis function.
-            The smaller the granularity, the more centers will be used.
-            Default to 0.1.
-        rbf_stddev (float, str):
-            The standard deviation of the radial basis function. If 'auto',
-            'distance_granularity' will be used as standard deviation.
-            Default to 'auto'.
+            Number of output units.
+        use_edge_features (bool):
+            Whether or not to use edge features. Default to False.
+        apply_relu_activation (bool):
+            Whether to apply relu activation before aggregation step. Only relevant
+            if use_edge_features is set to True. Default to False.
         self_projection (bool):
             Whether to apply self projection. Default to True.
         batch_norm: (bool):
             Whether to apply batch normalization to the output. Default to True.
         residual: (bool)
             Whether to add skip connection to the output. Default to True.
         dropout: (float, None):
             Dropout applied to the output of the layer. Default to None.
         activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the output of the layer. Default to None.
+            Activation function applied to the output of the layer. Default to 'relu'.
         use_bias (bool):
             Whether the layer should use biases. Default to True.
         kernel_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the kernels. Default to
-            tf.keras.initializers.GlorotUniform().
+            tf.keras.initializers.TruncatedNormal(stddev=0.005).
         bias_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the biases. Default to
             tf.keras.initializers.Constant(0.).
         kernel_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the kernels. Default to None.
         bias_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the biases. Default to None.
@@ -128,34 +146,33 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
-        .. [#] https://arxiv.org/pdf/1706.08566.pdf
-    """
-
+        .. [#] https://arxiv.org/pdf/2003.00982.pdf
+        .. [#] https://arxiv.org/pdf/1810.00826.pdf
+        .. [#] https://arxiv.org/pdf/1905.12265.pdf
+    '''
 
     def __init__(
         self,
         units: Optional[int] = None,
-        distance_min: float = -1.0,
-        distance_max: float = 18.0,
-        distance_granularity: float = 0.1,
-        rbf_stddev: Optional[Union[float, str]] = 'auto',
+        use_edge_features: bool = False,
+        apply_relu_activation: bool = False,
         self_projection: bool = True,
         batch_norm: bool = True,
         residual: bool = True,
         dropout: Optional[float] = None,
-        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = None,
+        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
         use_bias: bool = True,
         kernel_initializer: Union[
             str, initializers.Initializer
-        ] = initializers.GlorotUniform(),
+        ] = initializers.TruncatedNormal(stddev=0.005),
         bias_initializer: Union[
             str, initializers.Initializer
         ] = initializers.Constant(0.),
         kernel_regularizer: Optional[regularizers.Regularizer] = None,
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
@@ -174,88 +191,89 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
-        self.activation = shifted_softplus
+        self.batch_norm = batch_norm
+        self.activation = activations.get('relu')
         self.apply_self_projection = self_projection
-        self.distance_min = distance_min
-        self.distance_max = distance_max
-        self.distance_granularity = distance_granularity
-        self.rbf_stddev = rbf_stddev
-
-        self.rbf = _radial_basis.RadialBasis(
-            self.distance_min,
-            self.distance_max,
-            self.distance_granularity,
-            self.rbf_stddev
-        )
+        self.use_edge_features = use_edge_features
+        self.apply_relu_activation = apply_relu_activation
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
 
-        self.filter_generator_1 = self.get_dense(self.units, self.activation)
-        self.filter_generator_2 = self.get_dense(self.units, self.activation)
+        if edge_feature_shape is None:
+            self.use_edge_features = False
 
-        self.node_projection_1 = self.get_dense(self.units)
-        self.node_projection_2 = self.get_dense(self.units, self.activation)
-        self.node_projection_3 = self.get_dense(self.units)
+        self.projection_1 = self.get_dense(self.units)
+        self.projection_2 = self.get_dense(self.units)
+        self.epsilon = self.add_weight(
+            shape=(),
+            initializer='zeros',
+            regularizer=None,
+            trainable=True,
+            name='epsilon')
+
+        node_dim = node_feature_shape[-1]
+        if self.use_edge_features:
+            edge_dim = edge_feature_shape[-1]
+            if edge_dim != node_dim:
+                self.edge_projection = self.get_dense(node_dim)
+
+        if self.batch_norm:
+            self.batch_norm = layers.BatchNormalization()
+        else:
+            self.batch_norm = None
 
         if self.apply_self_projection:
-            self.self_projection = self.get_dense(self.units)
+           self.self_projection = self.get_dense(self.units)
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
-        cosine_weight = cosine_weight_from_distance(tensor.edge_feature),
-        rbf_feature = self.rbf(tensor.edge_feature)
-        rbf_weight = self.filter_generator_2(
-            self.filter_generator_1(rbf_feature))
-
-        node_feature = self.node_projection_1(tensor.node_feature)
-
-        rbf_weight *= cosine_weight
-
-        node_feature = propagate_node_features(
-            node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
-            edge_src=tensor.edge_src,
-            edge_weight=rbf_weight,
-            mode='mean')
+        if not self.use_edge_features:
+            node_feature_aggregated = propagate_node_features(
+                node_feature=tensor.node_feature,
+                edge_dst=tensor.edge_dst,
+                edge_src=tensor.edge_src)
+        else:
+            node_feature_src = tf.gather(tensor.node_feature, tensor.edge_src)
+            if hasattr(self, 'edge_projection'):
+                edge_feature_updated = self.edge_projection(tensor.edge_feature)
+                tensor = tensor.update({'edge_feature': edge_feature_updated})
+            node_feature_src += tensor.edge_feature
+            if self.apply_relu_activation:
+                node_feature_src = tf.nn.relu(node_feature_src)
+            node_feature_aggregated = tf.math.unsorted_segment_sum(
+                node_feature_src, tensor.edge_dst, tf.shape(tensor.node_feature)[0])
+            
+        node_feature = (
+            (1 + self.epsilon) * tensor.node_feature + node_feature_aggregated)
+
+        node_feature = self.projection_1(node_feature)
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
-        node_feature = self.node_projection_3(
-            self.node_projection_2(node_feature))
+        if self.batch_norm is not None:
+            node_feature = self.batch_norm(node_feature)
+
+        node_feature = self.activation(node_feature)
+
+        node_feature = self.projection_2(node_feature)
 
         return tensor.update({'node_feature': node_feature})
 
     def get_config(self):
         base_config = super().get_config()
-        base_config.update({
+        config = {
             'self_projection': self.apply_self_projection,
-            'distance_min': self.distance_min,
-            'distance_max': self.distance_max,
-            'distance_granularity': self.distance_granularity,
-            'rbf_stddev': self.rbf_stddev
-        })
+            'use_edge_features': self.use_edge_features,
+            'apply_relu_activation': self.apply_relu_activation
+        }
+        base_config.update(config)
         return base_config
-
-
-def shifted_softplus(x):
-    return tf.math.log(0.5 * tf.math.exp(x) + 0.5)
-
-def cosine_weight_from_distance(
-    distance: tf.Tensor,
-    distance_cutoff: float = 10.,
-    dtype: tf.DType = tf.float32,
-) -> tf.Tensor:
-    """Passes distances (floating point values) to a cosine function to obtain
-    weights for associated source nodes. Outputted values (also floating point
-    values) are in range [0, 1].
-    """
-    return (0.5 * (tf.math.cos((distance / distance_cutoff) * np.pi) + 1))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `molgraph-0.3.1/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.3.2/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.3.2/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/ops.py` & `molgraph-0.3.2/molgraph/layers/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.3.2/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.3.2/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.3.2/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.3.2/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.3.2/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.3.2/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.3.2/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/preprocessing/projection.py` & `molgraph-0.3.2/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.3.2/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/readout/node_readout.py` & `molgraph-0.3.2/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/readout/segment_pool.py` & `molgraph-0.3.2/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/readout/set_gather.py` & `molgraph-0.3.2/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.3.2/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/losses/link_losses.py` & `molgraph-0.3.2/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/losses/masked_losses.py` & `molgraph-0.3.2/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/metrics/masked_metrics.py` & `molgraph-0.3.2/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/metrics/mean_relative_error.py` & `molgraph-0.3.2/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/models/dgin.py` & `molgraph-0.3.2/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/models/dmpnn.py` & `molgraph-0.3.2/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.3.2/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/models/interpretability/saliency.py` & `molgraph-0.3.2/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/models/mpnn.py` & `molgraph-0.3.2/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/tensors/_graph_tensor.py` & `molgraph-0.3.2/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.3.2/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph/tensors/graph_tensor.py` & `molgraph-0.3.2/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/molgraph.egg-info/PKG-INFO` & `molgraph-0.3.2/molgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.1
+Version: 0.3.2
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.1/molgraph.egg-info/SOURCES.txt` & `molgraph-0.3.2/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.1/setup.py` & `molgraph-0.3.2/setup.py`

 * *Files identical despite different names*

