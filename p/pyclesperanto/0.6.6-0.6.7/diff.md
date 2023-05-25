# Comparing `tmp/pyclesperanto-0.6.6.tar.gz` & `tmp/pyclesperanto-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclesperanto-0.6.6.tar", last modified: Wed May 24 11:39:06 2023, max compression
+gzip compressed data, was "pyclesperanto-0.6.7.tar", last modified: Thu May 25 14:50:34 2023, max compression
```

## Comparing `pyclesperanto-0.6.6.tar` & `pyclesperanto-0.6.7.tar`

### file list

```diff
@@ -1,97 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.225739 pyclesperanto-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.213739 pyclesperanto-0.6.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.213739 pyclesperanto-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/.github/workflows/build_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-24 11:39:06.225739 pyclesperanto-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.213739 pyclesperanto-0.6.6/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)    92866 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/benchmarking/benchmark_basic_operations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59529 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/benchmarking/benchmark_gaussian.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60126 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/benchmarking/benchmark_histogram.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    53631 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/benchmarking/benchmark_mini_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60985 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/benchmarking/benchmark_otsu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   105858 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/benchmarking/benchmarking_tribolium_workflow.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.217739 pyclesperanto-0.6.6/demos/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/add_image_and_scalar.cl
--rw-r--r--   0 runner    (1001) docker     (123)   329805 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/cell_segmentation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/explore_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   222151 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/find_local_maxima.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   141526 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/image_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   626680 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/image_filtering.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.217739 pyclesperanto-0.6.6/demos/images/
--rw-r--r--   0 runner    (1001) docker     (123)    51553 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/cell_segmentation.png
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/explore_API.png
--rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/find_local_maxima.png
--rw-r--r--   0 runner    (1001) docker     (123)    44227 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/image_filtering.png
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/labeled_blobs.png
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/multi-gpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/images/tribolium3d_segmentation.png
--rw-r--r--   0 runner    (1001) docker     (123)   262922 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/multi_gpu_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   277298 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/process_blobs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   389183 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/process_tribolium.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   221181 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/demos/run_custom_kernel.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.217739 pyclesperanto-0.6.6/developer_docs/
--rw-r--r--   0 runner    (1001) docker     (123)   152772 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/developer_docs/API_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.221739 pyclesperanto-0.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.221739 pyclesperanto-0.6.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.221739 pyclesperanto-0.6.6/pyclesperanto/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_functionalities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_image_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_memory_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_tier1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_tier2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_tier3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_tier4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_tier5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_tier6.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyclesperanto/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.221739 pyclesperanto-0.6.6/pyclesperanto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-24 11:39:06.000000 pyclesperanto-0.6.6/pyclesperanto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-24 11:39:06.000000 pyclesperanto-0.6.6/pyclesperanto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:39:06.000000 pyclesperanto-0.6.6/pyclesperanto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 11:39:06.000000 pyclesperanto-0.6.6/pyclesperanto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 11:39:06.000000 pyclesperanto-0.6.6/pyclesperanto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.221739 pyclesperanto-0.6.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/scripts/build-opencl-linux.sh
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/scripts/build-opencl-macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/scripts/build-opencl-windows.sh
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/scripts/generate-tiers-package.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:39:06.225739 pyclesperanto-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.221739 pyclesperanto-0.6.6/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)      569 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/tests/test_connected_components_labeling_box.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/tests/test_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:39:06.225739 pyclesperanto-0.6.6/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleEnumType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleGateway.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleImage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleMemory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleProcessor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleTier1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleTier2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleTier3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleTier4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleTier5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/cleTier6.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/pyclesperanto.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-24 11:38:52.000000 pyclesperanto-0.6.6/wrapper/pyclesperanto.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.885628 pyclesperanto-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.865627 pyclesperanto-0.6.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.865627 pyclesperanto-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/.github/workflows/build_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-25 14:50:34.885628 pyclesperanto-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.869628 pyclesperanto-0.6.7/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)    92866 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/benchmarking/benchmark_basic_operations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59529 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/benchmarking/benchmark_gaussian.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60126 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/benchmarking/benchmark_histogram.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    53631 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/benchmarking/benchmark_mini_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60985 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/benchmarking/benchmark_otsu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   105858 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/benchmarking/benchmarking_tribolium_workflow.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.873628 pyclesperanto-0.6.7/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/add_image_and_scalar.cl
+-rw-r--r--   0 runner    (1001) docker     (123)   329805 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/cell_segmentation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/explore_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   222151 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/find_local_maxima.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   141526 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/image_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   626680 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/image_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.873628 pyclesperanto-0.6.7/demos/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    51553 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/cell_segmentation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/explore_API.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/find_local_maxima.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44227 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/image_filtering.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/labeled_blobs.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/multi-gpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/images/tribolium3d_segmentation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   262922 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/multi_gpu_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   277298 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/process_blobs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   389183 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/process_tribolium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   221181 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/demos/run_custom_kernel.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.873628 pyclesperanto-0.6.7/developer_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   152772 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/developer_docs/API_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.877627 pyclesperanto-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.877627 pyclesperanto-0.6.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.877627 pyclesperanto-0.6.7/pyclesperanto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_functionalities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_image_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_memory_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44227 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_tier1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_tier2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_tier3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_tier4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_tier5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_tier6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyclesperanto/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.881628 pyclesperanto-0.6.7/pyclesperanto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-25 14:50:34.000000 pyclesperanto-0.6.7/pyclesperanto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 14:50:34.000000 pyclesperanto-0.6.7/pyclesperanto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:50:34.000000 pyclesperanto-0.6.7/pyclesperanto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 14:50:34.000000 pyclesperanto-0.6.7/pyclesperanto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:50:34.000000 pyclesperanto-0.6.7/pyclesperanto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.881628 pyclesperanto-0.6.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/scripts/build-opencl-linux.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/scripts/build-opencl-macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/scripts/build-opencl-windows.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/scripts/generate-tiers-package.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:50:34.885628 pyclesperanto-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.881628 pyclesperanto-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_tier1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_tier2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_tier3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_tier4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_tier5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/tests/test_tier6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:34.885628 pyclesperanto-0.6.7/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleEnumType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleGateway.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleMemory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleProcessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleTier1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleTier2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleTier3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleTier4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleTier5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/cleTier6.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/pyclesperanto.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 14:50:22.000000 pyclesperanto-0.6.7/wrapper/pyclesperanto.hpp
```

### Comparing `pyclesperanto-0.6.6/.github/dependabot.yml` & `pyclesperanto-0.6.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/.github/workflows/build_and_test.yml` & `pyclesperanto-0.6.7/.github/workflows/build_and_test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -55,9 +55,13 @@
       - name: Tests
         shell: bash -l {0}
         run: |
           pytest -v --cov=./ --cov-report=xml
 
       - name: Coverage
         uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
