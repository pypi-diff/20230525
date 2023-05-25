# Comparing `tmp/draggan-1.0.5.tar.gz` & `tmp/draggan-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-z6mwnlfh/draggan-1.0.5.tar", last modified: Thu May 25 15:04:53 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-z_nvt3js/draggan-1.0.6.tar", last modified: Thu May 25 16:52:04 2023, max compression
```

## Comparing `draggan-1.0.5.tar` & `draggan-1.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 15:04:53.000000 draggan-1.0.5/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5195 2023-05-25 13:40:32.000000 draggan-1.0.5/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.5/draggan/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.5/draggan/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      873 2023-05-25 08:31:09.000000 draggan-1.0.5/draggan/app.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.5/draggan/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.5/draggan/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.5/draggan/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.5/draggan/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:35:13.000000 draggan-1.0.5/draggan/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.5/draggan/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.5/draggan/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.5/draggan/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:21.000000 draggan-1.0.5/draggan/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.5/draggan/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12819 2023-05-25 15:02:58.000000 draggan-1.0.5/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       18 2023-05-25 15:04:53.000000 draggan-1.0.5/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-25 15:04:53.000000 draggan-1.0.5/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      620 2023-05-25 15:04:32.000000 draggan-1.0.5/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.5/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.5/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.5/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 15:04:53.000000 draggan-1.0.5/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 14:03:01.000000 draggan-1.0.5/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.5/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:49:11.000000 draggan-1.0.5/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:07.000000 draggan-1.0.5/stylegan2/op/upfirdn2d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 16:52:04.000000 draggan-1.0.6/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5302 2023-05-25 15:13:46.000000 draggan-1.0.6/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.6/draggan/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.6/draggan/api.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      873 2023-05-25 08:31:09.000000 draggan-1.0.6/draggan/app.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.6/draggan/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.6/draggan/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.6/draggan/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.6/draggan/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:35:13.000000 draggan-1.0.6/draggan/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.6/draggan/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.6/draggan/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.6/draggan/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:21.000000 draggan-1.0.6/draggan/stylegan2/op/upfirdn2d.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.6/draggan/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12819 2023-05-25 15:02:58.000000 draggan-1.0.6/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-05-25 16:52:04.000000 draggan-1.0.6/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-25 16:52:04.000000 draggan-1.0.6/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      616 2023-05-25 16:52:00.000000 draggan-1.0.6/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.6/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.6/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.6/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 16:52:04.000000 draggan-1.0.6/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 14:03:01.000000 draggan-1.0.6/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.6/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:49:11.000000 draggan-1.0.6/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:07.000000 draggan-1.0.6/stylegan2/op/upfirdn2d.py
```

### Comparing `draggan-1.0.5/README.md` & `draggan-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 pip install draggan
 ```
 
 Launch the Gradio demo
 
 ```bash
 python -m draggan.web
+# running on cpu
+python -m draggan.web --device cpu
 ```
 
 ### Clone and Install 
 
 Ensure you have a GPU and CUDA installed. We use Python 3.7 for testing, other versions (>= 3.7) of Python should work too, but not tested. We recommend to use [Conda](https://conda.io/projects/conda/en/stable/user-guide/install/download.html) to prepare all the requirements.
 
 For Windows users, you might encounter some issues caused by StyleGAN custom ops, youd could find some solutions from the [issues pannel](https://github.com/Zeqiang-Lai/DragGAN/issues). We are also working on a more friendly package without setup.
@@ -100,16 +102,18 @@
 conda create -n draggan python=3.7
 conda activate draggan
 pip install -r requirements.txt
 ```
 
 Launch the Gradio demo
 
-```
+```bash
 python gradio_app.py
+# running on cpu
+python gradio_app.py --device cpu
 ```
 
 > If you have any issue for downloading the checkpoint, you could manually download it from [here](https://huggingface.co/aaronb/StyleGAN2/tree/main) and put it into the folder `checkpoints`.
 
 ## Citation
 
 ```bibtex
```

### Comparing `draggan-1.0.5/draggan/api.py` & `draggan-1.0.6/draggan/api.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/app.py` & `draggan-1.0.6/draggan/app.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/inversion.py` & `draggan-1.0.6/draggan/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/lpips/base_model.py` & `draggan-1.0.6/draggan/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/lpips/dist_model.py` & `draggan-1.0.6/draggan/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/lpips/networks_basic.py` & `draggan-1.0.6/draggan/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/lpips/pretrained_networks.py` & `draggan-1.0.6/draggan/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/lpips/util.py` & `draggan-1.0.6/draggan/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/model.py` & `draggan-1.0.6/draggan/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/conv2d_gradfix.py` & `draggan-1.0.6/draggan/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/fused_act.py` & `draggan-1.0.6/draggan/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/fused_bias_act.cpp` & `draggan-1.0.6/draggan/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.0.6/draggan/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/upfirdn2d.cpp` & `draggan-1.0.6/draggan/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/upfirdn2d.py` & `draggan-1.0.6/draggan/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.0.6/draggan/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan/web.py` & `draggan-1.0.6/draggan/web.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/draggan.egg-info/SOURCES.txt` & `draggan-1.0.6/draggan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/setup.py` & `draggan-1.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='draggan',
-    packages=find_packages(),
-    version='1.0.5',
+    packages=['draggan'],
+    version='1.0.6',
     package_data={
         'draggan': ['stylegan2/op/fused_bias_act.cpp', 'stylegan2/op/upfirdn2d.cpp',
                     'stylegan2/op/fused_bias_act_kernel.cu', 'stylegan2/op/upfirdn2d_kernel.cu'], 
     },
     include_package_data=True,
     install_requires=[
         'gradio==3.28.1',
```

### Comparing `draggan-1.0.5/stylegan2/inversion.py` & `draggan-1.0.6/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/lpips/base_model.py` & `draggan-1.0.6/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/lpips/dist_model.py` & `draggan-1.0.6/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/lpips/networks_basic.py` & `draggan-1.0.6/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/lpips/pretrained_networks.py` & `draggan-1.0.6/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/lpips/util.py` & `draggan-1.0.6/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/model.py` & `draggan-1.0.6/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/op/conv2d_gradfix.py` & `draggan-1.0.6/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/op/fused_act.py` & `draggan-1.0.6/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.5/stylegan2/op/upfirdn2d.py` & `draggan-1.0.6/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

