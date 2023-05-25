# Comparing `tmp/ddsp-3.6.0.tar.gz` & `tmp/ddsp-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddsp-3.6.0.tar", last modified: Fri Apr 28 01:27:41 2023, max compression
+gzip compressed data, was "ddsp-3.7.0.tar", last modified: Thu May 25 02:28:12 2023, max compression
```

## Comparing `ddsp-3.6.0.tar` & `ddsp-3.7.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)       63 2023-04-28 01:27:41.000000 ddsp-3.6.0/setup.cfg
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13253 2023-04-28 01:27:39.000000 ddsp-3.6.0/README.md
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-28 01:27:41.000000 ddsp-3.6.0/PKG-INFO
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3240 2023-04-28 01:27:39.000000 ddsp-3.6.0/setup.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3873 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/effects_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11482 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/synths.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/colab/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/colab/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10035 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/colab/colab_utils.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1139 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/test_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      908 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3753 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/processors_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    63698 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/core.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19427 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/spectral_ops.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      794 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/version.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9610 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/processors.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11158 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/spectral_ops_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13484 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/effects.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3189 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/losses_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10127 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/heuristics.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/models/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11984 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/inverse_synthesis.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2482 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/autoencoder.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1594 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2834 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/autoencoder_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4715 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/model.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    23617 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/midi_autoencoder.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9529 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/metrics_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9122 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/eval_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9400 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/decoders.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8503 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/preprocessing.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    21779 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19583 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/inference.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8753 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/nn_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7919 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/plotting.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2292 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/preprocessing_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1182 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8700 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/ddsp_run.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19956 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/metrics.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     6810 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/trainers.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    15113 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/encoders.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    16563 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/summaries.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8307 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/evaluators.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/models/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/vst_32k.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/vst_48k.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2453 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/vst.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1854 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1049 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/solo_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/__init__.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/optimization/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      416 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/optimization/base.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/optimization/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      116 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/optimization/base_tpu.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/datasets/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      224 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/base.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      351 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/tfrecord.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      475 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/nsynth.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/eval/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      176 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/heuristic_power.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      170 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/heuristic.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      158 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/basic_f0_ld_twm.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      150 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/midi_ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      138 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/basic_f0_ld.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      119 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/basic.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/papers/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      217 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/tiny_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      221 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/nsynth_ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      267 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/solo_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/__init__.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1881 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      730 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      472 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/finetune_model.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      679 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    12720 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/ddsp_export.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2885 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/cloud.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13804 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/postprocessing.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11770 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/train_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4177 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/decoders_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    49484 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/nn.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3010 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/heuristics_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/docker/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3441 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/task_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      640 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9500 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/ddsp_ai_platform.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     5036 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/task.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/data_preparation/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4406 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10303 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      692 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3852 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10070 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/synthetic_data.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7832 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2970 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/cloud_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    36651 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/core_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    40636 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/losses.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3744 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/dags_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7416 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/dags.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3736 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/synths_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      427 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/requires.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3282 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/SOURCES.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/PKG-INFO
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      424 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/entry_points.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)        1 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/dependency_links.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)        5 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/top_level.txt
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11384 2023-05-25 02:28:11.000000 ddsp-3.7.0/LICENSE
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      641 2023-05-25 02:28:12.599936 ddsp-3.7.0/PKG-INFO
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13253 2023-05-25 02:28:11.000000 ddsp-3.7.0/README.md
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.591935 ddsp-3.7.0/ddsp/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      908 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.591935 ddsp-3.7.0/ddsp/colab/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/colab/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10035 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/colab/colab_utils.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    63698 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/core.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    36651 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/core_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7416 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/dags.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3744 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/dags_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13484 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/effects.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3873 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/effects_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    40636 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/losses.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3189 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/losses_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9610 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/processors.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3753 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/processors_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19427 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/spectral_ops.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11158 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/spectral_ops_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11482 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/synths.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3736 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/synths_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1139 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/test_util.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.595936 ddsp-3.7.0/ddsp/training/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1182 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2885 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/cloud.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2970 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/cloud_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    21779 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.595936 ddsp-3.7.0/ddsp/training/data_preparation/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      692 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data_preparation/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4406 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3852 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10303 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7832 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10070 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/data_preparation/synthetic_data.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    12720 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/ddsp_export.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8700 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/ddsp_run.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9400 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/decoders.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4177 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/decoders_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.595936 ddsp-3.7.0/ddsp/training/docker/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      640 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/docker/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9500 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/docker/ddsp_ai_platform.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     5036 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/docker/task.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3441 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/docker/task_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    15113 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/encoders.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9122 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/eval_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8307 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/evaluators.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.595936 ddsp-3.7.0/ddsp/training/gin/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.595936 ddsp-3.7.0/ddsp/training/gin/datasets/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/datasets/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      224 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/datasets/base.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      475 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/datasets/nsynth.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      351 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/datasets/tfrecord.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/eval/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      119 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/basic.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      138 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/basic_f0_ld.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      158 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/basic_f0_ld_twm.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      170 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/heuristic.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      176 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/heuristic_power.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      150 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/eval/midi_ae.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/models/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1854 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1049 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/solo_instrument.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/models/vst/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/vst/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2453 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/vst/vst.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/vst/vst_32k.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/models/vst/vst_48k.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/optimization/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/optimization/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      416 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/optimization/base.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      116 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/optimization/base_tpu.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/papers/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/papers/iclr2020/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/iclr2020/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      221 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/iclr2020/nsynth_ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      267 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/iclr2020/solo_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      217 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/iclr2020/tiny_instrument.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/gin/papers/icml2020/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/icml2020/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      730 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      472 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/icml2020/finetune_model.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      679 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1881 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10127 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/heuristics.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3010 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/heuristics_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19583 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/inference.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    20031 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/metrics.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9529 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/metrics_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.599936 ddsp-3.7.0/ddsp/training/models/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1594 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/models/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2482 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/models/autoencoder.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2834 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/models/autoencoder_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11984 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/models/inverse_synthesis.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    23617 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/models/midi_autoencoder.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4715 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/models/model.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    49484 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/nn.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8753 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/nn_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7919 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/plotting.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13804 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/postprocessing.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8503 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/preprocessing.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2292 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/preprocessing_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    16563 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/summaries.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11770 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/train_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     6810 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/training/trainers.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      794 2023-05-25 02:28:11.000000 ddsp-3.7.0/ddsp/version.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-05-25 02:28:12.591935 ddsp-3.7.0/ddsp.egg-info/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      641 2023-05-25 02:28:12.000000 ddsp-3.7.0/ddsp.egg-info/PKG-INFO
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3290 2023-05-25 02:28:12.000000 ddsp-3.7.0/ddsp.egg-info/SOURCES.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)        1 2023-05-25 02:28:12.000000 ddsp-3.7.0/ddsp.egg-info/dependency_links.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      423 2023-05-25 02:28:12.000000 ddsp-3.7.0/ddsp.egg-info/entry_points.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      488 2023-05-25 02:28:12.000000 ddsp-3.7.0/ddsp.egg-info/requires.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)        5 2023-05-25 02:28:12.000000 ddsp-3.7.0/ddsp.egg-info/top_level.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)       63 2023-05-25 02:28:12.599936 ddsp-3.7.0/setup.cfg
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3301 2023-05-25 02:28:11.000000 ddsp-3.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ddsp-3.6.0/README.md` & `ddsp-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/PKG-INFO` & `ddsp-3.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ddsp
-Version: 3.6.0
+Version: 3.7.0
 Summary: Differentiable Digital Signal Processing 
 Home-page: http://github.com/magenta/ddsp
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
-Description: UNKNOWN
 Keywords: audio dsp signalprocessing machinelearning music
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: gcp
 Provides-Extra: data_preparation
 Provides-Extra: test