+          files: ./coverage.xml
+          fail_ci_if_error: true # optional (default = false)
```

### Comparing `pyclesperanto-0.6.6/.github/workflows/pages.yml` & `pyclesperanto-0.6.7/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/.github/workflows/wheels.yml` & `pyclesperanto-0.6.7/.github/workflows/wheels.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 name: Build & Deploy
 
 # Build on every branch push, tag push, and pull request change:
 on:
   push:
     branches: [main]
-    paths-ignore:
-      - '**.rst'
-      - '**.txt'
   pull_request:
     branches: [main]
   release:
-    types: [published]
+      types: [created]
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
@@ -51,15 +48,15 @@
   upload_all:
     name: Upload if release
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     # upload to PyPI on every tag starting with 'v'
     # if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
     # upload to PyPI on release event
-    # if: github.event_name == 'release' && github.event.action == 'created'
+    if: github.event_name == 'release' && success()
     steps:
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - uses: actions/download-artifact@v3
         with:
```

### Comparing `pyclesperanto-0.6.6/.gitignore` & `pyclesperanto-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/CMakeLists.txt` & `pyclesperanto-0.6.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/LICENSE` & `pyclesperanto-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/PKG-INFO` & `pyclesperanto-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: pyclesperanto
-Version: 0.6.6
+Version: 0.6.7
 Summary: GPU-accelerated image processing in python using OpenCL
 Author: Stephane Rigaud
 Author-email: stephane.rigaud@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/clEsperanto/pyclesperanto#README.md
 Project-URL: Source, https://github.com/clEsperanto/pyclesperanto/
 Project-URL: Issues, https://github.com/clEsperanto/pyclesperanto/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-clesperanto
