# Comparing `tmp/sdkit-1.0.97.tar.gz` & `tmp/sdkit-1.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkit-1.0.97.tar", last modified: Mon May 22 12:36:02 2023, max compression
+gzip compressed data, was "sdkit-1.0.98.tar", last modified: Thu May 25 10:04:23 2023, max compression
```

## Comparing `sdkit-1.0.97.tar` & `sdkit-1.0.98.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:02.372288 sdkit-1.0.97/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.97/LICENSE
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.97/MANIFEST.in
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-22 12:36:02.362004 sdkit-1.0.97/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.97/README.md
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-22 12:35:27.000000 sdkit-1.0.97/pyproject.toml
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.062153 sdkit-1.0.97/sdkit/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3719 2023-05-19 11:22:44.000000 sdkit-1.0.97/sdkit/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.361944 sdkit-1.0.97/sdkit/filter/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.97/sdkit/filter/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1197 2023-05-19 11:22:44.000000 sdkit-1.0.97/sdkit/filter/apply_filters.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/filter/gfpgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      870 2023-05-22 11:11:30.000000 sdkit-1.0.97/sdkit/filter/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.97/sdkit/filter/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.97/sdkit/filter/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.462202 sdkit-1.0.97/sdkit/generate/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.97/sdkit/generate/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9985 2023-05-16 10:02:05.000000 sdkit-1.0.97/sdkit/generate/image_generator.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.97/sdkit/generate/prompt_parser.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.646767 sdkit-1.0.97/sdkit/generate/sampler/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.97/sdkit/generate/sampler/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.97/sdkit/generate/sampler/default_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3396 2023-05-19 11:28:03.000000 sdkit-1.0.97/sdkit/generate/sampler/diffusers_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/generate/sampler/k_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.97/sdkit/generate/sampler/sampler_main.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.742153 sdkit-1.0.97/sdkit/generate/sampler/unipc_samplers/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.97/sdkit/generate/sampler/unipc_samplers/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.97/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.857266 sdkit-1.0.97/sdkit/models/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.97/sdkit/models/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/models/model_downloader.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:01.131972 sdkit-1.0.97/sdkit/models/model_loader/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1747 2023-05-19 11:22:44.000000 sdkit-1.0.97/sdkit/models/model_loader/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/models/model_loader/gfpgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:01.212297 sdkit-1.0.97/sdkit/models/model_loader/hypernetwork/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/models/model_loader/hypernetwork/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/models/model_loader/hypernetwork/hypernetwork.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      686 2023-05-22 10:50:46.000000 sdkit-1.0.97/sdkit/models/model_loader/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-10 14:38:42.000000 sdkit-1.0.97/sdkit/models/model_loader/lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.97/sdkit/models/model_loader/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.97/sdkit/models/model_loader/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:01.372022 sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11522 2023-05-19 13:05:48.000000 sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13171 2023-05-19 13:05:06.000000 sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/optimizations.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.97/sdkit/models/model_loader/vae.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:01.562085 sdkit-1.0.97/sdkit/models/models_db/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.97/sdkit/models/models_db/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:02.031999 sdkit-1.0.97/sdkit/models/models_db/configs/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v2-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v2-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v2-midas-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v2.1-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.97/sdkit/models/models_db/configs/v2.1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.97/sdkit/models/models_db/configs/x4-upscaling.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.97/sdkit/models/models_db/gfpgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.97/sdkit/models/models_db/realesrgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.97/sdkit/models/models_db/stable_diffusion.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.97/sdkit/models/models_db/vae.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/models/scan_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:02.102154 sdkit-1.0.97/sdkit/train/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.97/sdkit/train/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/train/merge_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:02.331771 sdkit-1.0.97/sdkit/utils/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-05-19 11:17:19.000000 sdkit-1.0.97/sdkit/utils/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.97/sdkit/utils/file_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.97/sdkit/utils/hash_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.97/sdkit/utils/http_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-05-19 11:18:10.000000 sdkit-1.0.97/sdkit/utils/image_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.97/sdkit/utils/latent_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.97/sdkit/utils/memory_utils.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-22 12:36:00.182179 sdkit-1.0.97/sdkit.egg-info/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-22 12:35:59.000000 sdkit-1.0.97/sdkit.egg-info/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2317 2023-05-22 12:35:59.000000 sdkit-1.0.97/sdkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-22 12:35:59.000000 sdkit-1.0.97/sdkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-22 12:35:59.000000 sdkit-1.0.97/sdkit.egg-info/requires.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-22 12:35:59.000000 sdkit-1.0.97/sdkit.egg-info/top_level.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-22 12:36:02.372288 sdkit-1.0.97/setup.cfg
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-19 11:22:44.000000 sdkit-1.0.97/setup.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.779315 sdkit-1.0.98/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.98/LICENSE
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.98/MANIFEST.in
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-25 10:04:23.779315 sdkit-1.0.98/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.98/README.md
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-25 10:03:47.000000 sdkit-1.0.98/pyproject.toml
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.221645 sdkit-1.0.98/sdkit/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3719 2023-05-19 11:22:44.000000 sdkit-1.0.98/sdkit/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.497653 sdkit-1.0.98/sdkit/filter/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.98/sdkit/filter/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1197 2023-05-19 11:22:44.000000 sdkit-1.0.98/sdkit/filter/apply_filters.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/filter/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      870 2023-05-22 11:11:30.000000 sdkit-1.0.98/sdkit/filter/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.98/sdkit/filter/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.98/sdkit/filter/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.585014 sdkit-1.0.98/sdkit/generate/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.98/sdkit/generate/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11798 2023-05-25 10:03:04.000000 sdkit-1.0.98/sdkit/generate/image_generator.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.98/sdkit/generate/prompt_parser.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.819646 sdkit-1.0.98/sdkit/generate/sampler/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.98/sdkit/generate/sampler/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.98/sdkit/generate/sampler/default_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3396 2023-05-19 11:28:03.000000 sdkit-1.0.98/sdkit/generate/sampler/diffusers_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/generate/sampler/k_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.98/sdkit/generate/sampler/sampler_main.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.985572 sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.116434 sdkit-1.0.98/sdkit/models/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.98/sdkit/models/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_downloader.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.446139 sdkit-1.0.98/sdkit/models/model_loader/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1747 2023-05-19 11:22:44.000000 sdkit-1.0.98/sdkit/models/model_loader/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_loader/gfpgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.536377 sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/hypernetwork.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      686 2023-05-22 10:50:46.000000 sdkit-1.0.98/sdkit/models/model_loader/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-24 10:30:04.000000 sdkit-1.0.98/sdkit/models/model_loader/lora.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.98/sdkit/models/model_loader/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.98/sdkit/models/model_loader/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.680603 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11522 2023-05-24 10:12:27.000000 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13171 2023-05-19 13:05:06.000000 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/optimizations.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.98/sdkit/models/model_loader/vae.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.894082 sdkit-1.0.98/sdkit/models/models_db/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.98/sdkit/models/models_db/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.466527 sdkit-1.0.98/sdkit/models/models_db/configs/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-midas-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.98/sdkit/models/models_db/configs/x4-upscaling.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.98/sdkit/models/models_db/gfpgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.98/sdkit/models/models_db/realesrgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.98/sdkit/models/models_db/stable_diffusion.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.98/sdkit/models/models_db/vae.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/scan_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.533247 sdkit-1.0.98/sdkit/train/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.98/sdkit/train/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/train/merge_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.750604 sdkit-1.0.98/sdkit/utils/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-05-19 11:17:19.000000 sdkit-1.0.98/sdkit/utils/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.98/sdkit/utils/file_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.98/sdkit/utils/hash_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/utils/http_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-05-19 11:18:10.000000 sdkit-1.0.98/sdkit/utils/image_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.98/sdkit/utils/latent_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.98/sdkit/utils/memory_utils.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.327643 sdkit-1.0.98/sdkit.egg-info/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2317 2023-05-25 10:04:21.000000 sdkit-1.0.98/sdkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/requires.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/top_level.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-25 10:04:23.779315 sdkit-1.0.98/setup.cfg
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-19 11:22:44.000000 sdkit-1.0.98/setup.py
```

### Comparing `sdkit-1.0.97/LICENSE` & `sdkit-1.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/PKG-INFO` & `sdkit-1.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.97
+Version: 1.0.98
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-1.0.97/README.md` & `sdkit-1.0.98/README.md`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/pyproject.toml` & `sdkit-1.0.98/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdkit"
-version = "1.0.97"
+version = "1.0.98"
 authors = [
   {name="cmdr2", email="secondary.cmdr2@gmail.com"},
 ]
 description = "sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!"
 readme = "README.md"
 requires-python = ">=3.8.5"
 classifiers = [
```

