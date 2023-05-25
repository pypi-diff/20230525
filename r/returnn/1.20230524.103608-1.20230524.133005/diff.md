# Comparing `tmp/returnn-1.20230524.103608.tar.gz` & `tmp/returnn-1.20230524.133005.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230524.103608.tar", last modified: Wed May 24 09:00:57 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230524.133005.tar", last modified: Wed May 24 12:00:47 2023, max compression
```

## Comparing `returnn-1.20230524.103608.tar` & `returnn-1.20230524.133005.tar`

### file list

```diff
@@ -1,445 +1,445 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 09:00:36.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-24 09:00:39.000000 returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157391 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151443 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   585937 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24344 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72175 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:00:57.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-24 09:00:34.000000 returnn-1.20230524.103608/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 12:00:25.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-24 12:00:29.000000 returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157391 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151443 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   585937 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24344 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72175 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:47.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-24 12:00:23.000000 returnn-1.20230524.133005/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230524.103608/.gitignore` & `returnn-1.20230524.133005/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/.gitmodules` & `returnn-1.20230524.133005/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/CHANGELOG.md` & `returnn-1.20230524.133005/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/CODEOWNERS` & `returnn-1.20230524.133005/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/CONTRIBUTING.md` & `returnn-1.20230524.133005/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/LICENSE` & `returnn-1.20230524.133005/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/MANIFEST.in` & `returnn-1.20230524.133005/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/PKG-INFO` & `returnn-1.20230524.133005/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230524.103608
+Version: 1.20230524.133005
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230524.103608/README.rst` & `returnn-1.20230524.133005/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/__init__.py` & `returnn-1.20230524.133005/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/12AX.cluster_map` & `returnn-1.20230524.133005/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-fwd.config` & `returnn-1.20230524.133005/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-horovod-mpi.py` & `returnn-1.20230524.133005/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230524.133005/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-hyper-param-tuning.config` & `returnn-1.20230524.133005/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-iter-dataset.py` & `returnn-1.20230524.133005/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-list-devices.py` & `returnn-1.20230524.133005/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-lua-torch-layer.config` & `returnn-1.20230524.133005/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230524.133005/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-returnn-as-framework.py` & `returnn-1.20230524.133005/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-rf.config` & `returnn-1.20230524.133005/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-rhn-enwik8.config` & `returnn-1.20230524.133005/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-sprint-interface.py` & `returnn-1.20230524.133005/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-att-copy.config` & `returnn-1.20230524.133005/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-attention.config` & `returnn-1.20230524.133005/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-enc-dec.config` & `returnn-1.20230524.133005/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230524.133005/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230524.133005/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230524.133005/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230524.133005/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230524.133005/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-rec-self-att.config` & `returnn-1.20230524.133005/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230524.133005/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230524.133005/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230524.133005/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-torch.config` & `returnn-1.20230524.133005/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230524.133005/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/demo.sh` & `returnn-1.20230524.133005/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230524.133005/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/README.txt` & `returnn-1.20230524.133005/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/config_demo` & `returnn-1.20230524.133005/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230524.133005/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/config_real` & `returnn-1.20230524.133005/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230524.133005/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/decode.py` & `returnn-1.20230524.133005/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230524.133005/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230524.133005/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230524.133005/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230524.133005/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230524.133005/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230524.133005/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230524.133005/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230524.133005/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/__init__.py` & `returnn-1.20230524.133005/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/__main__.py` & `returnn-1.20230524.133005/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/__old_mod_loader__.py` & `returnn-1.20230524.133005/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/__setup__.py` & `returnn-1.20230524.133005/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/config.py` & `returnn-1.20230524.133005/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/audio.py` & `returnn-1.20230524.133005/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/basic.py` & `returnn-1.20230524.133005/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/bundle_file.py` & `returnn-1.20230524.133005/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/cached.py` & `returnn-1.20230524.133005/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/cached2.py` & `returnn-1.20230524.133005/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/generating.py` & `returnn-1.20230524.133005/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/hdf.py` & `returnn-1.20230524.133005/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/lm.py` & `returnn-1.20230524.133005/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/map.py` & `returnn-1.20230524.133005/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/meta.py` & `returnn-1.20230524.133005/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/multi_proc.py` & `returnn-1.20230524.133005/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/normalization_data.py` & `returnn-1.20230524.133005/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/numpy_dump.py` & `returnn-1.20230524.133005/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/raw_wav.py` & `returnn-1.20230524.133005/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/sprint.py` & `returnn-1.20230524.133005/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/stereo.py` & `returnn-1.20230524.133005/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230524.133005/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/datasets/util/vocabulary.py` & `returnn-1.20230524.133005/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/engine/base.py` & `returnn-1.20230524.133005/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/engine/batch.py` & `returnn-1.20230524.133005/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230524.133005/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/edit.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/select.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/transform.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/extern/graph_editor/util.py` & `returnn-1.20230524.133005/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/__init__.py` & `returnn-1.20230524.133005/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/_backend.py` & `returnn-1.20230524.133005/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/_numpy_backend.py` & `returnn-1.20230524.133005/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/_utils.py` & `returnn-1.20230524.133005/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/array_.py` & `returnn-1.20230524.133005/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/attention.py` & `returnn-1.20230524.133005/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/cond.py` & `returnn-1.20230524.133005/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/const.py` & `returnn-1.20230524.133005/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/container.py` & `returnn-1.20230524.133005/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/conv.py` & `returnn-1.20230524.133005/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/device.py` & `returnn-1.20230524.133005/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/dims.py` & `returnn-1.20230524.133005/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/dropout.py` & `returnn-1.20230524.133005/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/dtype.py` & `returnn-1.20230524.133005/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/encoder/base.py` & `returnn-1.20230524.133005/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/encoder/conformer.py` & `returnn-1.20230524.133005/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/init.py` & `returnn-1.20230524.133005/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/linear.py` & `returnn-1.20230524.133005/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/loop.py` & `returnn-1.20230524.133005/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/loss.py` & `returnn-1.20230524.133005/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/math_.py` & `returnn-1.20230524.133005/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/matmul.py` & `returnn-1.20230524.133005/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/module.py` & `returnn-1.20230524.133005/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/normalization.py` & `returnn-1.20230524.133005/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/parameter.py` & `returnn-1.20230524.133005/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/rand.py` & `returnn-1.20230524.133005/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/rec.py` & `returnn-1.20230524.133005/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/reduce.py` & `returnn-1.20230524.133005/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/run_ctx.py` & `returnn-1.20230524.133005/returnn/frontend/run_ctx.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 We can either be in param-init stage,
 or in the main training loop,
 or forwarding loop.
 """
 
 from __future__ import annotations
-from typing import Optional, Union, Any, Sequence, Dict, List
+from typing import Optional, Union, Any, Sequence, Dict
 from dataclasses import dataclass
 from returnn.tensor import Tensor, Dim, TensorDict
 import returnn.frontend as rf
 from . import _backend
 
 
 __all__ = ["RunCtx", "Loss", "get_run_ctx", "init_train_step_run_ctx", "init_forward_step_run_ctx"]
@@ -33,15 +33,15 @@
     """
     Call this at the beginning of a new train step.
     """
     global _run_ctx
     _run_ctx = RunCtx(stage="train_step", train_flag=train_flag)
 
 
-def init_forward_step_run_ctx(expected_outputs: Optional[List[str]] = None):
+def init_forward_step_run_ctx(expected_outputs: Optional[TensorDict] = None):
     """
     Call this at the beginning of a new forward step.
     """
     global _run_ctx
     _run_ctx = RunCtx(stage="forward_step", expected_outputs=expected_outputs)
 
 
@@ -64,15 +64,15 @@
     or forwarding loop (doing recog, beam search, dumping whatever, ...).
 
     In training/eval, we expect that some loss is being defined via mark_as_loss().
     In forwarding, we expect that some output is being defined via mark_as_output().
     """
 
     def __init__(
-        self, *, stage: str, train_flag: Union[bool, Tensor] = False, expected_outputs: Optional[List[str]] = None
+        self, *, stage: str, train_flag: Union[bool, Tensor] = False, expected_outputs: Optional[TensorDict] = None
     ):
         """
         :param stage:
             - "init"
             - "train_step", also for eval, for mark_as_loss and get_total_loss
             - "forward_step", for mark_as_output
         """