```

### Comparing `pyclesperanto-0.6.6/README.md` & `pyclesperanto-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/benchmarking/benchmark_basic_operations.ipynb` & `pyclesperanto-0.6.7/benchmarking/benchmark_basic_operations.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/benchmarking/benchmark_gaussian.ipynb` & `pyclesperanto-0.6.7/benchmarking/benchmark_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/benchmarking/benchmark_histogram.ipynb` & `pyclesperanto-0.6.7/benchmarking/benchmark_histogram.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/benchmarking/benchmark_mini_pipeline.ipynb` & `pyclesperanto-0.6.7/benchmarking/benchmark_mini_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/benchmarking/benchmark_otsu.ipynb` & `pyclesperanto-0.6.7/benchmarking/benchmark_otsu.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/benchmarking/benchmarking_tribolium_workflow.ipynb` & `pyclesperanto-0.6.7/benchmarking/benchmarking_tribolium_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/add_image_and_scalar.cl` & `pyclesperanto-0.6.7/demos/add_image_and_scalar.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/cell_segmentation.ipynb` & `pyclesperanto-0.6.7/demos/cell_segmentation.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/explore_API.ipynb` & `pyclesperanto-0.6.7/demos/explore_API.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/find_local_maxima.ipynb` & `pyclesperanto-0.6.7/demos/find_local_maxima.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/image_API.ipynb` & `pyclesperanto-0.6.7/demos/image_API.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/image_filtering.ipynb` & `pyclesperanto-0.6.7/demos/image_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/cell_segmentation.png` & `pyclesperanto-0.6.7/demos/images/cell_segmentation.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/explore_API.png` & `pyclesperanto-0.6.7/demos/images/explore_API.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/find_local_maxima.png` & `pyclesperanto-0.6.7/demos/images/find_local_maxima.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/image_filtering.png` & `pyclesperanto-0.6.7/demos/images/image_filtering.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/labeled_blobs.png` & `pyclesperanto-0.6.7/demos/images/labeled_blobs.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/multi-gpu.png` & `pyclesperanto-0.6.7/demos/images/multi-gpu.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/images/tribolium3d_segmentation.png` & `pyclesperanto-0.6.7/demos/images/tribolium3d_segmentation.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/multi_gpu_demo.ipynb` & `pyclesperanto-0.6.7/demos/multi_gpu_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/process_blobs.ipynb` & `pyclesperanto-0.6.7/demos/process_blobs.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/process_tribolium.ipynb` & `pyclesperanto-0.6.7/demos/process_tribolium.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/demos/run_custom_kernel.ipynb` & `pyclesperanto-0.6.7/demos/run_custom_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/developer_docs/API_demo.ipynb` & `pyclesperanto-0.6.7/developer_docs/API_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/Makefile` & `pyclesperanto-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/make.bat` & `pyclesperanto-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/source/api.rst` & `pyclesperanto-0.6.7/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/source/conf.py` & `pyclesperanto-0.6.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/source/index.rst` & `pyclesperanto-0.6.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/source/install.rst` & `pyclesperanto-0.6.7/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/docs/source/usage.rst` & `pyclesperanto-0.6.7/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/__init__.py` & `pyclesperanto-0.6.7/pyclesperanto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,18 @@
     smaller_constant,
     smaller,
     smaller_or_equal_constant,
     smaller_or_equal,
     sum_z_projection,
     sum_y_projection,
     sum_x_projection,
