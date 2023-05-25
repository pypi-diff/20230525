# Comparing `tmp/draggan-1.0.3.tar.gz` & `tmp/draggan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-m_zcm20c/draggan-1.0.3.tar", last modified: Thu May 25 14:28:12 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-scidizzp/draggan-1.0.4.tar", last modified: Thu May 25 14:29:34 2023, max compression
```

## Comparing `draggan-1.0.3.tar` & `draggan-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 14:28:12.000000 draggan-1.0.3/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5195 2023-05-25 13:40:32.000000 draggan-1.0.3/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.3/draggan/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.3/draggan/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      873 2023-05-25 08:31:09.000000 draggan-1.0.3/draggan/app.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.3/draggan/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.3/draggan/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.3/draggan/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.3/draggan/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:35:13.000000 draggan-1.0.3/draggan/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.3/draggan/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.3/draggan/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.3/draggan/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:21.000000 draggan-1.0.3/draggan/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.3/draggan/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12461 2023-05-25 12:06:09.000000 draggan-1.0.3/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      102 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       18 2023-05-25 14:28:12.000000 draggan-1.0.3/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-25 14:28:12.000000 draggan-1.0.3/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      627 2023-05-25 14:25:35.000000 draggan-1.0.3/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.3/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.3/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.3/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:28:12.000000 draggan-1.0.3/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 14:03:01.000000 draggan-1.0.3/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.3/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:49:11.000000 draggan-1.0.3/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:07.000000 draggan-1.0.3/stylegan2/op/upfirdn2d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 14:29:34.000000 draggan-1.0.4/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5195 2023-05-25 13:40:32.000000 draggan-1.0.4/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.4/draggan/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.4/draggan/api.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      873 2023-05-25 08:31:09.000000 draggan-1.0.4/draggan/app.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.4/draggan/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.4/draggan/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.4/draggan/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.4/draggan/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:35:13.000000 draggan-1.0.4/draggan/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.4/draggan/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.4/draggan/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.4/draggan/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:21.000000 draggan-1.0.4/draggan/stylegan2/op/upfirdn2d.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.4/draggan/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12461 2023-05-25 12:06:09.000000 draggan-1.0.4/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       18 2023-05-25 14:29:34.000000 draggan-1.0.4/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-25 14:29:34.000000 draggan-1.0.4/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      620 2023-05-25 14:29:11.000000 draggan-1.0.4/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.4/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.4/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.4/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 14:29:34.000000 draggan-1.0.4/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 14:03:01.000000 draggan-1.0.4/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.4/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4293 2023-05-25 07:49:11.000000 draggan-1.0.4/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6690 2023-05-25 14:25:07.000000 draggan-1.0.4/stylegan2/op/upfirdn2d.py
```

### Comparing `draggan-1.0.3/README.md` & `draggan-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/api.py` & `draggan-1.0.4/draggan/api.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/app.py` & `draggan-1.0.4/draggan/app.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/inversion.py` & `draggan-1.0.4/draggan/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/lpips/base_model.py` & `draggan-1.0.4/draggan/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/lpips/dist_model.py` & `draggan-1.0.4/draggan/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/lpips/networks_basic.py` & `draggan-1.0.4/draggan/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/lpips/pretrained_networks.py` & `draggan-1.0.4/draggan/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/lpips/util.py` & `draggan-1.0.4/draggan/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/model.py` & `draggan-1.0.4/draggan/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/conv2d_gradfix.py` & `draggan-1.0.4/draggan/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/fused_act.py` & `draggan-1.0.4/draggan/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/fused_bias_act.cpp` & `draggan-1.0.4/draggan/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.0.4/draggan/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/upfirdn2d.cpp` & `draggan-1.0.4/draggan/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/upfirdn2d.py` & `draggan-1.0.4/draggan/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.0.4/draggan/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan/web.py` & `draggan-1.0.4/draggan/web.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/draggan.egg-info/SOURCES.txt` & `draggan-1.0.4/draggan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/setup.py` & `draggan-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='draggan',
     packages=find_packages(),
-    version='1.0.3',
+    version='1.0.4',
     package_data={
         'draggan': ['stylegan2/op/fused_bias_act.cpp', 'stylegan2/op/upfirdn2d.cpp',
                     'stylegan2/op/fused_bias_act_kernel.cu', 'stylegan2/op/upfirdn2d_kernel.cu'], 
     },
     include_package_data=True,
     install_requires=[
-        'gradio>=3.28',
+        'gradio==3.28.1',
         'tqdm',
         'torch>=1.8',
         'torchvision',
         'numpy',
         'ninja',
         'fire',
         'imageio',
         'imageio-ffmpeg',
         'scikit-image',
         'IPython',
-        
     ]
 )
```

### Comparing `draggan-1.0.3/stylegan2/inversion.py` & `draggan-1.0.4/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/lpips/base_model.py` & `draggan-1.0.4/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/lpips/dist_model.py` & `draggan-1.0.4/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/lpips/networks_basic.py` & `draggan-1.0.4/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/lpips/pretrained_networks.py` & `draggan-1.0.4/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/lpips/util.py` & `draggan-1.0.4/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/model.py` & `draggan-1.0.4/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/op/conv2d_gradfix.py` & `draggan-1.0.4/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/op/fused_act.py` & `draggan-1.0.4/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.3/stylegan2/op/upfirdn2d.py` & `draggan-1.0.4/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