### Comparing `sdkit-1.0.97/sdkit/__init__.py` & `sdkit-1.0.98/sdkit/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/filter/apply_filters.py` & `sdkit-1.0.98/sdkit/filter/apply_filters.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/filter/gfpgan.py` & `sdkit-1.0.98/sdkit/filter/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/filter/latent_upscaler.py` & `sdkit-1.0.98/sdkit/filter/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/filter/nsfw_checker.py` & `sdkit-1.0.98/sdkit/filter/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/image_generator.py` & `sdkit-1.0.98/sdkit/generate/image_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from contextlib import nullcontext
 
 import torch
 from pytorch_lightning import seed_everything
 from tqdm import trange
+from typing import Optional
 
 from sdkit import Context
 from sdkit.utils import (
     apply_color_profile,
     base64_str_to_img,
     gc,
     get_image_latent_and_mask,
@@ -35,14 +36,15 @@
     init_image_mask=None,
     prompt_strength: float = 0.8,
     preserve_init_image_color_profile=False,
     sampler_name: str = "euler_a",  # "ddim", "plms", "heun", "euler", "euler_a", "dpm2", "dpm2_a", "lms",
     # "dpm_solver_stability", "dpmpp_2s_a", "dpmpp_2m", "dpmpp_sde", "dpm_fast"
     # "dpm_adaptive"
     hypernetwork_strength: float = 0,
+    tiling = "none",
     lora_alpha: float = 0,
     sampler_params={},
     callback=None,
 ):
     req_args = locals()
 
     try:
@@ -72,14 +74,15 @@
                 init_image,
                 init_image_mask,
                 prompt_strength,
                 # preserve_init_image_color_profile,
                 sampler_name,
                 # hypernetwork_strength,
                 lora_alpha,
+                tiling,
                 # sampler_params,
                 callback,
             )
 
         if "hypernetwork" in context.models:
             context.models["hypernetwork"]["hypernetwork_strength"] = hypernetwork_strength
 
@@ -177,14 +180,15 @@
     # preserve_init_image_color_profile=False,
     sampler_name: str = "euler_a",  # "ddim", "plms", "heun", "euler", "euler_a", "dpm2", "dpm2_a", "lms",
     # "dpm_solver_stability", "dpmpp_2s_a", "dpmpp_2m", "dpmpp_sde", "dpm_fast"
     # "dpm_adaptive"
     # hypernetwork_strength: float = 0,
     lora_alpha: float = 0,
     # sampler_params={},
+    tiling = "none",
     callback=None,
 ):
     from diffusers import (
         StableDiffusionImg2ImgPipeline,
         StableDiffusionInpaintPipeline,
         StableDiffusionInpaintPipelineLegacy,
     )
@@ -252,14 +256,49 @@
         log.info("Applying LoRA..")
         if hasattr(context, "_last_lora_alpha"):
             apply_lora_model(context, -context._last_lora_alpha)  # undo the last LoRA apply
 
         apply_lora_model(context, lora_alpha)
         context._last_lora_alpha = lora_alpha
 
+    #--------------------------------------------------------------------------------------------------
+    #-- https://github.com/huggingface/diffusers/issues/2633
+    log.info("Applying tiling settings")
+    if tiling == "xy":
+       modex = "circular"
+       modey = "circular"
+    elif tiling == "x":
+       modex = "circular"
+       modey = "constant"
+    elif tiling == "y":
+       modex = "constant"
+       modey = "circular"
+    else:   
+       modex = "constant"
+       modey = "constant"
+
+    def asymmetricConv2DConvForward(self, input: torch.Tensor, weight: torch.Tensor, bias: Optional[torch.Tensor]):
+        F = torch.nn.functional
+        self.paddingX = (self._reversed_padding_repeated_twice[0], self._reversed_padding_repeated_twice[1], 0, 0)
+        self.paddingY = (0, 0, self._reversed_padding_repeated_twice[2], self._reversed_padding_repeated_twice[3])
+        working = F.pad(input, self.paddingX, mode=modex)
+        working = F.pad(working, self.paddingY, mode=modey)
+        return F.conv2d(working, weight, bias, self.stride, torch.nn.modules.utils._pair(0), self.dilation, self.groups)
+
+    targets = [operation_to_apply.vae, operation_to_apply.text_encoder, operation_to_apply.unet,]
+    conv_layers = []
+    for target in targets:
+        for module in target.modules():
+            if isinstance(module, torch.nn.Conv2d):
+                conv_layers.append(module)
+
+    for cl in conv_layers:
+        cl._conv_forward = asymmetricConv2DConvForward.__get__(cl, torch.nn.Conv2d)
+
+    #--------------------------------------------------------------------------------------------------
     log.info("Parsing the prompt..")
 
     # make the prompt embeds
     compel = model["compel"]
 
     # temporary hack until compel 1.1.4 is released
     if hasattr(operation_to_apply.text_encoder, "_hf_hook"):