+    detect_maxima,
 )
 from ._tier2 import (
     difference_of_gaussian,
-    detect_maxima_box,
     maximum_of_all_pixels,
     minimum_of_all_pixels,
     sum_of_all_pixels,
     extend_labeling_via_voronoi,
     top_hat_box,
 )
 from ._tier3 import (
@@ -101,11 +101,11 @@
 # Generic Import
 import os
 
 # Supports for ocl-icd find shipped OpenCL ICDs, cf.
 os.environ["PYCLESPERANTO_HOME"] = os.path.dirname(os.path.abspath(__file__))
 
 # redefine memory type for easy usage
-buffer = MemoryType.buffer
-image = MemoryType.image
+buffer = MemoryType.buffer()
+image = MemoryType.image()
 
 __common_alias__ = "cle"
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_decorators.py` & `pyclesperanto-0.6.7/pyclesperanto/_decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,41 +57,45 @@
         # will raise a TypeError if the provided arguments do not match the signature
         # https://docs.python.org/3/library/inspect.html#inspect.Signature.bind
         bound = sig.bind(*args, **kwargs)
         # set default values for missing arguments
         # https://docs.python.org/3/library/inspect.html#inspect.BoundArguments.apply_defaults
         bound.apply_defaults()
 
+        args_list = function.fullargspec.args
+        index = next((i for i, element in enumerate(args_list) if "input_image" in element), -1)
+        arg_name = args_list[index]
+
         # copy images to GPU, and create output array if necessary
         for key, value in bound.arguments.items():
             if (
                 is_image(value)
                 and key in sig.parameters
                 and sig.parameters[key].annotation is Image
             ):
                 bound.arguments[key] = push(value)
             if (
                 key in sig.parameters
                 and sig.parameters[key].annotation is Image
                 and value is None
             ):
-                sig2 = inspect.signature(output_creator)
+                # sig2 = inspect.signature(output_creator)
                 # bound.arguments[key] = output_creator(
                 #     *bound.args[0 : len(sig2.parameters)]
-                # )
-                input_image_index = function.fullargspec.args.index("input_image")
+                # )                
+                input_image_index = args_list.index(arg_name)
                 bound.arguments[key] = output_creator(
                     bound.args[input_image_index]
                 )
             if (
                 key in sig.parameters
                 and sig.parameters[key].annotation is Device
                 and value is None
             ):
-                input_image = bound.arguments["input_image"]
+                input_image = bound.arguments[arg_name]
                 bound.arguments[key] = input_image.device
                 # sig2 = inspect.signature(device_selector)
                 # bound.arguments[key] = device_selector()
 
         # call the decorated function
         return function(*bound.args, **bound.kwargs)
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_device.py` & `pyclesperanto-0.6.7/pyclesperanto/_device.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_functionalities.py` & `pyclesperanto-0.6.7/pyclesperanto/_functionalities.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_image.py` & `pyclesperanto-0.6.7/pyclesperanto/_image.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_image_operators.py` & `pyclesperanto-0.6.7/pyclesperanto/_image_operators.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_memory_operations.py` & `pyclesperanto-0.6.7/pyclesperanto/_memory_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         Handle of the empty GPU image
     """
     from ._image import cleImage
 
     if dtype is None:
         dtype = image.dtype
     if mtype is None:
-        mtype = image.mtype if isinstance(image, cleImage) else MemoryType.buffer
+        mtype = image.mtype if isinstance(image, cleImage) else MemoryType.buffer()
     if device is None:
         device = image.device if isinstance(image, cleImage) else get_device()
     return create(shape=tuple(image.shape), dtype=dtype, mtype=mtype, device=device)
 
 
 def push(
     array: Image, mtype: Optional[MemoryType] = None, device: Optional[Device] = None
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_tier1.py` & `pyclesperanto-0.6.7/pyclesperanto/_tier1.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_addImageAndScalar
     """
 
     from ._pyclesperanto import _AddImageAndScalarKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, scalar=float(scalar))
