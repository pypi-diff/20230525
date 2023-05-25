# Comparing `tmp/pytorch_msssim-0.2.1.tar.gz` & `tmp/pytorch_msssim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytorch_msssim-0.2.1.tar", last modified: Fri Aug 21 12:52:57 2020, max compression
+gzip compressed data, was "pytorch_msssim-1.0.0.tar", last modified: Thu May 25 17:15:45 2023, max compression
```

## Comparing `pytorch_msssim-0.2.1.tar` & `pytorch_msssim-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxr-x   0 maxinyin  (1001) maxinyin  (1001)        0 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)     8497 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/PKG-INFO
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)     6752 2020-08-21 12:52:21.000000 pytorch_msssim-0.2.1/README.md
-drwxrwxr-x   0 maxinyin  (1001) maxinyin  (1001)        0 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim/
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)       46 2020-08-21 12:48:24.000000 pytorch_msssim-0.2.1/pytorch_msssim/__init__.py
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)    10923 2020-08-21 12:48:24.000000 pytorch_msssim-0.2.1/pytorch_msssim/ssim.py
-drwxrwxr-x   0 maxinyin  (1001) maxinyin  (1001)        0 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim.egg-info/
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)     8497 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim.egg-info/PKG-INFO
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)      257 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim.egg-info/SOURCES.txt
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)        1 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim.egg-info/dependency_links.txt
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)        6 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim.egg-info/requires.txt
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)       15 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/pytorch_msssim.egg-info/top_level.txt
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)       38 2020-08-21 12:52:57.000000 pytorch_msssim-0.2.1/setup.cfg
--rw-rw-r--   0 maxinyin  (1001) maxinyin  (1001)      671 2020-08-21 12:50:12.000000 pytorch_msssim-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:15:45.744511 pytorch_msssim-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-25 17:15:45.744511 pytorch_msssim-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:15:45.740511 pytorch_msssim-1.0.0/pytorch_msssim/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/pytorch_msssim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/pytorch_msssim/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:15:45.740511 pytorch_msssim-1.0.0/pytorch_msssim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-25 17:15:45.000000 pytorch_msssim-1.0.0/pytorch_msssim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 17:15:45.000000 pytorch_msssim-1.0.0/pytorch_msssim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:15:45.000000 pytorch_msssim-1.0.0/pytorch_msssim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 17:15:45.000000 pytorch_msssim-1.0.0/pytorch_msssim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 17:15:45.000000 pytorch_msssim-1.0.0/pytorch_msssim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:15:45.744511 pytorch_msssim-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:15:45.744511 pytorch_msssim-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/tests/tests_comparisons_2d3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/tests/tests_comparisons_skimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/tests/tests_comparisons_tf_skimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/tests/tests_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-25 17:15:31.000000 pytorch_msssim-1.0.0/tests/tests_loss.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytorch_msssim-0.2.1/PKG-INFO` & `pytorch_msssim-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,167 @@
-Metadata-Version: 2.1
-Name: pytorch_msssim
-Version: 0.2.1
-Summary: Fast and differentiable MS-SSIM and SSIM for pytorch.
-Home-page: https://github.com/VainF/pytorch-msssim
-Author: Gongfan Fang
-Author-email: fgf@zju.edu.cn
-License: UNKNOWN
-Description: # Pytorch MS-SSIM
-        
-        Fast and differentiable MS-SSIM and SSIM for pytorch 1.0+
-        
-        <div>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/lcs.png" width="25%">
-        
-        Structural Similarity (SSIM):   
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ssim.png" width="50%">
-        
-        Multi-Scale Structural Similarity (MS-SSIM):  
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ms-ssim.png" width="55%">
-        </div>
-        
-        # Updates
-        ### _2020.08.21_
-        
-        3D image support from @FynnBe!  
-        
-        ### _2020.04.30_  
-        
-        Now (v0.2), **ssim & ms-ssim are calculated in the same way as tensorflow and skimage**, except that zero padding rather than symmetric padding is used during downsampling (there is no symmetric padding in pytorch). The comparison results between pytorch-msssim, tensorflow and skimage can be found in the Tests section.
-        
-        # Installation
-        
-        ```bash
-        pip install pytorch-msssim
-        ```
-        
-        # Usage
-        
-        Calculations will be on the same device as input images.
-        
-        ### 1. Basic Usage 
-        
-        ```python
-        from pytorch_msssim import ssim, ms_ssim, SSIM, MS_SSIM
-        # X: (N,3,H,W) a batch of non-negative RGB images (0~255)
-        # Y: (N,3,H,W)  
-        
-        # calculate ssim & ms-ssim for each image
-        ssim_val = ssim( X, Y, data_range=255, size_average=False) # return (N,)
-        ms_ssim_val = ms_ssim( X, Y, data_range=255, size_average=False ) #(N,)
-        
-        # set 'size_average=True' to get a scalar value as loss. see tests/tests_loss.py for more details
-        ssim_loss = 1 - ssim( X, Y, data_range=255, size_average=True) # return a scalar
-        ms_ssim_loss = 1 - ms_ssim( X, Y, data_range=255, size_average=True )
-        
-        # reuse the gaussian kernel with SSIM & MS_SSIM. 
-        ssim_module = SSIM(data_range=255, size_average=True, channel=3)
-        ms_ssim_module = MS_SSIM(data_range=255, size_average=True, channel=3)
-        
-        ssim_loss = 1 - ssim_module(X, Y)
-        ms_ssim_loss = 1 - ms_ssim_module(X, Y)
-        ```
-        ### 2. Normalized input
-        If you need to calculate MS-SSIM/SSIM on normalized images, please denormalize them to the range of [0, 1] or [0, 255] first.
-        
-        ```python
-        # X: (N,3,H,W) a batch of normalized images (-1 ~ 1)
-        # Y: (N,3,H,W)  
-        X = (X + 1) / 2  # [-1, 1] => [0, 1]
-        Y = (Y + 1) / 2  
-        ms_ssim_val = ms_ssim( X, Y, data_range=1, size_average=False ) #(N,)
-        ```
-        
-        ### 3. Enable nonnegative_ssim
-        
-        For ssim, it is recommended to set `nonnegative_ssim=True` to avoid negative results. However, this option is set to `False` by default to keep it consistent with tensorflow and skimage.
-        
-        For ms-ssim, there is no nonnegative_ssim option and the ssim reponses is forced to be non-negative to avoid NaN results.
-        
-        
-        # Tests and Examples
-        
-        ```bash
-        cd tests
-        ```
-        ### 1. Comparions between pytorch-msssim, skimage and tensorflow on CPU.
-        
-        ```bash
-        # requires tf2
-        python tests_comparisons_tf_skimage.py 
-        
-        # or skimage only
-        # python tests_comparisons_skimage.py 
-        ```
-        
-        Outputs:
-        
-        ```
-        Downloading test image...
-        ===================================
-                     Test SSIM
-        ===================================
-        ====> Single Image
-        Repeat 100 times
-        sigma=0.0 ssim_skimage=1.000000 (147.2605 ms), ssim_tf=1.000000 (343.4146 ms), ssim_torch=1.000000 (92.9151 ms)
-        sigma=10.0 ssim_skimage=0.932423 (147.5198 ms), ssim_tf=0.932661 (343.5191 ms), ssim_torch=0.932421 (95.6283 ms)
-        sigma=20.0 ssim_skimage=0.785744 (152.6441 ms), ssim_tf=0.785733 (343.4085 ms), ssim_torch=0.785738 (87.5639 ms)
-        sigma=30.0 ssim_skimage=0.636902 (145.5763 ms), ssim_tf=0.636902 (343.5312 ms), ssim_torch=0.636895 (90.4084 ms)
-        sigma=40.0 ssim_skimage=0.515798 (147.3798 ms), ssim_tf=0.515801 (344.8978 ms), ssim_torch=0.515791 (96.4440 ms)
-        sigma=50.0 ssim_skimage=0.422011 (148.2900 ms), ssim_tf=0.422007 (345.4076 ms), ssim_torch=0.422005 (86.3799 ms)
-        sigma=60.0 ssim_skimage=0.351139 (146.2039 ms), ssim_tf=0.351139 (343.4428 ms), ssim_torch=0.351133 (93.3445 ms)
-        sigma=70.0 ssim_skimage=0.296336 (145.5341 ms), ssim_tf=0.296337 (345.2255 ms), ssim_torch=0.296331 (92.6771 ms)
-        sigma=80.0 ssim_skimage=0.253328 (147.6655 ms), ssim_tf=0.253328 (343.1386 ms), ssim_torch=0.253324 (82.5985 ms)
-        sigma=90.0 ssim_skimage=0.219404 (142.6025 ms), ssim_tf=0.219405 (345.8275 ms), ssim_torch=0.219400 (100.9946 ms)
-        sigma=100.0 ssim_skimage=0.192681 (144.5597 ms), ssim_tf=0.192682 (346.5489 ms), ssim_torch=0.192678 (85.0229 ms)
-        Pass!
-        ====> Batch
-        Pass!
-        
-        
-        ===================================
-                     Test MS-SSIM
-        ===================================
-        ====> Single Image
-        Repeat 100 times
-        sigma=0.0 msssim_tf=1.000000 (671.5363 ms), msssim_torch=1.000000 (125.1403 ms)
-        sigma=10.0 msssim_tf=0.991137 (669.0296 ms), msssim_torch=0.991086 (113.4078 ms)
-        sigma=20.0 msssim_tf=0.967292 (670.5530 ms), msssim_torch=0.967281 (107.6428 ms)
-        sigma=30.0 msssim_tf=0.934875 (668.7717 ms), msssim_torch=0.934875 (111.3334 ms)
-        sigma=40.0 msssim_tf=0.897660 (669.0801 ms), msssim_torch=0.897658 (107.3700 ms)
-        sigma=50.0 msssim_tf=0.858956 (671.4629 ms), msssim_torch=0.858954 (100.9959 ms)
-        sigma=60.0 msssim_tf=0.820477 (670.5424 ms), msssim_torch=0.820475 (103.4489 ms)
-        sigma=70.0 msssim_tf=0.783511 (671.9357 ms), msssim_torch=0.783507 (113.9048 ms)
-        sigma=80.0 msssim_tf=0.749522 (672.3925 ms), msssim_torch=0.749518 (120.3891 ms)
-        sigma=90.0 msssim_tf=0.716221 (672.9066 ms), msssim_torch=0.716217 (118.3788 ms)
-        sigma=100.0 msssim_tf=0.684958 (675.2075 ms), msssim_torch=0.684953 (117.9481 ms)
-        Pass
-        ====> Batch
-        Pass
-        ```
-        
-        <div>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_0_ssim_1.0000.png"   width="20%">
-        <figcaption>ssim=1.0000</figcaption>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_50_ssim_0.4225.png"  width="20%">
-        <figcaption>ssim=0.4225</figcaption>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_100_ssim_0.1924.png"    width="20%">
-        <figcaption>ssim=0.1924</figcaption>
-        </div>
-        
-        ### 2. MS_SSIM as loss function
-        
-        See ['tests/tests_loss.py'](https://github.com/VainF/pytorch-msssim/tree/master/tests/tests_loss.py) for more details about how to use ssim or ms_ssim as loss functions
-        
-        ### 3. AutoEncoder
-        
-        See ['tests/ae_example'](https://github.com/VainF/pytorch-msssim/tree/master/tests/ae_example)
-        
-        ![results](https://github.com/VainF/Images/blob/master/pytorch_msssim/ae_ms_ssim.jpg)
-        *left: the original image, right: the reconstructed image*
-        
-        # References
-        
-        [https://github.com/jorge-pessoa/pytorch-msssim](https://github.com/jorge-pessoa/pytorch-msssim)  
-        [https://ece.uwaterloo.ca/~z70wang/research/ssim/](https://ece.uwaterloo.ca/~z70wang/research/ssim/)  
-        [https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf](https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf)  
-        [Matlab Code](https://ece.uwaterloo.ca/~z70wang/research/iwssim/)   
-        [ssim & ms-ssim from tensorflow](https://github.com/tensorflow/tensorflow/blob/v2.1.0/tensorflow/python/ops/image_ops_impl.py#L3314-L3438) 
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# Pytorch MS-SSIM
+
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://pepy.tech/badge/pytorch_msssim)](https://pepy.tech/project/pytorch_msssim)
+[![Latest Version](https://img.shields.io/badge/Latest%20Version-0.2.1-blue.svg)](https://github.com/VainF/pytorch_msssim/releases/latest)
+
+Fast and differentiable MS-SSIM and SSIM for pytorch.
+
+<div>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/lcs.png" width="25%">
+
+#### Structural Similarity (SSIM):   
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ssim.png" width="50%">
+
+#### Multi-Scale Structural Similarity (MS-SSIM):  
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ms-ssim.png" width="55%">
+</div>
+
+#### Why it is faster than other versions?
+
+Gaussian kernels used in SSIM & MS-SSIM are seperable. A [separable filter](https://en.wikipedia.org/wiki/Separable_filter) in image processing can be written as product of two more simple filters. Typically a 2-dimensional convolution operation is separated into two 1-dimensional filters. This reduces the computational costs on an $N\times M$ image with a $m\times n$ filter from $\mathcal{O}(M\cdot N \cdot m \cdot n)$ down to $\mathcal{O}(M\cdot N \cdot (m+n))$. More importantly, seperated kernels are more contiguous and thus cache-friendly than 2-D kernels, which effectively accelerates the computing of SSIM/MS-SSIM. 
+
+# Update
+#### _2020.08.21_ (v0.2.1)
+
+3D image support from [@FynnBe](https://github.com/FynnBe)!  
+
+#### _2020.04.30_ (v0.2)
+
+Now (v0.2), **ssim & ms-ssim can produce consistent results as tensorflow and skimage**. A benchmark (pytorch-msssim, tensorflow and skimage) can be found in the Tests section.
+
+# Installation
+
+```bash
+pip install pytorch-msssim
+```
+
+# Usage
+
+### 1. Basic Usage 
+
+```python
+from pytorch_msssim import ssim, ms_ssim, SSIM, MS_SSIM
+# X: (N,3,H,W) a batch of non-negative RGB images (0~255)
+# Y: (N,3,H,W)  
+
+# calculate ssim & ms-ssim for each image
+ssim_val = ssim( X, Y, data_range=255, size_average=False) # return (N,)
+ms_ssim_val = ms_ssim( X, Y, data_range=255, size_average=False ) #(N,)
+
+# set 'size_average=True' to get a scalar value as loss. see tests/tests_loss.py for more details
+ssim_loss = 1 - ssim( X, Y, data_range=255, size_average=True) # return a scalar
+ms_ssim_loss = 1 - ms_ssim( X, Y, data_range=255, size_average=True )
+
+# reuse the gaussian kernel with SSIM & MS_SSIM. 
+ssim_module = SSIM(data_range=255, size_average=True, channel=3) # channel=1 for grayscale images
+ms_ssim_module = MS_SSIM(data_range=255, size_average=True, channel=3)
+
+ssim_loss = 1 - ssim_module(X, Y)
+ms_ssim_loss = 1 - ms_ssim_module(X, Y)
+```
+### 2. Normalized input
+If you need to calculate MS-SSIM/SSIM on normalized images, please denormalize them to the range of [0, 1] or [0, 255] first.
+
+```python
+# X: (N,3,H,W) a batch of normalized images (-1 ~ 1)
+# Y: (N,3,H,W)  
+X = (X + 1) / 2  # [-1, 1] => [0, 1]
+Y = (Y + 1) / 2  
+ms_ssim_val = ms_ssim( X, Y, data_range=1, size_average=False ) #(N,)
+```
+
+### 3. Enable nonnegative_ssim
+
+For ssim, it is recommended to set `nonnegative_ssim=True` to avoid negative results. However, this option is set to `False` by default to keep it consistent with tensorflow and skimage.
+
+For ms-ssim, there is no nonnegative_ssim option and the ssim reponses is forced to be non-negative to avoid NaN results.
+
+
+# Tests and Examples
+
+```bash
+cd tests
+```
+### 1. Benchmark
+
+```bash
+# requires tf2
+python tests_comparisons_tf_skimage.py 
+
+# or skimage only
+# python tests_comparisons_skimage.py 
+```
+
+Outputs:
+
+```
+Downloading test image...
+===================================
+             Test SSIM
+===================================
+====> Single Image
+Repeat 100 times
+sigma=0.0 ssim_skimage=1.000000 (147.2605 ms), ssim_tf=1.000000 (343.4146 ms), ssim_torch=1.000000 (92.9151 ms)
+sigma=10.0 ssim_skimage=0.932423 (147.5198 ms), ssim_tf=0.932661 (343.5191 ms), ssim_torch=0.932421 (95.6283 ms)
+sigma=20.0 ssim_skimage=0.785744 (152.6441 ms), ssim_tf=0.785733 (343.4085 ms), ssim_torch=0.785738 (87.5639 ms)
+sigma=30.0 ssim_skimage=0.636902 (145.5763 ms), ssim_tf=0.636902 (343.5312 ms), ssim_torch=0.636895 (90.4084 ms)
+sigma=40.0 ssim_skimage=0.515798 (147.3798 ms), ssim_tf=0.515801 (344.8978 ms), ssim_torch=0.515791 (96.4440 ms)
+sigma=50.0 ssim_skimage=0.422011 (148.2900 ms), ssim_tf=0.422007 (345.4076 ms), ssim_torch=0.422005 (86.3799 ms)
+sigma=60.0 ssim_skimage=0.351139 (146.2039 ms), ssim_tf=0.351139 (343.4428 ms), ssim_torch=0.351133 (93.3445 ms)
+sigma=70.0 ssim_skimage=0.296336 (145.5341 ms), ssim_tf=0.296337 (345.2255 ms), ssim_torch=0.296331 (92.6771 ms)
+sigma=80.0 ssim_skimage=0.253328 (147.6655 ms), ssim_tf=0.253328 (343.1386 ms), ssim_torch=0.253324 (82.5985 ms)
+sigma=90.0 ssim_skimage=0.219404 (142.6025 ms), ssim_tf=0.219405 (345.8275 ms), ssim_torch=0.219400 (100.9946 ms)
+sigma=100.0 ssim_skimage=0.192681 (144.5597 ms), ssim_tf=0.192682 (346.5489 ms), ssim_torch=0.192678 (85.0229 ms)
+Pass!
+====> Batch
+Pass!
+
+
+===================================
+             Test MS-SSIM
+===================================
+====> Single Image
+Repeat 100 times
+sigma=0.0 msssim_tf=1.000000 (671.5363 ms), msssim_torch=1.000000 (125.1403 ms)
+sigma=10.0 msssim_tf=0.991137 (669.0296 ms), msssim_torch=0.991086 (113.4078 ms)
+sigma=20.0 msssim_tf=0.967292 (670.5530 ms), msssim_torch=0.967281 (107.6428 ms)
+sigma=30.0 msssim_tf=0.934875 (668.7717 ms), msssim_torch=0.934875 (111.3334 ms)
+sigma=40.0 msssim_tf=0.897660 (669.0801 ms), msssim_torch=0.897658 (107.3700 ms)
+sigma=50.0 msssim_tf=0.858956 (671.4629 ms), msssim_torch=0.858954 (100.9959 ms)
+sigma=60.0 msssim_tf=0.820477 (670.5424 ms), msssim_torch=0.820475 (103.4489 ms)
+sigma=70.0 msssim_tf=0.783511 (671.9357 ms), msssim_torch=0.783507 (113.9048 ms)
+sigma=80.0 msssim_tf=0.749522 (672.3925 ms), msssim_torch=0.749518 (120.3891 ms)
+sigma=90.0 msssim_tf=0.716221 (672.9066 ms), msssim_torch=0.716217 (118.3788 ms)
+sigma=100.0 msssim_tf=0.684958 (675.2075 ms), msssim_torch=0.684953 (117.9481 ms)
+Pass
+====> Batch
+Pass
+```
+
+<div>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_0_ssim_1.0000.png"   width="20%">
+<figcaption>ssim=1.0000</figcaption>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_50_ssim_0.4225.png"  width="20%">
+<figcaption>ssim=0.4225</figcaption>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_100_ssim_0.1924.png"    width="20%">
+<figcaption>ssim=0.1924</figcaption>
+</div>
+
+### 2. MS_SSIM as loss function
+
+See ['tests/tests_loss.py'](https://github.com/VainF/pytorch-msssim/tree/master/tests/tests_loss.py) for more details about how to use ssim or ms_ssim as loss functions
+
+### 3. AutoEncoder
+
+See ['tests/ae_example'](https://github.com/VainF/pytorch-msssim/tree/master/tests/ae_example)
+
+![results](https://github.com/VainF/Images/blob/master/pytorch_msssim/ae_ms_ssim.jpg)
+*left: the original image, right: the reconstructed image*
+
+# References
+
+[https://github.com/jorge-pessoa/pytorch-msssim](https://github.com/jorge-pessoa/pytorch-msssim)  
+[https://ece.uwaterloo.ca/~z70wang/research/ssim/](https://ece.uwaterloo.ca/~z70wang/research/ssim/)  
+[https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf](https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf)  
+[Matlab Code](https://ece.uwaterloo.ca/~z70wang/research/iwssim/)   
+[ssim & ms-ssim from tensorflow](https://github.com/tensorflow/tensorflow/blob/v2.1.0/tensorflow/python/ops/image_ops_impl.py#L3314-L3438)
```

### Comparing `pytorch_msssim-0.2.1/pytorch_msssim/ssim.py` & `pytorch_msssim-1.0.0/pytorch_msssim/ssim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Copyright 2020 by Gongfan Fang, Zhejiang University.
 # All rights reserved.
 import warnings
+from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn.functional as F
+from torch import Tensor
 
 
-def _fspecial_gauss_1d(size, sigma):
+def _fspecial_gauss_1d(size: int, sigma: float) -> Tensor:
     r"""Create 1-D gauss kernel
     Args:
         size (int): the size of gauss kernel
         sigma (float): sigma of normal distribution
-
     Returns:
         torch.Tensor: 1D kernel (1 x 1 x size)
     """
-    coords = torch.arange(size).to(dtype=torch.float)
+    coords = torch.arange(size, dtype=torch.float)
     coords -= size // 2
 
     g = torch.exp(-(coords ** 2) / (2 * sigma ** 2))
     g /= g.sum()
 
     return g.unsqueeze(0).unsqueeze(0)
 
 
-def gaussian_filter(input, win):
+def gaussian_filter(input: Tensor, win: Tensor) -> Tensor:
     r""" Blur input with 1-D kernel
     Args:
         input (torch.Tensor): a batch of tensors to be blurred
         window (torch.Tensor): 1-D gauss kernel
-
     Returns:
         torch.Tensor: blurred tensors
     """
     assert all([ws == 1 for ws in win.shape[1:-1]]), win.shape
     if len(input.shape) == 4:
         conv = F.conv2d
     elif len(input.shape) == 5:
@@ -50,27 +50,33 @@
             warnings.warn(
                 f"Skipping Gaussian Smoothing at dimension 2+{i} for input: {input.shape} and win size: {win.shape[-1]}"
             )
 
     return out
 
 
-def _ssim(X, Y, data_range, win, size_average=True, K=(0.01, 0.03)):
-
+def _ssim(
+    X: Tensor,
+    Y: Tensor,
+    data_range: float,
+    win: Tensor,
+    size_average: bool = True,
+    K: Union[Tuple[float, float], List[float]] = (0.01, 0.03)
+) -> Tuple[Tensor, Tensor]:
     r""" Calculate ssim index for X and Y
 
     Args:
         X (torch.Tensor): images
         Y (torch.Tensor): images
+        data_range (float or int): value range of input images. (usually 1.0 or 255)
         win (torch.Tensor): 1-D gauss kernel
-        data_range (float or int, optional): value range of input images. (usually 1.0 or 255)
         size_average (bool, optional): if size_average=True, ssim of all images will be averaged as a scalar
 
     Returns:
-        torch.Tensor: ssim results.
+        Tuple[torch.Tensor, torch.Tensor]: ssim results.
     """
     K1, K2 = K
     # batch, channel, [depth,] height, width = X.shape
     compensation = 1.0
 
     C1 = (K1 * data_range) ** 2
     C2 = (K2 * data_range) ** 2
@@ -93,24 +99,24 @@
 
     ssim_per_channel = torch.flatten(ssim_map, 2).mean(-1)
     cs = torch.flatten(cs_map, 2).mean(-1)
     return ssim_per_channel, cs
 
 
 def ssim(
-    X,
-    Y,
-    data_range=255,
-    size_average=True,
-    win_size=11,
-    win_sigma=1.5,
-    win=None,
-    K=(0.01, 0.03),
-    nonnegative_ssim=False,
-):
+    X: Tensor,
+    Y: Tensor,
+    data_range: float = 255,
+    size_average: bool = True,
+    win_size: int = 11,
+    win_sigma: float = 1.5,
+    win: Optional[Tensor] = None,
+    K: Union[Tuple[float, float], List[float]] = (0.01, 0.03),
+    nonnegative_ssim: bool = False,
+) -> Tensor:
     r""" interface of ssim
     Args:
         X (torch.Tensor): a batch of images, (N,C,H,W)
         Y (torch.Tensor): a batch of images, (N,C,H,W)
         data_range (float or int, optional): value range of input images. (usually 1.0 or 255)
         size_average (bool, optional): if size_average=True, ssim of all images will be averaged as a scalar
         win_size: (int, optional): the size of gauss kernel
@@ -119,25 +125,25 @@
         K (list or tuple, optional): scalar constants (K1, K2). Try a larger K2 constant (e.g. 0.4) if you get a negative or NaN results.
         nonnegative_ssim (bool, optional): force the ssim response to be nonnegative with relu
 
     Returns:
         torch.Tensor: ssim results
     """
     if not X.shape == Y.shape:
-        raise ValueError("Input images should have the same dimensions.")
+        raise ValueError(f"Input images should have the same dimensions, but got {X.shape} and {Y.shape}.")
 
     for d in range(len(X.shape) - 1, 1, -1):
         X = X.squeeze(dim=d)
         Y = Y.squeeze(dim=d)
 
     if len(X.shape) not in (4, 5):
         raise ValueError(f"Input images should be 4-d or 5-d tensors, but got {X.shape}")
 
-    if not X.type() == Y.type():
-        raise ValueError("Input images should have the same dtype.")
+    #if not X.type() == Y.type():
+    #    raise ValueError(f"Input images should have the same dtype, but got {X.type()} and {Y.type()}.")
 
     if win is not None:  # set win_size
         win_size = win.shape[-1]
 
     if not (win_size % 2 == 1):
         raise ValueError("Window size should be odd.")
 
@@ -152,17 +158,24 @@
     if size_average:
         return ssim_per_channel.mean()
     else:
         return ssim_per_channel.mean(1)
 
 
 def ms_ssim(
-    X, Y, data_range=255, size_average=True, win_size=11, win_sigma=1.5, win=None, weights=None, K=(0.01, 0.03)
-):
-
+    X: Tensor,
+    Y: Tensor,
+    data_range: float = 255,
+    size_average: bool = True,
+    win_size: int = 11,
+    win_sigma: float = 1.5,
+    win: Optional[Tensor] = None,
+    weights: Optional[List[float]] = None,
+    K: Union[Tuple[float, float], List[float]] = (0.01, 0.03)
+) -> Tensor:
     r""" interface of ms-ssim
     Args:
         X (torch.Tensor): a batch of images, (N,C,[T,]H,W)
         Y (torch.Tensor): a batch of images, (N,C,[T,]H,W)
         data_range (float or int, optional): value range of input images. (usually 1.0 or 255)
         size_average (bool, optional): if size_average=True, ssim of all images will be averaged as a scalar
         win_size: (int, optional): the size of gauss kernel
@@ -170,22 +183,22 @@
         win (torch.Tensor, optional): 1-D gauss kernel. if None, a new kernel will be created according to win_size and win_sigma
         weights (list, optional): weights for different levels
         K (list or tuple, optional): scalar constants (K1, K2). Try a larger K2 constant (e.g. 0.4) if you get a negative or NaN results.
     Returns:
         torch.Tensor: ms-ssim results
     """
     if not X.shape == Y.shape:
-        raise ValueError("Input images should have the same dimensions.")
+        raise ValueError(f"Input images should have the same dimensions, but got {X.shape} and {Y.shape}.")
 
     for d in range(len(X.shape) - 1, 1, -1):
         X = X.squeeze(dim=d)
         Y = Y.squeeze(dim=d)
 
-    if not X.type() == Y.type():
-        raise ValueError("Input images should have the same dtype.")
+    #if not X.type() == Y.type():
+    #    raise ValueError(f"Input images should have the same dtype, but got {X.type()} and {Y.type()}.")
 
     if len(X.shape) == 4:
         avg_pool = F.avg_pool2d
     elif len(X.shape) == 5:
         avg_pool = F.avg_pool3d
     else:
         raise ValueError(f"Input images should be 4-d or 5-d tensors, but got {X.shape}")
@@ -199,53 +212,53 @@
     smaller_side = min(X.shape[-2:])
     assert smaller_side > (win_size - 1) * (
         2 ** 4
     ), "Image size should be larger than %d due to the 4 downsamplings in ms-ssim" % ((win_size - 1) * (2 ** 4))
 
     if weights is None:
         weights = [0.0448, 0.2856, 0.3001, 0.2363, 0.1333]
-    weights = torch.FloatTensor(weights).to(X.device, dtype=X.dtype)
+    weights_tensor = X.new_tensor(weights)
 
     if win is None:
         win = _fspecial_gauss_1d(win_size, win_sigma)
         win = win.repeat([X.shape[1]] + [1] * (len(X.shape) - 1))
 
-    levels = weights.shape[0]
+    levels = weights_tensor.shape[0]
     mcs = []
     for i in range(levels):
         ssim_per_channel, cs = _ssim(X, Y, win=win, data_range=data_range, size_average=False, K=K)
 
         if i < levels - 1:
             mcs.append(torch.relu(cs))
             padding = [s % 2 for s in X.shape[2:]]
             X = avg_pool(X, kernel_size=2, padding=padding)
             Y = avg_pool(Y, kernel_size=2, padding=padding)
 
-    ssim_per_channel = torch.relu(ssim_per_channel)  # (batch, channel)
+    ssim_per_channel = torch.relu(ssim_per_channel)  # type: ignore  # (batch, channel)
     mcs_and_ssim = torch.stack(mcs + [ssim_per_channel], dim=0)  # (level, batch, channel)
-    ms_ssim_val = torch.prod(mcs_and_ssim ** weights.view(-1, 1, 1), dim=0)
+    ms_ssim_val = torch.prod(mcs_and_ssim ** weights_tensor.view(-1, 1, 1), dim=0)
 
     if size_average:
         return ms_ssim_val.mean()
     else:
         return ms_ssim_val.mean(1)
 
 
 class SSIM(torch.nn.Module):
     def __init__(
         self,
-        data_range=255,
-        size_average=True,
-        win_size=11,
-        win_sigma=1.5,
-        channel=3,
-        spatial_dims=2,
-        K=(0.01, 0.03),
-        nonnegative_ssim=False,
-    ):
+        data_range: float = 255,
+        size_average: bool = True,
+        win_size: int = 11,
+        win_sigma: float = 1.5,
+        channel: int = 3,
+        spatial_dims: int = 2,
+        K: Union[Tuple[float, float], List[float]] = (0.01, 0.03),
+        nonnegative_ssim: bool = False,
+    ) -> None:
         r""" class for ssim
         Args:
             data_range (float or int, optional): value range of input images. (usually 1.0 or 255)
             size_average (bool, optional): if size_average=True, ssim of all images will be averaged as a scalar
             win_size: (int, optional): the size of gauss kernel
             win_sigma: (float, optional): sigma of normal distribution
             channel (int, optional): input channels (default: 3)
@@ -257,38 +270,38 @@
         self.win_size = win_size
         self.win = _fspecial_gauss_1d(win_size, win_sigma).repeat([channel, 1] + [1] * spatial_dims)
         self.size_average = size_average
         self.data_range = data_range
         self.K = K
         self.nonnegative_ssim = nonnegative_ssim
 
-    def forward(self, X, Y):
+    def forward(self, X: Tensor, Y: Tensor) -> Tensor:
         return ssim(
             X,
             Y,
             data_range=self.data_range,
             size_average=self.size_average,
             win=self.win,
             K=self.K,
             nonnegative_ssim=self.nonnegative_ssim,
         )
 
 
 class MS_SSIM(torch.nn.Module):
     def __init__(
         self,
-        data_range=255,
-        size_average=True,
-        win_size=11,
-        win_sigma=1.5,
-        channel=3,
-        spatial_dims=2,
-        weights=None,
-        K=(0.01, 0.03),
-    ):
+        data_range: float = 255,
+        size_average: bool = True,
+        win_size: int = 11,
+        win_sigma: float = 1.5,
+        channel: int = 3,
+        spatial_dims: int = 2,
+        weights: Optional[List[float]] = None,
+        K: Union[Tuple[float, float], List[float]] = (0.01, 0.03),
+    ) -> None:
         r""" class for ms-ssim
         Args:
             data_range (float or int, optional): value range of input images. (usually 1.0 or 255)
             size_average (bool, optional): if size_average=True, ssim of all images will be averaged as a scalar
             win_size: (int, optional): the size of gauss kernel
             win_sigma: (float, optional): sigma of normal distribution
             channel (int, optional): input channels (default: 3)
@@ -300,15 +313,15 @@
         self.win_size = win_size
         self.win = _fspecial_gauss_1d(win_size, win_sigma).repeat([channel, 1] + [1] * spatial_dims)
         self.size_average = size_average
         self.data_range = data_range
         self.weights = weights
         self.K = K
 
-    def forward(self, X, Y):
+    def forward(self, X: Tensor, Y: Tensor) -> Tensor:
         return ms_ssim(
             X,
             Y,
             data_range=self.data_range,
             size_average=self.size_average,
             win=self.win,
             weights=self.weights,
```

### Comparing `pytorch_msssim-0.2.1/pytorch_msssim.egg-info/PKG-INFO` & `pytorch_msssim-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,180 @@
 Metadata-Version: 2.1
-Name: pytorch-msssim
-Version: 0.2.1
+Name: pytorch_msssim
+Version: 1.0.0
 Summary: Fast and differentiable MS-SSIM and SSIM for pytorch.
 Home-page: https://github.com/VainF/pytorch-msssim
 Author: Gongfan Fang
-Author-email: fgf@zju.edu.cn
-License: UNKNOWN
-Description: # Pytorch MS-SSIM
-        
-        Fast and differentiable MS-SSIM and SSIM for pytorch 1.0+
-        
-        <div>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/lcs.png" width="25%">
-        
-        Structural Similarity (SSIM):   
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ssim.png" width="50%">
-        
-        Multi-Scale Structural Similarity (MS-SSIM):  
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ms-ssim.png" width="55%">
-        </div>
-        
-        # Updates
-        ### _2020.08.21_
-        
-        3D image support from @FynnBe!  
-        
-        ### _2020.04.30_  
-        
-        Now (v0.2), **ssim & ms-ssim are calculated in the same way as tensorflow and skimage**, except that zero padding rather than symmetric padding is used during downsampling (there is no symmetric padding in pytorch). The comparison results between pytorch-msssim, tensorflow and skimage can be found in the Tests section.
-        
-        # Installation
-        
-        ```bash
-        pip install pytorch-msssim
-        ```
-        
-        # Usage
-        
-        Calculations will be on the same device as input images.
-        
-        ### 1. Basic Usage 
-        
-        ```python
-        from pytorch_msssim import ssim, ms_ssim, SSIM, MS_SSIM
-        # X: (N,3,H,W) a batch of non-negative RGB images (0~255)
-        # Y: (N,3,H,W)  
-        
-        # calculate ssim & ms-ssim for each image
-        ssim_val = ssim( X, Y, data_range=255, size_average=False) # return (N,)
-        ms_ssim_val = ms_ssim( X, Y, data_range=255, size_average=False ) #(N,)
-        
-        # set 'size_average=True' to get a scalar value as loss. see tests/tests_loss.py for more details
-        ssim_loss = 1 - ssim( X, Y, data_range=255, size_average=True) # return a scalar
-        ms_ssim_loss = 1 - ms_ssim( X, Y, data_range=255, size_average=True )
-        
-        # reuse the gaussian kernel with SSIM & MS_SSIM. 
-        ssim_module = SSIM(data_range=255, size_average=True, channel=3)
-        ms_ssim_module = MS_SSIM(data_range=255, size_average=True, channel=3)
-        
-        ssim_loss = 1 - ssim_module(X, Y)
-        ms_ssim_loss = 1 - ms_ssim_module(X, Y)
-        ```
-        ### 2. Normalized input
-        If you need to calculate MS-SSIM/SSIM on normalized images, please denormalize them to the range of [0, 1] or [0, 255] first.
-        
-        ```python
-        # X: (N,3,H,W) a batch of normalized images (-1 ~ 1)
-        # Y: (N,3,H,W)  
-        X = (X + 1) / 2  # [-1, 1] => [0, 1]
-        Y = (Y + 1) / 2  
-        ms_ssim_val = ms_ssim( X, Y, data_range=1, size_average=False ) #(N,)
-        ```
-        
-        ### 3. Enable nonnegative_ssim
-        
-        For ssim, it is recommended to set `nonnegative_ssim=True` to avoid negative results. However, this option is set to `False` by default to keep it consistent with tensorflow and skimage.
-        
-        For ms-ssim, there is no nonnegative_ssim option and the ssim reponses is forced to be non-negative to avoid NaN results.
-        
-        
-        # Tests and Examples
-        
-        ```bash
-        cd tests
-        ```
-        ### 1. Comparions between pytorch-msssim, skimage and tensorflow on CPU.
-        
-        ```bash
-        # requires tf2
-        python tests_comparisons_tf_skimage.py 
-        
-        # or skimage only
-        # python tests_comparisons_skimage.py 
-        ```
-        
-        Outputs:
-        
-        ```
-        Downloading test image...
-        ===================================
-                     Test SSIM
-        ===================================
-        ====> Single Image
-        Repeat 100 times
-        sigma=0.0 ssim_skimage=1.000000 (147.2605 ms), ssim_tf=1.000000 (343.4146 ms), ssim_torch=1.000000 (92.9151 ms)
-        sigma=10.0 ssim_skimage=0.932423 (147.5198 ms), ssim_tf=0.932661 (343.5191 ms), ssim_torch=0.932421 (95.6283 ms)
-        sigma=20.0 ssim_skimage=0.785744 (152.6441 ms), ssim_tf=0.785733 (343.4085 ms), ssim_torch=0.785738 (87.5639 ms)
-        sigma=30.0 ssim_skimage=0.636902 (145.5763 ms), ssim_tf=0.636902 (343.5312 ms), ssim_torch=0.636895 (90.4084 ms)
-        sigma=40.0 ssim_skimage=0.515798 (147.3798 ms), ssim_tf=0.515801 (344.8978 ms), ssim_torch=0.515791 (96.4440 ms)
-        sigma=50.0 ssim_skimage=0.422011 (148.2900 ms), ssim_tf=0.422007 (345.4076 ms), ssim_torch=0.422005 (86.3799 ms)
-        sigma=60.0 ssim_skimage=0.351139 (146.2039 ms), ssim_tf=0.351139 (343.4428 ms), ssim_torch=0.351133 (93.3445 ms)
-        sigma=70.0 ssim_skimage=0.296336 (145.5341 ms), ssim_tf=0.296337 (345.2255 ms), ssim_torch=0.296331 (92.6771 ms)
-        sigma=80.0 ssim_skimage=0.253328 (147.6655 ms), ssim_tf=0.253328 (343.1386 ms), ssim_torch=0.253324 (82.5985 ms)
-        sigma=90.0 ssim_skimage=0.219404 (142.6025 ms), ssim_tf=0.219405 (345.8275 ms), ssim_torch=0.219400 (100.9946 ms)
-        sigma=100.0 ssim_skimage=0.192681 (144.5597 ms), ssim_tf=0.192682 (346.5489 ms), ssim_torch=0.192678 (85.0229 ms)
-        Pass!
-        ====> Batch
-        Pass!
-        
-        
-        ===================================
-                     Test MS-SSIM
-        ===================================
-        ====> Single Image
-        Repeat 100 times
-        sigma=0.0 msssim_tf=1.000000 (671.5363 ms), msssim_torch=1.000000 (125.1403 ms)
-        sigma=10.0 msssim_tf=0.991137 (669.0296 ms), msssim_torch=0.991086 (113.4078 ms)
-        sigma=20.0 msssim_tf=0.967292 (670.5530 ms), msssim_torch=0.967281 (107.6428 ms)
-        sigma=30.0 msssim_tf=0.934875 (668.7717 ms), msssim_torch=0.934875 (111.3334 ms)
-        sigma=40.0 msssim_tf=0.897660 (669.0801 ms), msssim_torch=0.897658 (107.3700 ms)
-        sigma=50.0 msssim_tf=0.858956 (671.4629 ms), msssim_torch=0.858954 (100.9959 ms)
-        sigma=60.0 msssim_tf=0.820477 (670.5424 ms), msssim_torch=0.820475 (103.4489 ms)
-        sigma=70.0 msssim_tf=0.783511 (671.9357 ms), msssim_torch=0.783507 (113.9048 ms)
-        sigma=80.0 msssim_tf=0.749522 (672.3925 ms), msssim_torch=0.749518 (120.3891 ms)
-        sigma=90.0 msssim_tf=0.716221 (672.9066 ms), msssim_torch=0.716217 (118.3788 ms)
-        sigma=100.0 msssim_tf=0.684958 (675.2075 ms), msssim_torch=0.684953 (117.9481 ms)
-        Pass
-        ====> Batch
-        Pass
-        ```
-        
-        <div>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_0_ssim_1.0000.png"   width="20%">
-        <figcaption>ssim=1.0000</figcaption>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_50_ssim_0.4225.png"  width="20%">
-        <figcaption>ssim=0.4225</figcaption>
-        <img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_100_ssim_0.1924.png"    width="20%">
-        <figcaption>ssim=0.1924</figcaption>
-        </div>
-        
-        ### 2. MS_SSIM as loss function
-        
-        See ['tests/tests_loss.py'](https://github.com/VainF/pytorch-msssim/tree/master/tests/tests_loss.py) for more details about how to use ssim or ms_ssim as loss functions
-        
-        ### 3. AutoEncoder
-        
-        See ['tests/ae_example'](https://github.com/VainF/pytorch-msssim/tree/master/tests/ae_example)
-        
-        ![results](https://github.com/VainF/Images/blob/master/pytorch_msssim/ae_ms_ssim.jpg)
-        *left: the original image, right: the reconstructed image*
-        
-        # References
-        
-        [https://github.com/jorge-pessoa/pytorch-msssim](https://github.com/jorge-pessoa/pytorch-msssim)  
-        [https://ece.uwaterloo.ca/~z70wang/research/ssim/](https://ece.uwaterloo.ca/~z70wang/research/ssim/)  
-        [https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf](https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf)  
-        [Matlab Code](https://ece.uwaterloo.ca/~z70wang/research/iwssim/)   
-        [ssim & ms-ssim from tensorflow](https://github.com/tensorflow/tensorflow/blob/v2.1.0/tensorflow/python/ops/image_ops_impl.py#L3314-L3438) 
-        
-Platform: UNKNOWN
+Author-email: gongfan@u.nus.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Pytorch MS-SSIM
+
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://pepy.tech/badge/pytorch_msssim)](https://pepy.tech/project/pytorch_msssim)
+[![Latest Version](https://img.shields.io/badge/Latest%20Version-0.2.1-blue.svg)](https://github.com/VainF/pytorch_msssim/releases/latest)
+
+Fast and differentiable MS-SSIM and SSIM for pytorch.
+
+<div>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/lcs.png" width="25%">
+
+#### Structural Similarity (SSIM):   
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ssim.png" width="50%">
+
+#### Multi-Scale Structural Similarity (MS-SSIM):  
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/ms-ssim.png" width="55%">
+</div>
+
+#### Why it is faster than other versions?
+
+Gaussian kernels used in SSIM & MS-SSIM are seperable. A [separable filter](https://en.wikipedia.org/wiki/Separable_filter) in image processing can be written as product of two more simple filters. Typically a 2-dimensional convolution operation is separated into two 1-dimensional filters. This reduces the computational costs on an $N\times M$ image with a $m\times n$ filter from $\mathcal{O}(M\cdot N \cdot m \cdot n)$ down to $\mathcal{O}(M\cdot N \cdot (m+n))$. More importantly, seperated kernels are more contiguous and thus cache-friendly than 2-D kernels, which effectively accelerates the computing of SSIM/MS-SSIM. 
+
+# Update
+#### _2020.08.21_ (v0.2.1)
+
+3D image support from [@FynnBe](https://github.com/FynnBe)!  
+
+#### _2020.04.30_ (v0.2)
+
+Now (v0.2), **ssim & ms-ssim can produce consistent results as tensorflow and skimage**. A benchmark (pytorch-msssim, tensorflow and skimage) can be found in the Tests section.
+
+# Installation
+
+```bash
+pip install pytorch-msssim
+```
+
+# Usage
+
+### 1. Basic Usage 
+
+```python
+from pytorch_msssim import ssim, ms_ssim, SSIM, MS_SSIM
+# X: (N,3,H,W) a batch of non-negative RGB images (0~255)
+# Y: (N,3,H,W)  
+
+# calculate ssim & ms-ssim for each image
+ssim_val = ssim( X, Y, data_range=255, size_average=False) # return (N,)
+ms_ssim_val = ms_ssim( X, Y, data_range=255, size_average=False ) #(N,)
+
+# set 'size_average=True' to get a scalar value as loss. see tests/tests_loss.py for more details
+ssim_loss = 1 - ssim( X, Y, data_range=255, size_average=True) # return a scalar
+ms_ssim_loss = 1 - ms_ssim( X, Y, data_range=255, size_average=True )
+
+# reuse the gaussian kernel with SSIM & MS_SSIM. 
+ssim_module = SSIM(data_range=255, size_average=True, channel=3) # channel=1 for grayscale images
+ms_ssim_module = MS_SSIM(data_range=255, size_average=True, channel=3)
+
+ssim_loss = 1 - ssim_module(X, Y)
+ms_ssim_loss = 1 - ms_ssim_module(X, Y)
+```
+### 2. Normalized input
+If you need to calculate MS-SSIM/SSIM on normalized images, please denormalize them to the range of [0, 1] or [0, 255] first.
+
+```python
+# X: (N,3,H,W) a batch of normalized images (-1 ~ 1)
+# Y: (N,3,H,W)  
+X = (X + 1) / 2  # [-1, 1] => [0, 1]
+Y = (Y + 1) / 2  
+ms_ssim_val = ms_ssim( X, Y, data_range=1, size_average=False ) #(N,)
+```
+
+### 3. Enable nonnegative_ssim
+
+For ssim, it is recommended to set `nonnegative_ssim=True` to avoid negative results. However, this option is set to `False` by default to keep it consistent with tensorflow and skimage.
+
+For ms-ssim, there is no nonnegative_ssim option and the ssim reponses is forced to be non-negative to avoid NaN results.
+
+
+# Tests and Examples
+
+```bash
+cd tests
+```
+### 1. Benchmark
+
+```bash
+# requires tf2
+python tests_comparisons_tf_skimage.py 
+
+# or skimage only
+# python tests_comparisons_skimage.py 
+```
+
+Outputs:
+
+```
+Downloading test image...
+===================================
+             Test SSIM
+===================================
+====> Single Image
+Repeat 100 times
+sigma=0.0 ssim_skimage=1.000000 (147.2605 ms), ssim_tf=1.000000 (343.4146 ms), ssim_torch=1.000000 (92.9151 ms)
+sigma=10.0 ssim_skimage=0.932423 (147.5198 ms), ssim_tf=0.932661 (343.5191 ms), ssim_torch=0.932421 (95.6283 ms)
+sigma=20.0 ssim_skimage=0.785744 (152.6441 ms), ssim_tf=0.785733 (343.4085 ms), ssim_torch=0.785738 (87.5639 ms)
+sigma=30.0 ssim_skimage=0.636902 (145.5763 ms), ssim_tf=0.636902 (343.5312 ms), ssim_torch=0.636895 (90.4084 ms)
+sigma=40.0 ssim_skimage=0.515798 (147.3798 ms), ssim_tf=0.515801 (344.8978 ms), ssim_torch=0.515791 (96.4440 ms)
+sigma=50.0 ssim_skimage=0.422011 (148.2900 ms), ssim_tf=0.422007 (345.4076 ms), ssim_torch=0.422005 (86.3799 ms)
+sigma=60.0 ssim_skimage=0.351139 (146.2039 ms), ssim_tf=0.351139 (343.4428 ms), ssim_torch=0.351133 (93.3445 ms)
+sigma=70.0 ssim_skimage=0.296336 (145.5341 ms), ssim_tf=0.296337 (345.2255 ms), ssim_torch=0.296331 (92.6771 ms)
+sigma=80.0 ssim_skimage=0.253328 (147.6655 ms), ssim_tf=0.253328 (343.1386 ms), ssim_torch=0.253324 (82.5985 ms)
+sigma=90.0 ssim_skimage=0.219404 (142.6025 ms), ssim_tf=0.219405 (345.8275 ms), ssim_torch=0.219400 (100.9946 ms)
+sigma=100.0 ssim_skimage=0.192681 (144.5597 ms), ssim_tf=0.192682 (346.5489 ms), ssim_torch=0.192678 (85.0229 ms)
+Pass!
+====> Batch
+Pass!
+
+
+===================================
+             Test MS-SSIM
+===================================
+====> Single Image
+Repeat 100 times
+sigma=0.0 msssim_tf=1.000000 (671.5363 ms), msssim_torch=1.000000 (125.1403 ms)
+sigma=10.0 msssim_tf=0.991137 (669.0296 ms), msssim_torch=0.991086 (113.4078 ms)
+sigma=20.0 msssim_tf=0.967292 (670.5530 ms), msssim_torch=0.967281 (107.6428 ms)
+sigma=30.0 msssim_tf=0.934875 (668.7717 ms), msssim_torch=0.934875 (111.3334 ms)
+sigma=40.0 msssim_tf=0.897660 (669.0801 ms), msssim_torch=0.897658 (107.3700 ms)
+sigma=50.0 msssim_tf=0.858956 (671.4629 ms), msssim_torch=0.858954 (100.9959 ms)
+sigma=60.0 msssim_tf=0.820477 (670.5424 ms), msssim_torch=0.820475 (103.4489 ms)
+sigma=70.0 msssim_tf=0.783511 (671.9357 ms), msssim_torch=0.783507 (113.9048 ms)
+sigma=80.0 msssim_tf=0.749522 (672.3925 ms), msssim_torch=0.749518 (120.3891 ms)
+sigma=90.0 msssim_tf=0.716221 (672.9066 ms), msssim_torch=0.716217 (118.3788 ms)
+sigma=100.0 msssim_tf=0.684958 (675.2075 ms), msssim_torch=0.684953 (117.9481 ms)
+Pass
+====> Batch
+Pass
+```
+
+<div>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_0_ssim_1.0000.png"   width="20%">
+<figcaption>ssim=1.0000</figcaption>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_50_ssim_0.4225.png"  width="20%">
+<figcaption>ssim=0.4225</figcaption>
+<img src="https://github.com/VainF/Images/blob/master/pytorch_msssim/simga_100_ssim_0.1924.png"    width="20%">
+<figcaption>ssim=0.1924</figcaption>
+</div>
+
+### 2. MS_SSIM as loss function
+
+See ['tests/tests_loss.py'](https://github.com/VainF/pytorch-msssim/tree/master/tests/tests_loss.py) for more details about how to use ssim or ms_ssim as loss functions
+
+### 3. AutoEncoder
+
+See ['tests/ae_example'](https://github.com/VainF/pytorch-msssim/tree/master/tests/ae_example)
+
+![results](https://github.com/VainF/Images/blob/master/pytorch_msssim/ae_ms_ssim.jpg)
+*left: the original image, right: the reconstructed image*
+
+# References
+
+[https://github.com/jorge-pessoa/pytorch-msssim](https://github.com/jorge-pessoa/pytorch-msssim)  
+[https://ece.uwaterloo.ca/~z70wang/research/ssim/](https://ece.uwaterloo.ca/~z70wang/research/ssim/)  
+[https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf](https://ece.uwaterloo.ca/~z70wang/publications/msssim.pdf)  
+[Matlab Code](https://ece.uwaterloo.ca/~z70wang/research/iwssim/)   
+[ssim & ms-ssim from tensorflow](https://github.com/tensorflow/tensorflow/blob/v2.1.0/tensorflow/python/ops/image_ops_impl.py#L3314-L3438)
```

### Comparing `pytorch_msssim-0.2.1/setup.py` & `pytorch_msssim-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytorch_msssim",
-    version="0.2.1",
+    version="1.0.0",
     author="Gongfan Fang",
-    author_email="fgf@zju.edu.cn",
+    author_email="gongfan@u.nus.edu",
     description="Fast and differentiable MS-SSIM and SSIM for pytorch.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VainF/pytorch-msssim",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=['torch']
-)
+)
```

