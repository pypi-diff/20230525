# Comparing `tmp/ANNarchy-4.7.2.2.tar.gz` & `tmp/ANNarchy-4.7.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANNarchy-4.7.2.2.tar", last modified: Wed Mar 15 15:06:26 2023, max compression
+gzip compressed data, was "ANNarchy-4.7.2.3.tar", last modified: Thu May 25 07:32:25 2023, max compression
```

## Comparing `ANNarchy-4.7.2.2.tar` & `ANNarchy-4.7.2.3.tar`

### file list

```diff
@@ -1,269 +1,273 @@
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.393387 ANNarchy-4.7.2.2/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.342659 ANNarchy-4.7.2.2/ANNarchy/
--rw-r--r--   0 vitay      (501) staff       (20)     1989 2023-03-08 10:59:19.000000 ANNarchy-4.7.2.2/ANNarchy/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.348494 ANNarchy-4.7.2.2/ANNarchy/core/
--rw-r--r--   0 vitay      (501) staff       (20)    27962 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/core/ConnectorMethods.py
--rw-r--r--   0 vitay      (501) staff       (20)    13851 2022-12-14 10:26:52.000000 ANNarchy-4.7.2.2/ANNarchy/core/Dendrite.py
--rw-r--r--   0 vitay      (501) staff       (20)    28338 2022-12-14 10:45:42.000000 ANNarchy-4.7.2.2/ANNarchy/core/Global.py
--rw-r--r--   0 vitay      (501) staff       (20)    19614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/IO.py
--rw-r--r--   0 vitay      (501) staff       (20)    35087 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/Monitor.py
--rw-r--r--   0 vitay      (501) staff       (20)    34361 2023-03-08 10:56:07.000000 ANNarchy-4.7.2.2/ANNarchy/core/Network.py
--rw-r--r--   0 vitay      (501) staff       (20)     7309 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/NetworkManager.py
--rw-r--r--   0 vitay      (501) staff       (20)     8453 2023-03-08 10:56:07.000000 ANNarchy-4.7.2.2/ANNarchy/core/Neuron.py
--rw-r--r--   0 vitay      (501) staff       (20)    32634 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/Population.py
--rw-r--r--   0 vitay      (501) staff       (20)    12829 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/core/PopulationView.py
--rw-r--r--   0 vitay      (501) staff       (20)     6876 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/Profiler.py
--rw-r--r--   0 vitay      (501) staff       (20)    65190 2023-03-08 10:56:07.000000 ANNarchy-4.7.2.2/ANNarchy/core/Projection.py
--rw-r--r--   0 vitay      (501) staff       (20)     8383 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.2/ANNarchy/core/Random.py
--rw-r--r--   0 vitay      (501) staff       (20)    10098 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/Simulate.py
--rw-r--r--   0 vitay      (501) staff       (20)    95403 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/SpecificPopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)    15140 2022-10-11 07:59:47.000000 ANNarchy-4.7.2.2/ANNarchy/core/SpecificProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)     5803 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/ANNarchy/core/Synapse.py
--rw-r--r--   0 vitay      (501) staff       (20)     3463 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)        1 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/ANNarchy/core/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.349351 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/
--rw-r--r--   0 vitay      (501) staff       (20)     1683 2022-05-18 09:30:59.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Connector.pxd
--rw-r--r--   0 vitay      (501) staff       (20)    21582 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Connector.pyx
--rw-r--r--   0 vitay      (501) staff       (20)      924 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Coordinates.pxd
--rw-r--r--   0 vitay      (501) staff       (20)     4941 2022-01-07 10:51:43.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Coordinates.pyx
--rw-r--r--   0 vitay      (501) staff       (20)     2866 2022-02-02 12:38:23.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Transformations.pyx
--rw-r--r--   0 vitay      (501) staff       (20)        0 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/__init__.pxd
--rw-r--r--   0 vitay      (501) staff       (20)      405 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.349584 ANNarchy-4.7.2.2/ANNarchy/extensions/
--rw-r--r--   0 vitay      (501) staff       (20)       21 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.350096 ANNarchy-4.7.2.2/ANNarchy/extensions/ann_to_snn_conversion/
--rw-r--r--   0 vitay      (501) staff       (20)     9131 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
--rw-r--r--   0 vitay      (501) staff       (20)     3621 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
--rw-r--r--   0 vitay      (501) staff       (20)       48 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.351271 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/
--rw-r--r--   0 vitay      (501) staff       (20)    12839 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/AccProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)     2928 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/BoldModel.py
--rw-r--r--   0 vitay      (501) staff       (20)    10439 2023-03-08 10:56:07.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/BoldMonitor.py
--rw-r--r--   0 vitay      (501) staff       (20)    15160 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/NormProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)    27888 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/PredefinedModels.py
--rw-r--r--   0 vitay      (501) staff       (20)      386 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/bold/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.353534 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/
--rw-r--r--   0 vitay      (501) staff       (20)    42897 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Convolve.py
--rw-r--r--   0 vitay      (501) staff       (20)     3005 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/ConvolveTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     9368 2023-03-08 10:59:39.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Copy.py
--rw-r--r--   0 vitay      (501) staff       (20)     4502 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/CopyTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    24982 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Pooling.py
--rw-r--r--   0 vitay      (501) staff       (20)    14070 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/PoolingTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    14093 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Transpose.py
--rw-r--r--   0 vitay      (501) staff       (20)     1583 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)      858 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.353906 ANNarchy-4.7.2.2/ANNarchy/extensions/diagonal/
--rw-r--r--   0 vitay      (501) staff       (20)    16351 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/diagonal/DiagonalProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)       50 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/diagonal/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.354488 ANNarchy-4.7.2.2/ANNarchy/extensions/hybrid/
--rw-r--r--   0 vitay      (501) staff       (20)    20781 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/hybrid/HybridPopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       72 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/hybrid/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.354906 ANNarchy-4.7.2.2/ANNarchy/extensions/image/
--rw-r--r--   0 vitay      (501) staff       (20)     9944 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/image/ImagePopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       62 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/image/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.355405 ANNarchy-4.7.2.2/ANNarchy/extensions/tensorboard/
--rw-r--r--   0 vitay      (501) staff       (20)    12742 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/tensorboard/Logger.py
--rw-r--r--   0 vitay      (501) staff       (20)       26 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/tensorboard/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.355828 ANNarchy-4.7.2.2/ANNarchy/extensions/weightsharing/
--rw-r--r--   0 vitay      (501) staff       (20)    51579 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/weightsharing/SharedProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)      206 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.2/ANNarchy/extensions/weightsharing/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.358313 ANNarchy-4.7.2.2/ANNarchy/generator/
--rw-r--r--   0 vitay      (501) staff       (20)    42289 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/CodeGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    38169 2023-02-02 10:33:27.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Compiler.py
--rw-r--r--   0 vitay      (501) staff       (20)    10654 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/generator/MonitorGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.360077 ANNarchy-4.7.2.2/ANNarchy/generator/Population/
--rw-r--r--   0 vitay      (501) staff       (20)    59484 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/CUDAGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    26498 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/CUDATemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    41946 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/OpenMPGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    14427 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/OpenMPTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    20938 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/PopulationGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    37140 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/SingleThreadGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    13356 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/SingleThreadTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)      142 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Population/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.361026 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/
--rw-r--r--   0 vitay      (501) staff       (20)    14883 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/CPP11Profile.py
--rw-r--r--   0 vitay      (501) staff       (20)     8646 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/CUDAProfile.py
--rw-r--r--   0 vitay      (501) staff       (20)     6963 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/PAPIProfile.py
--rw-r--r--   0 vitay      (501) staff       (20)     3947 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/ProfileGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    31714 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/ProfileTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)      159 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Profile/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.363392 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.366540 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/
--rw-r--r--   0 vitay      (501) staff       (20)    14633 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    11089 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    11052 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    36964 2023-02-02 10:33:27.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    13010 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
--rw-r--r--   0 vitay      (501) staff       (20)    12651 2023-03-08 10:56:07.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    15654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
--rw-r--r--   0 vitay      (501) staff       (20)    19628 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)    11220 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    15997 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)    15664 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)     8341 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/HYB.py
--rw-r--r--   0 vitay      (501) staff       (20)    10511 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1514 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    71166 2023-03-08 10:56:07.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDAGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.369156 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/
--rw-r--r--   0 vitay      (501) staff       (20)     8715 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    13744 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)     3654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    37572 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)     8436 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR_P.py
--rw-r--r--   0 vitay      (501) staff       (20)     8172 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     6031 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
--rw-r--r--   0 vitay      (501) staff       (20)    19185 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)     4756 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     8759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     5111 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)    51527 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/LIL.py
--rw-r--r--   0 vitay      (501) staff       (20)    22149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/LIL_P.py
--rw-r--r--   0 vitay      (501) staff       (20)     4136 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1565 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    60362 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMPGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    49850 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/ProjectionGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.371555 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/
--rw-r--r--   0 vitay      (501) staff       (20)     8717 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    11194 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)     3413 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    37503 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)     7292 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    17125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)     4489 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
--rw-r--r--   0 vitay      (501) staff       (20)     4792 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     4570 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     8588 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)    14808 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)     4607 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/HYB.py
--rw-r--r--   0 vitay      (501) staff       (20)    45456 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/LIL.py
--rw-r--r--   0 vitay      (501) staff       (20)     4120 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1671 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    57762 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThreadGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)      233 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Projection/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    54049 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/PyxGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    15018 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Sanity.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.373035 ANNarchy-4.7.2.2/ANNarchy/generator/Template/
--rw-r--r--   0 vitay      (501) staff       (20)    29830 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Template/BaseTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    16113 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Template/GlobalOperationTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     2426 2023-03-08 12:12:59.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Template/MakefileTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    19390 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Template/MonitorTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    14699 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Template/PyxTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)        0 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Template/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    15650 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/generator/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)       30 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.2/ANNarchy/generator/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.379047 ANNarchy-4.7.2.2/ANNarchy/include/
--rw-r--r--   0 vitay      (501) staff       (20)    26125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/BSRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     6674 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/BSRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    17338 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/include/COOMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8165 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/COOMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9119 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8274 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     7660 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrixCUDAT.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    22237 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrixT.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    21843 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/include/CSRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8971 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/CSRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    30517 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/DenseMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8778 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/DenseMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    10925 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/DenseMatrixOffsets.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    32735 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/ELLMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9264 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/ELLMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    30967 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/ELLRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    10305 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/ELLRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    19241 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/HYBMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     5284 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/HYBMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9991 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/include/LILInvMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    37614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/LILMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    23769 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/include/PartitionedMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    25554 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/SELLMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9628 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/include/SELLMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     1092 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/include/Specific.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     1430 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/ANNarchy/include/helper_functions.hpp
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.380028 ANNarchy-4.7.2.2/ANNarchy/models/
--rw-r--r--   0 vitay      (501) staff       (20)    45126 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.2/ANNarchy/models/Neurons.py
--rw-r--r--   0 vitay      (501) staff       (20)    11837 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.2/ANNarchy/models/Synapses.py
--rw-r--r--   0 vitay      (501) staff       (20)      352 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/ANNarchy/models/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.382700 ANNarchy-4.7.2.2/ANNarchy/parser/
--rw-r--r--   0 vitay      (501) staff       (20)    14933 2022-12-14 10:44:43.000000 ANNarchy-4.7.2.2/ANNarchy/parser/AnalyseNeuron.py
--rw-r--r--   0 vitay      (501) staff       (20)    21510 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/parser/AnalyseSynapse.py
--rw-r--r--   0 vitay      (501) staff       (20)    14105 2022-12-14 10:44:52.000000 ANNarchy-4.7.2.2/ANNarchy/parser/CoupledEquations.py
--rw-r--r--   0 vitay      (501) staff       (20)    28867 2023-01-25 13:19:23.000000 ANNarchy-4.7.2.2/ANNarchy/parser/Equation.py
--rw-r--r--   0 vitay      (501) staff       (20)    28842 2023-01-25 13:19:23.000000 ANNarchy-4.7.2.2/ANNarchy/parser/Extraction.py
--rw-r--r--   0 vitay      (501) staff       (20)     4336 2022-12-05 16:13:02.000000 ANNarchy-4.7.2.2/ANNarchy/parser/Function.py
--rw-r--r--   0 vitay      (501) staff       (20)     6049 2022-12-05 16:13:18.000000 ANNarchy-4.7.2.2/ANNarchy/parser/ITE.py
--rw-r--r--   0 vitay      (501) staff       (20)     3032 2023-01-22 11:22:00.000000 ANNarchy-4.7.2.2/ANNarchy/parser/ParserTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     7633 2022-12-05 16:13:32.000000 ANNarchy-4.7.2.2/ANNarchy/parser/StringManipulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       86 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/ANNarchy/parser/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.384235 ANNarchy-4.7.2.2/ANNarchy/parser/report/
--rw-r--r--   0 vitay      (501) staff       (20)    16861 2023-01-25 15:17:04.000000 ANNarchy-4.7.2.2/ANNarchy/parser/report/LatexParser.py
--rw-r--r--   0 vitay      (501) staff       (20)    22678 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/ANNarchy/parser/report/LatexReport.py
--rw-r--r--   0 vitay      (501) staff       (20)    15846 2021-04-01 06:34:12.000000 ANNarchy-4.7.2.2/ANNarchy/parser/report/MarkdownReport.py
--rw-r--r--   0 vitay      (501) staff       (20)     1985 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.2/ANNarchy/parser/report/Report.py
--rw-r--r--   0 vitay      (501) staff       (20)        0 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/ANNarchy/parser/report/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.384346 ANNarchy-4.7.2.2/ANNarchy/thirdparty/
--rw-r--r--   0 vitay      (501) staff       (20)    26759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/ANNarchy/thirdparty/randutils.hpp
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.343715 ANNarchy-4.7.2.2/ANNarchy.egg-info/
--rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-03-15 15:06:26.000000 ANNarchy-4.7.2.2/ANNarchy.egg-info/PKG-INFO
--rw-r--r--   0 vitay      (501) staff       (20)     8558 2023-03-15 15:06:26.000000 ANNarchy-4.7.2.2/ANNarchy.egg-info/SOURCES.txt
--rw-r--r--   0 vitay      (501) staff       (20)        1 2023-03-15 15:06:26.000000 ANNarchy-4.7.2.2/ANNarchy.egg-info/dependency_links.txt
--rw-r--r--   0 vitay      (501) staff       (20)        1 2021-04-13 07:32:27.000000 ANNarchy-4.7.2.2/ANNarchy.egg-info/not-zip-safe
--rw-r--r--   0 vitay      (501) staff       (20)       36 2023-03-15 15:06:26.000000 ANNarchy-4.7.2.2/ANNarchy.egg-info/requires.txt
--rw-r--r--   0 vitay      (501) staff       (20)        9 2023-03-15 15:06:26.000000 ANNarchy-4.7.2.2/ANNarchy.egg-info/top_level.txt
--rw-r--r--   0 vitay      (501) staff       (20)    18092 2017-07-25 21:20:59.000000 ANNarchy-4.7.2.2/LICENSE
--rw-r--r--   0 vitay      (501) staff       (20)      274 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.2/MANIFEST.in
--rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-03-15 15:06:26.393462 ANNarchy-4.7.2.2/PKG-INFO
--rw-r--r--   0 vitay      (501) staff       (20)     1803 2023-03-08 10:57:16.000000 ANNarchy-4.7.2.2/README.md
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.341180 ANNarchy-4.7.2.2/examples/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.384691 ANNarchy-4.7.2.2/examples/ann_to_snn/
--rw-r--r--   0 vitay      (501) staff       (20)      991 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/examples/ann_to_snn/demo.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.385378 ANNarchy-4.7.2.2/examples/bar_learning/
--rw-r--r--   0 vitay      (501) staff       (20)     1844 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/examples/bar_learning/BarLearning.py
--rw-r--r--   0 vitay      (501) staff       (20)     2104 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.2/examples/bar_learning/BarLearningGPU.py
--rw-r--r--   0 vitay      (501) staff       (20)     1610 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.2/examples/bar_learning/Viz.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.385858 ANNarchy-4.7.2.2/examples/bold_monitor/
--rw-r--r--   0 vitay      (501) staff       (20)     2529 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.2/examples/bold_monitor/BOLD.py
--rw-r--r--   0 vitay      (501) staff       (20)     3003 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.2/examples/bold_monitor/BOLD_two_inputs.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.386142 ANNarchy-4.7.2.2/examples/gap_junctions/
--rw-r--r--   0 vitay      (501) staff       (20)      888 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/examples/gap_junctions/GapJunctions.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.386389 ANNarchy-4.7.2.2/examples/hodgkin_huxley/
--rw-r--r--   0 vitay      (501) staff       (20)     2496 2023-01-25 13:19:23.000000 ANNarchy-4.7.2.2/examples/hodgkin_huxley/HodgkinHuxley.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.386865 ANNarchy-4.7.2.2/examples/homeostatic_stdp/
--rw-r--r--   0 vitay      (501) staff       (20)     5062 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/homeostatic_stdp/Ramp.py
--rw-r--r--   0 vitay      (501) staff       (20)     7059 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/homeostatic_stdp/SORF.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.387066 ANNarchy-4.7.2.2/examples/hybrid/
--rw-r--r--   0 vitay      (501) staff       (20)     2865 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/hybrid/Hybrid.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.387615 ANNarchy-4.7.2.2/examples/image/
--rw-r--r--   0 vitay      (501) staff       (20)     6193 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/examples/image/Image.py
--rw-r--r--   0 vitay      (501) staff       (20)     7210 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/examples/image/Webcam.ipynb
--rw-r--r--   0 vitay      (501) staff       (20)     2959 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/examples/image/Webcam.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.387889 ANNarchy-4.7.2.2/examples/izhikevich/
--rw-r--r--   0 vitay      (501) staff       (20)     1901 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.2/examples/izhikevich/Izhikevich.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.388108 ANNarchy-4.7.2.2/examples/multinetwork/
--rw-r--r--   0 vitay      (501) staff       (20)     1973 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.2/examples/multinetwork/MultiNetwork.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.388641 ANNarchy-4.7.2.2/examples/neural_field/
--rw-r--r--   0 vitay      (501) staff       (20)     1849 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/examples/neural_field/BubbleWorld.pyx
--rw-r--r--   0 vitay      (501) staff       (20)     1490 2020-03-10 16:42:35.000000 ANNarchy-4.7.2.2/examples/neural_field/NeuralField.py
--rw-r--r--   0 vitay      (501) staff       (20)     2281 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.2/examples/neural_field/Viz.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.389905 ANNarchy-4.7.2.2/examples/pyNN/
--rw-r--r--   0 vitay      (501) staff       (20)     1644 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/pyNN/AEIF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     2251 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/pyNN/EIF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1427 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/pyNN/IF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1361 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/pyNN/IF_curr_alpha.py
--rw-r--r--   0 vitay      (501) staff       (20)     1316 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/pyNN/non_linear_synapse.py
--rw-r--r--   0 vitay      (501) staff       (20)     2646 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/pyNN/short_term_plasticity2.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.390064 ANNarchy-4.7.2.2/examples/refractoriness/
--rw-r--r--   0 vitay      (501) staff       (20)     1070 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/refractoriness/Refractoriness.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.390224 ANNarchy-4.7.2.2/examples/simple_stdp/
--rw-r--r--   0 vitay      (501) staff       (20)     2208 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/examples/simple_stdp/SimpleSTDPModel.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.390392 ANNarchy-4.7.2.2/examples/structural_plasticity/
--rw-r--r--   0 vitay      (501) staff       (20)     1923 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/examples/structural_plasticity/StructuralPlasticity.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.392298 ANNarchy-4.7.2.2/examples/tensorboard/
--rw-r--r--   0 vitay      (501) staff       (20)  1014400 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.2/examples/tensorboard/BasalGanglia.ipynb
--rw-r--r--   0 vitay      (501) staff       (20)   208036 2021-07-27 06:26:43.000000 ANNarchy-4.7.2.2/examples/tensorboard/BayesianOptimization.ipynb
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.392703 ANNarchy-4.7.2.2/examples/tsodyks_markram/
--rw-r--r--   0 vitay      (501) staff       (20)     3872 2020-09-29 13:24:31.000000 ANNarchy-4.7.2.2/examples/tsodyks_markram/TsodyksMarkram.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-03-15 15:06:26.393181 ANNarchy-4.7.2.2/examples/vogels_abbott/
--rw-r--r--   0 vitay      (501) staff       (20)     1940 2020-09-29 13:24:31.000000 ANNarchy-4.7.2.2/examples/vogels_abbott/COBA.py
--rw-r--r--   0 vitay      (501) staff       (20)     1809 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.2/examples/vogels_abbott/CUBA.py
--rw-r--r--   0 vitay      (501) staff       (20)       82 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.2/requirements.txt
--rw-r--r--   0 vitay      (501) staff       (20)      101 2023-03-15 15:06:26.393684 ANNarchy-4.7.2.2/setup.cfg
--rw-r--r--   0 vitay      (501) staff       (20)    10946 2023-03-08 10:58:38.000000 ANNarchy-4.7.2.2/setup.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.868828 ANNarchy-4.7.2.3/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.819674 ANNarchy-4.7.2.3/ANNarchy/
+-rw-r--r--   0 vitay      (501) staff       (20)     1989 2023-05-25 07:29:05.000000 ANNarchy-4.7.2.3/ANNarchy/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.825003 ANNarchy-4.7.2.3/ANNarchy/core/
+-rw-r--r--   0 vitay      (501) staff       (20)    27962 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/ConnectorMethods.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13851 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Dendrite.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28338 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Global.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/IO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    35087 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/Monitor.py
+-rw-r--r--   0 vitay      (501) staff       (20)    34361 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/Network.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7309 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/NetworkManager.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8453 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/Neuron.py
+-rw-r--r--   0 vitay      (501) staff       (20)    32634 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Population.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12829 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/PopulationView.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6876 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Profiler.py
+-rw-r--r--   0 vitay      (501) staff       (20)    65222 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/core/Projection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8383 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/ANNarchy/core/Random.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10098 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/Simulate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    95403 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/SpecificPopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/SpecificProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5803 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/Synapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3463 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/core/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.825823 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/
+-rw-r--r--   0 vitay      (501) staff       (20)     1683 2022-05-18 09:30:59.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)    21582 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)      924 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)     4941 2022-01-07 10:51:43.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)     2866 2022-02-02 12:38:23.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Transformations.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/__init__.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)      405 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.826001 ANNarchy-4.7.2.3/ANNarchy/extensions/
+-rw-r--r--   0 vitay      (501) staff       (20)       21 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.826455 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/
+-rw-r--r--   0 vitay      (501) staff       (20)     9131 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3621 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
+-rw-r--r--   0 vitay      (501) staff       (20)       48 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.827787 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/
+-rw-r--r--   0 vitay      (501) staff       (20)    12839 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/AccProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2928 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldModel.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10439 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldMonitor.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15160 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/NormProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)    27888 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/PredefinedModels.py
+-rw-r--r--   0 vitay      (501) staff       (20)      386 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.829730 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/
+-rw-r--r--   0 vitay      (501) staff       (20)    42897 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Convolve.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3005 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/ConvolveTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     9368 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Copy.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4502 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/CopyTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    24982 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Pooling.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14070 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/PoolingTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14093 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Transpose.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1583 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)      858 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.830069 ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/
+-rw-r--r--   0 vitay      (501) staff       (20)    16351 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/DiagonalProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)       50 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.830458 ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/
+-rw-r--r--   0 vitay      (501) staff       (20)    20781 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/HybridPopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       72 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.830909 ANNarchy-4.7.2.3/ANNarchy/extensions/image/
+-rw-r--r--   0 vitay      (501) staff       (20)     9944 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/image/ImagePopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       62 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/image/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.831357 ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/
+-rw-r--r--   0 vitay      (501) staff       (20)    12742 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/Logger.py
+-rw-r--r--   0 vitay      (501) staff       (20)       26 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.832106 ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/
+-rw-r--r--   0 vitay      (501) staff       (20)    51579 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/SharedProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)      206 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.834235 ANNarchy-4.7.2.3/ANNarchy/generator/
+-rw-r--r--   0 vitay      (501) staff       (20)    42289 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/CodeGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    38169 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Compiler.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10654 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/MonitorGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.835903 ANNarchy-4.7.2.3/ANNarchy/generator/Population/
+-rw-r--r--   0 vitay      (501) staff       (20)    59484 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDAGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    26498 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDATemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    41946 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14427 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    20938 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/PopulationGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13356 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)      142 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.836799 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/
+-rw-r--r--   0 vitay      (501) staff       (20)    14883 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CPP11Profile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8646 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CUDAProfile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6963 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/PAPIProfile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3947 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    31714 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)      159 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.838911 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.841756 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/
+-rw-r--r--   0 vitay      (501) staff       (20)    14633 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11089 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11052 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    36964 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13010 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12651 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19628 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11220 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15997 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15664 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8341 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/HYB.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10511 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1514 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    72468 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDAGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.844078 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/
+-rw-r--r--   0 vitay      (501) staff       (20)     8715 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13744 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37572 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8436 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8172 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6031 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19185 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4756 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5111 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    51527 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4136 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1565 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    60579 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMPGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    49850 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/ProjectionGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.847124 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/
+-rw-r--r--   0 vitay      (501) staff       (20)     8717 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11194 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3413 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37503 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7292 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    17125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4489 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4792 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4570 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8588 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14808 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4607 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/HYB.py
+-rw-r--r--   0 vitay      (501) staff       (20)    45456 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/LIL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4120 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1671 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    57963 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThreadGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)      233 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    54049 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/PyxGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15018 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Sanity.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.848614 ANNarchy-4.7.2.3/ANNarchy/generator/Template/
+-rw-r--r--   0 vitay      (501) staff       (20)    29830 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/BaseTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    16113 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/GlobalOperationTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2426 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/MakefileTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19390 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/MonitorTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14699 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/PyxTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15650 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)       30 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/generator/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.853227 ANNarchy-4.7.2.3/ANNarchy/include/
+-rw-r--r--   0 vitay      (501) staff       (20)    26125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     6674 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    17338 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/COOMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8165 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/COOMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9119 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8274 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     7660 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDAT.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    22237 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixT.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    21843 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8971 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    30517 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8778 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10925 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixOffsets.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    32735 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9264 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    30967 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10305 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    19241 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     5284 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9991 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/LILInvMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    37614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/LILMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    23769 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/PartitionedMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    25554 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9628 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     1092 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/Specific.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     1430 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/helper_functions.hpp
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.854385 ANNarchy-4.7.2.3/ANNarchy/models/
+-rw-r--r--   0 vitay      (501) staff       (20)    45126 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/models/Neurons.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11837 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/models/Synapses.py
+-rw-r--r--   0 vitay      (501) staff       (20)      352 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/models/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.857325 ANNarchy-4.7.2.3/ANNarchy/parser/
+-rw-r--r--   0 vitay      (501) staff       (20)    15017 2023-05-24 12:05:12.000000 ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseNeuron.py
+-rw-r--r--   0 vitay      (501) staff       (20)    21586 2023-05-24 12:08:11.000000 ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseSynapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14166 2023-05-24 12:05:32.000000 ANNarchy-4.7.2.3/ANNarchy/parser/CoupledEquations.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28868 2023-05-24 12:05:45.000000 ANNarchy-4.7.2.3/ANNarchy/parser/Equation.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28842 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/parser/Extraction.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4336 2022-12-05 16:13:02.000000 ANNarchy-4.7.2.3/ANNarchy/parser/Function.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6049 2022-12-05 16:13:18.000000 ANNarchy-4.7.2.3/ANNarchy/parser/ITE.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3032 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/parser/ParserTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7633 2022-12-05 16:13:32.000000 ANNarchy-4.7.2.3/ANNarchy/parser/StringManipulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       86 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/parser/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.858782 ANNarchy-4.7.2.3/ANNarchy/parser/report/
+-rw-r--r--   0 vitay      (501) staff       (20)    16861 2023-01-25 15:17:04.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexParser.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22678 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexReport.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15846 2021-04-01 06:34:12.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/MarkdownReport.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1985 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/Report.py
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.858864 ANNarchy-4.7.2.3/ANNarchy/thirdparty/
+-rw-r--r--   0 vitay      (501) staff       (20)    26759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/thirdparty/randutils.hpp
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.820472 ANNarchy-4.7.2.3/ANNarchy.egg-info/
+-rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/PKG-INFO
+-rw-r--r--   0 vitay      (501) staff       (20)     8626 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2021-04-13 07:32:27.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/not-zip-safe
+-rw-r--r--   0 vitay      (501) staff       (20)       36 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/requires.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        9 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/top_level.txt
+-rw-r--r--   0 vitay      (501) staff       (20)    18092 2017-07-25 21:20:59.000000 ANNarchy-4.7.2.3/LICENSE
+-rw-r--r--   0 vitay      (501) staff       (20)      274 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/MANIFEST.in
+-rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-05-25 07:32:25.868924 ANNarchy-4.7.2.3/PKG-INFO
+-rw-r--r--   0 vitay      (501) staff       (20)     1803 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/README.md
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.818329 ANNarchy-4.7.2.3/examples/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.859231 ANNarchy-4.7.2.3/examples/ann_to_snn/
+-rw-r--r--   0 vitay      (501) staff       (20)      991 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/examples/ann_to_snn/demo.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.859916 ANNarchy-4.7.2.3/examples/bar_learning/
+-rw-r--r--   0 vitay      (501) staff       (20)     1844 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/bar_learning/BarLearning.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2104 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/examples/bar_learning/BarLearningGPU.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1610 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/examples/bar_learning/Viz.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.860384 ANNarchy-4.7.2.3/examples/bold_monitor/
+-rw-r--r--   0 vitay      (501) staff       (20)     2529 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.3/examples/bold_monitor/BOLD.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3003 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.3/examples/bold_monitor/BOLD_two_inputs.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.860583 ANNarchy-4.7.2.3/examples/gap_junctions/
+-rw-r--r--   0 vitay      (501) staff       (20)      888 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/gap_junctions/GapJunctions.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.860816 ANNarchy-4.7.2.3/examples/hodgkin_huxley/
+-rw-r--r--   0 vitay      (501) staff       (20)     2496 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/examples/hodgkin_huxley/HodgkinHuxley.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.861264 ANNarchy-4.7.2.3/examples/homeostatic_stdp/
+-rw-r--r--   0 vitay      (501) staff       (20)     5062 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/homeostatic_stdp/Ramp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7059 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/homeostatic_stdp/SORF.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.861512 ANNarchy-4.7.2.3/examples/hybrid/
+-rw-r--r--   0 vitay      (501) staff       (20)     2865 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/hybrid/Hybrid.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.862109 ANNarchy-4.7.2.3/examples/image/
+-rw-r--r--   0 vitay      (501) staff       (20)     6193 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/examples/image/Image.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7210 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/examples/image/Webcam.ipynb
+-rw-r--r--   0 vitay      (501) staff       (20)     2959 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/examples/image/Webcam.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.862337 ANNarchy-4.7.2.3/examples/izhikevich/
+-rw-r--r--   0 vitay      (501) staff       (20)     1901 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/examples/izhikevich/Izhikevich.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.862522 ANNarchy-4.7.2.3/examples/multinetwork/
+-rw-r--r--   0 vitay      (501) staff       (20)     1973 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/examples/multinetwork/MultiNetwork.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.863233 ANNarchy-4.7.2.3/examples/neural_field/
+-rw-r--r--   0 vitay      (501) staff       (20)     1849 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/examples/neural_field/BubbleWorld.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)     1490 2020-03-10 16:42:35.000000 ANNarchy-4.7.2.3/examples/neural_field/NeuralField.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2281 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/examples/neural_field/Viz.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864318 ANNarchy-4.7.2.3/examples/pyNN/
+-rw-r--r--   0 vitay      (501) staff       (20)     1644 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/AEIF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2251 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/EIF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1427 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/IF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1361 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/IF_curr_alpha.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1316 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/non_linear_synapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2646 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/short_term_plasticity2.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864461 ANNarchy-4.7.2.3/examples/refractoriness/
+-rw-r--r--   0 vitay      (501) staff       (20)     1070 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/refractoriness/Refractoriness.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864602 ANNarchy-4.7.2.3/examples/simple_stdp/
+-rw-r--r--   0 vitay      (501) staff       (20)     2208 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/simple_stdp/SimpleSTDPModel.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864742 ANNarchy-4.7.2.3/examples/structural_plasticity/
+-rw-r--r--   0 vitay      (501) staff       (20)     1923 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/structural_plasticity/StructuralPlasticity.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.866572 ANNarchy-4.7.2.3/examples/tensorboard/
+-rw-r--r--   0 vitay      (501) staff       (20)  1014400 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/tensorboard/BasalGanglia.ipynb
+-rw-r--r--   0 vitay      (501) staff       (20)   208036 2021-07-27 06:26:43.000000 ANNarchy-4.7.2.3/examples/tensorboard/BayesianOptimization.ipynb
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.867072 ANNarchy-4.7.2.3/examples/tsodyks_markram/
+-rw-r--r--   0 vitay      (501) staff       (20)     3872 2023-04-12 10:39:20.000000 ANNarchy-4.7.2.3/examples/tsodyks_markram/TsodyksMarkram.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.867883 ANNarchy-4.7.2.3/examples/vogels_abbott/
+-rw-r--r--   0 vitay      (501) staff       (20)     1940 2020-09-29 13:24:31.000000 ANNarchy-4.7.2.3/examples/vogels_abbott/COBA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1809 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/vogels_abbott/CUBA.py
+-rw-r--r--   0 vitay      (501) staff       (20)       82 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/requirements.txt
+-rw-r--r--   0 vitay      (501) staff       (20)      101 2023-05-25 07:32:25.869173 ANNarchy-4.7.2.3/setup.cfg
+-rw-r--r--   0 vitay      (501) staff       (20)    10946 2023-05-25 07:28:05.000000 ANNarchy-4.7.2.3/setup.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.868586 ANNarchy-4.7.2.3/tests/
+-rw-r--r--   0 vitay      (501) staff       (20)     1122 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/tests/test_CUDA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1062 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/tests/test_openmp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/tests/test_single_thread.py
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/__init__.py` & `ANNarchy-4.7.2.3/ANNarchy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,11 +42,11 @@
 # if the script terminates
 import atexit
 atexit.register(check_profile_results)
 atexit.register(clear)
 
 # Version
 __version__ = '4.7'