@@ -176,48 +176,79 @@
         :param tensor:
         :param name:
         :param dims: this specifies the order of the dims of the output, such that it is well-defined
             for some external application.
             If not specified, we try to infer BTF or BF as default, if that works, otherwise it will be an error.
         """
         assert self.stage == "forward_step"
+
+        if self.expected_outputs is not None:
+            assert (
+                name in self.expected_outputs.data
+            ), f"mark_as_output: unexpected output {name!r}, we expect outputs: {self.expected_outputs}"
+        expected_output = self.expected_outputs.data[name] if self.expected_outputs else None
+        if dims is None and expected_output:
+            dims = expected_output.dims
+        if dims is not None and expected_output:
+            assert (
+                expected_output.dims == dims
+            ), f"mark_as_output: {name!r} dims mismatch from expected output, given {dims}, expected {expected_output}"
+
         if not isinstance(tensor, Tensor):
             assert isinstance(tensor, _backend.global_backend.RawTensorType)
             tensor = rf.convert_to_tensor(tensor, dims=dims)
             # In case it was not specified, just accept whatever order we got.
             dims = tensor.dims
-        assert name not in self.outputs.data
+
         if dims is None:
             # We try some reasonable defaults, specifically: BTF or BF.
             dims = _default_dim_order(tensor)
         assert set(dims) == set(tensor.dims), f"mark_as_output: tensor {tensor} does not have the dims {dims}"
         tensor = tensor.copy_transpose(dims, allow_int=False)
         tensor = tensor.copy(name=name)
+        assert name not in self.outputs.data
         self.outputs.data[name] = tensor
 
-        # Sanity check: expected outputs should coincide with raw keys of output, including output sizes.
-        if self.expected_outputs is not None:
-            raw_outputs = self.outputs.as_raw_tensor_dict()
-            for k in self.expected_outputs:
-                assert (
-                    k in raw_outputs.keys()
-                ), f"Expected model output '{k}' not found in actual model output keys {list(raw_outputs.keys())}"
+        if expected_output:  # Sanity checks for expected output
+            assert expected_output.dims == tensor.dims, (
+                f"mark_as_output: {name!r} dims mismatch from expected output,"
+                f" given {dims}, expected {expected_output}"
+            )
+            assert expected_output.dtype == tensor.dtype, (
+                f"mark_as_output: {name!r} dtype mismatch from expected output,"
+                f" given {tensor.dtype}, expected {expected_output.dtype}"
+            )
+            assert expected_output.sparse_dim == tensor.sparse_dim, (
+                f"mark_as_output: {name!r} sparse_dim mismatch from expected output,"
+                f" given {tensor.sparse_dim}, expected {expected_output.sparse_dim}"
+            )
 
     def mark_as_default_output(self, tensor: Union[Tensor, Any], *, shape: Optional[Sequence[Dim]] = None) -> None:
         """
         Calls mark_as_output(tensor, "output", shape=shape).
 
         Mark this as the default output.
         See :func:`Frontend.mark_as_default_output` for more details.
 
         :param tensor:
         :param shape:
         """
         self.mark_as_output(tensor, "output", dims=shape)
 
+    def check_outputs_complete(self):
+        """
+        If expected outputs are given, check that all expected outputs are present.
+        """
+        if self.expected_outputs:
+            assert set(self.expected_outputs.data.keys()) == set(self.outputs.data.keys()), (
+                f"check_outputs_complete: expected outputs {self.expected_outputs} do not match"
+                f" actual outputs {self.outputs}"
+            )
+            # We don't need to check the dims, dtype, etc, as this is already done in mark_as_output.
+
     def total_loss(self) -> Union[Tensor, float]:
         """
         :return: total loss, as it is used for backpropagation
         """
         assert self.stage == "train_step"
         assert self.losses, "call rf.get_run_ctx().mark_as_loss(...)"
         loss = 0.0
```

### Comparing `returnn-1.20230524.103608/returnn/frontend/signal.py` & `returnn-1.20230524.133005/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/state.py` & `returnn-1.20230524.133005/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/tensor_array.py` & `returnn-1.20230524.133005/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/frontend/types.py` & `returnn-1.20230524.133005/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/import_/common.py` & `returnn-1.20230524.133005/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/import_/git.py` & `returnn-1.20230524.133005/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/import_/import_.py` & `returnn-1.20230524.133005/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/learning_rate_control.py` & `returnn-1.20230524.133005/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/log.py` & `returnn-1.20230524.133005/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/native_op.cpp` & `returnn-1.20230524.133005/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/native_op.py` & `returnn-1.20230524.133005/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/pretrain.py` & `returnn-1.20230524.133005/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/sprint/cache.py` & `returnn-1.20230524.133005/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/sprint/control.py` & `returnn-1.20230524.133005/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/sprint/error_signals.py` & `returnn-1.20230524.133005/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/sprint/extern_interface.py` & `returnn-1.20230524.133005/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/sprint/interface.py` & `returnn-1.20230524.133005/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/_dim_extra.py` & `returnn-1.20230524.133005/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/_tensor_extra.py` & `returnn-1.20230524.133005/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230524.133005/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230524.133005/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230524.133005/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/dim.py` & `returnn-1.20230524.133005/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/marked_dim.py` & `returnn-1.20230524.133005/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/tensor.py` & `returnn-1.20230524.133005/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/tensor_dict.py` & `returnn-1.20230524.133005/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tensor/utils.py` & `returnn-1.20230524.133005/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/compat.py` & `returnn-1.20230524.133005/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/data_pipeline.py` & `returnn-1.20230524.133005/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/distributed.py` & `returnn-1.20230524.133005/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/engine.py` & `returnn-1.20230524.133005/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230524.133005/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230524.133005/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/horovod.py` & `returnn-1.20230524.133005/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230524.133005/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/layers/base.py` & `returnn-1.20230524.133005/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/layers/basic.py` & `returnn-1.20230524.133005/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/layers/rec.py` & `returnn-1.20230524.133005/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/layers/segmental_model.py` & `returnn-1.20230524.133005/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/layers/signal_processing.py` & `returnn-1.20230524.133005/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/layers/variable.py` & `returnn-1.20230524.133005/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/native_op.py` & `returnn-1.20230524.133005/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/network.py` & `returnn-1.20230524.133005/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/sprint.py` & `returnn-1.20230524.133005/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/updater.py` & `returnn-1.20230524.133005/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/util/basic.py` & `returnn-1.20230524.133005/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/util/data.py` & `returnn-1.20230524.133005/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/util/ken_lm.py` & `returnn-1.20230524.133005/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/tf/util/open_fst.py` & `returnn-1.20230524.133005/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/data/pipeline.py` & `returnn-1.20230524.133005/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230524.133005/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/data/tensor_utils.py` & `returnn-1.20230524.133005/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/engine.py` & `returnn-1.20230524.133005/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/frontend/_backend.py` & `returnn-1.20230524.133005/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/frontend/_rand.py` & `returnn-1.20230524.133005/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/frontend/bridge.py` & `returnn-1.20230524.133005/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/torch/updater.py` & `returnn-1.20230524.133005/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/basic.py` & `returnn-1.20230524.133005/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/better_exchook.py` & `returnn-1.20230524.133005/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/bpe.py` & `returnn-1.20230524.133005/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/debug.py` & `returnn-1.20230524.133005/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/debug_helpers.py` & `returnn-1.20230524.133005/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/fsa.py` & `returnn-1.20230524.133005/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230524.133005/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/pprint.py` & `returnn-1.20230524.133005/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/py-to-pickle.cpp` & `returnn-1.20230524.133005/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/sig_proc.py` & `returnn-1.20230524.133005/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn/util/task_system.py` & `returnn-1.20230524.133005/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/returnn.egg-info/PKG-INFO` & `returnn-1.20230524.133005/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230524.103608
+Version: 1.20230524.133005
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230524.103608/returnn.egg-info/SOURCES.txt` & `returnn-1.20230524.133005/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/setup.py` & `returnn-1.20230524.133005/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/DummySprintExec.py` & `returnn-1.20230524.133005/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230524.133005/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230524.133005/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230524.133005/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/_set_num_threads1.py` & `returnn-1.20230524.133005/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/_setup_test_env.py` & `returnn-1.20230524.133005/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/bpe-unicode-demo.codes` & `returnn-1.20230524.133005/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/bpe-unicode-demo.vocab` & `returnn-1.20230524.133005/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/lexicon_opt.isyms` & `returnn-1.20230524.133005/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/lexicon_opt.jpg` & `returnn-1.20230524.133005/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/lint_common.py` & `returnn-1.20230524.133005/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/pycharm-inspect.py` & `returnn-1.20230524.133005/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/pylint.py` & `returnn-1.20230524.133005/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/returnn-as-framework.py` & `returnn-1.20230524.133005/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/rf_utils.py` & `returnn-1.20230524.133005/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/spelling.dic` & `returnn-1.20230524.133005/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_Config.py` & `returnn-1.20230524.133005/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_Dataset.py` & `returnn-1.20230524.133005/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_Fsa.py` & `returnn-1.20230524.133005/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_GeneratingDataset.py` & `returnn-1.20230524.133005/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_HDFDataset.py` & `returnn-1.20230524.133005/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_LearningRateControl.py` & `returnn-1.20230524.133005/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_Log.py` & `returnn-1.20230524.133005/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_MultiProcDataset.py` & `returnn-1.20230524.133005/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_PTDataset.py` & `returnn-1.20230524.133005/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_Pretrain.py` & `returnn-1.20230524.133005/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_ResNet.py` & `returnn-1.20230524.133005/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_SprintDataset.py` & `returnn-1.20230524.133005/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_SprintInterface.py` & `returnn-1.20230524.133005/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFEngine.py` & `returnn-1.20230524.133005/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFNativeOp.py` & `returnn-1.20230524.133005/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFNetworkLayer.py` & `returnn-1.20230524.133005/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230524.133005/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230524.133005/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFUpdater.py` & `returnn-1.20230524.133005/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TFUtil.py` & `returnn-1.20230524.133005/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TF_determinism.py` & `returnn-1.20230524.133005/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TaskSystem.py` & `returnn-1.20230524.133005/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230524.133005/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_TranslationDataset.py` & `returnn-1.20230524.133005/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_Util.py` & `returnn-1.20230524.133005/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_demos.py` & `returnn-1.20230524.133005/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_fork_exec.py` & `returnn-1.20230524.133005/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_hdf_dump.py` & `returnn-1.20230524.133005/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_array.py` & `returnn-1.20230524.133005/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_attention.py` & `returnn-1.20230524.133005/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_base.py` & `returnn-1.20230524.133005/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_cond.py` & `returnn-1.20230524.133005/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_container.py` & `returnn-1.20230524.133005/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_conv.py` & `returnn-1.20230524.133005/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_encoder_conformer.py` & `returnn-1.20230524.133005/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_loop.py` & `returnn-1.20230524.133005/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_math.py` & `returnn-1.20230524.133005/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_normalization.py` & `returnn-1.20230524.133005/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_rec.py` & `returnn-1.20230524.133005/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_reduce.py` & `returnn-1.20230524.133005/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_rf_signal.py` & `returnn-1.20230524.133005/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_tensor.py` & `returnn-1.20230524.133005/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_tools.py` & `returnn-1.20230524.133005/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_torch_frontend.py` & `returnn-1.20230524.133005/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tests/test_torch_internal_frontend.py` & `returnn-1.20230524.133005/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/analyze-dataset-batches.py` & `returnn-1.20230524.133005/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/bliss-collect-seq-lens.py` & `returnn-1.20230524.133005/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/bliss-dump-text.py` & `returnn-1.20230524.133005/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/bliss-get-segment-names.py` & `returnn-1.20230524.133005/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/bliss-to-ogg-zip.py` & `returnn-1.20230524.133005/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/bpe-create-lexicon.py` & `returnn-1.20230524.133005/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/calculate-word-error-rate.py` & `returnn-1.20230524.133005/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/cleanup-old-models.py` & `returnn-1.20230524.133005/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/collect-orth-symbols.py` & `returnn-1.20230524.133005/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/collect-words.py` & `returnn-1.20230524.133005/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/compile_native_op.py` & `returnn-1.20230524.133005/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/compile_tf_graph.py` & `returnn-1.20230524.133005/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/debug-dump-search-scores.py` & `returnn-1.20230524.133005/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/debug-plot-search-scores.py` & `returnn-1.20230524.133005/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/dump-dataset-raw-strings.py` & `returnn-1.20230524.133005/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/dump-dataset.py` & `returnn-1.20230524.133005/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/dump-forward-stats.py` & `returnn-1.20230524.133005/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/dump-forward.py` & `returnn-1.20230524.133005/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/dump-network-json.py` & `returnn-1.20230524.133005/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/dump-pickle.py` & `returnn-1.20230524.133005/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230524.133005/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/get-attention-weights.py` & `returnn-1.20230524.133005/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/get-best-model-epoch.py` & `returnn-1.20230524.133005/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/hdf_dump.py` & `returnn-1.20230524.133005/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230524.133005/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/import-blocks-mt-model.py` & `returnn-1.20230524.133005/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/import-t2t-mt-model.py` & `returnn-1.20230524.133005/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/Makefile` & `returnn-1.20230524.133005/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/README.md` & `returnn-1.20230524.133005/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/example/README.md` & `returnn-1.20230524.133005/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230524.133005/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230524.133005/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230524.133005/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/file.h` & `returnn-1.20230524.133005/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230524.133005/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230524.133005/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/main.cc` & `returnn-1.20230524.133005/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230524.133005/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230524.133005/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230524.133005/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/tf_avg_checkpoints.py` & `returnn-1.20230524.133005/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/tf_inspect_checkpoint.py` & `returnn-1.20230524.133005/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/tf_inspect_summary_log.py` & `returnn-1.20230524.133005/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230524.103608/tools/torch_export_to_onnx.py` & `returnn-1.20230524.133005/tools/torch_export_to_onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     def __call__(self, data: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """
         Wrapper to forward_step from the config.
         """
         extern_data = self.extern_data.copy_template()
         extern_data.assign_from_raw_tensor_dict_(data)
         self.forward_step_func(model=self.model, extern_data=extern_data)
+        rf.get_run_ctx().check_outputs_complete()
         return rf.get_run_ctx().outputs.as_raw_tensor_dict()
 
 
 class ForwardModuleRF(_RFModuleAsPTModule):
     """
     Wrapper of a RETURNN frontend module that's meant to call forward_step from the config when called.
     """
@@ -105,14 +106,15 @@
     def __call__(self, data: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """
         Wrapper to forward_step from the config.
         """
         extern_data = self.extern_data.copy_template()
         extern_data.assign_from_raw_tensor_dict_(data)
         self.forward_step_func(model=self.rf_module, extern_data=extern_data)
+        rf.get_run_ctx().check_outputs_complete()
         return rf.get_run_ctx().outputs.as_raw_tensor_dict()
 
 
 def main():
     """
     Main entry point
     """
@@ -139,15 +141,15 @@
     model_outputs_raw_keys = []
     for k, v in model_outputs.data.items():
         model_outputs_raw_keys.append(k)
         for i, dim in enumerate(v.dims):
             if dim.is_batch_dim() or dim.is_dynamic():
                 model_outputs_raw_keys.append(f"{k}:size{i}")
 
-    rf.init_forward_step_run_ctx(expected_outputs=model_outputs_raw_keys)
+    rf.init_forward_step_run_ctx(expected_outputs=model_outputs)
     rf.set_random_seed(42)
 
     get_model_func = config.typed_value("get_model")
     assert get_model_func, "get_model() isn't specified in the config passed as a parameter."
     model = get_model_func()
     loaded_checkpoint = torch.load(args.checkpoint)
 
@@ -170,18 +172,20 @@
     tensor_dict_numpy_to_torch_(extern_data)
     extern_data_raw = extern_data.as_raw_tensor_dict()
 
     if is_pt_module:
         model.load_state_dict(loaded_checkpoint["model"])
         model.eval()
         pt_model_fwd = ForwardModulePT(model, forward_step_func, extern_data)
-    else:
+    elif is_rf_module:
         pt_model_fwd = ForwardModuleRF(model, forward_step_func, extern_data)
         pt_model_fwd.load_state_dict(loaded_checkpoint["model"])
         pt_model_fwd.eval()
+    else:
+        assert False, "PT/RF module?"  # should not get here
 
     dynamic_axes = {}
     for k, v in list(extern_data.data.items()) + list(model_outputs.data.items()):
         dynamic_axes[k] = {i: dim.name for i, dim in enumerate(v.dims) if dim.is_dynamic() or dim.is_batch_dim()}
         for i, dim in enumerate(v.dims):
             if dim.dyn_size_ext:
                 dynamic_axes[f"{k}:size{i}"] = {
```