-Provides-Extra: gcp
+License-File: LICENSE
```

### Comparing `ddsp-3.6.0/setup.py` & `ddsp-3.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,34 +34,34 @@
     packages=setuptools.find_packages(),
     package_data={
         '': ['*.gin'],
     },
     scripts=[],
     install_requires=[
         'absl-py',
-        'cloudml-hypertune',
+        'cloudml-hypertune<=0.1.0.dev6',
         'crepe<=0.0.12',
         'dill<=0.3.4',
         'future',
         'gin-config>=0.3.0',
         'google-cloud-storage',
         'hmmlearn<=0.2.7',
-        'librosa',
-        'pydub',
+        'librosa<=0.10',
+        'pydub<=0.25.1',
         'protobuf<=3.20',  # temporary fix for proto dependency bug
-        'mir_eval',
+        'mir_eval<=0.7',
         'note_seq<0.0.4',
         'numpy<1.24',
-        'scipy',
+        'scipy<=1.10.1',
         'six',
-        'tensorflow',
+        'tensorflow<=2.11',
         'tensorflowjs<3.19',
-        'tensorflow-probability',
-        'tensorflow-datasets',
-        'tflite_support'
+        'tensorflow-probability<=0.19',
+        'tensorflow-datasets<=4.9',
+        'tflite_support<=0.1'
     ],
     extras_require={
         'gcp': [
             'gevent', 'google-api-python-client', 'google-compute-engine',
             'oauth2client'
         ],
         'data_preparation': [
```

### Comparing `ddsp-3.6.0/ddsp/effects_test.py` & `ddsp-3.7.0/ddsp/effects_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/synths.py` & `ddsp-3.7.0/ddsp/synths.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/colab/__init__.py` & `ddsp-3.7.0/ddsp/colab/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/colab/colab_utils.py` & `ddsp-3.7.0/ddsp/colab/colab_utils.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/test_util.py` & `ddsp-3.7.0/ddsp/test_util.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/__init__.py` & `ddsp-3.7.0/ddsp/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/processors_test.py` & `ddsp-3.7.0/ddsp/processors_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/core.py` & `ddsp-3.7.0/ddsp/core.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/spectral_ops.py` & `ddsp-3.7.0/ddsp/spectral_ops.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/version.py` & `ddsp-3.7.0/ddsp/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 r"""Separate file for storing the current version of DDSP.
 
 Stored in a separate file so that setup.py can reference the version without
 pulling in all the dependencies in __init__.py.
 """
 
-__version__ = '3.6.0'
+__version__ = '3.7.0'
```

### Comparing `ddsp-3.6.0/ddsp/processors.py` & `ddsp-3.7.0/ddsp/processors.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/spectral_ops_test.py` & `ddsp-3.7.0/ddsp/spectral_ops_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/effects.py` & `ddsp-3.7.0/ddsp/effects.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/losses_test.py` & `ddsp-3.7.0/ddsp/losses_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/heuristics.py` & `ddsp-3.7.0/ddsp/training/heuristics.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/models/inverse_synthesis.py` & `ddsp-3.7.0/ddsp/training/models/inverse_synthesis.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/models/autoencoder.py` & `ddsp-3.7.0/ddsp/training/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/models/__init__.py` & `ddsp-3.7.0/ddsp/training/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/models/autoencoder_test.py` & `ddsp-3.7.0/ddsp/training/models/autoencoder_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/models/model.py` & `ddsp-3.7.0/ddsp/training/models/model.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/models/midi_autoencoder.py` & `ddsp-3.7.0/ddsp/training/models/midi_autoencoder.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/metrics_test.py` & `ddsp-3.7.0/ddsp/training/metrics_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/eval_util.py` & `ddsp-3.7.0/ddsp/training/eval_util.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/decoders.py` & `ddsp-3.7.0/ddsp/training/decoders.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/preprocessing.py` & `ddsp-3.7.0/ddsp/training/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data.py` & `ddsp-3.7.0/ddsp/training/data.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/inference.py` & `ddsp-3.7.0/ddsp/training/inference.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/nn_test.py` & `ddsp-3.7.0/ddsp/training/nn_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/plotting.py` & `ddsp-3.7.0/ddsp/training/plotting.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/preprocessing_test.py` & `ddsp-3.7.0/ddsp/training/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/__init__.py` & `ddsp-3.7.0/ddsp/training/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/ddsp_run.py` & `ddsp-3.7.0/ddsp/training/ddsp_run.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/metrics.py` & `ddsp-3.7.0/ddsp/training/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 import numpy as np
 import tensorflow.compat.v2 as tf
 
 # Global values for evaluation.
 MIN_F0_CONFIDENCE = 0.85
 OUTLIER_MIDI_THRESH = 12
 
+# pytype: disable=signature-mismatch  # overriding-parameter-count-checks
+
 
 # ---------------------- Helper Functions --------------------------------------
 def squeeze(input_vector):
   """Ensure vector only has one axis of dimensionality."""
   if input_vector.ndim > 1:
     return np.squeeze(input_vector)
   else:
```

### Comparing `ddsp-3.6.0/ddsp/training/trainers.py` & `ddsp-3.7.0/ddsp/training/trainers.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/encoders.py` & `ddsp-3.7.0/ddsp/training/encoders.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/summaries.py` & `ddsp-3.7.0/ddsp/training/summaries.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/evaluators.py` & `ddsp-3.7.0/ddsp/training/evaluators.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/vst/vst_32k.gin` & `ddsp-3.7.0/ddsp/training/gin/models/vst/vst_32k.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/vst/vst_48k.gin` & `ddsp-3.7.0/ddsp/training/gin/models/vst/vst_48k.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/vst/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/vst/vst.gin` & `ddsp-3.7.0/ddsp/training/gin/models/vst/vst.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/ae.gin` & `ddsp-3.7.0/ddsp/training/gin/models/ae.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/models/solo_instrument.gin` & `ddsp-3.7.0/ddsp/training/gin/models/solo_instrument.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/optimization/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/datasets/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/models/vst/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/eval/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/papers/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/papers/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/papers/iclr2020/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin` & `ddsp-3.7.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/__init__.py` & `ddsp-3.7.0/ddsp/training/gin/papers/icml2020/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin` & `ddsp-3.7.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin` & `ddsp-3.7.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/ddsp_export.py` & `ddsp-3.7.0/ddsp/training/ddsp_export.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/cloud.py` & `ddsp-3.7.0/ddsp/training/cloud.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/postprocessing.py` & `ddsp-3.7.0/ddsp/training/postprocessing.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/train_util.py` & `ddsp-3.7.0/ddsp/training/train_util.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/decoders_test.py` & `ddsp-3.7.0/ddsp/training/decoders_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/nn.py` & `ddsp-3.7.0/ddsp/training/nn.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/heuristics_test.py` & `ddsp-3.7.0/ddsp/training/heuristics_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/docker/task_test.py` & `ddsp-3.7.0/ddsp/training/docker/task_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/docker/__init__.py` & `ddsp-3.7.0/ddsp/training/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/docker/ddsp_ai_platform.py` & `ddsp-3.7.0/ddsp/training/docker/ddsp_ai_platform.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/docker/task.py` & `ddsp-3.7.0/ddsp/training/docker/task.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py` & `ddsp-3.7.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py` & `ddsp-3.7.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data_preparation/__init__.py` & `ddsp-3.7.0/ddsp/training/data_preparation/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py` & `ddsp-3.7.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data_preparation/synthetic_data.py` & `ddsp-3.7.0/ddsp/training/data_preparation/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py` & `ddsp-3.7.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/training/cloud_test.py` & `ddsp-3.7.0/ddsp/training/cloud_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/core_test.py` & `ddsp-3.7.0/ddsp/core_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/losses.py` & `ddsp-3.7.0/ddsp/losses.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/dags_test.py` & `ddsp-3.7.0/ddsp/dags_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/dags.py` & `ddsp-3.7.0/ddsp/dags.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp/synths_test.py` & `ddsp-3.7.0/ddsp/synths_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.6.0/ddsp.egg-info/SOURCES.txt` & `ddsp-3.7.0/ddsp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 ddsp/__init__.py
 ddsp/core.py
 ddsp/core_test.py
 ddsp/dags.py
```

### Comparing `ddsp-3.6.0/ddsp.egg-info/PKG-INFO` & `ddsp-3.7.0/ddsp.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ddsp
-Version: 3.6.0
+Version: 3.7.0
 Summary: Differentiable Digital Signal Processing 
 Home-page: http://github.com/magenta/ddsp
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
-Description: UNKNOWN
 Keywords: audio dsp signalprocessing machinelearning music
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: gcp
 Provides-Extra: data_preparation
 Provides-Extra: test
-Provides-Extra: gcp
+License-File: LICENSE
```