+    op(device, src=input_image, dst=output_image, value=float(scalar))
     return output_image
 
 
 @plugin_function
 def add_images_weighted(
     input_image1: Image,
     input_image2: Image,
@@ -81,16 +81,16 @@
     from ._pyclesperanto import _AddImagesWeightedKernel_Call as op
 
     op(
         device,
         src1=input_image1,
         src2=input_image2,
         dst=output_image,
-        weight1=float(factor1),
-        weight2=float(factor2),
+        w1=float(factor1),
+        w2=float(factor2),
     )
     return output_image
 
 
 @plugin_function
 def gaussian_blur(
     input_image: Image,
@@ -495,77 +495,77 @@
     return output_image
 
 
 @plugin_function
 def greater_or_equal_constant(
     input_image: Image,
     output_image: Image = None,
-    scalar: float = 0,
+    constant: float = 0,
     device: Device = None,
 ) -> Image:
     """Determines if an images A is greater or equal a given scalar b.
 
     f(a, b) = 1 if a >= b; 0 otherwise.
 
     Parameters
     ----------
     input_image : Image
         image to be compared
     output_image : Image, optional
         The output image where results are written into.
-    scalar : Number, default 0
+    constant : Number, default 0
     device : Device, optional
         The device where the operation should take place on.
 
     Returns
     -------
     output_image : Image
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_greaterOrEqualConstant
     """
     from ._pyclesperanto import _GreaterOrEqualConstantKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, scalar=float(scalar))
+    op(device, src=input_image, dst=output_image, value=float(constant))
     return output_image
 
 
 @plugin_function
 def greater_constant(
     input_image: Image,
     output_image: Image = None,
-    scalar: float = 0,
+    constant: float = 0,
     device: Device = None,
 ) -> Image:
     """Determines if an images A is greater a given scalar b.
 
     f(a, b) = 1 if a > b; 0 otherwise.
 
     Parameters
     ----------
     input_image : Image
         image to be compared
     output_image : Image, optional
         The output image where results are written into.
-    scalar : Number, default 0
+    constant : Number, default 0
     device : Device, optional
         The device where the operation should take place on.
 
     Returns
     -------
     output_image : Image
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_greaterConstant
     """
     from ._pyclesperanto import _GreaterConstantKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, scalar=float(scalar))
+    op(device, src=input_image, dst=output_image, value=float(constant))
     return output_image
 
 
 @plugin_function
 def greater_or_equal(
     input_image1: Image,
     input_image2: Image,
@@ -782,14 +782,51 @@
     output_image : Image
     """
     from ._pyclesperanto import _BinarySubtractKernel_Call as op
 
     op(device, src1=input_image1, src2=input_image2, dst=output_image)
     return output_image
 
+@plugin_function
+def detect_maxima(
+    input_image: Image,
+    output_image: Image = None,
+    device: Device = None,
+) -> Image:
+    """Detects local maxima in a given square/cubic neighborhood.
+
+    Pixels in the resulting image are set to 1 if there is no other pixel in a
+    given radius which has a
+    higher intensity, and to 0 otherwise.
+
+    Parameters
+    ----------
+    input_image : Image
+        The input image to be processed.
+    output_image : Image, optional
+        The output image where results are written into.
+    device : Device, optional
+        The device to be used for computation.
+
+    Returns
+    -------
+    output_image: Image
+
+    References
+    ----------
+    .. [1] https://clij.github.io/clij2-docs/reference_detectMaximaBox
+    """
+    from ._pyclesperanto import _DetectMaximaKernel_Call as op
+
+    op(
+        device,
+        src=input_image,
+        dst=output_image,
+    )
+    return output_image
 
 @plugin_function
 def dilate_sphere(
     input_image: Image,
     output_image: Image = None,
     device: Device = None,
 ) -> Image:
@@ -854,15 +891,15 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_equalConstant
     """
     from ._pyclesperanto import _EqualConstantKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, constant=constant)