-__release__ = '4.7.2.2'
+__release__ = '4.7.2.3'
 
 print( 'ANNarchy ' + __version__ + ' (' + __release__ + \
                     ') on ' + sys.platform + ' (' + os.name + ').' )
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/ConnectorMethods.py` & `ANNarchy-4.7.2.3/ANNarchy/core/ConnectorMethods.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Dendrite.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Dendrite.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Global.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Global.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/IO.py` & `ANNarchy-4.7.2.3/ANNarchy/core/IO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Monitor.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Monitor.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Network.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Network.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/NetworkManager.py` & `ANNarchy-4.7.2.3/ANNarchy/core/NetworkManager.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Neuron.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Neuron.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Population.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Population.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/PopulationView.py` & `ANNarchy-4.7.2.3/ANNarchy/core/PopulationView.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Profiler.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Profiler.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Projection.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
         else:
             # If the number of elements is too small, the split
             # might not be efficient.
             if self.post.size < Global.OMP_MIN_NB_NEURONS:
                 self._no_split_matrix = True
             else:
-                self._no_split_matrix = False
+                self._no_split_matrix = Global.config["disable_split_matrix"]
 
         # In particular for spiking models, the parallelization on the
         # inner or outer loop can make a performance difference
         if self._no_split_matrix:
             # LIL and CSR are parallelized on inner loop
             # to prevent cost of atomic operations
             self._parallel_pattern = 'inner_loop'
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Random.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Random.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Simulate.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Simulate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/SpecificPopulation.py` & `ANNarchy-4.7.2.3/ANNarchy/core/SpecificPopulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/SpecificProjection.py` & `ANNarchy-4.7.2.3/ANNarchy/core/SpecificProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Synapse.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Synapse.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/Utils.py` & `ANNarchy-4.7.2.3/ANNarchy/core/Utils.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Connector.pxd` & `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pxd`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Connector.pyx` & `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Coordinates.pxd` & `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pxd`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Coordinates.pyx` & `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/core/cython_ext/Transformations.pyx` & `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Transformations.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/bold/AccProjection.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/AccProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/bold/BoldModel.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldModel.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/bold/BoldMonitor.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldMonitor.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/bold/NormProjection.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/NormProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/bold/PredefinedModels.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/PredefinedModels.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Convolve.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Convolve.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/ConvolveTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/ConvolveTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Copy.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Copy.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/CopyTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/CopyTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Pooling.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Pooling.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/PoolingTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/PoolingTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Transpose.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Transpose.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/Utils.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Utils.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/convolution/__init__.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/diagonal/DiagonalProjection.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/DiagonalProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/hybrid/HybridPopulation.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/HybridPopulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/image/ImagePopulation.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/image/ImagePopulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/tensorboard/Logger.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/Logger.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/extensions/weightsharing/SharedProjection.py` & `ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/SharedProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/CodeGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/CodeGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Compiler.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Compiler.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/MonitorGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/MonitorGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/CUDAGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDAGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/CUDATemplates.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDATemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/OpenMPGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/OpenMPTemplates.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/PopulationGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/PopulationGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/SingleThreadGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Population/SingleThreadTemplates.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Profile/CPP11Profile.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CPP11Profile.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Profile/CUDAProfile.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CUDAProfile.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Profile/PAPIProfile.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/PAPIProfile.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Profile/ProfileGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Profile/ProfileTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/BSR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/BaseTemplates.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/COO.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/COO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/CSR_Vector.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/Dense.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/Dense_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/ELL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/ELLR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELLR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/HYB.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/HYB.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/SELL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/SELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDA/__init__.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/CUDAGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDAGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,21 +674,43 @@
         for var in proj.synapse_type.description['pre_spike']:
             if var['name'] == "g_target":   # synaptic transmission
                 # compute psp
                 psp_code += "%(float_prec)s tmp = %(psp)s\n" % {
                     'psp': var['cpp'].split('=')[1] % ids,
                     'float_prec': Global.config['precision']
                 }