@@ -282,14 +321,15 @@
 
     log.info("Made negative prompt embeds")
     cmd["prompt_embeds"], cmd["negative_prompt_embeds"] = compel.pad_conditioning_tensors_to_same_length(
         [cmd["prompt_embeds"], cmd["negative_prompt_embeds"]]
     )
 
     log.info("Done parsing the prompt")
+    #--------------------------------------------------------------------------------------------------
 
     # apply
     log.info(f"applying: {operation_to_apply}")
     log.info(f"Running on diffusers: {cmd}")
 
     return operation_to_apply(**cmd).images
```

### Comparing `sdkit-1.0.97/sdkit/generate/prompt_parser.py` & `sdkit-1.0.98/sdkit/generate/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/sampler/default_samplers.py` & `sdkit-1.0.98/sdkit/generate/sampler/default_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/sampler/diffusers_samplers.py` & `sdkit-1.0.98/sdkit/generate/sampler/diffusers_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/sampler/k_samplers.py` & `sdkit-1.0.98/sdkit/generate/sampler/k_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/sampler/sampler_main.py` & `sdkit-1.0.98/sdkit/generate/sampler/sampler_main.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/sampler/unipc_samplers/__init__.py` & `sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py` & `sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_downloader.py` & `sdkit-1.0.98/sdkit/models/model_downloader.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/__init__.py` & `sdkit-1.0.98/sdkit/models/model_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/gfpgan.py` & `sdkit-1.0.98/sdkit/models/model_loader/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/hypernetwork/__init__.py` & `sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/hypernetwork/hypernetwork.py` & `sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/hypernetwork.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/latent_upscaler.py` & `sdkit-1.0.98/sdkit/models/model_loader/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/lora.py` & `sdkit-1.0.98/sdkit/models/model_loader/lora.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/nsfw_checker.py` & `sdkit-1.0.98/sdkit/models/model_loader/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/realesrgan.py` & `sdkit-1.0.98/sdkit/models/model_loader/realesrgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/__init__.py` & `sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py` & `sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/stable_diffusion/optimizations.py` & `sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/optimizations.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/model_loader/vae.py` & `sdkit-1.0.98/sdkit/models/model_loader/vae.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/__init__.py` & `sdkit-1.0.98/sdkit/models/models_db/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v1-inference.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v1-inpainting-inference.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v2-inference-v.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v2-inference.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v2-inpainting-inference.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v2-midas-inference.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v2.1-inference-v.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/v2.1-inference.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/configs/x4-upscaling.yaml` & `sdkit-1.0.98/sdkit/models/models_db/configs/x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/gfpgan.json` & `sdkit-1.0.98/sdkit/models/models_db/gfpgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/realesrgan.json` & `sdkit-1.0.98/sdkit/models/models_db/realesrgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/models/models_db/stable_diffusion.json` & `sdkit-1.0.98/sdkit/models/models_db/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/train/merge_models.py` & `sdkit-1.0.98/sdkit/train/merge_models.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/__init__.py` & `sdkit-1.0.98/sdkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/file_utils.py` & `sdkit-1.0.98/sdkit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/hash_utils.py` & `sdkit-1.0.98/sdkit/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/http_utils.py` & `sdkit-1.0.98/sdkit/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/image_utils.py` & `sdkit-1.0.98/sdkit/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/latent_utils.py` & `sdkit-1.0.98/sdkit/utils/latent_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit/utils/memory_utils.py` & `sdkit-1.0.98/sdkit/utils/memory_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.97/sdkit.egg-info/PKG-INFO` & `sdkit-1.0.98/sdkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.97
+Version: 1.0.98
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-1.0.97/sdkit.egg-info/SOURCES.txt` & `sdkit-1.0.98/sdkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

