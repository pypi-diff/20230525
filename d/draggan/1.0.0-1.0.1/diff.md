# Comparing `tmp/draggan-1.0.0.tar.gz` & `tmp/draggan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-wj5wj_ew/draggan-1.0.0.tar", last modified: Thu May 25 07:53:05 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-otk7kdwu/draggan-1.0.1.tar", last modified: Thu May 25 12:10:52 2023, max compression
```

## Comparing `draggan-1.0.0.tar` & `draggan-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 07:53:05.000000 draggan-1.0.0/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3906 2023-05-25 03:33:44.000000 draggan-1.0.0/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.0/draggan/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.0/draggan/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:07:16.000000 draggan-1.0.0/draggan/app.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.0/draggan/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.0/draggan/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.0/draggan/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.0/draggan/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:35:13.000000 draggan-1.0.0/draggan/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.0/draggan/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.0/draggan/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.0/draggan/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6689 2023-05-25 07:35:19.000000 draggan-1.0.0/draggan/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.0/draggan/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12463 2023-05-25 07:48:03.000000 draggan-1.0.0/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      102 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       18 2023-05-25 07:53:05.000000 draggan-1.0.0/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-25 07:53:05.000000 draggan-1.0.0/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      627 2023-05-25 07:43:50.000000 draggan-1.0.0/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.0/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.0/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.0/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:53:05.000000 draggan-1.0.0/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:48:40.000000 draggan-1.0.0/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.0/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:49:11.000000 draggan-1.0.0/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6689 2023-05-25 07:49:17.000000 draggan-1.0.0/stylegan2/op/upfirdn2d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 12:10:52.000000 draggan-1.0.1/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4661 2023-05-25 08:08:00.000000 draggan-1.0.1/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.1/draggan/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.1/draggan/api.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      873 2023-05-25 08:31:09.000000 draggan-1.0.1/draggan/app.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.1/draggan/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.1/draggan/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.1/draggan/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.1/draggan/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:35:13.000000 draggan-1.0.1/draggan/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.1/draggan/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.1/draggan/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.1/draggan/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6689 2023-05-25 07:35:19.000000 draggan-1.0.1/draggan/stylegan2/op/upfirdn2d.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.1/draggan/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12461 2023-05-25 12:06:09.000000 draggan-1.0.1/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      102 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       18 2023-05-25 12:10:52.000000 draggan-1.0.1/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-25 12:10:52.000000 draggan-1.0.1/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      627 2023-05-25 12:06:23.000000 draggan-1.0.1/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.1/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.1/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.1/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 12:10:52.000000 draggan-1.0.1/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 07:48:40.000000 draggan-1.0.1/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.1/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:49:11.000000 draggan-1.0.1/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6689 2023-05-25 07:49:17.000000 draggan-1.0.1/stylegan2/op/upfirdn2d.py
```

### Comparing `draggan-1.0.0/README.md` & `draggan-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 # DragGAN
+[![PyPI](https://img.shields.io/pypi/v/draggan)](https://pypi.org/project/draggan/) 
 
 :boom:  [`Colab Demo`](https://colab.research.google.com/github/Zeqiang-Lai/DragGAN/blob/master/colab.ipynb) | [`InternGPT Free Online Demo`](https://github.com/OpenGVLab/InternGPT)
-<!--  [`Online Demo`](https://6a05f355a8f139550c.gradio.live/)  -->
-<!-- > Note that the link of online demo will be updated regularly. -->
+
+```bash
+pip install draggan
+```
 
 > **An out-of-box online demo is integrated in [InternGPT](https://github.com/OpenGVLab/InternGPT) - a super cool pointing-language-driven visual interactive system. Enjoy for free.:lollipop:**
 > 
 > Note for Colab, remember to select a GPU via `Runtime/Change runtime type` (`代码执行程序/更改运行时类型`).
-> 
-> Due to the limitation of GAN inversion, it is possible that your custom images are distorted. Besides, it is also possible the manipulations fail due to the limitation of our implementation.
 
 Unofficial implementation of [Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
 
 <p float="left">
   <img src="assets/mouse.gif" width="200" />
   <img src="assets/nose.gif" width="200" /> 
   <img src="assets/cat.gif" width="200" />
   <img src="assets/horse.gif" width="200" />
 </p>
 
+## News
+
 :star2: **What's New**
 
-This project is now a sub-project of [InternGPT](https://github.com/OpenGVLab/InternGPT) for interactive image editing. Future updates of more cool tools beyond DragGAN would be added in [InternGPT](https://github.com/OpenGVLab/InternGPT). 
+- [2023/5/25] DragGAN is on PyPI, simple install via `pip install draggan`. Also addressed the common CUDA problems https://github.com/Zeqiang-Lai/DragGAN/issues/38  https://github.com/Zeqiang-Lai/DragGAN/issues/12
+- [2023/5/25] We now support StyleGAN2-ada with much higher quality and more types of images. Try it by selecting models started with "ada".
+- [2023/5/24] Custom Image with GAN inversion is supported, but it is possible that your custom images are distorted  due to the limitation of GAN inversion. Besides, it is also possible the manipulations fail due to the limitation of our implementation.
+
+:star2: **Changelog**
 
 - [ ] Tweak performance.
-- [ ] Improving installation experience.
+- [x] Improving installation experience, DragGAN is now on [PyPI](https://pypi.org/project/draggan).
 - [ ] Automatically determining the number of iterations.
-- [x] We now support StyleGAN2-Ada with much higher quality and more types of images. 
+- [x] Support StyleGAN2-ada.
 - [x] Integrate into [InternGPT](https://github.com/OpenGVLab/InternGPT)
 - [x] Custom Image with GAN inversion.
 - [x] Download generated image and generation trajectory.
 - [x] Controlling generation process with GUI.
 - [x] Automatically download stylegan2 checkpoint.
 - [x] Support movable region, multiple handle points.
 - [x] Gradio and Colab Demo.
 
+> This project is now a sub-project of [InternGPT](https://github.com/OpenGVLab/InternGPT) for interactive image editing. Future updates of more cool tools beyond DragGAN would be added in [InternGPT](https://github.com/OpenGVLab/InternGPT). 
 
 ## How it Work ?
 
 Check out the original [paper](https://vcai.mpi-inf.mpg.de/projects/DragGAN/) for the backend algorithm and math.
 
 ![demo](assets/paper.png)
 
@@ -48,19 +56,37 @@
 
 
 
 
 
 ## Running Locally
 
+### With PyPI
+
+```bash
+conda create -n draggan python=3.7
+conda activate draggan
+pip install draggan
+```
+
+Launch the Gradio demo
+
+```bash
+python -m draggan.web
+```
+
+### Clone and Install 
+
 Ensure you have a GPU and CUDA installed. We use Python 3.7 for testing, other versions (>= 3.7) of Python should work too, but not tested. We recommend to use [Conda](https://conda.io/projects/conda/en/stable/user-guide/install/download.html) to prepare all the requirements.
 
 For Windows users, you might encounter some issues caused by StyleGAN custom ops, youd could find some solutions from the [issues pannel](https://github.com/Zeqiang-Lai/DragGAN/issues). We are also working on a more friendly package without setup.
 
 ```bash
+git clone https://github.com/Zeqiang-Lai/DragGAN.git
+cd DragGAN
 conda create -n draggan python=3.7
 conda activate draggan
 pip install -r requirements.txt
 ```
 
 Launch the Gradio demo
 
@@ -68,15 +94,15 @@
 python gradio_app.py
 ```
 
 > If you have any issue for downloading the checkpoint, you could manually download it from [here](https://huggingface.co/aaronb/StyleGAN2/tree/main) and put it into the folder `checkpoints`.
 
 ## Acknowledgement
 
-[Official DragGAN](https://github.com/XingangPan/DragGAN) &ensp; [StyleGAN2](https://github.com/NVlabs/stylegan2)  &ensp; [StyleGAN2-pytorch](https://github.com/rosinality/stylegan2-pytorch)
+[Official DragGAN](https://github.com/XingangPan/DragGAN) &ensp; [StyleGAN2](https://github.com/NVlabs/stylegan2)  &ensp; [StyleGAN2-pytorch](https://github.com/rosinality/stylegan2-pytorch)  &ensp; [StyleGAN2-Ada](https://github.com/NVlabs/stylegan2-ada-pytorch)
 
 <!-- https://github.com/omertov/encoder4editing -->
 
 ## Citation
 
 ```bibtex
 @inproceedings{pan2023draggan,
```

### Comparing `draggan-1.0.0/draggan/api.py` & `draggan-1.0.1/draggan/api.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/inversion.py` & `draggan-1.0.1/draggan/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/lpips/base_model.py` & `draggan-1.0.1/draggan/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/lpips/dist_model.py` & `draggan-1.0.1/draggan/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/lpips/networks_basic.py` & `draggan-1.0.1/draggan/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/lpips/pretrained_networks.py` & `draggan-1.0.1/draggan/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/lpips/util.py` & `draggan-1.0.1/draggan/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/model.py` & `draggan-1.0.1/draggan/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/conv2d_gradfix.py` & `draggan-1.0.1/draggan/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/fused_act.py` & `draggan-1.0.1/draggan/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/fused_bias_act.cpp` & `draggan-1.0.1/draggan/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.0.1/draggan/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/upfirdn2d.cpp` & `draggan-1.0.1/draggan/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/upfirdn2d.py` & `draggan-1.0.1/draggan/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.0.1/draggan/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/draggan/web.py` & `draggan-1.0.1/draggan/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,19 +242,19 @@
         model = gr.State(wrapped_model)
         sample_z = torch.randn([1, 512], device=device)
         latent, noise = wrapped_model.g_ema.prepare([sample_z])
         sample, F = wrapped_model.g_ema.generate(latent, noise)
 
         gr.Markdown(
             """
-            # DragGAN (Unofficial)
+            # DragGAN
             
             Unofficial implementation of [Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
             
-            [Github](https://github.com/Zeqiang-Lai/DragGAN) | [Official Implementation](https://github.com/XingangPan/DragGAN) (Not released yet)
+            [Our Implementation](https://github.com/Zeqiang-Lai/DragGAN) | [Official Implementation](https://github.com/XingangPan/DragGAN) (Not released yet)
 
             ## Tutorial
             
             1. (Optional) Draw a mask indicate the movable region.
             2. Setup a least one pair of handle point and target point.
             3. Click "Drag it". 
             
@@ -269,15 +269,15 @@
             - **Please upload your image at `Setup Handle Points` pannel.** Upload it from `Draw a Mask` would cause errors for now.
             - Due to the limitation of GAN inversion, 
                 - You might wait roughly 1 minute to see the GAN version of the uploaded image.
                 - The shown image might be slightly difference from the uploaded one.
                 - It could also fail to invert the uploaded image and generate very poor results.
                 - Idealy, you should choose the closest model of the uploaded image. For example, choose `stylegan2-ffhq-config-f.pt` for human face. `stylegan2-cat-config-f.pt` for cat.
                 
-            > Please fire an issue if you have encounted any problem. Also don't forgot to give a star to the [Official Repo](https://github.com/XingangPan/DragGAN), [this project](https://github.com/Zeqiang-Lai/DragGAN) could not exist without it.
+            > Please fire an issue if you have encounted any problem. Also don't forgot to give a star to the [Official Repo](https://github.com/XingangPan/DragGAN), [our project](https://github.com/Zeqiang-Lai/DragGAN) could not exist without it.
             """,
         )
         state = gr.State({
             'latent': latent,
             'noise': noise,
             'F': F,
             'sample': sample,
```

### Comparing `draggan-1.0.0/draggan.egg-info/SOURCES.txt` & `draggan-1.0.1/draggan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/setup.py` & `draggan-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='draggan',
     packages=find_packages(),
-    version='1.0.0',
+    version='1.0.1',
     package_data={
         'draggan': ['stylegan2/op/fused_bias_act.cpp', 'stylegan2/op/upfirdn2d.cpp',
                     'stylegan2/op/fused_bias_act_kernel.cu', 'stylegan2/op/upfirdn2d_kernel.cu'], 
     },
     include_package_data=True,
     install_requires=[
         'gradio>=3.28',
```

### Comparing `draggan-1.0.0/stylegan2/inversion.py` & `draggan-1.0.1/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/lpips/base_model.py` & `draggan-1.0.1/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/lpips/dist_model.py` & `draggan-1.0.1/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/lpips/networks_basic.py` & `draggan-1.0.1/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/lpips/pretrained_networks.py` & `draggan-1.0.1/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/lpips/util.py` & `draggan-1.0.1/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/model.py` & `draggan-1.0.1/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/op/conv2d_gradfix.py` & `draggan-1.0.1/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/op/fused_act.py` & `draggan-1.0.1/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.0/stylegan2/op/upfirdn2d.py` & `draggan-1.0.1/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

