# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230523.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230523.tar", last modified: Tue May 23 12:40:06 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230524.tar", last modified: Wed May 24 12:49:13 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230523.tar` & `tensorcircuit-nightly-0.9.1.dev20230524.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.502299 tensorcircuit-nightly-0.9.1.dev20230523/
--rw-r--r--   0 runner    (1001) docker     (122)    25259 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-23 12:40:06.502299 tensorcircuit-nightly-0.9.1.dev20230523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18675 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.490298 tensorcircuit-nightly-0.9.1.dev20230523/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.490298 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 12:40:06.502299 tensorcircuit-nightly-0.9.1.dev20230523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-23 12:40:00.000000 tensorcircuit-nightly-0.9.1.dev20230523/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.494298 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-23 12:39:59.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    43418 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.494298 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.498299 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-23 12:40:06.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-23 12:40:06.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:40:06.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-23 12:40:06.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-23 12:40:06.000000 tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:40:06.502299 tensorcircuit-nightly-0.9.1.dev20230523/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47713 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-23 12:16:42.000000 tensorcircuit-nightly-0.9.1.dev20230523/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.123372 tensorcircuit-nightly-0.9.1.dev20230524/
+-rw-r--r--   0 runner    (1001) docker     (122)    25259 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21379 2023-05-24 12:49:13.123372 tensorcircuit-nightly-0.9.1.dev20230524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18925 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6311 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.083371 tensorcircuit-nightly-0.9.1.dev20230524/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.091372 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 12:49:13.123372 tensorcircuit-nightly-0.9.1.dev20230524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-24 12:49:04.000000 tensorcircuit-nightly-0.9.1.dev20230524/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.099372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-24 12:49:04.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43418 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.103372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.103372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.107372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.107372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.111372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.111372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.111372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.115372 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21379 2023-05-24 12:49:12.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-24 12:49:12.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 12:49:12.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-24 12:49:12.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-24 12:49:12.000000 tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:49:13.119372 tensorcircuit-nightly-0.9.1.dev20230524/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47713 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-24 12:16:46.000000 tensorcircuit-nightly-0.9.1.dev20230524/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230524/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230524/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230524/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230524/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230523
+Version: 0.9.1.dev20230524
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -226,26 +226,32 @@
         
         ### Stark-DTC
         
         For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
         
         Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
         
-        ### EMQAOA-DARBO
+        ### RA-Training
         
-        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
         
-        Reference paper: https://arxiv.org/abs/2303.14877.
+        Reference paper: https://arxiv.org/abs/2303.08154.
         
         ### TenCirChem
         
         [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
         
         Reference paper: https://arxiv.org/abs/2303.10825.
         
+        ### EMQAOA-DARBO
+        
+        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        
+        Reference paper: https://arxiv.org/abs/2303.14877.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: jax
 Provides-Extra: torch
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/README.md` & `tensorcircuit-nightly-0.9.1.dev20230524/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -218,18 +218,24 @@
 
 ### Stark-DTC
 
 For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
 
 Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
 
-### EMQAOA-DARBO
+### RA-Training
 
-For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
 
-Reference paper: https://arxiv.org/abs/2303.14877.
+Reference paper: https://arxiv.org/abs/2303.08154.
 
 ### TenCirChem
 
 [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
 
 Reference paper: https://arxiv.org/abs/2303.10825.
+
+### EMQAOA-DARBO
+
+For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+
+Reference paper: https://arxiv.org/abs/2303.14877.
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230524/README_cn.md`

 * *Files 3% similar despite different names*

```diff
@@ -163,18 +163,24 @@
 
 ### Stark-DTC
 
 数值验证 Stark 多体局域化稳定的离散时间晶体，类似的 Floquet 系统模拟请参考 [例子](/examples/timeevolution_trotter.py)。
 
 参考论文: https://arxiv.org/abs/2208.02866 (PRL)。
 
-### EMQAOA-DARBO
+### RA-Training
 
-数值模拟和带错误消除的真实量子硬件实验验证 QAOA 优化的代码请参考 [项目](https://github.com/sherrylixuecheng/EMQAOA-DARBO)。
+利用我们提出的随机量子门激活策略训练优化变分量子算法的实现请参考 [项目](https://github.com/ls-iastu/RAtraining).
 
-参考论文: https://arxiv.org/abs/2303.14877。
+参考论文: https://arxiv.org/abs/2303.08154.
 
 ### TenCirChem
 
 [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) 是高效的，专注于处理和计算分子性质的量子计算软件。其基于 TensorCircuit 并为量子化学任务进行了专门的优化。
 
 参考论文: https://arxiv.org/abs/2303.10825。
+
+### EMQAOA-DARBO
+
+数值模拟和带错误消除的真实量子硬件实验验证 QAOA 优化的代码请参考 [项目](https://github.com/sherrylixuecheng/EMQAOA-DARBO)。
+
+参考论文: https://arxiv.org/abs/2303.14877。
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/index.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230524/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230524/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230523"
+__version__ = "0.9.1.dev20230524"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230523
+Version: 0.9.1.dev20230524
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -226,26 +226,32 @@
         
         ### Stark-DTC
         
         For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
         
         Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
         
-        ### EMQAOA-DARBO
+        ### RA-Training
         
-        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
         
-        Reference paper: https://arxiv.org/abs/2303.14877.
+        Reference paper: https://arxiv.org/abs/2303.08154.
         
         ### TenCirChem
         
         [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
         
         Reference paper: https://arxiv.org/abs/2303.10825.
         
+        ### EMQAOA-DARBO
+        
+        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        
+        Reference paper: https://arxiv.org/abs/2303.14877.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: jax
 Provides-Extra: torch
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230524/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230523/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230524/tests/test_van.py`

 * *Files identical despite different names*