+    op(device, src=input_image, dst=output_image, value=constant)
     return output_image
 
 
 @plugin_function
 def equal(
     input_image1: Image,
     input_image2: Image,
@@ -1060,15 +1097,15 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_subtractImageFromScalar
     """
     from ._pyclesperanto import _SubtractImageFromScalarKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, scalar=float(scalar))
+    op(device, src=input_image, dst=output_image, value=float(scalar))
     return output_image
 
 
 @plugin_function
 def sobel(
     input_image: Image,
     output_image: Image = None,
@@ -1264,15 +1301,15 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_multiplyImageAndScalar
     """
     from ._pyclesperanto import _MultiplyImageAndScalarKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, scalar=float(scalar))
+    op(device, src=input_image, dst=output_image, value=float(scalar))
     return output_image
 
 
 @plugin_function
 def not_equal_constant(
     input_image: Image,
     output_image: Image = None,
@@ -1300,15 +1337,15 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_notEqualConstant
     """
     from ._pyclesperanto import _NotEqualConstantKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, constant=float(constant))
+    op(device, src=input_image, dst=output_image, value=float(constant))
     return output_image
 
 
 @plugin_function
 def not_equal(
     input_image1: Image,
     input_image2: Image,
@@ -1372,23 +1409,23 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_power
     """
     from ._pyclesperanto import _PowerKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, exponent=float(exponent))
+    op(device, src=input_image, dst=output_image, scalar=float(exponent))
     return output_image
 
 
 @plugin_function
 def power_images(
     input_image1: Image,
     input_image2: Image,
-    output_image: Image,
+    output_image: Image = None,
     device: Device = None,
 ) -> Image:
     """Computes all pairs of pixels x and y value x to the power of y.
 
     <pre>f(x, y) = x ^ y</pre>
 
     Parameters
@@ -1444,15 +1481,15 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_smallerConstant
     """
     from ._pyclesperanto import _SmallerConstantKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, constant=float(constant))