+                # Operation (g_target is replaced by sum in 'cpp')
+                operation = re.search(r'sum (.*?)=', var['cpp']).group(1).strip() + "="
+                if operation == "+=":
+                    ids.update({'atomicOp': "atomicAdd"})
+                elif operation == "-=":
+                    ids.update({'atomicOp': "atomicSub"})
+                elif operation == "=":
+                    ids.update({'atomicOp': "atomicExch"})
+                else:
+                    Global._error("The operator '"+operation+"' is not supported in psp-statements on CUDA devices yet.")
+
                 # apply to all targets
                 target_list = proj.target if isinstance(proj.target, list) else [proj.target]
                 for target in sorted(list(set(target_list))):
-                    if proj._storage_order == "post_to_pre":
-                        psp_code += "atomicAdd(&g_%(target)s[post_rank], tmp);\n" % {'target': target}
+                    # multiple targets
+                    ids['target'] = target
+
+                    # Check for special cases
+                    if ids['atomicOp'] == "atomicExch" and Global._check_precision("double"):
+                        # HD (12th April 2023): atomicExch is not defined for double, so we need to use the long long type-cast version
+                        psp_code += "atomicExch((unsigned long long int*)&g_%(target)s%(post_index)s, __double_as_longlong(tmp));\n" % ids
                     else:
-                        psp_code += "atomicAdd(&g_%(target)s[col_idx[syn_idx]], tmp);\n" % {'target': target}
+                        psp_code += "%(atomicOp)s(&g_%(target)s%(post_index)s, tmp);\n" % ids
+
+                    # Boundary code is optional
+                    bound_code = get_bounds(var)
+                    if len(bound_code) != 0:
+                        bound_code = bound_code.replace("g_target%(local_index)s", "g_"+target+"%(post_index)s")
+                        psp_code += bound_code % ids
 
             else:
                 condition = ""
                 # Check conditions to update the variable
                 if var['name'] == 'w': # Surround it by the learning flag
                     condition = "plasticity"
 
@@ -1595,19 +1617,19 @@
 
             header_dict = {
                 'kernel_args': kernel_args_global,
             }
             header_dict.update(ids)
             header += self._templates['synapse_update']['global']['header'] % header_dict
 
-            call_dict = {
+            call_dict = deepcopy(ids)
+            call_dict.update({
                 'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
                 'kernel_args_call': kernel_args_call_global,
-            }
-            call_dict.update(ids)
+            })
             global_call = self._templates['synapse_update']['global']['call'] % call_dict
 
         if semiglobal_eq.strip() != '':
             body_dict = {
                 'kernel_args': kernel_args_semiglobal,
                 'semiglobal_eqs': semiglobal_eq,
                 'pre_loop': semiglobal_pre_code,
@@ -1617,19 +1639,19 @@
 
             header_dict = {
                 'kernel_args': kernel_args_semiglobal,
             }
             header_dict.update(ids)
             header += self._templates['synapse_update']['semiglobal']['header'] % header_dict
 
-            call_dict = {
+            call_dict = deepcopy(ids)
+            call_dict.update({
                 'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
                 'kernel_args_call': kernel_args_call_semiglobal,
-            }
-            call_dict.update(ids)
+            })
             semiglobal_call = self._templates['synapse_update']['semiglobal']['call'] % call_dict
 
         if local_eq.strip() != '':
             body_dict = {
                 'conn_args': conn_header,
                 'kernel_args': kernel_args_local,
                 'local_eqs': local_eq,
@@ -1641,27 +1663,27 @@
             header_dict = {
                 'conn_args': conn_header,
                 'kernel_args': kernel_args_local
             }
             header_dict.update(ids)
             header += self._templates['synapse_update']['local']['header'] % header_dict
 
-            call_dict = {
+            call_dict = deepcopy(ids)
+            call_dict.update({
                 'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
                 'conn_args_call': conn_call,
                 'kernel_args_call': kernel_args_call_local
-            }
-            call_dict.update(ids)
+            })
             local_call = self._templates['synapse_update']['local']['call'] % call_dict
 
         call = self._templates['synapse_update']['call'] % {
             'id_proj': proj.id,
             'post': proj.post.id,
             'pre': proj.pre.id,
-            'target': proj.target,
+            'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
             'global_call': global_call,
             'semiglobal_call': semiglobal_call,
             'local_call': local_call,
             'float_prec': Global.config['precision']
         }
 
         # Profiling
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/BSR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/COO.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/COO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR_P.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/Dense.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/Dense_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/ELL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/ELLR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELLR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/LIL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/LIL_P.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/SELL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/SELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMP/__init__.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/OpenMPGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMPGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
                 else:
                     if single_matrix:
                         self._templates.update(CSR_T_OpenMP.conn_templates)
                         self._template_ids.update(CSR_T_OpenMP.conn_ids)
                     else:
                         self._templates.update(CSR_T_Sliced_OpenMP.conn_templates)
                         self._template_ids.update(CSR_T_Sliced_OpenMP.conn_ids)
-        
+
         elif proj._storage_format == "coo":
             if proj.synapse_type.type == "rate":
                 # Rate-coded models coordinate format
                 if single_matrix:
                     self._templates.update(COO_OpenMP.conn_templates)
                     self._template_ids.update(COO_OpenMP.conn_ids)
                 else:
@@ -651,16 +651,16 @@
                         psp = psp.replace(
                             '%(pre_prefix)s'+var+'%(global_index)s',
                             '%(pre_prefix)s_delayed_'+var+'%(delay_u)s'
                         )
 
         # OpenMP run modifiers
         schedule = "" if not 'psp_schedule' in proj._omp_config.keys() else proj._omp_config['psp_schedule']
-        
-        # In case of a uniform delay we preload the variable and then provide as 
+
+        # In case of a uniform delay we preload the variable and then provide as
         # thread local argument to the worker threads
         pre_copy = ""
         first_privates = ""
         if proj.max_delay > 1 and proj.uniform_delay != -1:
 
             for var in dependencies:
                 if var in proj.pre.neuron_type.description['local']:
@@ -838,14 +838,16 @@
         # Analyse all elements of pre_spike
         for eq in proj.synapse_type.description['pre_spike']:
             # g_target is treated differently
             # Must be at the end of the equations
             if eq['name'] == 'g_target':
                 # PSP form
                 g_target = eq['cpp'].split('=')[1]
+                # Operation (g_target is replaced by sum in 'cpp')
+                operation = re.search(r'sum (.*?)=', eq['cpp']).group(1).strip() + "="
                 # Check targets
                 if isinstance(proj.target, str):
                     targets = [proj.target]
                 else:
                     targets = proj.target
                 g_target_code = ""
                 for target in targets:
@@ -858,26 +860,27 @@
                         )
 
                     target_dict = {
                         'post_prefix': ids['post_prefix'],
                         'target': target,
                         'g_target': g_target % ids,
                         'eq': eq['eq'],
-                        'post_index': ids['post_index']
+                        'post_index': ids['post_index'],
+                        'operation': operation
                     }
 
                     # access to post variable migth require atomic
                     # operation ( added later if needed )
                     if proj.max_delay > 1 and proj.uniform_delay == -1: # TODO: openMP is switched off for non uniform delays
                         g_target_code += """
-            %(post_prefix)sg_%(target)s%(post_index)s += %(g_target)s
+            %(post_prefix)sg_%(target)s%(post_index)s %(operation)s %(g_target)s
 """% target_dict
                     elif proj.disable_omp or Global.config['num_threads'] == 1:
                         g_target_code += """
-            %(post_prefix)sg_%(target)s%(post_index)s += %(g_target)s
+            %(post_prefix)sg_%(target)s%(post_index)s %(operation)s %(g_target)s
 """% target_dict
                     else:
                         raise NotImplementedError
 
                     # Determine bounds
                     for key, val in eq['bounds'].items():
                         if not key in ['min', 'max']:
@@ -886,15 +889,15 @@
                             value = str(float(val))
                         except: # TODO: more complex operations
                             value = val % ids
 
                         g_target_code += """
             if (%(post_prefix)sg_%(target)s%(post_index)s %(op)s %(val)s)
                 %(post_prefix)sg_%(target)s%(post_index)s = %(val)s;
-""" % {'id_post': proj.post.id, 'target': target, 'post_index': ids['post_index'], 'op': "<" if key == 'min' else '>', 'val': value}
+""" % {'post_prefix': ids['post_prefix'], 'target': target, 'post_index': ids['post_index'], 'op': "<" if key == 'min' else '>', 'val': value}
 
             else:
                 # process equations in pre_spike which
                 # are not 'g_target'
 
                 condition = ""
                 # Check conditions to update the variable
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/ProjectionGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/ProjectionGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/BSR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/COO.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/COO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/CSR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/CSR_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense_PV.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/Dense_T.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/ELL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/ELLR.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELLR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/HYB.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/HYB.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/LIL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/LIL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/SELL.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/SELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThread/__init__.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Projection/SingleThreadGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThreadGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         # as well as the matrix orientation.
         if proj._storage_format == "lil":
             if proj._storage_order == "post_to_pre":
                 self._templates.update(LIL_SingleThread.conn_templates)
                 self._template_ids.update(LIL_SingleThread.conn_ids)
             else:
                 raise Global.InvalidConfiguration("    "+proj.name+": storage_format = " + proj._storage_format + " and storage_order = " + proj._storage_order )
-        
+
         elif proj._storage_format == "coo":
             if proj._storage_order == "post_to_pre":
                 self._templates.update(COO_SingleThread.conn_templates)
                 self._template_ids.update(COO_SingleThread.conn_ids)
             else:
                 raise Global.InvalidConfiguration("    "+proj.name+": storage_format = " + proj._storage_format + " and storage_order = " + proj._storage_order )
 
@@ -592,15 +592,15 @@
         psp_prefix = tabify("%(float_prec)s sum;" % {'float_prec': Global.config['precision']}, 2)
 
         # Choose the corresponding summation template
         try:
             template = self._templates['rate_coded_sum']
         except KeyError:
            Global.CodeGeneratorException("    SingleThreadGenerator: no template for this configuration available")
- 
+
         # The psp uses in almost all cases one time the pre-synaptic index,
         # therefore I want to spare the usage of the explicit rk_pre variable.
         if proj._storage_format == "lil":
             ids['pre_index'] = "[pre_rank[i][j]]"
             ids['post_index'] = "[post_rank[i]]"
         elif proj._storage_format == "csr":
             ids['pre_index'] = "[col_idx[j]]"
@@ -656,18 +656,18 @@
                         )
                     else:
                         psp = psp.replace(
                             '%(pre_prefix)s'+var+'%(global_index)s',
                             '%(pre_prefix)s_delayed_'+var+'%(delay_u)s'
                         )
 
-        # If there is a uniform delay, the performance can be improved by 
+        # If there is a uniform delay, the performance can be improved by
         # pre_loading the delayed variable in advance.
         pre_copy = ""
-        if proj.max_delay > 1 and proj.uniform_delay != -1: 
+        if proj.max_delay > 1 and proj.uniform_delay != -1:
             for var in dependencies:
                 if var in proj.pre.neuron_type.description['local']:
                     pre_copy += "std::vector<%(float_prec)s> _pre_" + var + " = %(pre_prefix)s_delayed_" + var + "%(delay_u)s;"
                     psp = psp.replace(
                         '%(pre_prefix)s_delayed_'+var+'%(delay_u)s%(pre_index)s',
                         '_pre_'+var+'%(pre_index)s'
                     )
@@ -814,14 +814,16 @@
         # Analyse all elements of pre_spike
         for eq in proj.synapse_type.description['pre_spike']:
             # g_target is treated differently
             # Must be at the end of the equations
             if eq['name'] == 'g_target':
                 # PSP form
                 g_target = eq['cpp'].split('=')[1]
+                # Operation (g_target is replaced by sum in 'cpp')
+                operation = re.search(r'sum (.*?)=', eq['cpp']).group(1).strip() + "="
                 # Check targets
                 if isinstance(proj.target, str):
                     targets = [proj.target]
                 else:
                     targets = proj.target
 
                 g_target_code = ""
@@ -837,17 +839,18 @@
                     # update post-synaptic potential code
                     target_dict = {
                         'post_prefix': ids['post_prefix'],
                         'target': target,
                         'g_target': g_target % ids,
                         'eq': eq['eq'],
                         'post_index': ids['post_index'],
+                        'operation': operation
                     }
                     g_target_code += """
-            %(post_prefix)sg_%(target)s%(post_index)s += %(g_target)s
+            %(post_prefix)sg_%(target)s%(post_index)s %(operation)s %(g_target)s
 """% target_dict
 
                     # Determine bounds
                     for key, val in eq['bounds'].items():
                         if not key in ['min', 'max']:
                             continue
                         try:
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/PyxGenerator.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/PyxGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Sanity.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Sanity.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Template/BaseTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Template/BaseTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Template/GlobalOperationTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Template/GlobalOperationTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Template/MakefileTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Template/MakefileTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Template/MonitorTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Template/MonitorTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Template/PyxTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Template/PyxTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/generator/Utils.py` & `ANNarchy-4.7.2.3/ANNarchy/generator/Utils.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/BSRMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/BSRMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/COOMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/COOMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/COOMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/COOMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrixCUDAT.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDAT.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/CSRCMatrixT.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixT.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/CSRMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/CSRMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/DenseMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/DenseMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/DenseMatrixOffsets.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixOffsets.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/ELLMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/ELLMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/ELLRMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/ELLRMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/HYBMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/HYBMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/LILInvMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/LILInvMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/LILMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/LILMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/PartitionedMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/PartitionedMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/SELLMatrix.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/SELLMatrixCUDA.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/Specific.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/Specific.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/include/helper_functions.hpp` & `ANNarchy-4.7.2.3/ANNarchy/include/helper_functions.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/models/Neurons.py` & `ANNarchy-4.7.2.3/ANNarchy/models/Neurons.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/models/Synapses.py` & `ANNarchy-4.7.2.3/ANNarchy/models/Synapses.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/AnalyseNeuron.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseNeuron.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,15 @@
                 description,
                 method = method,
                 untouched = untouched
             )
             code = translator.parse()
             dependencies += translator.dependencies()
             num_flops = translator.num_flops
+        
         else: # An if-then-else statement
             code, deps = translate_ITE(
                         variable['name'],
                         eq,
                         condition,
                         description,
                         untouched )
@@ -321,17 +322,18 @@
             cpp_eq = re.sub(r'([^\w]*)'+f['name']+'\(',
                             r'\1'+f['name'] + '(', ' ' + cpp_eq).strip()
 
         # Store the result
         variable['pre_loop'] = pre_loop # Things to be declared before the for loop (eg. dt)
         variable['cpp'] = cpp_eq # the C++ equation
         variable['switch'] = switch # switch value of ODE
-        variable['untouched'] = untouched # may be needed later
-        variable['method'] = method # may be needed later
-        variable['dependencies'] = list(set(dependencies)) # may be needed later
+        variable['transformed_eq'] = eq # the equation with untouched terms
+        variable['untouched'] = untouched # untouched vocabulary
+        variable['method'] = method # numerical method
+        variable['dependencies'] = list(set(dependencies)) # list of dependencies
         variable['num_flops'] = num_flops
 
         # If the method is implicit or midpoint, the equations must be solved concurrently (depend on v[t+1])
         if method in ['implicit', 'midpoint', 'rk4'] and switch is not None:
             concurrent_odes.append(variable)
 
     # After all variables are processed, do it again if they are concurrent
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/AnalyseSynapse.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseSynapse.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,15 @@
         for f in description['functions']:
             cpp_eq = re.sub(r'([^\w]*)'+f['name']+'\(', r'\1'+ f['name'] + '(', ' ' + cpp_eq).strip()
 
         # Store the result
         variable['pre_loop'] = pre_loop # Things to be declared before the for loop (eg. dt)
         variable['cpp'] = cpp_eq # the C++ equation
         variable['switch'] = switch # switch value id ODE
+        variable['transformed_eq'] = eq # the equation with untouched terms
         variable['untouched'] = untouched # may be needed later
         variable['method'] = method # may be needed later
         variable['dependencies'] = dependencies
         variable['num_flops'] = num_flops
 
         # If the method is implicit or midpoint, the equations must be solved concurrently (depend on v[t+1])
         if method in ['implicit', 'midpoint'] and switch is not None:
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/CoupledEquations.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/CoupledEquations.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,37 +153,43 @@
         return self.variables
 
 
 
     def solve_midpoint(self, expression_list):
         "Midpoint method"
 
-        expression_list = {}
         equations = {}
         evaluations = {}
 
         # Pre-processing to replace the gradient
-        for name, expression in self.expression_list.items():
+        for name, expression in expression_list.items():
+            
             # transform the expression to suppress =
             if '=' in expression:
                 expression = expression.replace('=', '- (')
                 expression += ')'
+            
             # Suppress spaces to extract dvar/dt
             expression = expression.replace(' ', '')
-            # Transform the gradient into a difference TODO: more robust...
-            expression = expression.replace('d'+name+'/dt', '_gradient_'+name)
-            self.local_dict['_gradient_'+name] = Symbol('_gradient_'+name)
+            
+            # Transform the gradient into a difference TODO: more robust..            
+            expression = expression.replace('d'+name+'/dt', '_grad_var_'+name)
+            new_var = Symbol('_grad_var_'+name)
+            self.local_dict['_grad_var_'+name] = new_var
+            
             expression_list[name] = expression
 
+
         for name, expression in expression_list.items():
+
             analysed = self.parse_expression(expression,
                 local_dict = self.local_dict
             )
             equations[name] = analysed
-            evaluations[name] = solve(analysed, self.local_dict['_gradient_'+name])
+            evaluations[name] = solve(analysed, self.local_dict['_grad_var_'+name])
 
         # Compute the k = f(x, t)
         ks = {}
         for name, evaluation in evaluations.items():
             ks[name] = Global.config['precision'] + ' _k_' + name + ' = ' + self.c_code(evaluation[0]) + ';'
 
         # New dictionary replacing x by x+dt/2*k)
@@ -195,15 +201,15 @@
 
         # Compute the new values _x_new = f(x + dt/2*_k)
         news = {}
         for name, expression in expression_list.items():
             tmp_analysed = self.parse_expression(expression,
                 local_dict = tmp_dict
             )
-            solved = solve(tmp_analysed, self.local_dict['_gradient_'+name])
+            solved = solve(tmp_analysed, self.local_dict['_grad_var_'+name])
             news[name] = Global.config['precision'] + ' _' + name + ' = ' + self.c_code(solved[0]) + ';'
 
         # Compute the switches
         switches = {}
         for name, expression in expression_list.items():
             switches[name] = ccode(self.local_dict[name]) + ' += dt * _' + name + ' ;'
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/Equation.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/Equation.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,14 +286,15 @@
         self.num_flops += 2                          # apply increment
 
         # Return result
         return [{}, explicit_code, switch]
 
 
     def midpoint(self, expression):
+
         "Midpoint method."
         expression = expression.replace('d'+self.name+'/dt', '_grad_var_')
         new_var = sp.Symbol('_grad_var_')
         self.local_dict['_grad_var_'] = new_var
 
         analysed = self.parse_expression(expression,
             local_dict = self.local_dict
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/Extraction.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/Extraction.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/Function.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/Function.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/ITE.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/ITE.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/ParserTemplate.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/ParserTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/StringManipulation.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/StringManipulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/report/LatexParser.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexParser.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/report/LatexReport.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexReport.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/report/MarkdownReport.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/report/MarkdownReport.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/parser/report/Report.py` & `ANNarchy-4.7.2.3/ANNarchy/parser/report/Report.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy/thirdparty/randutils.hpp` & `ANNarchy-4.7.2.3/ANNarchy/thirdparty/randutils.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/ANNarchy.egg-info/PKG-INFO` & `ANNarchy-4.7.2.3/ANNarchy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANNarchy
-Version: 4.7.2.2
+Version: 4.7.2.3
 Summary: Artificial Neural Networks architect
 Home-page: http://www.tu-chemnitz.de/informatik/KI/projects/ANNarchy/index.php
 Download-URL: https://bitbucket.org/annarchy/annarchy
 Author: Julien Vitay, Helge Uelo Dinkelbach and Fred Hamker
 Author-email: julien.vitay@informatik.tu-chemnitz.de
 License: GPLv2+
 Keywords: neural simulator
```

### Comparing `ANNarchy-4.7.2.2/ANNarchy.egg-info/SOURCES.txt` & `ANNarchy-4.7.2.3/ANNarchy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -215,8 +215,11 @@
 examples/refractoriness/Refractoriness.py
 examples/simple_stdp/SimpleSTDPModel.py
 examples/structural_plasticity/StructuralPlasticity.py
 examples/tensorboard/BasalGanglia.ipynb
 examples/tensorboard/BayesianOptimization.ipynb
 examples/tsodyks_markram/TsodyksMarkram.py
 examples/vogels_abbott/COBA.py
-examples/vogels_abbott/CUBA.py
+examples/vogels_abbott/CUBA.py
+tests/test_CUDA.py
+tests/test_openmp.py
+tests/test_single_thread.py
```

### Comparing `ANNarchy-4.7.2.2/LICENSE` & `ANNarchy-4.7.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/PKG-INFO` & `ANNarchy-4.7.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANNarchy
-Version: 4.7.2.2
+Version: 4.7.2.3
 Summary: Artificial Neural Networks architect
 Home-page: http://www.tu-chemnitz.de/informatik/KI/projects/ANNarchy/index.php
 Download-URL: https://bitbucket.org/annarchy/annarchy
 Author: Julien Vitay, Helge Uelo Dinkelbach and Fred Hamker
 Author-email: julien.vitay@informatik.tu-chemnitz.de
 License: GPLv2+
 Keywords: neural simulator
```

### Comparing `ANNarchy-4.7.2.2/README.md` & `ANNarchy-4.7.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/ann_to_snn/demo.py` & `ANNarchy-4.7.2.3/examples/ann_to_snn/demo.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/bar_learning/BarLearning.py` & `ANNarchy-4.7.2.3/examples/bar_learning/BarLearning.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/bar_learning/BarLearningGPU.py` & `ANNarchy-4.7.2.3/examples/bar_learning/BarLearningGPU.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/bar_learning/Viz.py` & `ANNarchy-4.7.2.3/examples/bar_learning/Viz.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/bold_monitor/BOLD.py` & `ANNarchy-4.7.2.3/examples/bold_monitor/BOLD.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/bold_monitor/BOLD_two_inputs.py` & `ANNarchy-4.7.2.3/examples/bold_monitor/BOLD_two_inputs.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/gap_junctions/GapJunctions.py` & `ANNarchy-4.7.2.3/examples/gap_junctions/GapJunctions.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/hodgkin_huxley/HodgkinHuxley.py` & `ANNarchy-4.7.2.3/examples/hodgkin_huxley/HodgkinHuxley.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/homeostatic_stdp/Ramp.py` & `ANNarchy-4.7.2.3/examples/homeostatic_stdp/Ramp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/homeostatic_stdp/SORF.py` & `ANNarchy-4.7.2.3/examples/homeostatic_stdp/SORF.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/hybrid/Hybrid.py` & `ANNarchy-4.7.2.3/examples/hybrid/Hybrid.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/image/Image.py` & `ANNarchy-4.7.2.3/examples/image/Image.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/image/Webcam.ipynb` & `ANNarchy-4.7.2.3/examples/image/Webcam.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/image/Webcam.py` & `ANNarchy-4.7.2.3/examples/image/Webcam.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/izhikevich/Izhikevich.py` & `ANNarchy-4.7.2.3/examples/izhikevich/Izhikevich.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/multinetwork/MultiNetwork.py` & `ANNarchy-4.7.2.3/examples/multinetwork/MultiNetwork.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/neural_field/BubbleWorld.pyx` & `ANNarchy-4.7.2.3/examples/neural_field/BubbleWorld.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/neural_field/NeuralField.py` & `ANNarchy-4.7.2.3/examples/neural_field/NeuralField.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/neural_field/Viz.py` & `ANNarchy-4.7.2.3/examples/neural_field/Viz.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/pyNN/AEIF_cond_exp.py` & `ANNarchy-4.7.2.3/examples/pyNN/AEIF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/pyNN/EIF_cond_exp.py` & `ANNarchy-4.7.2.3/examples/pyNN/EIF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/pyNN/IF_cond_exp.py` & `ANNarchy-4.7.2.3/examples/pyNN/IF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/pyNN/IF_curr_alpha.py` & `ANNarchy-4.7.2.3/examples/pyNN/IF_curr_alpha.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/pyNN/non_linear_synapse.py` & `ANNarchy-4.7.2.3/examples/pyNN/non_linear_synapse.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/pyNN/short_term_plasticity2.py` & `ANNarchy-4.7.2.3/examples/pyNN/short_term_plasticity2.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/refractoriness/Refractoriness.py` & `ANNarchy-4.7.2.3/examples/refractoriness/Refractoriness.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/simple_stdp/SimpleSTDPModel.py` & `ANNarchy-4.7.2.3/examples/simple_stdp/SimpleSTDPModel.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/structural_plasticity/StructuralPlasticity.py` & `ANNarchy-4.7.2.3/examples/structural_plasticity/StructuralPlasticity.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/tensorboard/BasalGanglia.ipynb` & `ANNarchy-4.7.2.3/examples/tensorboard/BasalGanglia.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/tensorboard/BayesianOptimization.ipynb` & `ANNarchy-4.7.2.3/examples/tensorboard/BayesianOptimization.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/tsodyks_markram/TsodyksMarkram.py` & `ANNarchy-4.7.2.3/examples/tsodyks_markram/TsodyksMarkram.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/vogels_abbott/COBA.py` & `ANNarchy-4.7.2.3/examples/vogels_abbott/COBA.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/examples/vogels_abbott/CUBA.py` & `ANNarchy-4.7.2.3/examples/vogels_abbott/CUBA.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.2/setup.py` & `ANNarchy-4.7.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     'numpy',
     'scipy',
     'matplotlib',
     'cython',
     'sympy'
 ]
 
-release = '4.7.2.2'
+release = '4.7.2.3'
 print("Installing ANNarchy", release)
 py_version, py_major, python_include, python_libpath, cython_major = python_environment()
 print("\tPython", py_version, "(", sys.executable, ')')
 print("\tIncludes:", python_include)
 print("\tLibraries:", python_libpath)
 print("\tCython:", cython_major)
 print("\tNumpy:", np.get_include())
```