+    op(device, src=input_image, dst=output_image, value=float(constant))
     return output_image
 
 
 @plugin_function
 def smaller(
     input_image1: Image,
     input_image2: Image,
@@ -1516,15 +1553,15 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_smallerOrEqualConstant
     """
     from ._pyclesperanto import _SmallerOrEqualConstantKernel_Call as op
 
-    op(device, src=input_image, dst=output_image, constant=float(constant))
+    op(device, src=input_image, dst=output_image, value=float(constant))
     return output_image
 
 
 @plugin_function
 def smaller_or_equal(
     input_image1: Image,
     input_image2: Image,
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_tier2.py` & `pyclesperanto-0.6.7/pyclesperanto/_tier2.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,66 +62,14 @@
         sigma1_z=float(sigma1_z),
         sigma2_x=float(sigma2_x),
         sigma2_y=float(sigma2_y),
         sigma2_z=float(sigma2_z),
     )
     return output_image
 
-
-@plugin_function
-def detect_maxima_box(
-    input_image: Image,
-    output_image: Image = None,
-    radius_x: int = 0,
-    radius_y: int = 0,
-    radius_z: int = 0,
-    device: Device = None,
-) -> Image:
-    """Detects local maxima in a given square/cubic neighborhood.
-
-    Pixels in the resulting image are set to 1 if there is no other pixel in a
-    given radius which has a
-    higher intensity, and to 0 otherwise.
-
-    Parameters
-    ----------
-    input_image : Image
-        The input image to be processed.
-    output_image : Image, optional
-        The output image where results are written into.
-    radius_x : int, default 0
-        Radius of the square/cubic neighborhood in x
-    radius_y : int, default 0
-        Radius of the square/cubic neighborhood in y
-    radius_z : int, default 0
-        Radius of the square/cubic neighborhood in z
-    device : Device, optional
-        The device to be used for computation.
-
-    Returns
-    -------
-    output_image: Image
-
-    References
-    ----------
-    .. [1] https://clij.github.io/clij2-docs/reference_detectMaximaBox
-    """
-    from ._pyclesperanto import _DetectMaximaBoxKernel_Call as op
-
-    op(
-        device,
-        src=input_image,
-        dst=output_image,
-        radius_x=int(radius_x),
-        radius_y=int(radius_y),
-        radius_z=int(radius_z),
-    )
-    return output_image
-
-
 @plugin_function
 def maximum_of_all_pixels(
     input_image: Image,
     output_image: Image = None,
     device: Device = None,
 ) -> Image:
     """Determines the maximum of all pixels in a given image.
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_tier3.py` & `pyclesperanto-0.6.7/pyclesperanto/_tier3.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     from ._pyclesperanto import _HistogramKernel_Call as op
     import math
 
     op(
         device,
         src=input_image,
         dst=output_image,
+        bin=int(bins),
         min_intensity=math.inf,
         max_intensity=math.inf,
-        bins=int(bins),
     )
     return output_image
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_tier4.py` & `pyclesperanto-0.6.7/pyclesperanto/_tier4.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_tier5.py` & `pyclesperanto-0.6.7/pyclesperanto/_tier5.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,9 +32,9 @@
 
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_maskedVoronoiLabeling
     """
     from ._pyclesperanto import _MaskedVoronoiLabelingKernel_Call as op
 
-    op(device, src=input_image, mask=mask_image, dst=output_image)
+    op(device, src=input_image, dst=output_image, mask=mask_image)
     return output_image
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_tier6.py` & `pyclesperanto-0.6.7/pyclesperanto/_tier6.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto/_types.py` & `pyclesperanto-0.6.7/pyclesperanto/_types.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/pyclesperanto.egg-info/PKG-INFO` & `pyclesperanto-0.6.7/pyclesperanto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: pyclesperanto
-Version: 0.6.6
+Version: 0.6.7
 Summary: GPU-accelerated image processing in python using OpenCL
 Author: Stephane Rigaud
 Author-email: stephane.rigaud@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/clEsperanto/pyclesperanto#README.md
 Project-URL: Source, https://github.com/clEsperanto/pyclesperanto/
 Project-URL: Issues, https://github.com/clEsperanto/pyclesperanto/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-clesperanto
```

### Comparing `pyclesperanto-0.6.6/pyclesperanto.egg-info/SOURCES.txt` & `pyclesperanto-0.6.7/pyclesperanto.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -60,16 +60,22 @@
 pyclesperanto.egg-info/dependency_links.txt
 pyclesperanto.egg-info/requires.txt
 pyclesperanto.egg-info/top_level.txt
 scripts/build-opencl-linux.sh
 scripts/build-opencl-macos.sh
 scripts/build-opencl-windows.sh
 scripts/generate-tiers-package.ipynb
-tests/test_connected_components_labeling_box.py
+tests/test_core.py
 tests/test_import.py
+tests/test_tier1.py
+tests/test_tier2.py
+tests/test_tier3.py
+tests/test_tier4.py
+tests/test_tier5.py
+tests/test_tier6.py
 wrapper/cleEnumType.cpp
 wrapper/cleGateway.cpp
 wrapper/cleImage.cpp
 wrapper/cleMemory.cpp
 wrapper/cleProcessor.cpp
 wrapper/cleTier1.cpp
 wrapper/cleTier2.cpp
```

### Comparing `pyclesperanto-0.6.6/pyproject.toml` & `pyclesperanto-0.6.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [tool.pytest.ini_options]
 addopts = "-ra -q"
 testpaths = [
   "tests",
 ]
 
 [tool.cibuildwheel]
-build = ["cp37-*", "cp38-*", "cp39-*", "cp310-*", "cp311-*"]
+build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
 build-frontend = "build"
 build-verbosity = 1
 test-command = "pytest {project}/tests/test_import.py"
 test-requires = ["numpy", "pytest", "pytest-cov", "pytest-benchmark"]
 
 [tool.cibuildwheel.linux]
 before-all = [
```

### Comparing `pyclesperanto-0.6.6/scripts/build-opencl-linux.sh` & `pyclesperanto-0.6.7/scripts/build-opencl-linux.sh`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/scripts/build-opencl-macos.sh` & `pyclesperanto-0.6.7/scripts/build-opencl-macos.sh`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/scripts/build-opencl-windows.sh` & `pyclesperanto-0.6.7/scripts/build-opencl-windows.sh`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/scripts/generate-tiers-package.ipynb` & `pyclesperanto-0.6.7/scripts/generate-tiers-package.ipynb`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/setup.py` & `pyclesperanto-0.6.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -45,21 +45,15 @@
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Scientific/Engineering :: Image Processing",
         "Topic :: Scientific/Engineering :: Information Analysis",
-        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: BSD License",
     ],
     project_urls={
         "Documentation": "https://github.com/clEsperanto/pyclesperanto#README.md",
         "Source": "https://github.com/clEsperanto/pyclesperanto/",
         "Issues": "https://github.com/clEsperanto/pyclesperanto/issues",
```

### Comparing `pyclesperanto-0.6.6/wrapper/cleEnumType.cpp` & `pyclesperanto-0.6.7/wrapper/cleEnumType.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/wrapper/cleGateway.cpp` & `pyclesperanto-0.6.7/wrapper/cleGateway.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/wrapper/cleImage.cpp` & `pyclesperanto-0.6.7/wrapper/cleImage.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/wrapper/cleMemory.cpp` & `pyclesperanto-0.6.7/wrapper/cleMemory.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,17 @@
     }
     else if (pybind11::dtype::from_args(dtype).is(pybind11::dtype("uint8")))
     {
         return cle::Memory::AllocateMemory(device, c_shape, cle::DataType::UINT8, mtype);
     }
     else
     {
-        throw std::runtime_error("Unsupported data type");
+        std::cerr << "Warning: Unknown data type. Using float32 as default." << std::endl;
+        return cle::Memory::AllocateMemory(device, c_shape, cle::DataType::FLOAT32, mtype);
+        // throw std::runtime_error("Unsupported data type");
     }
 }
 
 template <typename Type>
 auto Push(const std::shared_ptr<cle::Processor> &device, const pybind11::array_t<Type, pybind11::array::c_style | pybind11::array::forcecast> &nd_array, const cle::MemoryType &mtype) -> cle::Image
 {
     pybind11::buffer_info arr = nd_array.request();
```

### Comparing `pyclesperanto-0.6.6/wrapper/cleProcessor.cpp` & `pyclesperanto-0.6.7/wrapper/cleProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/wrapper/cleTier1.cpp` & `pyclesperanto-0.6.7/wrapper/cleTier1.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/wrapper/cleTier2.cpp` & `pyclesperanto-0.6.7/wrapper/cleTier2.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.6.6/wrapper/cleTier3.cpp` & `pyclesperanto-0.6.7/wrapper/cleTier3.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -6,9 +6,9 @@
       m.def("_DifferenceOfGaussianKernel_Call", &cle::DifferenceOfGaussianKernel_Call, "", pybind11::arg("device"),
             pybind11::arg("src"), pybind11::arg("dst"), pybind11::arg("sigma1_x"), pybind11::arg("sigma1_y"), pybind11::arg("sigma1_z"), pybind11::arg("sigma2_x"), pybind11::arg("sigma2_y"), pybind11::arg("sigma2_z"));
 
       m.def("_CloseIndexGapsInLabelMapKernel_Call", &cle::CloseIndexGapsInLabelMapKernel_Call, pybind11::arg("device"),
             "", pybind11::arg("src"), pybind11::arg("dst"), pybind11::arg("value"));
 
       m.def("_HistogramKernel_Call", &cle::HistogramKernel_Call, "", pybind11::arg("device"), pybind11::arg("src"),
-            pybind11::arg("dst"), pybind11::arg("min_intensity"), pybind11::arg("max_intensity"), pybind11::arg("bins"));
-}
+            pybind11::arg("dst"), pybind11::arg("bin"), pybind11::arg("min_intensity"), pybind11::arg("max_intensity"));
+}
```

### Comparing `pyclesperanto-0.6.6/wrapper/pyclesperanto.hpp` & `pyclesperanto-0.6.7/wrapper/pyclesperanto.hpp`

 * *Files identical despite different names*

