# Comparing `tmp/optimum-graphcore-0.6.0.tar.gz` & `tmp/optimum-graphcore-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-graphcore-0.6.0.tar", last modified: Wed Apr  5 13:07:22 2023, max compression
+gzip compressed data, was "optimum-graphcore-0.6.1.tar", last modified: Thu May 25 15:28:44 2023, max compression
```

## Comparing `optimum-graphcore-0.6.0.tar` & `optimum-graphcore-0.6.1.tar`

### file list

```diff
@@ -1,112 +1,123 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)     9032 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     7990 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:21.998644 optimum-graphcore-0.6.0/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2619 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/data/
--rw-rw-r--   0 michael   (1000) michael   (1000)      885 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/data/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5913 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/data/data_collator.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/
--rw-rw-r--   0 michael   (1000) michael   (1000)      204 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)      211 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 michael   (1000) michael   (1000)      311 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4708 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      227 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17462 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1732 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    63463 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/generation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    19589 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/ipu_configuration.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5749 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/modelcard.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22931 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/modeling_utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/models/
--rw-rw-r--   0 michael   (1000) michael   (1000)      892 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/models/bart/
--rw-rw-r--   0 michael   (1000) michael   (1000)      883 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/bart/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    46346 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/bart/modeling_bart.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.002644 optimum-graphcore-0.6.0/optimum/graphcore/models/bert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1032 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/bert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6831 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/bert/bert_fused_attention.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    23084 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/bert/modeling_bert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/
--rw-rw-r--   0 michael   (1000) michael   (1000)      849 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2800 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/modeling_convnext.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1016 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/optimized_convnextlayer.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/deberta/
--rw-rw-r--   0 michael   (1000) michael   (1000)      978 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/deberta/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22921 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/deberta/modeling_deberta.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/distilbert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1035 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/distilbert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15640 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/distilbert/modeling_distilbert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      924 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    16032 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1606 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1918 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10205 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/groupbert_attention.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3334 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/groupbert_convolution.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2929 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/groupbert_ffn.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    35622 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/modeling_groupbert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/hubert/
--rw-rw-r--   0 michael   (1000) michael   (1000)      848 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/hubert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6667 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/hubert/ipu_layer_drop.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2975 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/hubert/modeling_hubert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/lxmert/
--rw-rw-r--   0 michael   (1000) michael   (1000)      843 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/lxmert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6199 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/lxmert/modeling_lxmert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/roberta/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1017 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/roberta/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    14933 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/roberta/modeling_roberta.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/t5/
--rw-rw-r--   0 michael   (1000) michael   (1000)      839 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/t5/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    20724 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/t5/modeling_t5.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/vit/
--rw-rw-r--   0 michael   (1000) michael   (1000)      839 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/vit/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2155 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/vit/modeling_vit.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      866 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4396 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7587 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    24241 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/models/whisper/
--rw-rw-r--   0 michael   (1000) michael   (1000)      849 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/whisper/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27660 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/models/whisper/modeling_whisper.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)    19822 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/pipelines/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1208 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/pipelines/fill_mask.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3060 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/pipelines/text2text_generation.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3233 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/pipelines/token_classification.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3890 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/pipelines/zero_shot_classification.py
--rw-rw-r--   0 michael   (1000) michael   (1000)   105063 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/trainer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/trainer_pt_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10994 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/trainer_seq2seq.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2266 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/trainer_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    46301 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/training_args.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2879 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/optimum/graphcore/training_args_seq2seq.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum/graphcore/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1128 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/optimum/graphcore/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-04-05 12:53:24.000000 optimum-graphcore-0.6.0/optimum/graphcore/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     9032 2023-04-05 13:07:21.000000 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     3792 2023-04-05 13:07:21.000000 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 13:07:21.000000 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 12:57:36.000000 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      244 2023-04-05 13:07:21.000000 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-04-05 13:07:21.000000 optimum-graphcore-0.6.0/optimum_graphcore.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)      674 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      811 2023-04-05 13:07:22.010644 optimum-graphcore-0.6.0/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2232 2023-04-05 13:07:13.000000 optimum-graphcore-0.6.0/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-05 13:07:22.006644 optimum-graphcore-0.6.0/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    22910 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3338 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/tests/test_examples_match_transformers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    19221 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/tests/test_ipu_configuration.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1809 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.0/tests/test_modeling_common.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12714 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/tests/test_pipelined_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    61898 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.0/tests/test_trainer.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8905 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.713887 optimum-graphcore-0.6.1/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2680 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/data/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      885 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/data/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5927 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/data/data_collator.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      204 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      211 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      311 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4641 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      227 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17507 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1732 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/generation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      709 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13526 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/attention_mixin.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6733 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/logits_process.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20117 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/on_device_generation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    86113 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    39210 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/ipu_configuration.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5749 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/modelcard.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    30935 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/modeling_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/models/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      897 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/models/bart/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      883 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bart/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    49792 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bart/modeling_bart.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1032 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6831 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/bert_fused_attention.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22148 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/modeling_bert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      849 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2801 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/modeling_convnext.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1016 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/optimized_convnextlayer.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      978 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22415 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/modeling_deberta.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1035 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15150 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/modeling_distilbert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      924 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15345 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/modeling_gpt2.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1606 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1918 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10205 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_attention.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3334 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_convolution.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2929 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_ffn.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35160 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/modeling_groupbert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      848 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6667 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/ipu_layer_drop.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8003 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/modeling_hubert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      843 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6199 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/modeling_lxmert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      841 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27199 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/modeling_mt5.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1017 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14463 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/modeling_roberta.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/t5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      839 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/t5/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    21486 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/t5/modeling_t5.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/vit/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      839 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/vit/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2156 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/vit/modeling_vit.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      866 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4396 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7587 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    24383 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      972 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2193 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/feature_extraction_whisper.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    21496 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/modeling_whisper.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1226 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/processing_whisper.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20004 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1208 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/fill_mask.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3060 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/text2text_generation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3233 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/token_classification.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3890 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/zero_shot_classification.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)   107693 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer_pt_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12049 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer_seq2seq.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2266 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    47190 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/training_args.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2879 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/training_args_seq2seq.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1128 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-05-25 15:19:12.000000 optimum-graphcore-0.6.1/optimum/graphcore/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4214 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 12:57:36.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      674 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      811 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2236 2023-05-25 15:19:28.000000 optimum-graphcore-0.6.1/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22929 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3338 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25361 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_ipu_configuration.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     1809 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/tests/test_modeling_common.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5702 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_modeling_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12759 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_pipelined_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    61891 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_trainer.py
```

### Comparing `optimum-graphcore-0.6.0/LICENSE` & `optimum-graphcore-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/MANIFEST.in` & `optimum-graphcore-0.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/PKG-INFO` & `optimum-graphcore-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-graphcore
-Version: 0.6.0
+Version: 0.6.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://huggingface.co/hardware
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,training,ipu
 Classifier: Development Status :: 3 - Alpha
@@ -17,33 +17,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: quality
 License-File: LICENSE
 
+[![examples](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-examples.yml/badge.svg)](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-examples.yml) [![pipelines](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-pipelines.yml/badge.svg)](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-pipelines.yml)
+
 <p align="center">
     <img src="readme_logo.png" />
 </p>
 
 # Optimum Graphcore
 
 🤗 Optimum Graphcore is the interface between the 🤗 Transformers library and [Graphcore IPUs](https://www.graphcore.ai/products/ipu).
-It provides a set of tools enabling model parallelization and loading on IPUs, training and fine-tuning on all the tasks already supported by Transformers while being compatible with the Hugging Face Hub and every model available on it out of the box.
+It provides a set of tools enabling model parallelization and loading on IPUs, training, fine-tuning and inference on all the tasks already supported by 🤗 Transformers while being compatible with the 🤗 Hub and every model available on it out of the box.
 
 ## What is an Intelligence Processing Unit (IPU)?
 Quote from the Hugging Face [blog post](https://huggingface.co/blog/graphcore#what-is-an-intelligence-processing-unit):
 >IPUs are the processors that power Graphcore’s IPU-POD datacenter compute systems. This new type of processor is designed to support the very specific computational requirements of AI and machine learning. Characteristics such as fine-grained parallelism, low precision arithmetic, and the ability to handle sparsity have been built into our silicon.
 
 > Instead of adopting a SIMD/SIMT architecture like GPUs, Graphcore’s IPU uses a massively parallel, MIMD architecture, with ultra-high bandwidth memory placed adjacent to the processor cores, right on the silicon die.
 
 > This design delivers high performance and new levels of efficiency, whether running today’s most popular models, such as BERT and EfficientNet, or exploring next-generation AI applications.
 
 ## Poplar SDK setup
-A Poplar SDK environment needs to be enabled to use this library. Please refer to Graphcore's [Getting Started](https://docs.graphcore.ai/en/latest/getting-started.html) guide.
+A Poplar SDK environment needs to be enabled to use this library. Please refer to Graphcore's [Getting Started](https://docs.graphcore.ai/en/latest/getting-started.html) guides.
 
 ## Install
 To install the latest release of this package:
 
 `pip install optimum-graphcore`
 
 Optimum Graphcore is a fast-moving project, and you may want to install from source.
@@ -71,17 +73,17 @@
 Please install the requirements for every example:
 
 ```
 cd <example-folder>
 pip install -r requirements.txt
 ```
 
-## How to use it?
+## How to use Optimum Graphcore
 🤗 Optimum Graphcore was designed with one goal in mind: **make training and evaluation straightforward for any 🤗 Transformers user while leveraging the complete power of IPUs.**
-It requires minimal compared to using 🤗 Transformers.
+It requires minimal changes if you are already using 🤗 Transformers.
 
 To immediately use a model on a given input (text, image, audio, ...), we support the `pipeline` API:
 
 ```diff
 ->>> from transformers import pipeline
 +>>> from optimum.graphcore import pipeline
 
@@ -117,28 +119,30 @@
      model=model,
 +    ipu_config=ipu_config,
      args=training_args,
      train_dataset=train_dataset if training_args.do_train else None,
      ...  # Other arguments
 ```
 
-For more information, check our [documentation](https://huggingface.co/docs/optimum/graphcore_index)
+For more information, refer to the full [🤗 Optimum Graphcore documentation](https://huggingface.co/docs/optimum/graphcore_index).
 
-## Supported Models
+## Supported models
 The following model architectures and tasks are currently supported by 🤗 Optimum Graphcore:
-|            | Pre-Training | Masked LM | Causal LM | Seq2Seq LM (Summarization, Translation, etc) | Text Classification | Token Classification | Question Answering | Multiple Choice | Image Classification |
-|------------|--------------|-----------|-----------|----------------------------------------------|-------------------------|----------------------|--------------------|-----------------|----------------------|
-| BART       | ✅            |           | ❌         | ✅                                            | ✅                       |                      | ❌                  |                 |                      |
-| BERT       | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| ConvNeXt   | ✅            |           |           |                                              |                         |                      |                    |                 | ✅                    |
-| DeBERTa    | ✅            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  |                 |                      |
-| DistilBERT | ❌            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| GPT-2      | ✅            |           | ✅         |                                              | ✅                       | ✅                    |                    |                 |                      |
-| [GroupBERT](https://arxiv.org/abs/2106.05822)   | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| HuBERT     | ❌            |           |           |                                              | ✅                       |                      |                    |                 |                      |
-| LXMERT     | ❌            |           |           |                                              |                         |                      | ✅                  |                 |                      |
-| RoBERTa    | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| T5         | ✅            |           |           | ✅                                            |                         |                      |                    |                 |                      |
-| ViT        | ❌            |           |           |                                              |                         |                      |                    |                 | ✅                    |
-| Wav2Vec2   | ✅            |           |           |                                              |                         |                      |                    |                 |                      |
+|            | Pre-Training | Masked LM | Causal LM | Seq2Seq LM (Summarization, Translation, etc) | Sequence Classification | Token Classification | Question Answering | Multiple Choice | Image Classification | CTC |
+|------------|--------------|-----------|-----------|----------------------------------------------|-------------------------|----------------------|--------------------|-----------------|----------------------| ------------ |
+| BART       | ✅            |           | ❌         | ✅                                            | ✅                       |                      | ❌                  |                 |                      |             |
+| BERT       | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| ConvNeXt   | ✅            |           |           |                                              |                         |                      |                    |                 | ✅                    |             |
+| DeBERTa    | ✅            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  |                 |                      |             |
+| DistilBERT | ❌            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| GPT-2      | ✅            |           | ✅         |                                              | ✅                       | ✅                    |                    |                 |                      |             |
+| [GroupBERT](https://arxiv.org/abs/2106.05822)   | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| HuBERT     | ❌            |           |           |                                              | ✅                       |                      |                    |                 |                      |       ✅      |
+| LXMERT     | ❌            |           |           |                                              |                         |                      | ✅                  |                 |                      |             |
+| RoBERTa    | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| T5         | ✅            |           |           | ✅                                            |                         |                      |                    |                 |                      |             |
+| ViT        | ❌            |           |           |                                              |                         |                      |                    |                 | ✅                    |             |
+| Wav2Vec2   | ✅            |           |           |                                              |                         |                      |                    |                 |                      |      ✅        |
+| Whisper   |    ❌          |           |           |                    ✅                           |                          |                      |                    |                 |                      |              |
+
 
 If you find any issue while using those, please open an issue or a pull request.
```

### Comparing `optimum-graphcore-0.6.0/README.md` & `optimum-graphcore-0.6.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+[![examples](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-examples.yml/badge.svg)](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-examples.yml) [![pipelines](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-pipelines.yml/badge.svg)](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-pipelines.yml)
+
 <p align="center">
     <img src="readme_logo.png" />
 </p>
 
 # Optimum Graphcore
 
 🤗 Optimum Graphcore is the interface between the 🤗 Transformers library and [Graphcore IPUs](https://www.graphcore.ai/products/ipu).
-It provides a set of tools enabling model parallelization and loading on IPUs, training and fine-tuning on all the tasks already supported by Transformers while being compatible with the Hugging Face Hub and every model available on it out of the box.
+It provides a set of tools enabling model parallelization and loading on IPUs, training, fine-tuning and inference on all the tasks already supported by 🤗 Transformers while being compatible with the 🤗 Hub and every model available on it out of the box.
 
 ## What is an Intelligence Processing Unit (IPU)?
 Quote from the Hugging Face [blog post](https://huggingface.co/blog/graphcore#what-is-an-intelligence-processing-unit):
 >IPUs are the processors that power Graphcore’s IPU-POD datacenter compute systems. This new type of processor is designed to support the very specific computational requirements of AI and machine learning. Characteristics such as fine-grained parallelism, low precision arithmetic, and the ability to handle sparsity have been built into our silicon.
 
 > Instead of adopting a SIMD/SIMT architecture like GPUs, Graphcore’s IPU uses a massively parallel, MIMD architecture, with ultra-high bandwidth memory placed adjacent to the processor cores, right on the silicon die.
 
 > This design delivers high performance and new levels of efficiency, whether running today’s most popular models, such as BERT and EfficientNet, or exploring next-generation AI applications.
 
 ## Poplar SDK setup
-A Poplar SDK environment needs to be enabled to use this library. Please refer to Graphcore's [Getting Started](https://docs.graphcore.ai/en/latest/getting-started.html) guide.
+A Poplar SDK environment needs to be enabled to use this library. Please refer to Graphcore's [Getting Started](https://docs.graphcore.ai/en/latest/getting-started.html) guides.
 
 ## Install
 To install the latest release of this package:
 
 `pip install optimum-graphcore`
 
 Optimum Graphcore is a fast-moving project, and you may want to install from source.
@@ -48,17 +50,17 @@
 Please install the requirements for every example:
 
 ```
 cd <example-folder>
 pip install -r requirements.txt
 ```
 
-## How to use it?
+## How to use Optimum Graphcore
 🤗 Optimum Graphcore was designed with one goal in mind: **make training and evaluation straightforward for any 🤗 Transformers user while leveraging the complete power of IPUs.**
-It requires minimal compared to using 🤗 Transformers.
+It requires minimal changes if you are already using 🤗 Transformers.
 
 To immediately use a model on a given input (text, image, audio, ...), we support the `pipeline` API:
 
 ```diff
 ->>> from transformers import pipeline
 +>>> from optimum.graphcore import pipeline
 
@@ -94,28 +96,30 @@
      model=model,
 +    ipu_config=ipu_config,
      args=training_args,
      train_dataset=train_dataset if training_args.do_train else None,
      ...  # Other arguments
 ```
 
-For more information, check our [documentation](https://huggingface.co/docs/optimum/graphcore_index)
+For more information, refer to the full [🤗 Optimum Graphcore documentation](https://huggingface.co/docs/optimum/graphcore_index).
 
-## Supported Models
+## Supported models
 The following model architectures and tasks are currently supported by 🤗 Optimum Graphcore:
-|            | Pre-Training | Masked LM | Causal LM | Seq2Seq LM (Summarization, Translation, etc) | Text Classification | Token Classification | Question Answering | Multiple Choice | Image Classification |
-|------------|--------------|-----------|-----------|----------------------------------------------|-------------------------|----------------------|--------------------|-----------------|----------------------|
-| BART       | ✅            |           | ❌         | ✅                                            | ✅                       |                      | ❌                  |                 |                      |
-| BERT       | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| ConvNeXt   | ✅            |           |           |                                              |                         |                      |                    |                 | ✅                    |
-| DeBERTa    | ✅            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  |                 |                      |
-| DistilBERT | ❌            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| GPT-2      | ✅            |           | ✅         |                                              | ✅                       | ✅                    |                    |                 |                      |
-| [GroupBERT](https://arxiv.org/abs/2106.05822)   | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| HuBERT     | ❌            |           |           |                                              | ✅                       |                      |                    |                 |                      |
-| LXMERT     | ❌            |           |           |                                              |                         |                      | ✅                  |                 |                      |
-| RoBERTa    | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| T5         | ✅            |           |           | ✅                                            |                         |                      |                    |                 |                      |
-| ViT        | ❌            |           |           |                                              |                         |                      |                    |                 | ✅                    |
-| Wav2Vec2   | ✅            |           |           |                                              |                         |                      |                    |                 |                      |
+|            | Pre-Training | Masked LM | Causal LM | Seq2Seq LM (Summarization, Translation, etc) | Sequence Classification | Token Classification | Question Answering | Multiple Choice | Image Classification | CTC |
+|------------|--------------|-----------|-----------|----------------------------------------------|-------------------------|----------------------|--------------------|-----------------|----------------------| ------------ |
+| BART       | ✅            |           | ❌         | ✅                                            | ✅                       |                      | ❌                  |                 |                      |             |
+| BERT       | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| ConvNeXt   | ✅            |           |           |                                              |                         |                      |                    |                 | ✅                    |             |
+| DeBERTa    | ✅            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  |                 |                      |             |
+| DistilBERT | ❌            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| GPT-2      | ✅            |           | ✅         |                                              | ✅                       | ✅                    |                    |                 |                      |             |
+| [GroupBERT](https://arxiv.org/abs/2106.05822)   | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| HuBERT     | ❌            |           |           |                                              | ✅                       |                      |                    |                 |                      |       ✅      |
+| LXMERT     | ❌            |           |           |                                              |                         |                      | ✅                  |                 |                      |             |
+| RoBERTa    | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| T5         | ✅            |           |           | ✅                                            |                         |                      |                    |                 |                      |             |
+| ViT        | ❌            |           |           |                                              |                         |                      |                    |                 | ✅                    |             |
+| Wav2Vec2   | ✅            |           |           |                                              |                         |                      |                    |                 |                      |      ✅        |
+| Whisper   |    ❌          |           |           |                    ✅                           |                          |                      |                    |                 |                      |              |
+
 
 If you find any issue while using those, please open an issue or a pull request.
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from .models.gpt2 import (
     PipelinedGPT2ForSequenceClassification,
     PipelinedGPT2ForTokenClassification,
     PipelinedGPT2LMHeadModel,
 )
 from .models.hubert import PipelinedHubertForSequenceClassification
 from .models.lxmert import PipelinedLxmertForQuestionAnswering
+from .models.mt5 import PipelinedMT5ForConditionalGeneration
 from .models.roberta import (
     PipelinedRobertaForMaskedLM,
     PipelinedRobertaForMultipleChoice,
     PipelinedRobertaForQuestionAnswering,
     PipelinedRobertaForSequenceClassification,
     PipelinedRobertaForTokenClassification,
 )
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/data/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/data/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/data/data_collator.py` & `optimum-graphcore-0.6.1/optimum/graphcore/data/data_collator.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from transformers.data import DataCollatorForLanguageModeling
 from transformers.data.data_collator import DataCollator
 from transformers.tokenization_utils_base import BatchEncoding
 
 
 def pad_on_batch_axis(batch_size: int) -> Callable[[DataCollator], DataCollator]:
     """
-    Creates a DataCollator wrapper that pads the batches generated by the DataCollator on the batch axis to generate
+    Creates a `DataCollator` wrapper that pads the batches generated by `DataCollator` on the batch axis to generate
     fixed size batches. It implements the padding by repeating elements of the batch to reach the padded sized.
     """
 
     def pad_tensor(x: Tensor) -> Tensor:
         if batch_size != x.size(0):
             repeat_dims = torch.ones(x.ndim, dtype=int, requires_grad=False)
             num_repeats = batch_size // x.size(0) + 1
@@ -55,16 +55,18 @@
     def __init__(self, max_seq_length, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.max_seq_length = max_seq_length
         self.max_num_masked_tokens = self._calculate_max_num_masked_tokens(max_seq_length)
 
     def _calculate_max_num_masked_tokens(self, max_seq_length):
         """
-        Get the max number of masked tokens. The number of masked tokens follows a binomial distribution. We approximate
-        the binomial distribution with an Gaussian distribution and cap the maximum number of masked tokens to 2 standard
+        Gets the maximum number of masked tokens.
+
+        The number of masked tokens follows a binomial distribution. We approximate
+        the binomial distribution with a Gaussian distribution and cap the maximum number of masked tokens to two standard
         deviations above the mean.
         """
         import math
 
         mean = max_seq_length * self.mlm_probability
         var = max_seq_length * self.mlm_probability * (1 - self.mlm_probability)
         std = math.sqrt(var)
@@ -80,15 +82,15 @@
         # Necessary for poptorch.DataLoaderMode.AsyncRebatched which can handle dictionaries but not BatchEncoding.
         if isinstance(batch, BatchEncoding):
             batch = dict(batch)
         return batch
 
     def torch_mask_tokens(self, inputs: Any, special_tokens_mask: Optional[Any] = None) -> Tuple[Any, Any]:
         """
-        Prepare masked tokens inputs/labels for masked language modeling: 80% MASK, 10% random, 10% original.
+        Prepare masked token inputs/labels for masked language modeling: 80% MASK, 10% random, 10% original.
         """
         import torch
 
         labels = inputs.clone()
         # We sample a few tokens in each sequence for MLM training (with probability `self.mlm_probability`)
         probability_matrix = torch.full(labels.shape, self.mlm_probability)
         if special_tokens_mask is None:
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py` & `optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from optimum.utils import logging
 
-from ....ipu_configuration import ALLOWED_POD_TYPES
+from ....training_args import ALLOWED_N_IPU
 
 
 logger = logging.get_logger(__name__)
 
 
 INFERENCE_ENGINES_TO_MODEL_NAMES = {
     "stable-diffusion-v1": "CompVis/stable-diffusion-v1-4",  # this is a guess
@@ -77,37 +77,37 @@
 
 def get_default_ipu_configs(
     engine: str = "stable-diffusion-512-v2-0",
     height: int = 512,
     width: int = 512,
     num_prompts: int = 1,
     num_images_per_prompt: int = 1,
-    pod_type: str = "pod4",
+    n_ipu: int = 4,
     **common_kwargs,
 ):
     if engine not in INFERENCE_ENGINES_TO_MODEL_NAMES:
         raise ValueError(f"{engine} should be one of {', '.join(INFERENCE_ENGINES_TO_MODEL_NAMES)}")
-    if pod_type not in ALLOWED_POD_TYPES:
+    if n_ipu not in ALLOWED_N_IPU:
         raise ValueError(
-            f"{pod_type} is not a correct value for a POD type, supported POD types: {', '.join(ALLOWED_POD_TYPES)}"
+            f"{n_ipu=} is not a valid value for a Pod type, supported Pod types: {', '.join(ALLOWED_N_IPU)}"
         )
 
     default_image_dim = 768 if "768" in engine else 512
     if default_image_dim == 768 and height < default_image_dim and width < default_image_dim:
         logger.warn(
-            "Generating an image of a size smaller than 768x768 with a checkpoint finetuned for 768x768 "
+            "Generating an image smaller than 768x768 with a checkpoint fine-tuned for 768x768 "
             "can lead to images of poor quality."
         )
 
     model_ipu_configs = INFERENCE_ENGINES_TO_IPU_CONFIGS[engine]
 
     unet_ipu_config = model_ipu_configs["unet"]
-    text_encoder_ipu_config = model_ipu_configs["text_encoder"] if pod_type != "pod4" else None
-    vae_ipu_config = model_ipu_configs["vae"] if pod_type != "pod4" else None
-    safety_checker_ipu_config = model_ipu_configs["safety_checker"] if pod_type != "pod4" else None
+    text_encoder_ipu_config = model_ipu_configs["text_encoder"] if n_ipu > 4 else None
+    vae_ipu_config = model_ipu_configs["vae"] if n_ipu > 4 else None
+    safety_checker_ipu_config = model_ipu_configs["safety_checker"] if n_ipu > 4 else None
 
     # Set the micro batch size at 1 for now.
     common_kwargs["inference_device_iterations"] = num_prompts * num_images_per_prompt
 
     unet_ipu_config = {**unet_ipu_config, **common_kwargs}
     if text_encoder_ipu_config:
         text_encoder_ipu_config = {**text_encoder_ipu_config, **common_kwargs}
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py` & `optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 
 
 logger = logging.get_logger(__name__)
 
 
 class IPUSlicedAttnProcessor:
     """
-    SlicedAttnProcessor but we slice across the query sequence length instead of across heads.
-    NB: this ignores the `slice_size` factor since we interpret it differently and use a value that is
+    `SlicedAttnProcessor` but sliced across the query sequence length instead of across heads.
+
+    Note: This ignores the `slice_size` factor since we interpret it differently and use a value that is
     derived from the sequence length based on an empirical attention matrix memory target.
     """
 
     def __init__(self, attn_matrix_target_mem_mb: int):
         if attn_matrix_target_mem_mb < 1:
             raise ValueError(f"`attn_matrix_target_mem_mb` {attn_matrix_target_mem_mb} must be a positive integer.")
 
@@ -168,17 +169,20 @@
             self.up_blocks[1].attentions[2], "up_blocks[1].attentions[2]", ipu_id=3
         )
 
         return self
 
 
 class UNetCastingWrapper(torch.nn.Module):
-    """Schedulers differ in the dtype they store the timesteps in, so changing a
-    scheduler would trigger a recompilation as the input dtype would change. This wrapper
-    simply ensures that the timestep dtype provided to the PoplarExecutor is consistent."""
+    """
+    Ensures that the timestep dtype provided to `PoplarExecutor` is consistent.
+
+    Schedulers differ in the dtype they store the timesteps in, so changing a
+    scheduler would trigger a recompilation as the input dtype would change. This wrapper ensures that the data types are consistent.
+    """
 
     def __init__(self, unet, input_dtype=torch.float16, output_dtype=torch.float32):
         super().__init__()
         self.unet = unet
         self.input_dtype = input_dtype
         self.output_dtype = output_dtype
 
@@ -409,15 +413,15 @@
         )
 
     def set_attention_slice(self, slice_size: Optional[int]):
         # Another side effect of letting this go through is that CrossAttention could set
         # a different processor than what we intended, so do the simple thing for now.
         logger.warn(
             "Attention slicing is enabled by default. Specifying a custom value "
-            "for the `slice_size` is currently unsupported."
+            "for `slice_size` is currently unsupported."
         )
 
     def detach_from_device(self):
         for module in [self.text_encoder, self.unet.unet, self.vae, self.safety_checker]:
             if not isinstance(module, poptorch.PoplarExecutor):
                 continue
             if module.isAttachedToDevice():
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py` & `optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/generation_utils.py` & `optimum-graphcore-0.6.1/optimum/graphcore/generation/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import contextlib
+import copy
 import json
 import os
 import warnings
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Union
 
 import torch
 from torch import nn
 
 import poptorch
 from optimum.utils import logging
 from transformers.generation.stopping_criteria import validate_stopping_criteria
@@ -38,20 +39,36 @@
     GreedySearchOutput,
     LogitsProcessorList,
     SampleDecoderOnlyOutput,
     SampleEncoderDecoderOutput,
     SampleOutput,
     StoppingCriteriaList,
 )
-from transformers.modeling_outputs import ModelOutput
+from transformers.modeling_outputs import BaseModelOutput, ModelOutput
 from transformers.pytorch_utils import torch_int_div
+from transformers.utils.versions import require_version
+
+from .logits_process import IPULogitsProcessors
+from .on_device_generation import (
+    OnDeviceBeamSearch,
+    OnDeviceGenerationModel,
+    OnDeviceGenerationModelOutput,
+    OnDeviceGreedySearch,
+)
 
 
 logger = logging.get_logger(__name__)
 
+MODELS_SUPPORTING_KV_CACHE = set()
+
+
+def supports_kv_cache(pipelined_cls):
+    MODELS_SUPPORTING_KV_CACHE.add(pipelined_cls)
+    return pipelined_cls
+
 
 @contextlib.contextmanager
 def graph_profile_dir_append(append: str):
     if poplar_engine_options_original := os.getenv("POPLAR_ENGINE_OPTIONS"):
         poplar_engine_options_modified = json.loads(poplar_engine_options_original)
         if autoreport_directory := poplar_engine_options_modified.get("autoReport.directory"):
             poplar_engine_options_modified["autoReport.directory"] = autoreport_directory + append
@@ -63,75 +80,177 @@
             os.environ["POPLAR_ENGINE_OPTIONS"] = poplar_engine_options_original
 
 
 class _IndexedInputLinear(nn.Module):
     """
     Wrapper layer for `Linear` that performs a `dynamic_slice` on the input
     before executing the linear. The intended use is as an optimized replacement of the
-    LM Head in the Decoder for text generation inference.
-    The slice is performed on the position `self.index` of the input tensor, where
-    `self.index` is a PyTorch buffer.
+    LM Head in the Decoder for text generation inference when KV caching is disabled.
+    The slice is performed on the position `self._generation_step` of the input tensor, where
+    `self._generation_step` is a PyTorch buffer.
     """
 
     def __init__(self, linear_layer):
         super().__init__()
         self.wrapped_linear = linear_layer
-        self.register_buffer("index", torch.tensor([0], dtype=torch.int32))
+        self.register_buffer("_generation_step", torch.tensor([0], dtype=torch.int32), persistent=False)
 
     def forward(self, x):
-        x = poptorch.dynamic_slice(x, 1, self.index, 1, 1)
+        x = poptorch.dynamic_slice(x, 1, self._generation_step, 1, 1)
         return self.wrapped_linear(x)
 
 
 class DecoderWrapper(nn.Module):
     """
     Fast wrapper for decoder part of text generation models.
+
+    Updates the appropriate buffers for the modules which need to know the current generation step.
     Only returns the logits from the last generated token to reduce IO costs.
     """
 
     def __init__(self, pipelined_model):
         super().__init__()
         self.pipelined_model = pipelined_model
-        # Replace the LM-head with the faster _IndexedInputLinear layer
-        self.pipelined_model.set_output_embeddings(_IndexedInputLinear(self.pipelined_model.get_output_embeddings()))
 
-    def forward(self, t, **model_inputs):
+        # With KV caching, some modules may need to know the current decoding step and beam indices.
+        # Getting this information to them can either be done by copying it into buffers, or
+        # by subclassing the entire decoder model just to change the forward signatures and passing these
+        # as arguments. For now, go with the former, but it's not set in stone.
+        self._modules_with_attributes_in_buffers = {
+            attr: [module for module in self.pipelined_model.modules() if hasattr(module, attr)]
+            for attr in ["_beam_idx", "_generation_step"]
+        }
+
+    def register_encoder_output_buffers(self, output_buffers: Dict[str, torch.Tensor]):
+        for name in sorted(output_buffers):
+            self.register_buffer(name, output_buffers[name], persistent=False)
+
+    def _get_buffered_outputs(self) -> Dict:
+        kwargs = {}
+        if hasattr(self, "encoder_last_hidden_state"):
+            kwargs["encoder_outputs"] = BaseModelOutput(last_hidden_state=self.encoder_last_hidden_state)
+        if hasattr(self, "encoder_attention_mask"):
+            kwargs["attention_mask"] = self.encoder_attention_mask
+        return kwargs
+
+    def forward(self, t, beam_idx=None, **model_inputs):
         """
         Args:
             t : (`torch.Tensor(int)`) Tensor with single int representing the current length of the sequence being generated
+            beam_idx: (`torch.LongTensor` of shape `(batch_size * num_beams,)`):
+                Beam indices indicating to which beam the tokens were added, required for reordering the on-device KV cache.
             model_inputs : Regular model_inputs passed to the wrapped model.
         Returns:
             The output logits at position `t` only
         """
-        # Update the index buffer in the _IndexedInputLinear layer
-        self.pipelined_model.get_output_embeddings().index.copy_(t)
+        for module in self._modules_with_attributes_in_buffers["_generation_step"]:
+            module._generation_step.copy_(t)
+
+        # When generation is done on host, the beam_idx has to be provided as an input.
+        # When generation is done on device, the beam_idx is stored in a separate buffer.
+        if beam_idx is None:
+            if hasattr(self.pipelined_model, "generation_strategy") and hasattr(
+                self.pipelined_model.generation_strategy, "_cached_beam_idx"
+            ):
+                beam_idx = self.pipelined_model.generation_strategy._cached_beam_idx.int()
+        for module in self._modules_with_attributes_in_buffers["_beam_idx"]:
+            if beam_idx is None:
+                raise ValueError(
+                    "A module registered a `beam_idx` buffer, but the pipelined model is not called with such, "
+                    "or the on device beam search did not register `_cached_beam_idx`. For the first case, "
+                    "`beam_idx` can be provided to the model via `prepare_inputs_for_generation`."
+                )
+            module._beam_idx.copy_(beam_idx)
 
         # Run the decoder
-        outputs = self.pipelined_model(**model_inputs)
-        return type(outputs)(
-            loss=None,
-            logits=outputs.logits,
-        )
+        kwargs = self._get_buffered_outputs()
+        outputs = self.pipelined_model(**model_inputs, **kwargs)
+        if isinstance(outputs, ModelOutput) and not isinstance(outputs, OnDeviceGenerationModelOutput):
+            outputs = type(outputs)(
+                logits=outputs.logits,
+            )
+        return outputs
 
 
 class IPUGenerationMixin(GenerationMixin):
+
+    """
+    Enable optimization for encoder-decoder text generation where the encoder outputs
+    are cached on the Decoder device using buffers.
+    """
+
+    use_encoder_output_buffer = False
+
+    @property
+    def encoder_output_buffer_enabled(self) -> bool:
+        return self.config.is_encoder_decoder and self.use_encoder_output_buffer
+
     def _pad_tensors_to_max_len(self, tensor: torch.Tensor, max_length: int, pad_token_id: int) -> torch.Tensor:
         return nn.functional.pad(tensor, (0, max_length - tensor.shape[1]), "constant", pad_token_id)
 
-    def _call_generate(self, *args, cur_token_id: int, **kwargs):
-        t = self._get_cur_token_logits_tensor(cur_token_id)
+    def _ensure_generation_step_progression(self, generation_step):
+        if not hasattr(self, "_previous_generation_step"):
+            self._previous_generation_step = generation_step
+            return
+        if generation_step <= self._previous_generation_step and generation_step != 0:
+            raise ValueError("`generation_step` must increase, or begin from 0.")
+        self._previous_generation_step = generation_step
+
+    def _call_generate(
+        self,
+        *args,
+        generation_step: int,
+        on_device_generation_model_ctr: Optional[Callable[[torch.nn.Module], torch.nn.Module]] = None,
+        **kwargs,
+    ):
+        self._ensure_generation_step_progression(generation_step)
+        t = self._get_generation_step_tensor(generation_step, ascending=on_device_generation_model_ctr is not None)
         if not hasattr(self, "poptorch_decoder"):
-            wrapper = DecoderWrapper(self.eval())
-            decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
-            self.poptorch_decoder = poptorch.inferenceModel(wrapper, decoder_ipu_config.to_options(for_inference=True))
+            generation_model = self
+            if on_device_generation_model_ctr is not None:
+                generation_model = on_device_generation_model_ctr(self)
+            decoder_wrapper = DecoderWrapper(generation_model.eval())
+
+            if os.getenv("DEBUG_RUN_DECODER_ON_CPU", False):
+                self.poptorch_decoder = decoder_wrapper
+            else:
+                decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
+                decoder_options = decoder_ipu_config.to_options(for_inference=True)
+
+                if self.encoder_output_buffer_enabled:
+                    require_version(
+                        "poptorch>=3.3", "Updatable encoder output buffer optimization only available in poptorch>=3.3"
+                    )
+                    named_buffers = {"encoder_last_hidden_state": kwargs["encoder_outputs"]["last_hidden_state"]}
+                    if kwargs.get("attention_mask") is not None:
+                        named_buffers["encoder_attention_mask"] = kwargs["attention_mask"].half()
+                    decoder_wrapper.register_encoder_output_buffers(named_buffers)
+                    decoder_options.updatableNamedBuffers(list(named_buffers.keys()))
+
+                self.poptorch_decoder = poptorch.inferenceModel(decoder_wrapper, decoder_options)
+
+        if self.encoder_output_buffer_enabled:
+            kwargs.pop("encoder_outputs", None)
+            kwargs.pop("attention_mask", None)
 
         # This will trigger a compile first time it's ran
-        with graph_profile_dir_append("/decoder"):
+        with graph_profile_dir_append("/decoder" if self.config.is_encoder_decoder else ""):
             return self.poptorch_decoder(*args, t=t, **kwargs)
 
+    def _update_model_buffers_if_needed(self, model_kwargs):
+        """
+        If decoder model then we cache the encoder values inside pytorch buffers to reduce the IO cost
+        """
+        if not (self.encoder_output_buffer_enabled and hasattr(self, "poptorch_decoder")):
+            return
+        self.poptorch_decoder.encoder_last_hidden_state.copy_(model_kwargs["encoder_outputs"]["last_hidden_state"])
+        if model_kwargs.get("attention_mask") is not None:
+            self.poptorch_decoder.encoder_attention_mask.copy_(model_kwargs["attention_mask"].half())
+        self.poptorch_decoder.copyNamedBuffersToDevice()
+
     def _prepare_encoder_decoder_kwargs_for_generation(
         self, inputs_tensor: torch.Tensor, model_kwargs, model_input_name: Optional[str] = None
     ) -> Dict[str, Any]:
         # 1. get encoder
         encoder = self.get_encoder()
 
         # 2. prepare encoder args and encoder kwargs from model kwargs
@@ -145,37 +264,72 @@
         # 3. make sure that encoder returns `ModelOutput`
         model_input_name = model_input_name if model_input_name is not None else self.main_input_name
         encoder_kwargs["return_dict"] = True
         encoder_kwargs[model_input_name] = inputs_tensor
 
         if not hasattr(self, "poptorch_encoder"):
             # Use split encoder ipu_config for encoder/decoder models
-            self.poptorch_encoder = poptorch.inferenceModel(
-                encoder.eval(), self.encoder_ipu_config.to_options(for_inference=True)
-            )
+            if os.getenv("DEBUG_RUN_ENCODER_ON_CPU", False):
+                self.poptorch_encoder = encoder.eval()
+            else:
+                self.poptorch_encoder = poptorch.inferenceModel(
+                    encoder.eval(), self.encoder_ipu_config.to_options(for_inference=True)
+                )
         with graph_profile_dir_append("/encoder"):
             model_kwargs["encoder_outputs"]: ModelOutput = self.poptorch_encoder(**encoder_kwargs)
 
         return model_kwargs
 
     def detachFromDevice(self):
         if hasattr(self, "poptorch_encoder"):
             self.poptorch_encoder.detachFromDevice()
         if hasattr(self, "poptorch_decoder"):
             self.poptorch_decoder.detachFromDevice()
 
-    def _get_cur_token_logits_tensor(self, token_id):
-        # returns a 1 dimensional tensor of the form [device_iterations * replication factor]
-        # with all elements equal to token_id.
-        # token_id is the current token being decoded, it
-        # is required in order to return only the logits for this token
-        return (
-            torch.ones(self.ipu_config.inference_device_iterations * self.ipu_config.inference_replication_factor)
-            * token_id
+    def _get_generation_step_tensor(self, generation_step, ascending=False):
+        # Returns a 1 dimensional tensor of the form [device_iterations * replication factor]
+        # with all elements equal to generation_step.
+        # This ensures the dimensions are as expected by any parallelism options.
+        decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
+        per_replica = (
+            torch.arange(decoder_ipu_config.inference_device_iterations) + generation_step
+            if ascending
+            else torch.ones(decoder_ipu_config.inference_device_iterations) * generation_step
         )
+        return per_replica.repeat(decoder_ipu_config.inference_replication_factor)
+
+    def _maybe_ensure_kv_cache_supported(self, use_cache):
+        if not use_cache or hasattr(self, "_poptorch_decoder"):
+            return
+
+        if use_cache and self.__class__ not in MODELS_SUPPORTING_KV_CACHE:
+            raise ValueError(
+                f"{self.__class__} does not support KV caching. Pipelined models can be "
+                "decorated using `supports_kv_cache` once they support static KV caching."
+            )
+
+        model_has_kv_cache_initialized = any(getattr(m, "kv_cache_initialized", False) for m in self.modules())
+        if use_cache and not model_has_kv_cache_initialized:
+            raise ValueError(
+                f"{self.__class__.__name__} supports KV caching and `use_cache=True`, but no KV caches have been initialized. "
+                f"Please pass `use_cache=True` to the `parallelize` method of {self.__class__.__name__}."
+            )
+
+    def change_lm_head_to_indexed_input_linear(self, restore: bool):
+        """Changes the LM head with the faster _IndexedInputLinear layer.
+
+        Args:
+            restore: whether to restore the LM head to the original version or not.
+        """
+        if restore:
+            lm_head = self.get_output_embeddings()
+            if lm_head.__class__ == _IndexedInputLinear:
+                self.set_output_embeddings(lm_head.wrapped_linear)
+        else:
+            self.set_output_embeddings(_IndexedInputLinear(self.get_output_embeddings()))
 
     # Modified from https://github.com/huggingface/transformers/blob/v4.20.1/src/transformers/generation_utils.py#L1532
     def greedy_search(
         self,
         input_ids: torch.LongTensor,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
@@ -299,49 +453,65 @@
         # if model is an encoder-decoder, retrieve encoder attention weights and hidden states
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
-        # Change: disable use_cache because it can't be statically compiled
-        if model_kwargs.get("use_cache"):
-            raise ValueError("use_cache=True is currently not supported")
+        use_cache = model_kwargs.get("use_cache", False)
+        self._maybe_ensure_kv_cache_supported(use_cache)
+
+        self._update_model_buffers_if_needed(model_kwargs)
+
+        # Change: intercept to optionally run the entire generation loop on device
+        if self.on_device_generation_steps > 0:
+            return self._on_device_greedy_search(
+                input_ids,
+                logits_processor=logits_processor,
+                stopping_criteria=stopping_criteria,
+                pad_token_id=pad_token_id,
+                eos_token_id=eos_token_id,
+                max_length=max_length,
+                return_dict_in_generate=return_dict_in_generate,
+                **model_kwargs,
+            )
 
         # keep track of which sequences are already finished
         unfinished_sequences = input_ids.new(input_ids.shape[0]).fill_(1)
         cur_len = input_ids.shape[-1]
 
         while True:
             # Change: remove synced_gpu code
             # Change: add input max_length padding
-            input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
+            if not use_cache:
+                input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
 
-            # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
-                    model_kwargs["attention_mask"], stopping_criteria.max_length, 0
-                )
+                # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
+                        model_kwargs["attention_mask"], stopping_criteria.max_length, 0
+                    )
 
             # prepare model inputs
             model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
             # forward pass to get next token
             outputs = self._call_generate(
-                cur_token_id=cur_len - 1,
+                generation_step=cur_len - 1,
                 **model_inputs,
                 return_dict=True,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
             )
 
             # Change: Remove padding and restore to actual length
-            input_ids = input_ids[:, :cur_len]
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
+            if not use_cache:
+                input_ids = input_ids[:, :cur_len]
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
 
             # Change: remove synced_gpu code
 
             next_token_logits = outputs.logits[:, -1, :]
 
             # pre-process distribution
             next_tokens_scores = logits_processor(input_ids, next_token_logits)
@@ -529,14 +699,16 @@
         if max_length is not None:
             warnings.warn(
                 "`max_length` is deprecated in this function, use"
                 " `stopping_criteria=StoppingCriteriaList(MaxLengthCriteria(max_length=max_length))` instead.",
                 UserWarning,
             )
             stopping_criteria = validate_stopping_criteria(stopping_criteria, max_length)
+        else:
+            max_length = stopping_criteria.max_length
         if len(stopping_criteria) == 0:
             warnings.warn("You don't have defined any stopping_criteria, this will likely loop forever", UserWarning)
         pad_token_id = pad_token_id if pad_token_id is not None else self.config.pad_token_id
         eos_token_id = eos_token_id if eos_token_id is not None else self.config.eos_token_id
         output_scores = output_scores if output_scores is not None else self.config.output_scores
         output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
         output_hidden_states = (
@@ -568,46 +740,63 @@
         # if model is an encoder-decoder, retrieve encoder attention weights and hidden states
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
-        # Change: disable use_cache because it can't be statically compiled
-        if model_kwargs.get("use_cache"):
-            raise ValueError("use_cache=True is currently not supported")
+        use_cache = model_kwargs.get("use_cache", False)
+        self._maybe_ensure_kv_cache_supported(use_cache)
+
+        self._update_model_buffers_if_needed(model_kwargs)
+
+        # Change: intercept to optionally run the entire generation loop on device
+        if self.on_device_generation_steps > 0:
+            return self._on_device_beam_search(
+                input_ids,
+                beam_scorer=beam_scorer,
+                logits_processor=logits_processor,
+                stopping_criteria=stopping_criteria,
+                pad_token_id=pad_token_id,
+                eos_token_id=eos_token_id,
+                max_length=max_length,
+                return_dict_in_generate=return_dict_in_generate,
+                **model_kwargs,
+            )
 
         beam_scores = torch.zeros((batch_size, num_beams), dtype=torch.float, device=input_ids.device)
         beam_scores[:, 1:] = -1e9
         beam_scores = beam_scores.view((batch_size * num_beams,))
 
         while True:
             # Change: remove synced_gpu code
             # Change: add input max_length padding
-            input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
+            if not use_cache:
+                input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
 
-            # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
-                    model_kwargs["attention_mask"], stopping_criteria.max_length, 0
-                )
+                # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
+                        model_kwargs["attention_mask"], stopping_criteria.max_length, 0
+                    )
 
             model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
             outputs = self._call_generate(
-                cur_token_id=cur_len - 1,
+                generation_step=cur_len - 1,
                 **model_inputs,
                 return_dict=True,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
             )
             # Change: Remove padding and restore to actual length
-            input_ids = input_ids[:, :cur_len]
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
+            if not use_cache:
+                input_ids = input_ids[:, :cur_len]
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
 
             # Change: remove synced_gpu code
 
             # Change: cast to float on cpu
             next_token_logits = outputs.logits[:, -1, :].float()
             # hack: adjust tokens for Marian. For Marian we have to make sure that the `pad_token_id`
             # cannot be generated both before and after the `nn.functional.log_softmax` operation.
@@ -666,14 +855,16 @@
             input_ids = torch.cat([input_ids[beam_idx, :], beam_next_tokens.unsqueeze(-1)], dim=-1)
 
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
             if model_kwargs["past"] is not None:
                 model_kwargs["past"] = self._reorder_cache(model_kwargs["past"], beam_idx)
+            # Change: add beam_idx to model_kwargs so KV caching can be made aware of it on device
+            model_kwargs["beam_idx"] = beam_idx
 
             if return_dict_in_generate and output_scores:
                 beam_indices = tuple((beam_indices[beam_idx[i]] + (beam_idx[i],) for i in range(len(beam_indices))))
 
             # increase cur_len
             cur_len = cur_len + 1
 
@@ -863,50 +1054,57 @@
         # if model is an encoder-decoder, retrieve encoder attention weights and hidden states
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
-        # Change: disable use_cache because it can't be statically compiled
-        if model_kwargs.get("use_cache"):
-            raise ValueError("use_cache=True is currently not supported")
+        use_cache = model_kwargs.get("use_cache", False)
+        self._maybe_ensure_kv_cache_supported(use_cache)
+
+        self._update_model_buffers_if_needed(model_kwargs)
+
+        # Change: intercept to optionally run the entire generation loop on device
+        if self.on_device_generation_steps > 0:
+            return self._on_device_sample()
 
         # keep track of which sequences are already finished
         unfinished_sequences = input_ids.new(input_ids.shape[0]).fill_(1)
         cur_len = input_ids.shape[-1]
 
         # auto-regressive generation
         while True:
             # Change: remove synced_gpu code
             # Change: add input max_length padding
-            input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
+            if not use_cache:
+                input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
 
-            # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
-                    model_kwargs["attention_mask"], stopping_criteria.max_length, 0
-                )
+                # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
+                        model_kwargs["attention_mask"], stopping_criteria.max_length, 0
+                    )
 
             # prepare model inputs
             model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
             # forward pass to get next token
             outputs = self._call_generate(
-                cur_token_id=cur_len - 1,
+                generation_step=cur_len - 1,
                 **model_inputs,
                 return_dict=True,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
             )
 
             # Change: Remove padding and restore to actual length
-            input_ids = input_ids[:, :cur_len]
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
+            if not use_cache:
+                input_ids = input_ids[:, :cur_len]
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
 
             # Change: remove synced_gpu code
 
             # Change: cast to float on cpu
             next_token_logits = outputs.logits[:, -1, :].float()
 
             # pre-process distribution
@@ -1140,45 +1338,52 @@
         # if model is an encoder-decoder, retrieve encoder attention weights and hidden states
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
-        # Change: disable use_cache because it can't be statically compiled
-        if model_kwargs.get("use_cache"):
-            raise ValueError("use_cache=True is currently not supported")
+        use_cache = model_kwargs.get("use_cache", False)
+        self._maybe_ensure_kv_cache_supported(use_cache)
+
+        self._update_model_buffers_if_needed(model_kwargs)
+
+        # Change: intercept to optionally run the entire generation loop on device
+        if self.on_device_generation_steps > 0:
+            return self._on_device_beam_sample()
 
         beam_scores = torch.zeros((batch_size, num_beams), dtype=torch.float, device=input_ids.device)
         beam_scores = beam_scores.view((batch_size * num_beams,))
 
         while True:
             # Change: remove synced_gpu code
             # Change: add input max_length padding
-            input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
+            if not use_cache:
+                input_ids = self._pad_tensors_to_max_len(input_ids, stopping_criteria.max_length, pad_token_id)
 
-            # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
-                    model_kwargs["attention_mask"], stopping_criteria.max_length, 0
-                )
+                # Change: For a seq2seq model such as BART, the "attention_mask" is the encoder/cross attention mask and it does not require padding.
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = self._pad_tensors_to_max_len(
+                        model_kwargs["attention_mask"], stopping_criteria.max_length, 0
+                    )
 
             model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
             outputs = self._call_generate(
-                cur_token_id=cur_len - 1,
+                generation_step=cur_len - 1,
                 **model_inputs,
                 return_dict=True,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
             )
             # Change: Remove padding and restore to actual length
-            input_ids = input_ids[:, :cur_len]
-            if not self.config.is_encoder_decoder:
-                model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
+            if not use_cache:
+                input_ids = input_ids[:, :cur_len]
+                if not self.config.is_encoder_decoder:
+                    model_kwargs["attention_mask"] = model_kwargs["attention_mask"][:, :cur_len]
 
             # Change: remove synced_gpu code
 
             # Change: cast to float on cpu
             next_token_logits = outputs.logits[:, -1, :].float()
 
             # hack: adjust tokens for Marian. For Marian we have to make sure that the `pad_token_id`
@@ -1242,14 +1447,16 @@
             input_ids = torch.cat([input_ids[beam_idx, :], beam_next_tokens.unsqueeze(-1)], dim=-1)
 
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
             if model_kwargs["past"] is not None:
                 model_kwargs["past"] = self._reorder_cache(model_kwargs["past"], beam_idx)
+            # Change: add beam_idx to model_kwargs so KV caching can be made aware of it on device
+            model_kwargs["beam_idx"] = beam_idx
 
             if return_dict_in_generate and output_scores:
                 beam_indices = tuple((beam_indices[beam_idx[i]] + (beam_idx[i],) for i in range(len(beam_indices))))
 
             # increase cur_len
             cur_len = cur_len + 1
 
@@ -1290,7 +1497,279 @@
                     scores=scores,
                     beam_indices=sequence_outputs["beam_indices"],
                     attentions=decoder_attentions,
                     hidden_states=decoder_hidden_states,
                 )
         else:
             return sequence_outputs["sequences"]
+
+    on_device_generation_steps: int = 0
+
+    def set_on_device_generation_steps(self, value: Optional[int] = 0):
+        self.on_device_generation_steps = value
+        if value == 0:
+            del self.on_device_generation_steps
+
+    def _adapt_logits_processor_for_on_device_generation(self, logits_processor: LogitsProcessorList, vocab_size: int):
+        adapted_processors = []
+        for processor in logits_processor:
+            ipu_processor_cls = IPULogitsProcessors.get(processor.__class__, None)
+            if ipu_processor_cls is None:
+                raise NotImplementedError(f"{processor.__class__.__name__} is not supported yet to run on IPU.")
+
+            try:
+                ipu_processor = ipu_processor_cls.from_model(processor, vocab_size)
+            except AttributeError:
+                ipu_processor = copy.deepcopy(processor)
+                ipu_processor.__class__ = ipu_processor_cls
+            adapted_processors.append(ipu_processor)
+        return LogitsProcessorList(adapted_processors)
+
+    def _adapt_stopping_criteria_for_on_device_generation(
+        self, stopping_criteria: StoppingCriteriaList, on_device_generation_steps: int
+    ):
+        adapted_stopping_criteria = []
+        for stopping_criterion in stopping_criteria:
+            if hasattr(stopping_criterion, "max_length"):
+                max_length = stopping_criterion.max_length
+                new_max_length = max_length - on_device_generation_steps
+                logger.info(
+                    f"Temporarily adapting `max_length` from {max_length} to {new_max_length} for on device generation."
+                )
+                stopping_criterion = copy.deepcopy(stopping_criterion)
+                stopping_criterion.max_length = new_max_length
+            adapted_stopping_criteria.append(stopping_criterion)
+        return StoppingCriteriaList(adapted_stopping_criteria)
+
+    def _prepare_inputs_for_on_device_generation(self, model_inputs, on_device_generation_steps, batch_size):
+        """
+        A model-agnostic version of `prepare_inputs_for_generation` whose main purpose is to duplicate
+        decoder inputs by `on_device_generation_steps=inference_device_iterations` and perform additional input validation.
+        Since we are duplicating tensors, we restrict duplication to `torch.Tensor` and the exceptional case of
+        `encoder_outputs.last_hidden_state`.
+        """
+        adapted_model_inputs = {}
+        for k, v in model_inputs.items():
+            if k in ("attention_mask", "encoder_outputs") and self.encoder_output_buffer_enabled:
+                # These inputs will copied onto device via buffers, so we don't need to duplicate them.
+                adapted_model_inputs[k] = v
+                continue
+            if k == "beam_idx":
+                # With on-device generation, beam_idx at each step is handled through buffers.
+                continue
+
+            if torch.is_tensor(v):
+                if v.shape[0] != batch_size:
+                    raise ValueError(f"Unexpected size in dim 0 for {k}, expected {batch_size}.")
+                v = v.repeat(on_device_generation_steps, *(1 for _ in range(v.ndim - 1)))
+            elif k == "encoder_outputs":
+                v_type = type(v)
+                if not isinstance(v, BaseModelOutput):
+                    raise ValueError(
+                        "Expected `encoder_outputs` to be an instance of `BaseModelOutput`, " f"received {v_type}."
+                    )
+                v = v.last_hidden_state
+                v = v.repeat(on_device_generation_steps, *(1 for _ in range(v.ndim - 1)))
+                v = v_type(last_hidden_state=v)
+            elif v is None:
+                pass
+            elif isinstance(v, (int, float, str, bool)):
+                pass
+            else:
+                raise TypeError(
+                    f"Unexpected type {type(v)} received for decoder input {k}. On device generation enforces "
+                    "stricter input validation to minimise unexpected errors. Improvements are always welcome."
+                )
+            adapted_model_inputs[k] = v
+        return adapted_model_inputs
+
+    def _on_device_greedy_search(
+        self,
+        input_ids: torch.Tensor,
+        logits_processor: LogitsProcessorList,
+        stopping_criteria: StoppingCriteriaList,
+        pad_token_id: int,
+        eos_token_id: int,
+        max_length: int,
+        return_dict_in_generate: Optional[bool] = False,
+        **model_kwargs,
+    ):
+        if not model_kwargs.get("use_cache", False):
+            raise NotImplementedError("On device greedy search assumes `use_cache=True`.")
+
+        if return_dict_in_generate:
+            raise NotImplementedError("On device greedy search assumes `return_dict_in_generate=False`.")
+
+        batch_size, context_length = input_ids.shape
+        vocab_size = self.get_output_embeddings().out_features
+
+        if context_length > 1:
+            raise ValueError("Context length (input_ids.shape[-1]) > 1 is not supported yet.")
+
+        if (max_length - context_length) % self.on_device_generation_steps != 0:
+            logger.info(
+                "`max_length - context_length` does not evenly divide `on_device_generation_steps` "
+                f"({max_length - context_length} vs {self.on_device_generation_steps}). Generation will be done "
+                f"{self.on_device_generation_steps} tokens at a time and stop short of `max_length` so as not to exceed it."
+            )
+
+        if self.ipu_config.inference_device_iterations != 1:
+            raise ValueError(
+                "On device generation expects `inference_device_iterations=1`, "
+                f"received {self.ipu_config.inference_device_iterations}. "
+                "For on device generation, `inference_device_iterations` will be set to "
+                f"`on_device_generation_steps={self.on_device_generation_steps}`."
+            )
+        if hasattr(self, "decoder_ipu_config"):
+            self.decoder_ipu_config.inference_device_iterations = self.on_device_generation_steps
+        else:
+            self.ipu_config.inference_device_iterations = self.on_device_generation_steps
+
+        logits_processor = self._adapt_logits_processor_for_on_device_generation(logits_processor, vocab_size)
+        stopping_criteria = self._adapt_stopping_criteria_for_on_device_generation(
+            stopping_criteria, self.on_device_generation_steps
+        )
+
+        # This function only has to be called at the beginning of generation since
+        # all necessary state should be stored in buffers on device.
+        model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
+
+        # A model-agnostic version of above mainly to duplicate inputs for device iterations.
+        model_inputs = self._prepare_inputs_for_on_device_generation(
+            model_inputs, self.on_device_generation_steps, batch_size
+        )
+
+        on_device_generation_model_ctr = lambda inst: OnDeviceGenerationModel(
+            inst,
+            batch_size=batch_size,
+            max_length=max_length,
+            pad_token_id=pad_token_id,
+            eos_token_id=eos_token_id,
+            logits_processor=logits_processor,
+            num_beams=1,
+            use_cache=True,
+        )
+
+        generation_step = 0
+        while True:
+            output = self._call_generate(
+                generation_step=generation_step,  # NB: equal to `cur_len - 1` since context_length=1
+                on_device_generation_model_ctr=on_device_generation_model_ctr,
+                **model_inputs,
+                return_dict=True,
+                output_attentions=False,
+                output_hidden_states=False,
+            )
+            next_tokens = output.generated_tokens.view(self.on_device_generation_steps, batch_size).T
+
+            # update generated ids, model inputs, and length for next step
+            input_ids = torch.cat([input_ids, next_tokens], dim=-1)
+
+            generation_step += self.on_device_generation_steps
+
+            # stop when each sentence is finished, or if we exceed the maximum length
+            if torch.any(output.done) or stopping_criteria(input_ids, ()):
+                break
+
+        return input_ids
+
+    def _on_device_beam_search(
+        self,
+        input_ids: torch.Tensor,
+        beam_scorer: BeamScorer,
+        logits_processor: LogitsProcessorList,
+        stopping_criteria: StoppingCriteriaList,
+        pad_token_id: int,
+        eos_token_id: int,
+        max_length: int,
+        return_dict_in_generate: Optional[bool] = False,
+        **model_kwargs,
+    ):
+        if not model_kwargs.get("use_cache", False):
+            raise NotImplementedError("On device beam search assumes `use_cache=True`.")
+
+        if return_dict_in_generate:
+            raise NotImplementedError("On device beam search assumes `return_dict_in_generate=False`.")
+
+        batch_size = len(beam_scorer._beam_hyps)
+        num_beams = beam_scorer.num_beams
+        batch_beam_size, context_length = input_ids.shape
+        vocab_size = self.get_output_embeddings().out_features
+
+        if context_length > 1:
+            raise ValueError("Context length (input_ids.shape[-1]) > 1 is not supported yet.")
+
+        if (max_length - context_length) % self.on_device_generation_steps != 0:
+            logger.info(
+                "`max_length - context_length` does not evenly divide `on_device_generation_steps` "
+                f"({max_length - context_length} vs {self.on_device_generation_steps}). Generation will be done "
+                f"{self.on_device_generation_steps} tokens at a time and stop short of `max_length` so as not to exceed it."
+            )
+
+        if self.ipu_config.inference_device_iterations != 1:
+            raise ValueError(
+                "On device generation expects `inference_device_iterations=1`, "
+                f"received {self.ipu_config.inference_device_iterations}. "
+                "For on device generation, `inference_device_iterations` will be set to "
+                f"`on_device_generation_steps={self.on_device_generation_steps}`."
+            )
+        if hasattr(self, "decoder_ipu_config"):
+            self.decoder_ipu_config.inference_device_iterations = self.on_device_generation_steps
+        else:
+            self.ipu_config.inference_device_iterations = self.on_device_generation_steps
+
+        logits_processor = self._adapt_logits_processor_for_on_device_generation(logits_processor, vocab_size)
+        stopping_criteria = self._adapt_stopping_criteria_for_on_device_generation(
+            stopping_criteria, self.on_device_generation_steps
+        )
+
+        # This function only has to be called at the beginning of generation since
+        # all necessary state should be stored in buffers on device.
+        model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
+
+        # A model-agnostic version of above mainly to duplicate inputs for device iterations.
+        model_inputs = self._prepare_inputs_for_on_device_generation(
+            model_inputs, self.on_device_generation_steps, batch_beam_size
+        )
+
+        on_device_generation_model_ctr = lambda inst: OnDeviceGenerationModel(
+            inst,
+            batch_size=batch_size,
+            max_length=max_length,
+            pad_token_id=pad_token_id,
+            eos_token_id=eos_token_id,
+            logits_processor=logits_processor,
+            num_beams=num_beams,
+            use_cache=True,
+            length_penalty=beam_scorer.length_penalty,
+            early_stopping=beam_scorer.do_early_stopping,
+        )
+
+        generation_step = 0
+        while True:
+            output = self._call_generate(
+                generation_step=generation_step,  # NB: equal to `cur_len - 1` since context_length=1
+                on_device_generation_model_ctr=on_device_generation_model_ctr,
+                **model_inputs,
+                return_dict=True,
+                output_attentions=False,
+                output_hidden_states=False,
+            )
+
+            generation_step += self.on_device_generation_steps
+
+            first_done = torch.argmax(output.done.int())
+
+            input_ids = output.generated_tokens[
+                first_done * batch_size : (first_done + 1) * batch_size, : context_length + generation_step
+            ].to(input_ids.dtype)
+
+            if torch.any(output.done) or stopping_criteria(input_ids, ()):
+                break
+
+        return input_ids
+
+    def _on_device_sample(self):
+        raise NotImplementedError("On device sampling is not supported.")
+
+    def _on_device_beam_sample(self):
+        raise NotImplementedError("On device beam sampling is not supported.")
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/modelcard.py` & `optimum-graphcore-0.6.1/optimum/graphcore/modelcard.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/modeling_utils.py` & `optimum-graphcore-0.6.1/optimum/graphcore/modeling_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,39 +7,34 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+from __future__ import annotations
 
 import copy
 from inspect import signature
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 import poptorch
 from optimum.utils import logging
 from transformers import PreTrainedModel
 
-from .ipu_configuration import IPUConfig
+from .ipu_configuration import IncompatibleIPUConfigError, IPUConfig
 
 
 logger = logging.get_logger(__name__)
 
 
-class IncompatibleIPUConfigError(Exception):
-    """An exception used when an IPU Config is incompatible with a model"""
-
-    pass
-
-
 _PRETRAINED_TO_PIPELINED_REGISTRY = {}
 
 
 def register(transformers_cls=None):
     def wrapper(cls):
         orig_cls = transformers_cls
         if orig_cls is None:
@@ -66,55 +61,55 @@
     elif isinstance(model, PipelineMixin):
         clone = copy.deepcopy(model)
         clone.ipu_config = copy.deepcopy(ipu_config)
         return clone
     else:
         if force:
             logger.warning(
-                f"No pipelined version exists for {model_cls.__name__}, creating it dynamically, it might not work as expected."
+                f"No pipelined version exists for {model_cls.__name__}, creating it dynamically so it might not work as expected."
             )
             pipelined_cls = type(f"Pipelined{model_cls.__name__}", (model_cls, PipelineMixin), {})
             return pipelined_cls.from_model(model)
 
         else:
             raise KeyError(f"{model_cls.__name__} pipelined version not found in registry.")
 
 
 class PipelineMixin:
     @classmethod
     def from_transformers(cls, model: PreTrainedModel, ipu_config: IPUConfig):
         """
-        Creates a pipeline model from a [`~transformers.PreTrainedModel`].
+        Creates a pipelined version of model from a [`~transformers.PreTrainedModel`] instance.
 
         Args:
             model ([`~transformers.PreTrainedModel`]):
                 The model to convert to a pipelined model.
             ipu_config ([`IPUConfig`]):
-                The IPUConfig of the pipelined model.
+                The `IPUConfig` instance of the pipelined model.
 
         Returns:
             The pipelined version of the model.
         """
         config = copy.deepcopy(model.config)
         pipelined_model = cls(config)
         pipelined_model.load_state_dict(model.state_dict())
         pipelined_model.ipu_config = copy.deepcopy(ipu_config)
         pipelined_model.training = model.training
         return pipelined_model
 
     @classmethod
     def from_pretrained_transformers(cls, model_name_or_path: str, ipu_config: IPUConfig, *model_args, **kwargs):
         """
-        Creates a pipeline model by using `from_pretrained`.
+        Creates a pipelined version of a model by using the `from_pretrained` function.
 
         Args:
             model_name_or_path (`str`):
                 The model name or path.
             ipu_config ([`IPUConfig`]):
-                The IPUConfig of the pipelined model.
+                The `IPUConfig` of the pipelined model.
             model_args (`Tuple[Any]`):
                 The positional arguments to use when instantiating the model.
             kwargs (`Dict[str, Any]`):
                 The keyword arguments to use when instantiating the model.
 
         Returns:
             The pipelined model.
@@ -130,19 +125,19 @@
         # Just needed so that .parallelize() does not throw an error
         clone.ipu_config = IPUConfig()
         return clone
 
     def _has_ipu_config_check(self):
         _ipu_config = getattr(self, "_ipu_config", None)
         if _ipu_config is None:
-            raise AttributeError("No IPUConfig was found, please set the ipu_config attribute")
+            raise AttributeError("No IPUConfig was found. Please set the ipu_config attribute")
 
     @property
     def ipu_config(self):
-        """Property that checks that the model has an [`IPUConfig`] attached, and returns it."""
+        """Checks that the model has an [`IPUConfig`] attached, and returns it."""
         self._has_ipu_config_check()
         return self._ipu_config
 
     @ipu_config.setter
     def ipu_config(self, value: IPUConfig):
         if not isinstance(value, IPUConfig):
             raise TypeError(f"ipu_config must be an instance of IPUConfig, but {type(value)} was provided")
@@ -153,37 +148,37 @@
         self._hooks = []
         self._has_ipu_config_check()
         return self
 
     def deparallelize(self):
         """
         Undoes the changes to the model done by `parallelize`.
-        You should call this before doing `save_pretrained` so that the `model.state_dict` is fully compatible with the
+        You should call this function before calling `save_pretrained` so that the `model.state_dict` dictionary is fully compatible with the
         original model.
         """
         # Remove hooks
         if hasattr(self, "_hooks"):
             for h in self._hooks:
                 h.remove()
         # Remove poptorch Blocks
         for m in self.modules():
             if m is not self:
                 poptorch.removeBlocks(m)
         return self
 
     def num_parameters(self, only_trainable: bool = False, exclude_embeddings: bool = False) -> int:
         """
-        Get number of (optionally, trainable or non-embeddings) parameters in the module.
+        Gets the number of (optionally, trainable or non-embeddings) parameters in the module.
 
         Args:
             only_trainable (:obj:`bool`, `optional`, defaults to :obj:`False`):
-                Whether or not to return only the number of trainable parameters
+                If `True`, only returns the number of trainable parameters.
 
             exclude_embeddings (:obj:`bool`, `optional`, defaults to :obj:`False`):
-                Whether or not to return only the number of non-embeddings parameters
+                If `True`, only returns the number of non-embeddings parameters.
 
         Returns:
             :obj:`int`: The number of parameters.
         """
 
         # TODO: actually overwrite this to handle SerializedEmbedding.
         if exclude_embeddings:
@@ -198,31 +193,47 @@
             return sum(p.numel() for p in self.parameters() if p.requires_grad or not only_trainable)
 
 
 def _expand_layers_per_ipu_wildcard(
     ipu_config: IPUConfig, target_number_of_layers: Optional[Union[int, List]] = None
 ) -> List[int]:
     """
-    Expand any wildcard values in `ipu_config.layers_per_ipu`.
+    Expands any wildcard values in `layers_per_ipu` of the IPU configuration.
 
     For example, if we have:
     ```
     layers_per_ipu = [-1, -1]
     target_number_of_layers = 9
     ```
     this function will expand the wildcard values to `layers_per_ipu = [4, 5]`
+
+    Args:
+    ipu_config ([`IPUConfig`]):
+        The `IPUConfig` instance of the model.
+
+    target_number_of_layers (:obj:`int` or `List[int]`, `optional`):
+        The total number of target layers.
+
+    Returns:
+        :obj:`List[int]`: The `layers_per_ipu` with wildcards replaced by the number of layers per IPU.
     """
-    layers_per_ipu = copy.deepcopy(ipu_config.layers_per_ipu)
-    ipus_per_replica = ipu_config.ipus_per_replica
+    layers_per_ipu = copy.deepcopy(ipu_config._layers_per_ipu)
+    layers_per_ipu_mode_str = ipu_config._get_managed_attr_mode_name("layers_per_ipu")
+    ipus_per_replica = ipu_config._ipus_per_replica
+    ipus_per_replica_mode_str = ipu_config._get_managed_attr_mode_name("ipus_per_replica")
 
     # Check inputs are valid
     if not all(isinstance(n, int) and n >= -1 for n in layers_per_ipu):
-        raise IncompatibleIPUConfigError("Invalid values in layers_per_ipu. " f"layers_per_ipu={layers_per_ipu}")
+        raise IncompatibleIPUConfigError(
+            f"Invalid values in {layers_per_ipu_mode_str}. {layers_per_ipu_mode_str}={layers_per_ipu}"
+        )
     if ipus_per_replica < 1:
-        raise IncompatibleIPUConfigError("Invalid value for ipus_per_replica. " f"ipus_per_replica={ipus_per_replica}")
+        raise IncompatibleIPUConfigError(
+            f"Invalid value for {ipus_per_replica_mode_str}. {ipus_per_replica_mode_str}={ipus_per_replica}"
+        )
 
     if target_number_of_layers is not None:
         if not isinstance(target_number_of_layers, int):
             target_number_of_layers = len(target_number_of_layers)
 
         # if ipus_per_replica is 1, then put everything on IPU0, ignoring layers_per_ipu
         if ipus_per_replica == 1:
@@ -248,138 +259,180 @@
                     layers_per_ipu[idx] = quotient
                 if remainder > 0:
                     # add any remainder layers to last wildcard IPU
                     layers_per_ipu[wildcard_idxs[-1]] += remainder
 
             elif len(layers_per_ipu) != ipus_per_replica:
                 raise IncompatibleIPUConfigError(
-                    "layers_per_ipu has non-default value set, but its length does not match ipus_per_replica. "
-                    f"layers_per_ipu={layers_per_ipu}, ipus_per_replica={ipus_per_replica}. "
+                    f"{layers_per_ipu_mode_str} has a non-default value set, but its length does not match {ipus_per_replica_mode_str}"
+                    f"{layers_per_ipu_mode_str}={layers_per_ipu}, {ipus_per_replica_mode_str}={ipus_per_replica}. "
                 )
             # no wildcards used
             elif sum(layers_per_ipu) != target_number_of_layers:
                 raise IncompatibleIPUConfigError(
-                    "layers_per_ipu does not define the correct number of layers for the current model."
+                    f"{layers_per_ipu_mode_str} does not define the correct number of layers for the current model."
                     " The current IPU Config specifies IPU assignments for "
                     f"{sum(layers_per_ipu)} layers but there are {target_number_of_layers} layers "
-                    f"in the model. layers_per_ipu={layers_per_ipu}"
+                    f"in the model. {layers_per_ipu_mode_str}={layers_per_ipu}"
                 )
     return layers_per_ipu
 
 
 def split_encoder_decoder_ipu_config(
     ipu_config: IPUConfig, num_encoder_layers: int, num_decoder_layers: int
 ) -> List[IPUConfig]:
     """
-    Given an `ipu_config` for an entire encoder-decoder model and the number of encoder and decoder layers,
-    this function will split the `ipu_config` into two separate configs:
-      `encoder_ipu_config` and `decoder_ipu_config`.
-    It will split the `ipu_config.layers_per_ipu` into two given the inputted numbers of encoder and decoder
-    layers.
+    Splits  an `IPUConfig` instance for an encoder-decoder model into a configuration for the encoder part and a configuration for the decoder part.
+
+    It also splits `layers_per_ipu` into two given the numbers of encoder and decoder layers.
 
     Example:
     ```
     >> ipu_config = IPUConfig(layers_per_ipu=[12, 12], ipus_per_replica=2)
     >> encoder_ipu_config, decoder_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 12, 12)
 
     >> encoder_ipu_config
     => IPUConfig(layers_ler_ipu=[12], ipus_per_replica=1)
 
     >> decoder_ipu_config
     => IPUConfig(layers_ler_ipu=[12], ipus_per_replica=1)
     ```
 
     Args:
-        ipu_config: The `IPUConfig` for the the whole encoder-decoder model
-        num_encoder_layers: Number of encoder layers in the model
-        num_decoder_layers: Number of decoder layers in the model
+        ipu_config:
+            The `IPUConfig` instance for the the whole encoder-decoder model.
+        num_encoder_layers:
+            The number of encoder layers in the model.
+        num_decoder_layers:
+            The number of decoder layers in the model.
 
     Returns:
-        encoder_ipu_config, decoder_ipu_config
+        The configuration for the encoder part, `encoder_ipu_config`, and the configuration for the decoder part, `decoder_ipu_config`.
     """
+
+    layers_per_ipu_mode_str = ipu_config._get_managed_attr_mode_name("layers_per_ipu")
+    ipus_per_replica_mode_str = ipu_config._get_managed_attr_mode_name("ipus_per_replica")
+
     # Need at least two IPUs to do the split
-    if ipu_config.ipus_per_replica < 2:
+    if ipu_config._ipus_per_replica < 2:
         raise IncompatibleIPUConfigError(
-            "Need ipus_per_replica of at least 2 to split ipu_config into encoder and decoder configs"
+            f"Need {ipus_per_replica_mode_str} to be at least 2 to split ipu_config into encoder and decoder configs"
         )
 
     ipu_configs = {name: copy.deepcopy(ipu_config) for name in ["encoder", "decoder"]}
 
     # Split layers_per_ipu between the given num layers
     layers_per_ipu = _expand_layers_per_ipu_wildcard(ipu_config, num_encoder_layers + num_decoder_layers)
     cumsum = [sum(layers_per_ipu[: i + 1]) for i in range(len(layers_per_ipu))]
     try:
         cut = [i + 1 for i, c in enumerate(cumsum) if c == num_encoder_layers]
         # Choose the cut index that's the highest power of 2
         cut = max([num for num in cut if num & (num - 1) == 0])
     except:
         raise IncompatibleIPUConfigError(
-            f"Unable to find valid split of ipu_config.layers_per_ipu\n"
+            f"Unable to find a valid split of ipu_config.{layers_per_ipu_mode_str}\n"
             "Arguments: \n"
-            f"\tipu_config.layers_per_ipu={ipu_config.layers_per_ipu}\n"
+            f"\tipu_config.{layers_per_ipu_mode_str}={ipu_config._layers_per_ipu}\n"
             f"\tnum_encoder_layers={num_encoder_layers}\n"
             f"\tnum_decoder_layers={num_decoder_layers}\n"
             "Possible causes: \n"
             "Encoder and decoder layers cannot be placed on the same IPUs.\n"
-            "The encoder and decoder layers_per_ipu splits each need a number of devices that's a power of 2."
+            f"The encoder and decoder {layers_per_ipu_mode_str} splits each need a number of devices that's a power of 2."
         )
-    ipu_configs["encoder"].layers_per_ipu = layers_per_ipu[:cut]
-    ipu_configs["decoder"].layers_per_ipu = layers_per_ipu[cut:]
+    ipu_configs["encoder"]._layers_per_ipu = layers_per_ipu[:cut]
+    ipu_configs["decoder"]._layers_per_ipu = layers_per_ipu[cut:]
+
+    # Split the per ipu configurations for SerializedEmbedding and SplitProjection if they have been provided
+    # Note that serialized layers across IPUs cannot be present in both the encoder and decoder
+    if ipu_config._serialized_embedding_splits_per_ipu is not None:
+        ipu_configs["encoder"]._serialized_embedding_splits_per_ipu = ipu_config._serialized_embedding_splits_per_ipu[
+            :cut
+        ]
+        ipu_configs["decoder"]._serialized_embedding_splits_per_ipu = None
+        # dec_split must contain all zeros, this layer cannot be split across the encoder and decoder
+        if sum(dec_split := ipu_config._serialized_embedding_splits_per_ipu[cut:]):
+            serialized_embedding_splits_per_ipu_mode_str = ipu_config._get_managed_attr_mode_name(
+                "serialized_embedding_splits_per_ipu"
+            )
+            raise ValueError(
+                "The `SerializedEmbedding` must have all splits placed on the encoder, but"
+                f" {serialized_embedding_splits_per_ipu_mode_str}={ipu_config._serialized_embedding_splits_per_ipu} results in"
+                f" {dec_split} being placed on the decoder"
+            )
+
+    if ipu_config._serialized_projection_splits_per_ipu is not None:
+        ipu_configs["encoder"]._serialized_projection_splits_per_ipu = None
+        ipu_configs[
+            "decoder"
+        ]._serialized_projection_splits_per_ipu = ipu_config._serialized_projection_splits_per_ipu[cut:]
+        if sum(enc_split := ipu_config._serialized_projection_splits_per_ipu[:cut]):
+            serialized_projection_splits_per_ipu_mode_str = ipu_config._get_managed_attr_mode_name(
+                "serialized_projection_splits_per_ipu"
+            )
+            raise ValueError(
+                "The `SplitProjection` must have all splits placed on the decoder, but"
+                f" {serialized_projection_splits_per_ipu_mode_str}={ipu_config._serialized_projection_splits_per_ipu} results in"
+                f" {enc_split} being placed on the encoder"
+            )
 
     # Modify the ipus_per_replica
-    ipu_configs["encoder"].ipus_per_replica = len(ipu_configs["encoder"].layers_per_ipu)
-    ipu_configs["decoder"].ipus_per_replica = len(ipu_configs["decoder"].layers_per_ipu)
+    ipu_configs["encoder"]._ipus_per_replica = len(ipu_configs["encoder"]._layers_per_ipu)
+    ipu_configs["decoder"]._ipus_per_replica = len(ipu_configs["decoder"]._layers_per_ipu)
 
     # Split matmul_proportion between the given num layers
-    matmul_proportion = ipu_config.matmul_proportion
+    matmul_proportion = ipu_config._matmul_proportion
     if isinstance(matmul_proportion, list):
-        ipu_configs["encoder"].matmul_proportion = matmul_proportion[:cut]
-        ipu_configs["decoder"].matmul_proportion = matmul_proportion[cut:]
+        ipu_configs["encoder"]._matmul_proportion = matmul_proportion[:cut]
+        ipu_configs["decoder"]._matmul_proportion = matmul_proportion[cut:]
 
     return ipu_configs.values()
 
 
 def get_layer_ipu(ipu_config: IPUConfig, target_number_of_layers: Optional[Union[int, List]] = None) -> List[int]:
     layers_per_ipu = _expand_layers_per_ipu_wildcard(ipu_config, target_number_of_layers)
 
-    # List of the IPU Id for each encoder layer
+    # List of the IPU Id for each layer
     layer_ipu: List[int] = []
     for ipu, n_layers in enumerate(layers_per_ipu):
         layer_ipu += [ipu] * n_layers
 
     return layer_ipu
 
 
 def recomputation_checkpoint(module: nn.Module) -> torch.utils.hooks.RemovableHandle:
     """Annotates the output of a module to be checkpointed instead of
-    recomputed"""
+    recomputed."""
 
     def recompute_outputs(module, inputs, outputs):
         if isinstance(outputs, torch.Tensor):
             return poptorch.recomputationCheckpoint(outputs)
         elif isinstance(outputs, tuple):
             return tuple(poptorch.recomputationCheckpoint(y) for y in outputs)
 
     return module.register_forward_hook(recompute_outputs)
 
 
 def outline_attribute(module: nn.Module, value: str):
     """Adds an attribute to a module. This attribute will be used
-    when comparing operation equivalence in outlining. For example:
+    when comparing operation equivalence in outlining.
+
+    For example:
 
+    ```
     layer1 = nn.Linear(...)
     layer2 = nn.Linear(...)
     layer3 = nn.Linear(...)
     layer4 = nn.Linear(...)
     outline_attribute(layer1, "A")
     outline_attribute(layer2, "A")
     outline_attribute(layer3, "B")
+    ```
 
-    The code for layer1 can be reused for layer2.
-    But it can't be used for layer3 or layer4.
+    The code for `layer1` can be reused for `layer2`, but
+    it can't be used for `layer3` or `layer4`.
     """
     context = poptorch.Attribute(__outline={"layer": value})
 
     def enable(*args):
         context.__enter__()
 
     def disable(*args):
@@ -389,56 +442,75 @@
     handles.append(module.register_forward_pre_hook(enable))
     handles.append(module.register_forward_hook(disable))
     return handles
 
 
 class SerializedEmbedding(nn.Module):
     """
-    Wrapper for `nn.Embedding` layer that performs the embedding look-up into
+    Wrapper for an `nn.Embedding` layer that performs the embedding look-up into
     smaller serialized steps in order to reduce memory in the embedding gradient
     calculation.
 
     Args:
-        embedding: A `nn.Embedding` to wrap
-        serialization_factor: The number of serialized embedding look-ups
+        embedding:
+            An `nn.Embedding` instance to wrap.
+        serialization_factor:
+            The number of serialized embedding look-ups.
     """
 
     def __init__(self, embedding: nn.Embedding, serialization_factor: int):
         super().__init__()
         self.serialization_factor = serialization_factor
         self.num_embeddings = embedding.num_embeddings
 
         # Num embeddings should be divisible by the serialization factor
         assert self.num_embeddings % self.serialization_factor == 0
         self.split_size = self.num_embeddings // self.serialization_factor
 
         freeze = not embedding.weight.requires_grad
+        self.padding_idx = embedding.padding_idx
         self.split_embeddings = nn.ModuleList(
             [
                 nn.Embedding.from_pretrained(
                     embedding.weight[i * self.split_size : (i + 1) * self.split_size, :].detach(),
                     freeze=freeze,
                     padding_idx=embedding.padding_idx if i == 0 else None,
                 )
                 for i in range(self.serialization_factor)
             ]
         )
 
-    def deserialize(self):
+    @classmethod
+    def from_model(cls, embedding: nn.Embedding, serialization_factor: int) -> SerializedEmbedding:
+        return cls(embedding, serialization_factor)
+
+    def parallelize(self, splits_per_ipu: List[int]):
+        for ipu_id, splits in enumerate(splits_per_ipu):
+            if splits:
+                from_split = sum(splits_per_ipu[:ipu_id])
+                to_split = from_split + splits - 1
+                shard_range = f"{from_split}-{to_split}" if from_split != to_split else f"{from_split}"
+                logger.info(f"Embedding splits: {shard_range} --> IPU {ipu_id}")
+                self.split_embeddings[from_split] = poptorch.BeginBlock(
+                    self.split_embeddings[from_split], ipu_id=ipu_id, user_id=f"Embedding-{shard_range}"
+                )
+        return self
+
+    def to_model(self) -> nn.Embedding:
         """
-        Deserialize the internal wrapped embedding layer and return it as a
+        Deserialize the internal wrapped embedding layer and return it as an
         `nn.Embedding` object.
 
         Returns:
-            `nn.Embedding` layer
+            An `nn.Embedding` layer.
         """
 
         freeze = not self.split_embeddings[0].weight.requires_grad
         return nn.Embedding.from_pretrained(
-            torch.vstack([l.weight for l in self.split_embeddings]), padding_idx=0, freeze=freeze
+            torch.vstack([l.weight for l in self.split_embeddings]), padding_idx=self.padding_idx, freeze=freeze
         )
 
     def forward(self, indices):
         # iterate through the splits
         x_sum = None
         for i in range(self.serialization_factor):
             # mask out the indices not in this split
@@ -465,22 +537,25 @@
     """
     Exactly equivalent to `nn.Linear` layer, but with the matrix multiplication replaced with
     a serialized matrix multiplication: `poptorch.serializedMatMul`.
     The matrix multiplication is split into separate smaller multiplications, calculated one after the other,
     to reduce the memory requirements of the multiplication and its gradient calculation.
 
     Args:
-        in_features: Size of each input sample
-        out_features: Size of each output sample
-        factor: Number of serialized multiplications. Must be a factor of
+        in_features:
+            Size of each input sample
+        out_features:
+            Size of each output sample
+        factor:
+            Number of serialized multiplications. Must be a factor of
             the dimension to serialize on.
-        bias: If set to False, the layer will not learn an additive bias.
-            Default: True
-        mode: Which dimension of the matmul to serialize on:
-            for matrix A (m by n) multiplied by matrix B (n by p).
+        bias: If set to `False`, the layer will not learn an additive bias.
+            Default: `True`.
+        mode: The dimension of the matmul to serialize on.
+            For matrix A (m by n) multiplied by matrix B (n by p).
             * InputChannels: Split across the input channels (dimension m).
             * ReducingDim: Split across the reducing dimension (n).
             * OutputChannels: Split across the output channels (dimension p).
             * Disabled: Same as an ordinary matrix multiplication.
     """
 
     def __init__(
@@ -491,29 +566,132 @@
         bias=False,
         mode=poptorch.MatMulSerializationMode.OutputChannels,
     ):
         super().__init__(in_features, out_features, bias)
         self.mode = mode
         self.factor = factor
 
+    @classmethod
+    def from_model(
+        cls, model: nn.Linear, factor: int, mode=poptorch.MatMulSerializationMode.OutputChannels
+    ) -> SerializedLinear:
+        clone = copy.deepcopy(model)
+        clone.__class__ = cls
+        clone.factor = factor
+        clone.mode = mode
+        return clone
+
+    def to_model(self) -> nn.Linear:
+        del self.factor
+        del self.mode
+        original = copy.deepcopy(self)
+        original.__class__ = nn.Linear
+        return original
+
     def forward(self, x):
-        if not self.training:
-            output = super().forward(x)
-        else:
-            output = poptorch.serializedMatMul(x, self.weight.t(), self.mode, self.factor)
-            if self.bias is not None:
-                output += self.bias
+        output = poptorch.serializedMatMul(x, self.weight.t(), self.mode, self.factor)
+        if self.bias is not None:
+            output += self.bias
         return output
 
 
+class SplitProjection(torch.nn.Module):
+    """
+    Exactly equivalent to `nn.Linear` layer, but with the linear layer split into
+    partial linear layers in order to reduce resident memory. The linear layer
+    is split along the reducing dimension `nn.Linear.in_features` in equal parts.
+    The forward call aggregates the partial sums obtained from each linear layer.
+
+    Args:
+        linear: A `nn.Linear` to wrap
+        serialization_factor: The number of partitions of the linear layer. This must
+            be a factor of linear.in_features
+    """
+
+    def __init__(
+        self,
+        linear: torch.nn.Linear,
+        serialization_factor: int,
+    ) -> None:
+        super().__init__()
+
+        self.in_features = linear.in_features
+        self.out_features = linear.out_features
+        if self.in_features % serialization_factor != 0:
+            raise ValueError(f"{linear.in_features=} must be divisible by {serialization_factor=}")
+
+        self.split_size = self.in_features // serialization_factor
+        self.split_linear_layers = torch.nn.ModuleList()
+        for i in range(0, self.in_features, self.split_size):
+            split_linear = torch.nn.Linear(self.split_size, self.out_features, bias=False, dtype=linear.weight.dtype)
+            # initialise linear layer using a section of `linear` weight,
+            with torch.no_grad():
+                split_linear.weight.copy_(linear.weight[:, i : i + self.split_size].detach())
+            self.split_linear_layers.append(split_linear)
+
+        self.bias = None
+        if linear.bias is not None:
+            self.bias = torch.nn.Parameter(torch.zeros_like(linear.bias))
+            with torch.no_grad():
+                self.bias.copy_(linear.bias.detach())
+
+    def forward(self, x):
+        # each linear layer processes a partition of the input
+        out = None
+        for i, split_linear_layer in enumerate(self.split_linear_layers):
+            h = split_linear_layer(x[..., i * self.split_size : (i + 1) * self.split_size])
+            if out is None:
+                out = h
+            else:
+                out += h
+        if self.bias is not None:
+            out += self.bias
+        return out
+
+    @classmethod
+    def from_model(cls, linear: torch.nn.Linear, serialization_factor: int) -> SplitProjection:
+        return cls(linear, serialization_factor)
+
+    def to_model(self) -> nn.Linear:
+        """
+        Merge the sub linear layers into one
+
+        Returns:
+            `nn.Linear` layer
+        """
+        dtype = self.split_linear_layers[0].weight.dtype
+        layer = nn.Linear(self.in_features, self.out_features, bias=self.bias is not None)
+        if dtype == torch.float16:
+            layer = layer.half()
+        with torch.no_grad():
+            layer.weight.copy_(torch.hstack([l.weight.detach() for l in self.split_linear_layers]))
+            if self.bias is not None:
+                layer.bias.copy_(self.bias)
+        return layer
+
+    def parallelize(self, splits_per_ipu: List[int]):
+        for ipu_id, splits in enumerate(splits_per_ipu):
+            if splits:
+                from_split = sum(splits_per_ipu[:ipu_id])
+                to_split = from_split + splits - 1
+                shard_range = f"{from_split}-{to_split}" if from_split != to_split else f"{from_split}"
+                logger.info(f"Linear splits: {shard_range} --> IPU {ipu_id}")
+                self.split_linear_layers[from_split] = poptorch.BeginBlock(
+                    self.split_linear_layers[from_split], ipu_id=ipu_id, user_id=f"Linear-{shard_range}"
+                )
+        return self
+
+
 class SharedEmbedding(nn.Module):
-    """Wrapper around the shared embedding between the encoder and the decoder stacks.
+    """
+    Wrapper around the shared embedding between the encoder and the decoder stacks.
 
     Attributes:
-        shared: The shared embedding layer.
+        shared:
+            The shared embedding layer.
     """
 
     def __init__(self, shared: nn.Embedding):
         super().__init__()
         self.shared = shared
 
     def _combine_inputs(self, input_ids: torch.Tensor, decoder_input_ids: torch.Tensor) -> Tuple[int, torch.Tensor]:
@@ -563,12 +741,12 @@
     """
     Gathers selected indices from a tensor by transforming the list of indices
     into a one-hot matrix and then multiplying the tensor by that matrix.
     """
 
     def forward(self, sequence, positions):
         """
-        Gather the vectors at the specific positions over a batch.
+        Gathers the vectors at the specific positions over a batch.
         """
         num_classes = int(sequence.shape[1])
         one_hot_positions = F.one_hot(positions, num_classes).to(dtype=sequence.dtype)
         return torch.matmul(one_hot_positions.detach(), sequence)
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import bart, bert, convnext, deberta, gpt2, groupbert, hubert, lxmert, roberta, t5, vit, wav2vec2, whisper
+from . import bart, bert, convnext, deberta, gpt2, groupbert, hubert, lxmert, mt5, roberta, t5, vit, wav2vec2, whisper
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/bart/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/bart/modeling_bart.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/bart/modeling_bart.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import copy
 import random
 from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 import poptorch
@@ -29,18 +30,19 @@
     Seq2SeqSequenceClassifierOutput,
 )
 from transformers.models.bart.modeling_bart import (
     BartAttention,
     BartDecoder,
     BartEncoder,
     BartEncoderLayer,
+    BartLearnedPositionalEmbedding,
     shift_tokens_right,
 )
 
-from ...generation_utils import IPUGenerationMixin, _IndexedInputLinear
+from ...generation import IPUAttentionMixin, IPUGenerationMixin, supports_kv_cache
 from ...modeling_utils import (
     PipelineMixin,
     SerializedLinear,
     SharedEmbedding,
     get_layer_ipu,
     recomputation_checkpoint,
     register,
@@ -79,15 +81,15 @@
     inverted_mask = 1.0 - expanded_mask
 
     # Using FLOAT16_LIMIT instead of -float("inf") to avoid NaNs on the IPUs.
     inverted_mask = -FLOAT16_LIMIT * inverted_mask
     return inverted_mask.to(dtype)
 
 
-class _BartAttentionWithoutException(BartAttention):
+class IPUBartAttention(BartAttention, IPUAttentionMixin):
     """The same as BartAttention without the attention mask shape check.
 
     This is needed because the original BartAttention checks that the attention mask shape is [bs, 1, tgt_len, src_len]
     but the pipelined implementation does not expand the mask, it just inserts dimensions, the shape is then
     [bs, 1, 1, src_len], and broadcasting does the rest.
     """
 
@@ -106,29 +108,28 @@
         # for the decoder
         is_cross_attention = key_value_states is not None
 
         bsz, tgt_len, _ = hidden_states.size()
 
         # get query proj
         query_states = self.q_proj(hidden_states) * self.scaling
-        # get key, value proj
-        if is_cross_attention and past_key_value is not None:
-            # reuse k,v, cross_attentions
-            key_states = past_key_value[0]
-            value_states = past_key_value[1]
-        elif is_cross_attention:
-            # cross_attentions
+        if key_value_states is not None:
+            # cross attention
             key_states = self._shape(self.k_proj(key_value_states), -1, bsz)
             value_states = self._shape(self.v_proj(key_value_states), -1, bsz)
-        elif past_key_value is not None:
-            # reuse k, v, self_attention
+        elif self.kv_cache_initialized:
+            # self attention with kv cache
             key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
             value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
-            key_states = torch.cat([past_key_value[0], key_states], dim=2)
-            value_states = torch.cat([past_key_value[1], value_states], dim=2)
+
+            if tgt_len != 1:
+                raise ValueError(f"KV cache expects tgt_len = 1, received {tgt_len}.")
+
+            key_states, value_states = self.add_to_kv_cache(key_states, value_states)
+            attention_mask = self.update_attention_mask(attention_mask)
         else:
             # self_attention
             key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
             value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
 
         if self.is_decoder:
             # if cross_attention save Tuple(torch.Tensor, torch.Tensor) of all cross attention key/value_states.
@@ -534,14 +535,42 @@
             past_key_values=next_cache,
             hidden_states=all_hidden_states,
             attentions=all_self_attns,
             cross_attentions=all_cross_attentions,
         )
 
 
+class IPUBartLearnedPositionalEmbedding(BartLearnedPositionalEmbedding):
+    """
+    This module learns positional embeddings up to a fixed maximum size.
+    """
+
+    @classmethod
+    def from_model(cls, model: BartLearnedPositionalEmbedding):
+        clone = copy.deepcopy(model)
+        clone.__class__ = cls
+        clone.register_buffer("_generation_step", torch.tensor([0], dtype=torch.int32), persistent=False)
+        return clone
+
+    def to_model(self) -> BartLearnedPositionalEmbedding:
+        del self._generation_step
+
+        original = copy.deepcopy(self)
+        original.__class__ = BartLearnedPositionalEmbedding
+        return original
+
+    def forward(self, input_ids: torch.Tensor, past_key_values_length: int = 0):
+        if input_ids.shape[-1] == 1:
+            # KV cache enabled.
+            del past_key_values_length
+            return poptorch.dynamic_slice(self.weight, 0, self._generation_step + self.offset, 1, 1)
+        else:
+            return super().forward(input_ids, past_key_values_length)
+
+
 class _BartModelWithSharedEmbedding(BartModel):
     @property
     def is_encoder_and_decoder_embeddings_computation_shared(self):
         return isinstance(self.shared, SharedEmbedding)
 
     def encoder_and_decoder_embeddings_computation(self, use_shared_embedding: bool):
         """Sets the BartModel shared embedding layer to SharedEmbedding that combines the computation under one layer.
@@ -569,25 +598,67 @@
             restore: whether to restore the encoder and decoder to their original version or not.
         """
         self.encoder.__class__ = BartEncoder if restore else _BartEncoderWithCustomExpandMask
         self.decoder.__class__ = BartDecoder if restore else _BartDecoderWithCustomMakeCausalAndExpandMask
         for layer in self.encoder.layers:
             layer.__class__ = BartEncoderLayer if restore else _BartEncoderLayerNoClamp
 
-    def change_bart_attention_class(self, restore: bool):
+    def change_bart_attention_class(self, restore: bool, **kwargs):
         """Changes the attention layers to either use the original BartAttention forward or
         BartAttentionWithoutException forward.
 
         Args:
             restore: whether to restore the attention layers to their original version or not.
         """
-        new_cls = BartAttention if restore else _BartAttentionWithoutException
-        for mod in self.modules():
-            if isinstance(mod, BartAttention):
-                mod.__class__ = new_cls
+        use_cache = kwargs.get("use_cache", False)
+        batch_size = kwargs.get("batch_size", 1)
+        max_length = kwargs.get("max_length", 128)
+        num_beams = kwargs.get("num_beams", 1)
+
+        for encoder_layer in self.encoder.layers:
+            if restore:
+                encoder_layer.self_attn = encoder_layer.self_attn.to_model(BartAttention)
+                continue
+
+            encoder_layer.self_attn = IPUBartAttention.from_model(
+                encoder_layer.self_attn,
+                use_cache=False,
+            )
+
+        for decoder_layer in self.decoder.layers:
+            if restore:
+                decoder_layer.self_attn = decoder_layer.self_attn.to_model(BartAttention)
+                decoder_layer.encoder_attn = decoder_layer.encoder_attn.to_model(BartAttention)
+                continue
+
+            decoder_layer.self_attn = IPUBartAttention.from_model(
+                decoder_layer.self_attn,
+                use_cache=use_cache,
+                batch_size=batch_size,
+                max_length=max_length,
+                num_beams=num_beams,
+                dtype=decoder_layer.self_attn.k_proj.weight.dtype,
+            )
+            decoder_layer.encoder_attn = IPUBartAttention.from_model(
+                decoder_layer.encoder_attn,
+                use_cache=False,
+            )
+
+    def change_decoder_positional_embedding(self, restore: bool):
+        """Changes the decoder positional embedding to support an optional static KV cache.
+
+        Args:
+            restore: whether to restore the decoder positional embedding to their original version or not.
+        """
+        position_embedding = self.decoder.embed_positions
+        self.decoder.embed_positions = (
+            position_embedding.to_model()
+            if restore
+            else IPUBartLearnedPositionalEmbedding.from_model(position_embedding)
+        )
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         decoder_input_ids=None,
         decoder_attention_mask=None,
@@ -680,17 +751,18 @@
             cross_attentions=decoder_outputs.cross_attentions,
             encoder_last_hidden_state=encoder_outputs.last_hidden_state,
             encoder_hidden_states=encoder_outputs.hidden_states,
             encoder_attentions=encoder_outputs.attentions,
         )
 
 
+@supports_kv_cache
 @register(BartForConditionalGeneration)
 class PipelinedBartForConditionalGeneration(BartForConditionalGeneration, PipelineMixin, IPUGenerationMixin):
-    def parallelize(self, for_generation=False):
+    def parallelize(self, for_generation=False, use_cache=False, **kwargs):
         """
         Transform the model to run in an IPU pipeline.
         - Adds pipeline stages to the model
         - (If enabled) Replaces the shared embedding with a SerializedEmbedding
         - Adds recomputation checkpoints
 
         Recommended usage:
@@ -700,29 +772,25 @@
         """
         super().parallelize()
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_lm_head = SerializedLinear(
-                self.config.d_model,
-                self.model.shared.num_embeddings,
-                self.ipu_config.embedding_serialization_factor,
-                bias=False,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
-            )
-            serialized_lm_head.load_state_dict(self.lm_head.state_dict())
-            self.lm_head = serialized_lm_head
+            self.lm_head = SerializedLinear.from_model(self.lm_head, self.ipu_config.embedding_serialization_factor)
             self.tie_weights()
 
         self.model.__class__ = _BartModelWithSharedEmbedding
-        self.model.encoder_and_decoder_embeddings_computation(True)
-        self.model.change_bart_encoder_and_decoder_classes(False)
-        self.model.change_bart_attention_class(False)
+        self.model.encoder_and_decoder_embeddings_computation(use_shared_embedding=True)
+        self.model.change_bart_encoder_and_decoder_classes(restore=False)
+        self.model.change_bart_attention_class(restore=False, use_cache=use_cache and for_generation, **kwargs)
+        self.model.change_decoder_positional_embedding(restore=False)
+        self.change_lm_head_to_indexed_input_linear(restore=not (for_generation and not use_cache))
+        self.use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
+        self.set_on_device_generation_steps(kwargs.get("on_device_generation_steps", 0))
 
         self.model.shared = poptorch.BeginBlock(self.model.shared, "Embedding", ipu_id=0)
         self.model.encoder.embed_positions = poptorch.BeginBlock(
             self.model.encoder.embed_positions, "Embedding", ipu_id=0
         )
         self.model.encoder.layernorm_embedding = poptorch.BeginBlock(
             self.model.encoder.layernorm_embedding, "Embedding", ipu_id=0
@@ -774,31 +842,44 @@
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         fully compatible with `transformers.BartForConditionalGeneration`.
         """
         super().deparallelize()
         self.model.encoder_and_decoder_embeddings_computation(False)
         self.model.change_bart_encoder_and_decoder_classes(True)
         self.model.change_bart_attention_class(True)
+        self.model.change_decoder_positional_embedding(restore=True)
         self.model.__class__ = BartModel
 
-        if self.lm_head.__class__ == _IndexedInputLinear:
-            self.lm_head = self.lm_head.wrapped_linear
+        self.change_lm_head_to_indexed_input_linear(restore=True)
+        self.set_on_device_generation_steps(0)
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            old_lm_head = nn.Linear(
-                self.config.d_model,
-                self.model.shared.num_embeddings,
-                bias=False,
-            )
-            old_lm_head.load_state_dict(self.lm_head.state_dict())
-            self.lm_head = old_lm_head
+        if isinstance(self.lm_head, SerializedLinear):
+            self.lm_head = self.lm_head.to_model()
             self.tie_weights()
 
         return self
 
+    def prepare_inputs_for_generation(
+        self, decoder_input_ids, past=None, use_cache=None, encoder_outputs=None, attention_mask=None, **kwargs
+    ):
+        # We don't use `past` for KV caching, and rely on `use_cache` instead.
+        beam_idx = None
+        if use_cache:
+            decoder_input_ids = decoder_input_ids[:, -1:]
+            beam_idx = kwargs.get("beam_idx", torch.arange(decoder_input_ids.shape[0], dtype=torch.long))
+
+        return {
+            "encoder_outputs": encoder_outputs,
+            "past_key_values": None,
+            "attention_mask": attention_mask,
+            "decoder_input_ids": decoder_input_ids,
+            "decoder_attention_mask": None,
+            "beam_idx": beam_idx,
+        }
+
     def forward(
         self,
         input_ids: torch.LongTensor = None,
         attention_mask: Optional[torch.Tensor] = None,
         decoder_input_ids: Optional[torch.LongTensor] = None,
         decoder_attention_mask: Optional[torch.LongTensor] = None,
         head_mask: Optional[torch.Tensor] = None,
@@ -862,17 +943,17 @@
         ```
         model = PipelinedBartForSequenceClassification(config).parallelize().half()
         ```
         """
         super().parallelize()
 
         self.model.__class__ = _BartModelWithSharedEmbedding
-        self.model.encoder_and_decoder_embeddings_computation(True)
-        self.model.change_bart_encoder_and_decoder_classes(False)
-        self.model.change_bart_attention_class(False)
+        self.model.encoder_and_decoder_embeddings_computation(use_shared_embedding=True)
+        self.model.change_bart_encoder_and_decoder_classes(restore=False)
+        self.model.change_bart_attention_class(restore=False)
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding --> IPU 0")
         self.model.shared = poptorch.BeginBlock(self.model.shared, "Embedding", ipu_id=0)
         self.model.encoder.embed_positions = poptorch.BeginBlock(
             self.model.encoder.embed_positions, "Embedding", ipu_id=0
         )
@@ -898,15 +979,15 @@
         for index, layer in enumerate(self.model.decoder.layers):
             ipu = layer_ipu[index + shift]
             if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
                 self._hooks.append(recomputation_checkpoint(layer))
             self.model.decoder.layers[index] = poptorch.BeginBlock(layer, f"Decoder{index}", ipu_id=ipu)
             logger.info(f"Decoder {index:<2} --> IPU {ipu}")
 
-        last_ipu = len(self.ipu_config.layers_per_ipu) - 1
+        last_ipu = layer_ipu[-1]
         logger.info(f"Classification Head Output --> IPU {last_ipu}")
         self.classification_head = poptorch.BeginBlock(
             self.classification_head, "Classification Head Output", ipu_id=last_ipu
         )
         logger.info("-----------------------------------------------------------")
         return self
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/bert/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/bert/bert_fused_attention.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/bert/bert_fused_attention.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/bert/modeling_bert.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/bert/modeling_bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,23 +74,17 @@
         super().parallelize()
 
         # Use faster fused-qkv self-attention
         for layer in self.bert.encoder.layer:
             layer.attention.self.__class__ = BertFusedSelfAttention
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_decoder = SerializedLinear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                self.ipu_config.embedding_serialization_factor,
-                bias=True,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
+            self.cls.predictions.decoder = SerializedLinear.from_model(
+                self.cls.predictions.decoder, self.ipu_config.embedding_serialization_factor
             )
-            serialized_decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-            self.cls.predictions.decoder = serialized_decoder
             self.tie_weights()
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding --> IPU 0")
         self.bert.embeddings = poptorch.BeginBlock(self.bert.embeddings, "Embedding", ipu_id=0)
         # Preventing the embeddings.LayerNorm from being outlined with the encoder.layer.LayerNorm
         # improves the tile mapping of the pipeline stashes
@@ -121,22 +115,16 @@
         compatible with the original model.
         """
         super().deparallelize()
 
         for layer in self.bert.encoder.layer:
             layer.attention.self.__class__ = BertSelfAttention
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            decoder = nn.Linear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                bias=True,
-            )
-            decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-            self.cls.predictions.decoder = decoder
+        if isinstance(self.cls.predictions.decoder, SerializedLinear):
+            self.cls.predictions.decoder = self.cls.predictions.decoder.to_model()
             self.tie_weights()
         return self
 
     def _init_weights(self, module):
         """Initialize the weights"""
 
         def truncated_normal_(tensor, mean=0, std=1):
@@ -246,23 +234,17 @@
         super().parallelize()
 
         # Use faster fused-qkv self-attention
         for layer in self.bert.encoder.layer:
             layer.attention.self.__class__ = BertFusedSelfAttention
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_decoder = SerializedLinear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                self.ipu_config.embedding_serialization_factor,
-                bias=True,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
+            self.cls.predictions.decoder = SerializedLinear.from_model(
+                self.cls.predictions.decoder, self.ipu_config.embedding_serialization_factor
             )
-            serialized_decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-            self.cls.predictions.decoder = serialized_decoder
             self.tie_weights()
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
         self.bert.embeddings = poptorch.BeginBlock(self.bert.embeddings, "Embedding", ipu_id=0)
         # Preventing the embeddings.LayerNorm from being outlined with the encoder.layer.LayerNorm
         # improves the tile mapping of the pipeline stashes
@@ -290,22 +272,16 @@
         compatible with the original model.
         """
         super().deparallelize()
 
         for layer in self.bert.encoder.layer:
             layer.attention.self.__class__ = BertSelfAttention
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            decoder = nn.Linear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                bias=True,
-            )
-            decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-            self.cls.predictions.decoder = decoder
+        if isinstance(self.cls.predictions.decoder, SerializedLinear):
+            self.cls.predictions.decoder = self.cls.predictions.decoder.to_model()
             self.tie_weights()
         return self
 
     def forward(
         self,
         input_ids: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
@@ -393,15 +369,15 @@
         # Use faster fused-qkv self-attention
         for layer in self.bert.encoder.layer:
             layer.attention.self.__class__ = BertFusedSelfAttention
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding --> IPU 0")
         if self.ipu_config.embedding_serialization_factor > 1:
-            self.bert.embeddings.word_embeddings = SerializedEmbedding(
+            self.bert.embeddings.word_embeddings = SerializedEmbedding.from_model(
                 self.bert.embeddings.word_embeddings, self.ipu_config.embedding_serialization_factor
             )
         self.bert.embeddings = poptorch.BeginBlock(self.bert.embeddings, "Embedding", ipu_id=0)
         hs = outline_attribute(self.bert.embeddings.LayerNorm, "embedding")
         self._hooks.extend(hs)
 
         layer_ipu = get_layer_ipu(self.ipu_config, self.bert.encoder.layer)
@@ -423,15 +399,15 @@
         super().deparallelize()
 
         for layer in self.bert.encoder.layer:
             layer.attention.self.__class__ = BertSelfAttention
 
         # Deserialize the serialized word embedding
         if self.ipu_config.embedding_serialization_factor > 1:
-            self.bert.embeddings.word_embeddings = self.bert.embeddings.word_embeddings.deserialize()
+            self.bert.embeddings.word_embeddings = self.bert.embeddings.word_embeddings.to_model()
         return self
 
 
 @register(BertForSequenceClassification)
 class PipelinedBertForSequenceClassification(BertForSequenceClassification, BertPipelineMixin):
     """
     BertForSequenceClassification transformed to run in an IPU pipeline.
@@ -440,15 +416,15 @@
     ```
     model = PipelinedBertForSequenceClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(BertForMultipleChoice)
@@ -460,15 +436,15 @@
     ```
     model = PipelinedBertForMultipleChoice(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(BertForTokenClassification)
@@ -480,15 +456,15 @@
     ```
     model = PipelinedBertForTokenClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(BertForQuestionAnswering)
@@ -500,15 +476,15 @@
     ```
     model = PipelinedBertForQuestionAnswering(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"QA Outputs --> IPU {last_ipu}")
         self.qa_outputs = poptorch.BeginBlock(self.qa_outputs, "QA Outputs", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/modeling_convnext.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/modeling_convnext.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         for stage_idx, stage in enumerate(self.convnext.encoder.stages):
             for layer_idx, layer in enumerate(stage.layers):
                 ipu = layer_ipu[global_layer_idx]
                 logger.info(f"Encoder stage {stage_idx}, convnext layer {layer_idx} --> IPU {ipu}")
                 layer = poptorch.BeginBlock(layer, f"Encoder_stage_{stage_idx}_layer_{layer_idx}", ipu_id=ipu)
                 global_layer_idx += 1
 
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Head --> IPU {last_ipu}")
         logger.info("---------------------------------------")
         self.convnext.layernorm = poptorch.BeginBlock(self.convnext.layernorm, "LayerNorm", ipu_id=last_ipu)
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier", ipu_id=last_ipu)
 
         return self
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/convnext/optimized_convnextlayer.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/optimized_convnextlayer.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/deberta/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/deberta/modeling_deberta.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/modeling_deberta.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,26 +301,20 @@
         """
         self._hooks = []
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
         if self.ipu_config.embedding_serialization_factor > 1:
             if isinstance(self, PipelinedDebertaForMaskedLM):
-                serialized_decoder = SerializedLinear(
-                    self.config.hidden_size,
-                    self.config.vocab_size,
-                    self.ipu_config.embedding_serialization_factor,
-                    bias=True,
-                    mode=poptorch.MatMulSerializationMode.OutputChannels,
+                self.cls.predictions.decoder = SerializedLinear.from_model(
+                    self.cls.predictions.decoder, self.ipu_config.embedding_serialization_factor
                 )
-                serialized_decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-                self.cls.predictions.decoder = serialized_decoder
                 self.tie_weights()
             else:
-                self.deberta.embeddings.word_embeddings = SerializedEmbedding(
+                self.deberta.embeddings.word_embeddings = SerializedEmbedding.from_model(
                     self.deberta.embeddings.word_embeddings, self.ipu_config.embedding_serialization_factor
                 )
 
         self.change_modules_for_ipu(False)
 
         self.deberta.embeddings = poptorch.BeginBlock(self.deberta.embeddings, "Embedding", ipu_id=0)
         hs = outline_attribute(self.deberta.embeddings.LayerNorm, "embedding")
@@ -349,26 +343,20 @@
         Undo the changes to the model done by `parallelize`.
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         compatible with the original model.
         """
         super().deparallelize()
         self.change_modules_for_ipu(True)
         if self.ipu_config.embedding_serialization_factor > 1:
-            if isinstance(self, PipelinedDebertaForMaskedLM):
-                decoder = nn.Linear(
-                    self.config.hidden_size,
-                    self.config.vocab_size,
-                    bias=True,
-                )
-                decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-                self.cls.predictions.decoder = decoder
+            if isinstance(self.cls.predictions.decoder, SerializedLinear):
+                self.cls.predictions.decoder = self.cls.predictions.decoder.to_model()
                 self.tie_weights()
             else:
                 # Deserialize the serialized word embedding
-                self.deberta.embeddings.word_embeddings = self.deberta.embeddings.word_embeddings.deserialize()
+                self.deberta.embeddings.word_embeddings = self.deberta.embeddings.word_embeddings.to_model()
         return self
 
 
 @register(DebertaForMaskedLM)
 class PipelinedDebertaForMaskedLM(DebertaForMaskedLM, DebertaPipelineMixin):
     """
     DebertaForMaskedLM transformed to run in an IPU pipeline.
@@ -454,15 +442,15 @@
     ```
     model = PipelinedDebertaForSequenceClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(DebertaForTokenClassification)
@@ -474,15 +462,15 @@
     ```
     model = PipelinedDebertaForTokenClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def deparallelize(self):
         super().deparallelize()
@@ -504,15 +492,15 @@
     ```
     model = PipelinedDebertaForQuestionAnswering(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"QA Outputs --> IPU {last_ipu}")
         self.qa_outputs = poptorch.BeginBlock(self.qa_outputs, "QA Outputs", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/distilbert/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/distilbert/modeling_distilbert.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/modeling_distilbert.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,24 +128,24 @@
         for layer in self.distilbert.transformer.layer:
             layer.attention.__class__ = IPUMultiHeadSelfAttention
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding --> IPU 0")
         is_masked_lm = isinstance(self, DistilBertForMaskedLM)
         if self.ipu_config.embedding_serialization_factor > 1 and not is_masked_lm:
-            self.distilbert.embeddings.word_embeddings = SerializedEmbedding(
+            self.distilbert.embeddings.word_embeddings = SerializedEmbedding.from_model(
                 self.distilbert.embeddings.word_embeddings, self.ipu_config.embedding_serialization_factor
             )
         self.distilbert.embeddings = poptorch.BeginBlock(self.distilbert.embeddings, "Embedding", 0)
 
         layer_ipu = get_layer_ipu(self.ipu_config, self.distilbert.transformer.layer)
         for index, layer in enumerate(self.distilbert.transformer.layer):
             ipu = layer_ipu[index]
             if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
-                recomputation_checkpoint(layer)
+                self._hooks.append(recomputation_checkpoint(layer))
             self.distilbert.transformer.layer[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
             logger.info(f"Encoder {index:<2} --> IPU {ipu}")
 
         return self
 
     def deparallelize(self):
         """
@@ -156,58 +156,46 @@
         super().deparallelize()
 
         for layer in self.distilbert.transformer.layer:
             layer.attention.__class__ = MultiHeadSelfAttention
 
         is_masked_lm = isinstance(self, DistilBertForMaskedLM)
         if self.ipu_config.embedding_serialization_factor > 1 and not is_masked_lm:
-            self.distilbert.embeddings.word_embeddings = self.distilbert.embeddings.word_embeddings.deserialize()
+            self.distilbert.embeddings.word_embeddings = self.distilbert.embeddings.word_embeddings.to_model()
 
         return self
 
 
 @register(DistilBertForMaskedLM)
 class PipelinedDistilBertForMaskedLM(DistilBertForMaskedLM, DistilBertPipelineMixin):
     def __init__(self, config):
         super().__init__(config)
         self.gather_indices = OnehotGather()
 
     def parallelize(self):
         super().parallelize()
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_vocab_projector = SerializedLinear(
-                self.config.dim,
-                self.config.vocab_size,
-                self.ipu_config.embedding_serialization_factor,
-                bias=True,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
+            self.vocab_projector = SerializedLinear.from_model(
+                self.vocab_projector, self.ipu_config.embedding_serialization_factor
             )
-            serialized_vocab_projector.load_state_dict(self.vocab_projector.state_dict())
-            self.vocab_projector = serialized_vocab_projector
             self.tie_weights()
 
         logger.info("LM Head --> IPU 0")
         self.vocab_transform = poptorch.BeginBlock(self.vocab_transform, "LM Head", ipu_id=0)
         self.vocab_layer_norm = poptorch.BeginBlock(self.vocab_layer_norm, "LM Head", ipu_id=0)
         self.vocab_projector = poptorch.BeginBlock(self.vocab_projector, "LM Head", ipu_id=0)
         logger.info("-----------------------------------------------------------")
         return self
 
     def deparallelize(self):
         super().deparallelize()
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            vocab_projector = nn.Linear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                bias=True,
-            )
-            vocab_projector.load_state_dict(self.vocab_projector.state_dict())
-            self.vocab_projector = vocab_projector
+        if isinstance(self.vocab_projector, SerializedLinear):
+            self.vocab_projector = self.vocab_projector.to_model()
             self.tie_weights()
 
     def forward(
         self,
         input_ids: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         head_mask: Optional[torch.Tensor] = None,
@@ -267,28 +255,28 @@
 
 
 @register(DistilBertForSequenceClassification)
 class PipelinedDistilBertForSequenceClassification(DistilBertForSequenceClassification, DistilBertPipelineMixin):
     def parallelize(self):
         super().parallelize()
 
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier --> IPU {last_ipu}")
         self.pre_classifier = poptorch.BeginBlock(self.pre_classifier, "Classifier", ipu_id=last_ipu)
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(DistilBertForQuestionAnswering)
 class PipelinedDistilBertForQuestionAnswering(DistilBertForQuestionAnswering, DistilBertPipelineMixin):
     def parallelize(self):
         super().parallelize()
 
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"QA Outputs --> IPU {last_ipu}")
         self.qa_outputs = poptorch.BeginBlock(self.qa_outputs, "QA Outputs", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
@@ -331,25 +319,25 @@
 
 
 @register(DistilBertForTokenClassification)
 class PipelinedDistilBertForTokenClassification(DistilBertForTokenClassification, DistilBertPipelineMixin):
     def parallelize(self):
         super().parallelize()
 
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(DistilBertForMultipleChoice)
 class PipelinedDistilBertForMultipleChoice(DistilBertForMultipleChoice, DistilBertPipelineMixin):
     def parallelize(self):
         super().parallelize()
 
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier --> IPU {last_ipu}")
         self.pre_classifier = poptorch.BeginBlock(self.pre_classifier, "Classifier", ipu_id=last_ipu)
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/modeling_gpt2.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/modeling_gpt2.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import poptorch
 from optimum.utils import logging
 from transformers import GPT2ForSequenceClassification, GPT2ForTokenClassification, GPT2LMHeadModel
 from transformers.modeling_outputs import CausalLMOutputWithCrossAttentions, SequenceClassifierOutputWithPast
 from transformers.models.gpt2.modeling_gpt2 import GPT2Attention
 
-from ...generation_utils import IPUGenerationMixin, _IndexedInputLinear
+from ...generation import IPUGenerationMixin
 from ...modeling_utils import (
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     outline_attribute,
     recomputation_checkpoint,
@@ -60,15 +60,15 @@
             new_vocab_size = (
                 math.ceil(self.config.vocab_size / self.ipu_config.embedding_serialization_factor)
                 * self.ipu_config.embedding_serialization_factor
             )
             if new_vocab_size > self.actual_vocab_size:
                 self.resize_token_embeddings(new_vocab_size)
 
-            self.transformer.wte = SerializedEmbedding(
+            self.transformer.wte = SerializedEmbedding.from_model(
                 self.transformer.wte, self.ipu_config.embedding_serialization_factor
             )
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
         self.transformer.wte = poptorch.BeginBlock(self.transformer.wte, "Token embedding", ipu_id=0)
         self.transformer.wpe = poptorch.BeginBlock(self.transformer.wpe, "Position embedding", ipu_id=0)
@@ -91,29 +91,29 @@
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         fully compatible with `transformers` models.
         """
         super().deparallelize()
 
         if self.ipu_config.embedding_serialization_factor > 1:
             # Deserialize the serialized word embedding
-            self.transformer.wte = self.transformer.wte.deserialize()
+            self.transformer.wte = self.transformer.wte.to_model()
 
             # Resize token embeddings back to origianl vocab_size
             if self.config.vocab_size > self.actual_vocab_size:
                 self.resize_token_embeddings(self.actual_vocab_size)
 
         # Switch back to non-optimized attention
         for layer in self.transformer.h:
             layer.attn.__class__ = GPT2Attention
         return self
 
 
 @register(GPT2LMHeadModel)
 class PipelinedGPT2LMHeadModel(GPT2LMHeadModel, PipelineMixin, IPUGenerationMixin):
-    def parallelize(self):
+    def parallelize(self, for_generation=False):
         """
         Transform the model to run in an IPU pipeline.
         - Adds pipeline stages to the model
         - Adds recomputation checkpoints
 
         Recommended usage:
         ```
@@ -133,25 +133,19 @@
                 math.ceil(self.config.vocab_size / self.ipu_config.embedding_serialization_factor)
                 * self.ipu_config.embedding_serialization_factor
             )
             if new_vocab_size > self.actual_vocab_size:
                 # There is a tie_weights operation in resize_token_embeddings so the lm_head's weight is also resized.
                 self.resize_token_embeddings(new_vocab_size)
 
-            serialized_lm_head = SerializedLinear(
-                self.config.n_embd,
-                self.config.vocab_size,  # Note that if padding is done, self.config.vocab_size == new_vocab_size
-                self.ipu_config.embedding_serialization_factor,
-                bias=False,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
-            )
-            serialized_lm_head.load_state_dict(self.lm_head.state_dict())
-            self.lm_head = serialized_lm_head
+            self.lm_head = SerializedLinear.from_model(self.lm_head, self.ipu_config.embedding_serialization_factor)
             self.tie_weights()
 
+        self.change_lm_head_to_indexed_input_linear(restore=not for_generation)
+
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Token Embedding     --> IPU 0")
         self.transformer.wte = poptorch.BeginBlock(self.transformer.wte, "Token embedding", ipu_id=0)
         logger.info("Position Embedding  --> IPU 0")
         self.transformer.wpe = poptorch.BeginBlock(self.transformer.wpe, "Position embedding", ipu_id=0)
         hs = outline_attribute(self.transformer.ln_f, "LayerNorm")
         self._hooks.extend(hs)
@@ -169,26 +163,18 @@
         self.lm_head = poptorch.BeginBlock(self.lm_head, "LM head", ipu_id=0)
         logger.info("-----------------------------------------------------------")
         return self
 
     def deparallelize(self):
         PipelineMixin.deparallelize(self)
 
-        if self.lm_head.__class__ == _IndexedInputLinear:
-            self.lm_head = self.lm_head.wrapped_linear
+        self.change_lm_head_to_indexed_input_linear(restore=True)
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            # Deserialize the serialized linear layer
-            old_lm_head = nn.Linear(
-                self.config.n_embd,
-                self.config.vocab_size,  # Note that if padding is done, self.config.vocab_size == new_vocab_size
-                bias=False,
-            )
-            old_lm_head.load_state_dict(self.lm_head.state_dict())
-            self.lm_head = old_lm_head
+        if isinstance(self.lm_head, SerializedLinear):
+            self.lm_head = self.lm_head.to_model()
             self.tie_weights()
 
             # Resize token embeddings back to origianl vocab_size.
             # There is a tie_weights operation in resize_token_embeddings so the lm_head's weight is also resized.
             if self.config.vocab_size > self.actual_vocab_size:
                 self.resize_token_embeddings(self.actual_vocab_size)
 
@@ -283,15 +269,15 @@
         )
 
 
 @register(GPT2ForSequenceClassification)
 class PipelinedGPT2ForSequenceClassification(GPT2ForSequenceClassification, GPT2PipelineMixin):
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Head       --> IPU {last_ipu}")
         self.score = poptorch.BeginBlock(self.score, "Score", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
@@ -339,12 +325,12 @@
         )
 
 
 @register(GPT2ForTokenClassification)
 class PipelinedGPT2ForTokenClassification(GPT2ForTokenClassification, GPT2PipelineMixin):
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Head       --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/groupbert_attention.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_attention.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/groupbert_convolution.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_convolution.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/groupbert_ffn.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_ffn.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/groupbert/modeling_groupbert.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/modeling_groupbert.py`

 * *Files 5% similar despite different names*

```diff
@@ -421,23 +421,17 @@
         - Adds pipeline stages to the model
         - (If enabled) Replaces the word embedding projection with a SerializedLinear layer
         - Adds recomputation checkpoints
         """
         super().parallelize()
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_decoder = SerializedLinear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                self.ipu_config.embedding_serialization_factor,
-                bias=True,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
+            self.cls.predictions.decoder = SerializedLinear.from_model(
+                self.cls.predictions.decoder, self.ipu_config.embedding_serialization_factor
             )
-            serialized_decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-            self.cls.predictions.decoder = serialized_decoder
             self.tie_weights()
 
         layer_ipu = get_layer_ipu(self.ipu_config, self.bert.encoder.layer)
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding --> IPU 0")
         self.bert.embeddings = poptorch.BeginBlock(self.bert.embeddings, "Embedding", ipu_id=0)
@@ -466,22 +460,16 @@
         """
         Undo the changes to the model done by `parallelize`.
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         compatible with the original model.
         """
         super().deparallelize()
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            decoder = nn.Linear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                bias=True,
-            )
-            decoder.load_state_dict(self.cls.predictions.decoder.state_dict())
-            self.cls.predictions.decoder = decoder
+        if isinstance(self.cls.predictions.decoder, SerializedLinear):
+            self.cls.predictions.decoder = self.cls.predictions.decoder.to_model()
             self.tie_weights()
         return self
 
     def _init_weights(self, module):
         """Initialize the weights"""
 
         def truncated_normal_(tensor, mean=0, std=1):
@@ -727,15 +715,15 @@
         super().parallelize()
 
         layer_ipu = get_layer_ipu(self.ipu_config, self.bert.encoder.layer)
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding --> IPU 0")
         if self.ipu_config.embedding_serialization_factor > 1:
-            self.bert.embeddings.word_embeddings = SerializedEmbedding(
+            self.bert.embeddings.word_embeddings = SerializedEmbedding.from_model(
                 self.bert.embeddings.word_embeddings, self.ipu_config.embedding_serialization_factor
             )
         self.bert.embeddings = poptorch.BeginBlock(self.bert.embeddings, "Embedding", ipu_id=0)
         hs = outline_attribute(self.bert.embeddings.LayerNorm, "embedding")
         self._hooks.extend(hs)
 
         for index, layer in enumerate(self.bert.encoder.layer):
@@ -753,15 +741,15 @@
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         compatible with the original model.
         """
         super().deparallelize()
 
         # Deserialize the serialized word embedding
         if self.ipu_config.embedding_serialization_factor > 1:
-            self.bert.embeddings.word_embeddings = self.bert.embeddings.word_embeddings.deserialize()
+            self.bert.embeddings.word_embeddings = self.bert.embeddings.word_embeddings.to_model()
         return self
 
 
 @register(GroupBertForSequenceClassification)
 class PipelinedGroupBertForSequenceClassification(GroupBertForSequenceClassification, BertPipelineMixin):
     """
     GroupBertForSequenceClassification transformed to run in an IPU pipeline.
@@ -770,15 +758,15 @@
     ```
     model = PipelinedGroupBertForSequenceClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(GroupBertForMultipleChoice)
@@ -790,15 +778,15 @@
     ```
     model = PipelinedGroupBertForMultipleChoice(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(GroupBertForTokenClassification)
@@ -810,15 +798,15 @@
     ```
     model = PipelinedGroupBertForTokenClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(GroupBertForQuestionAnswering)
@@ -830,15 +818,15 @@
     ```
     model = PipelinedGroupBertForQuestionAnswering(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"QA Outputs --> IPU {last_ipu}")
         self.qa_outputs = poptorch.BeginBlock(self.qa_outputs, "QA Outputs", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/hubert/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/hubert/ipu_layer_drop.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/ipu_layer_drop.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/lxmert/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/lxmert/modeling_lxmert.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/modeling_lxmert.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/roberta/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/roberta/modeling_roberta.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/modeling_roberta.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         - Adds recomputation checkpoints
         """
         super().parallelize()
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
         if self.ipu_config.embedding_serialization_factor > 1:
-            self.roberta.embeddings.word_embeddings = SerializedEmbedding(
+            self.roberta.embeddings.word_embeddings = SerializedEmbedding.from_model(
                 self.roberta.embeddings.word_embeddings, self.ipu_config.embedding_serialization_factor
             )
         self.roberta.embeddings = poptorch.BeginBlock(self.roberta.embeddings, "Embedding", ipu_id=0)
         hs = outline_attribute(self.roberta.embeddings.LayerNorm, "embedding")
         self._hooks.extend(hs)
 
         layer_ipu = get_layer_ipu(self.ipu_config, self.roberta.encoder.layer)
@@ -79,15 +79,15 @@
         Undo the changes to the model done by `parallelize`.
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         fully compatible with `transformers.RobertaForSequenceClassification`.
         """
         super().deparallelize()
         # Deserialize the serialized word embedding
         if self.ipu_config.embedding_serialization_factor > 1:
-            self.roberta.embeddings.word_embeddings = self.roberta.embeddings.word_embeddings.deserialize()
+            self.roberta.embeddings.word_embeddings = self.roberta.embeddings.word_embeddings.to_model()
         return self
 
 
 @register(RobertaForMaskedLM)
 class PipelinedRobertaForMaskedLM(RobertaForMaskedLM, PipelineMixin):
     """
     RobertaForMaskedLM transformed to run in an IPU pipeline.
@@ -108,23 +108,17 @@
         - Adds pipeline stages to the model
         - (If enabled) Replaces the word embedding projection with a SerializedLinear layer
         - Adds recomputation checkpoints
         """
         super().parallelize()
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_decoder = SerializedLinear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                self.ipu_config.embedding_serialization_factor,
-                bias=True,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
+            self.lm_head.decoder = SerializedLinear.from_model(
+                self.lm_head.decoder, self.ipu_config.embedding_serialization_factor
             )
-            serialized_decoder.load_state_dict(self.lm_head.decoder.state_dict())
-            self.lm_head.decoder = serialized_decoder
             self.tie_weights()
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
         self.roberta.embeddings = poptorch.BeginBlock(self.roberta.embeddings, "Embedding", ipu_id=0)
         hs = outline_attribute(self.roberta.embeddings.LayerNorm, "embedding")
         self._hooks.extend(hs)
@@ -147,22 +141,16 @@
         """
         Undo the changes to the model done by `parallelize`.
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         compatible with the original model.
         """
         super().deparallelize()
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            decoder = nn.Linear(
-                self.config.hidden_size,
-                self.config.vocab_size,
-                bias=True,
-            )
-            decoder.load_state_dict(self.lm_head.decoder.state_dict())
-            self.lm_head.decoder = decoder
+        if isinstance(self.lm_head.decoder, SerializedLinear):
+            self.lm_head.decoder = self.lm_head.decoder.to_model()
             self.tie_weights()
         return self
 
     def forward(
         self,
         input_ids: Optional[torch.LongTensor] = None,
         attention_mask: Optional[torch.FloatTensor] = None,
@@ -244,15 +232,15 @@
     ```
     model = PipelinedRobertaForSequenceClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(RobertaForMultipleChoice)
@@ -264,15 +252,15 @@
     ```
     model = PipelinedRobertaForMultipleChoice(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(RobertaForTokenClassification)
@@ -284,15 +272,15 @@
     ```
     model = PipelinedRobertaForTokenClassification(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Classifier Output --> IPU {last_ipu}")
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier Output", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
 
 @register(RobertaForQuestionAnswering)
@@ -304,15 +292,15 @@
     ```
     model = PipelinedRobertaForQuestionAnswering(config).parallelize().half()
     ```
     """
 
     def parallelize(self):
         super().parallelize()
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"QA Outputs --> IPU {last_ipu}")
         self.qa_outputs = poptorch.BeginBlock(self.qa_outputs, "QA Outputs", ipu_id=last_ipu)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/t5/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/t5/modeling_t5.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/t5/modeling_t5.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,32 +18,54 @@
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 import poptorch
 from optimum.utils import logging
 from transformers import T5ForConditionalGeneration
+from transformers.activations import NewGELUActivation
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
 from transformers.models.t5.modeling_t5 import __HEAD_MASK_WARNING_MSG, T5Block, T5Stack
 
-from ...generation_utils import IPUGenerationMixin, _IndexedInputLinear
+from ...generation import IPUGenerationMixin
 from ...modeling_utils import (
     PipelineMixin,
     SerializedLinear,
     SharedEmbedding,
     get_layer_ipu,
     recomputation_checkpoint,
     register,
     split_encoder_decoder_ipu_config,
 )
 
 
 logger = logging.get_logger(__name__)
 
 
+class UpCastWrapper(nn.Module):
+    def __init__(self, module: nn.Module, scale: float = 1.0):
+        super().__init__()
+        self.module = module
+        self.scale = scale
+
+    def forward(self, input):
+        return self.module(input).to(torch.float32) * self.scale
+
+
+class CustomGELU(NewGELUActivation):
+    # Work-around bug with torch.nn.GELU(approximate="tanh")
+    # TODO: Remove this when bug is fixed
+    def forward(self, input: Tensor) -> Tensor:
+        safe = torch.logical_and(-39 < input, input < 39)
+        safe_input = torch.where(safe, input, 0.0)
+        gelu = super().forward(safe_input)
+        relu = nn.functional.relu(input)
+        return torch.where(safe, gelu, relu)
+
+
 class CustomT5Block(T5Block):
     def forward(
         self,
         hidden_states,
         attention_mask=None,
         position_bias=None,
         encoder_hidden_states=None,
@@ -81,15 +103,19 @@
             past_key_value=self_attn_past_key_value,
             use_cache=use_cache,
             output_attentions=output_attentions,
         )
         hidden_states, present_key_value_state = self_attention_outputs[:2]
         attention_outputs = self_attention_outputs[2:]  # Keep self-attention outputs and relative position weights
 
-        # Change: Remove check for inf and fp16 clamping
+        # clamp inf values to enable fp16 training
+        # Custom: Remove check for inf
+        if hidden_states.dtype == torch.float16:
+            clamp_value = torch.tensor(torch.finfo(hidden_states.dtype).max - 1000, dtype=hidden_states.dtype)
+            hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
 
         do_cross_attention = self.is_decoder and encoder_hidden_states is not None
         if do_cross_attention:
             # the actual query length is unknown for cross attention
             # if using past key value states. Need to inject it here
             if present_key_value_state is not None:
                 query_length = present_key_value_state[0].shape[2]
@@ -105,54 +131,52 @@
                 past_key_value=cross_attn_past_key_value,
                 query_length=query_length,
                 use_cache=use_cache,
                 output_attentions=output_attentions,
             )
             hidden_states = cross_attention_outputs[0]
 
-            # Change: Remove check for inf and fp16 clamping
+            # clamp inf values to enable fp16 training
+            # Custom: Remove check for inf
+            if hidden_states.dtype == torch.float16:
+                clamp_value = torch.tensor(torch.finfo(hidden_states.dtype).max - 1000, dtype=hidden_states.dtype)
+                hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
 
             # Combine self attn and cross attn key value states
             if present_key_value_state is not None:
                 present_key_value_state = present_key_value_state + cross_attention_outputs[1]
 
             # Keep cross-attention outputs and relative position weights
             attention_outputs = attention_outputs + cross_attention_outputs[2:]
 
         # Apply Feed Forward layer
         hidden_states = self.layer[-1](hidden_states)
 
-        # Change: Remove check for inf and fp16 clamping
+        # clamp inf values to enable fp16 training
+        # Custom: Remove check for inf
+        if hidden_states.dtype == torch.float16:
+            clamp_value = torch.tensor(torch.finfo(hidden_states.dtype).max - 1000, dtype=hidden_states.dtype)
+            hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
 
         outputs = (hidden_states,)
 
         if use_cache:
             outputs = outputs + (present_key_value_state,) + attention_outputs
         else:
             outputs = outputs + attention_outputs
 
         return outputs  # hidden-states, present_key_value_states, (self-attention position bias), (self-attention weights), (cross-attention position bias), (cross-attention weights)
 
 
 class CustomT5Stack(T5Stack):
-    def invert_attention_mask(self, encoder_attention_mask: Tensor) -> Tensor:
-        if encoder_attention_mask.dim() == 3:
-            encoder_extended_attention_mask = encoder_attention_mask[:, None, :, :]
-        if encoder_attention_mask.dim() == 2:
-            encoder_extended_attention_mask = encoder_attention_mask[:, None, None, :]
-        # T5 has a mask that can compare sequence ids, we can simulate this here with this transposition
-        # Cf. https://github.com/tensorflow/mesh/blob/8d2465e9bc93129b913b5ccc6a59aa97abd96ec6/mesh_tensorflow
-        # /transformer/transformer_layers.py#L270
-        # encoder_extended_attention_mask = (encoder_extended_attention_mask ==
-        # encoder_extended_attention_mask.transpose(-1, -2))
-        encoder_extended_attention_mask = encoder_extended_attention_mask.to(dtype=self.dtype)  # fp16 compatibility
-
-        # Always use -1e4 to avoid NaN issues.
-        encoder_extended_attention_mask = (1.0 - encoder_extended_attention_mask) * -1e4
-        return encoder_extended_attention_mask
+    def invert_attention_mask(self, *args, **kwargs) -> Tensor:
+        return super().invert_attention_mask(*args, **kwargs) * 0.75
+
+    def get_extended_attention_mask(self, *args, **kwargs) -> Tensor:
+        return super().get_extended_attention_mask(*args, **kwargs) * 0.75
 
 
 @register(T5ForConditionalGeneration)
 class PipelinedT5ForConditionalGeneration(T5ForConditionalGeneration, PipelineMixin, IPUGenerationMixin):
     @property
     def is_encoder_and_decoder_embeddings_computation_shared(self):
         return isinstance(self.shared, SharedEmbedding)
@@ -171,53 +195,14 @@
                 self.shared = SharedEmbedding(self.shared)
         else:
             if isinstance(self.shared, nn.Embedding):
                 logger.warning("encoder and decoder embeddings computation is not shared")
             else:
                 self.shared = self.shared.shared
 
-    def scale_down_weights(self, factor: float = 1, restore: bool = False):
-        self.lm_scale_modifier = 1 if not restore else None
-        # self.lm_scale_modifier = nn.Parameter(torch.ones(self.config.d_model, dtype=torch.float16)) if not restore else None
-
-        emb_scaling = 1 / 32.0 * factor
-        att_v_scaling = 1 / 4.0 * factor
-        att_o_scaling = 1 / 8.0 * factor
-        ff_wi_scaling = 1 / 4.0 * factor
-        ff_wo_scaling = 1 / 4.0 * factor
-        ff_ln_scaling = 1 / 2.0 * factor
-
-        if restore:
-            emb_scaling = 1 / emb_scaling
-            att_v_scaling = 1 / att_v_scaling
-            att_o_scaling = 1 / att_o_scaling
-            ff_wi_scaling = 1 / ff_wi_scaling
-            ff_wo_scaling = 1 / ff_wo_scaling
-            ff_ln_scaling = 1 / ff_ln_scaling
-
-        with torch.no_grad():
-            self.shared.weight *= emb_scaling
-            for unit in self.encoder.block:
-                unit.layer[0].SelfAttention.v.weight *= att_v_scaling
-                unit.layer[0].SelfAttention.o.weight *= att_o_scaling
-                unit.layer[1].DenseReluDense.wi.weight *= ff_wi_scaling
-                unit.layer[1].DenseReluDense.wo.weight *= ff_wo_scaling
-                unit.layer[1].layer_norm.weight *= ff_ln_scaling
-            for unit in self.decoder.block:
-                unit.layer[0].SelfAttention.v.weight *= att_v_scaling
-                unit.layer[0].SelfAttention.o.weight *= att_o_scaling
-                unit.layer[1].EncDecAttention.v.weight *= att_v_scaling
-                unit.layer[1].EncDecAttention.o.weight *= att_o_scaling
-                unit.layer[2].DenseReluDense.wi.weight *= ff_wi_scaling
-                unit.layer[2].DenseReluDense.wo.weight *= ff_wo_scaling
-                unit.layer[2].layer_norm.weight *= ff_ln_scaling
-
-            if not restore:
-                self.lm_scale_modifier /= emb_scaling
-
     def parallelize(self, for_generation=False):
         """
         Transform the model to run in an IPU pipeline.
         - Adds pipeline stages to the model
         - (If enabled) Replaces the shared embedding with a SerializedEmbedding
         - Adds recomputation checkpoints
 
@@ -228,40 +213,64 @@
         """
         PipelineMixin.parallelize(self)
 
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
 
         if self.ipu_config.embedding_serialization_factor > 1:
-            serialized_lm_head = SerializedLinear(
-                self.config.d_model,
-                self.shared.num_embeddings,
-                self.ipu_config.embedding_serialization_factor,
-                bias=False,
-                mode=poptorch.MatMulSerializationMode.OutputChannels,
-            )
-            serialized_lm_head.load_state_dict(self.lm_head.state_dict())
-            self.lm_head = serialized_lm_head
+            self.lm_head = SerializedLinear.from_model(self.lm_head, self.ipu_config.embedding_serialization_factor)
             # TODO: is it needed to check?
             if self.config.tie_word_embeddings:
                 self.tie_weights()
 
-        # self.scale_down_weights(factor=1)
+        self.change_lm_head_to_indexed_input_linear(restore=not for_generation)
+
         self.encoder_and_decoder_embeddings_computation(True)
         self.shared = poptorch.BeginBlock(self.shared, "Embedding", ipu_id=0)
 
         # Use a custom T5Stack implementation because sharing the position bias causes OOM error
         self.encoder.__class__ = CustomT5Stack
         self.decoder.__class__ = CustomT5Stack
 
+        # Upcast input embeddings so that the residuals remain in FP32. This
+        # cast is reversed where necessary by the T5LayerNorm layers in:
+        # - first layer of T5LayerSelfAttention
+        # - first layer of T5LayerFF
+        # - final_layer_norm
+        # Which, conveniently, are all the places that this needs to happen.
+        # Therefore, so we just need to upcast immediately before the residual
+        # adds in T5LayerSelfAttention and T5LayerFF. This is handled in the
+        # for loop below.
+        self.encoder.embed_tokens = UpCastWrapper(self.encoder.embed_tokens)
+
         # Use a custom T5Block implementation that removes a dynamic if blocks that can't be statically traced
         for block in self.encoder.block:
             block.__class__ = CustomT5Block
+            # Dropout happens immediately before the residual add. Inserting a
+            # cast in T5LayerSelfAttention and T5LayerFF keeps the residual
+            # structure in FP32
+            block.layer[0].dropout = UpCastWrapper(block.layer[0].dropout)
+            # Scale down the weights for the T5LayerFF down-projection and
+            # then scale its output back up again after it is cast to FP32
+            scale = 8.0
+            with torch.no_grad():
+                block.layer[1].DenseReluDense.wo.weight /= scale
+            block.layer[1].dropout = UpCastWrapper(block.layer[1].dropout, scale)
+            # Prevent overflow in NewGELUActivation
+            if self.config.dense_act_fn == "gelu_new":
+                # TODO: Work-around bug with torch.nn.GELU(approximate="tanh"). Replace
+                # this with block.layer[1].DenseReluDense.act = torch.nn.GELU(approximate="tanh")
+                # when bug is fixed
+                block.layer[1].DenseReluDense.act = CustomGELU()
         for block in self.decoder.block:
             block.__class__ = CustomT5Block
+            # Work-around bug with torch.nn.GELU(approximate="tanh")
+            # TODO: Remove this when bug is fixed
+            if self.config.dense_act_fn == "gelu_new":
+                block.layer[2].DenseReluDense.act = CustomGELU()
 
         num_encoder_layers = len(self.encoder.block)
         num_decoder_layers = len(self.decoder.block)
 
         if for_generation:
             # If running for text generation we split the IPU config into two configs
             # because we run the encoder and decoder as separate Poplar executors.
@@ -306,35 +315,37 @@
         You should call this before doing `save_pretrained` so that the `model.state_dict` is
         fully compatible with `transformers.T5ForConditionalGeneration`.
         """
         # T5ForConditionalGeneration has a deparallelize method, so make sure that the PipelineMixin one is used here.
         PipelineMixin.deparallelize(self)
 
         self.encoder_and_decoder_embeddings_computation(False)
-        # self.scale_down_weights(factor=1, restore=True)
 
         self.encoder.__class__ = T5Stack
         self.decoder.__class__ = T5Stack
 
+        self.encoder.embed_tokens = self.encoder.embed_tokens.module
+
         for block in self.encoder.block:
             block.__class__ = T5Block
+            block.layer[0].dropout = block.layer[0].dropout.module
+            with torch.no_grad():
+                block.layer[1].DenseReluDense.wo.weight *= block.layer[1].dropout.scale
+            block.layer[1].dropout = block.layer[1].dropout.module
+            if self.config.dense_act_fn == "gelu_new":
+                block.layer[1].DenseReluDense.act = NewGELUActivation()
         for block in self.decoder.block:
             block.__class__ = T5Block
+            if self.config.dense_act_fn == "gelu_new":
+                block.layer[2].DenseReluDense.act = NewGELUActivation()
 
-        if self.lm_head.__class__ == _IndexedInputLinear:
-            self.lm_head = self.lm_head.wrapped_linear
+        self.change_lm_head_to_indexed_input_linear(restore=True)
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            old_lm_head = nn.Linear(
-                self.config.d_model,
-                self.shared.num_embeddings,
-                bias=False,
-            )
-            old_lm_head.load_state_dict(self.lm_head.state_dict())
-            self.lm_head = old_lm_head
+        if isinstance(self.lm_head, SerializedLinear):
+            self.lm_head = self.lm_head.to_model()
             # TODO: is it needed to check?
             if self.config.tie_word_embeddings:
                 self.tie_weights()
 
         return self
 
     def forward(
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/vit/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/vit/modeling_vit.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/vit/modeling_vit.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,13 +36,13 @@
                 # Put checkpoints on every encoder layer
                 h = recomputation_checkpoint(layer)
                 self._hooks.append(h)
             ipu = layer_ipu[index]
             logger.info(f"Encoder {index:<2} --> IPU {ipu}")
             self.vit.encoder.layer[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
 
-        last_ipu = self.ipu_config.ipus_per_replica - 1
+        last_ipu = self.ipu_config._ipus_per_replica - 1
         logger.info(f"Head       --> IPU {last_ipu}")
         logger.info("---------------------------------------")
         self.vit.layernorm = poptorch.BeginBlock(self.vit.layernorm, "LayerNorm", ipu_id=last_ipu)
         self.classifier = poptorch.BeginBlock(self.classifier, "Classifier", ipu_id=last_ipu)
         return self
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         # Conv layers
         for index, layer in enumerate(self.wav2vec2.feature_extractor.conv_layers):
             layers.append((f"Conv {index:<2}", layer))
         # Positional Embedding
         layers.append(("Positional Embedding", self.wav2vec2.encoder.pos_conv_embed))
         # Encoder layers
         for index, layer in enumerate(self.wav2vec2.encoder.layers):
-            recomputation_checkpoint(layer)
+            self._hooks.append(recomputation_checkpoint(layer))
             layers.append((f"Encoder {index:<2}", layer))
         # Project Hidden
         layers.append(("Project Hidden", self.project_hid))
         # Quantizer
         layers.append(("Quantizer", self.quantizer))
         # Project Quantizer
         layers.append(("Project Quantizer", self.project_q))
@@ -429,25 +429,25 @@
 
         self.wav2vec2.__class__ = IPUWav2Vec2Model
         self.freeze_feature_encoder()
         self.change_wav2vec2_encoder_class(False)
         self.change_wav2vec2_adapter_class(False)
         self.change_conv_eps(False)
 
-        if self.ipu_config.ipus_per_replica != 1:
+        if self.ipu_config._ipus_per_replica != 1:
             logger.info("---------- Device Allocation -----------")
             layers = []
             # Conv layers
             for index, layer in enumerate(self.wav2vec2.feature_extractor.conv_layers):
                 layers.append((f"Conv {index:<2}", layer))
             # Positional Embedding
             layers.append(("Positional Embedding", self.wav2vec2.encoder.pos_conv_embed))
             # Encoder layers
             for index, layer in enumerate(self.wav2vec2.encoder.layers):
-                recomputation_checkpoint(layer)
+                self._hooks.append(recomputation_checkpoint(layer))
                 layers.append((f"Encoder {index:<2}", layer))
             # Project Hidden
             layers.append(("Project Hidden", self.lm_head))
 
             layer_ipu = get_layer_ipu(self.ipu_config, layers)
 
             for i, (name, layer) in enumerate(layers):
@@ -513,17 +513,21 @@
             # when not being attended to
             labels_mask = labels >= 0
             target_lengths = labels_mask.sum(-1)
 
             # ctc_loss doesn't support fp16
             log_probs = torch.nn.functional.log_softmax(logits.float(), dim=-1).transpose(0, 1)
 
-            loss_fn = torch.nn.CTCLoss(blank=self.config.pad_token_id, reduction=self.config.ctc_loss_reduction)
-            loss = loss_fn(log_probs.float(), labels, input_lengths, target_lengths)
-            loss = poptorch.identity_loss(loss, "sum")
+            loss_fn = torch.nn.CTCLoss(
+                blank=self.config.pad_token_id,
+                reduction=self.config.ctc_loss_reduction,
+                zero_infinity=self.config.ctc_zero_infinity,
+            )
+            loss = loss_fn(log_probs, labels, input_lengths, target_lengths)
+            loss = poptorch.identity_loss(loss, "none")
 
         if not return_dict:
             if loss is not None:
                 return loss, logits
             return (logits, hidden_states)
         return CausalLMOutput(loss=loss, logits=logits, hidden_states=outputs.hidden_states)
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/whisper/__init__.py` & `optimum-graphcore-0.6.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# flake8: noqa
-# There's no way to ignore "F401 '...' imported but unused" warnings in this
-# module, but to preserve other warnings. So, don't check this module at all.
-
-# Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright 2021 The HuggingFace Team. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#      http://www.apache.org/licenses/LICENSE-2.0
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
 
-from .modeling_whisper import PipelinedWhisperForConditionalGeneration
+[tool.black]
+line-length = 119
+target-version = ['py38']
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/models/whisper/modeling_whisper.py` & `optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/modeling_whisper.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,37 +7,32 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import random
-from typing import List, Optional, Tuple, Union
+import copy
+from typing import Optional, Tuple
 
 import torch
 from torch import nn
 
 import poptorch
 from optimum.utils import logging
 from transformers import WhisperConfig
-from transformers.modeling_outputs import (
-    BaseModelOutput,
-    BaseModelOutputWithPastAndCrossAttentions,
-    Seq2SeqModelOutput,
-)
 from transformers.models.whisper.modeling_whisper import (
     WhisperAttention,
     WhisperDecoder,
-    WhisperEncoder,
     WhisperEncoderLayer,
     WhisperForConditionalGeneration,
+    WhisperPositionalEmbedding,
 )
 
-from ...generation_utils import IPUGenerationMixin, _IndexedInputLinear
+from ...generation import IPUAttentionMixin, IPUGenerationMixin, supports_kv_cache
 from ...modeling_utils import (
     PipelineMixin,
     get_layer_ipu,
     recomputation_checkpoint,
     register,
     split_encoder_decoder_ipu_config,
 )
@@ -78,14 +73,129 @@
     expanded_mask = mask[:, None, None, :].expand(bsz, 1, tgt_len, src_len).to(dtype)
 
     inverted_mask = 1.0 - expanded_mask
 
     return inverted_mask.masked_fill(inverted_mask.to(torch.bool), -FLOAT16_LIMIT)
 
 
+class IPUWhisperAttention(WhisperAttention, IPUAttentionMixin):
+    def forward(
+        self,
+        hidden_states: torch.Tensor,
+        key_value_states: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        attention_mask: Optional[torch.Tensor] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        output_attentions: bool = False,
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
+        bsz, tgt_len, _ = hidden_states.size()
+
+        query_states = self.q_proj(hidden_states) * self.scaling
+        if key_value_states is not None:
+            # cross attention
+            key_states = self._shape(self.k_proj(key_value_states), -1, bsz)
+            value_states = self._shape(self.v_proj(key_value_states), -1, bsz)
+        elif self.kv_cache_initialized:
+            # self attention with kv cache
+            key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
+            value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+
+            if tgt_len != 1:
+                raise ValueError(f"KV cache expects tgt_len = 1, received {tgt_len}.")
+
+            key_states, value_states = self.add_to_kv_cache(key_states, value_states)
+            attention_mask = self.update_attention_mask(attention_mask)
+        else:
+            # self attention
+            key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
+            value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+
+        if self.is_decoder:
+            # We handle the KV cache via buffers, not via the eager approach of passing the cache around.
+            # This is retained so upstream DecoderLayer can stay as is and that tests pass.
+            past_key_value = (key_states, value_states)
+
+        proj_shape = (bsz * self.num_heads, -1, self.head_dim)
+        query_states = self._shape(query_states, tgt_len, bsz).view(*proj_shape)
+        key_states = key_states.view(*proj_shape)
+        value_states = value_states.view(*proj_shape)
+
+        src_len = key_states.size(1)
+
+        # Change: optionally serialize attention, mainly intended for the encoder with large sequence length.
+        if self.is_attention_serialized:
+            if layer_head_mask is not None:
+                raise ValueError("layer_head_mask is not supported yet with serialized attention.")
+
+            if self.dropout or self.training:
+                raise ValueError("dropout is not supported yet with serialized attention.")
+
+            if attention_mask is not None:
+                if attention_mask.size() != (bsz, 1, tgt_len, src_len):
+                    raise ValueError(
+                        f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {attention_mask.size()}"
+                    )
+                attention_mask = attention_mask.view(bsz, tgt_len, src_len).repeat(self.num_heads, 1, 1)
+
+            attn_output = self.serialized_attention(query_states, key_states, value_states, 1.0, attention_mask)
+        else:
+            attn_weights = torch.bmm(query_states, key_states.transpose(1, 2))
+
+            if attn_weights.size() != (bsz * self.num_heads, tgt_len, src_len):
+                raise ValueError(
+                    f"Attention weights should be of size {(bsz * self.num_heads, tgt_len, src_len)}, but is"
+                    f" {attn_weights.size()}"
+                )
+
+            if attention_mask is not None:
+                if attention_mask.size() != (bsz, 1, tgt_len, src_len):
+                    raise ValueError(
+                        f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {attention_mask.size()}"
+                    )
+                attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len) + attention_mask
+                attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
+
+            attn_weights = nn.functional.softmax(attn_weights, dim=-1)
+
+            if layer_head_mask is not None:
+                if layer_head_mask.size() != (self.num_heads,):
+                    raise ValueError(
+                        f"Head mask for a single layer should be of size {(self.num_heads,)}, but is"
+                        f" {layer_head_mask.size()}"
+                    )
+                attn_weights = layer_head_mask.view(1, -1, 1, 1) * attn_weights.view(
+                    bsz, self.num_heads, tgt_len, src_len
+                )
+                attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
+
+            # Change: delete optional reshaping of attn_weights
+
+            attn_probs = nn.functional.dropout(attn_weights, p=self.dropout, training=self.training)
+
+            attn_output = torch.bmm(attn_probs, value_states)
+
+        if attn_output.size() != (bsz * self.num_heads, tgt_len, self.head_dim):
+            raise ValueError(
+                f"`attn_output` should be of size {(bsz, self.num_heads, tgt_len, self.head_dim)}, but is"
+                f" {attn_output.size()}"
+            )
+
+        attn_output = attn_output.view(bsz, self.num_heads, tgt_len, self.head_dim)
+        attn_output = attn_output.transpose(1, 2)
+
+        attn_output = attn_output.reshape(bsz, tgt_len, self.embed_dim)
+        attn_output = self.out_proj(attn_output)
+
+        # Change: modified check for output_attentions
+        if not output_attentions:
+            attn_weights = None
+
+        return attn_output, attn_weights, past_key_value
+
+
 class _WhisperEncoderLayerClamp(nn.Module):
     def __init__(self, config: WhisperConfig):
         super().__init__()
         self.embed_dim = config.d_model
         self.self_attn = WhisperAttention(
             embed_dim=self.embed_dim,
             num_heads=config.encoder_attention_heads,
@@ -147,126 +257,37 @@
 
         if output_attentions:
             outputs += (attn_weights,)
 
         return outputs
 
 
-class _WhisperEncoderWithCustomExpandMask(WhisperEncoder):
-    """
-    Transformer encoder consisting of *config.encoder_layers* self attention layers. Each layer is a
-    [`WhisperEncoderLayer`].
-
-    Args:
-        config: WhisperConfig
-        embed_tokens (nn.Embedding): output embedding
-    """
-
-    def forward(
-        self,
-        input_features,
-        attention_mask=None,
-        head_mask=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        r"""
-        Args:
-            input_features (`torch.LongTensor` of shape `(batch_size, feature_size, sequence_length)`):
-                Float values of mel features extracted from the raw speech waveform. Raw speech waveform can be
-                obtained by loading a `.flac` or `.wav` audio file into an array of type `List[float]` or a
-                `numpy.ndarray`, *e.g.* via the soundfile library (`pip install soundfile`). To prepare the array into
-                `input_features`, the [`WhisperFeatureExtractor`] should be used for extracting the mel features,
-                padding and conversion into a tensor of type `torch.FloatTensor`. See
-                [`~WhisperFeatureExtractor.__call__`]
-            attention_mask (`torch.Tensor`)`, *optional*):
-                Whisper does not support masking of the `input_features`, this argument is preserved for compatibility,
-                but it is not used. By default the silence in the input log mel spectrogram are ignored.
-            head_mask (`torch.Tensor` of shape `(encoder_layers, encoder_attention_heads)`, *optional*):
-                Mask to nullify selected heads of the attention modules. Mask values selected in `[0, 1]`:
-
-                - 1 indicates the head is **not masked**,
-                - 0 indicates the head is **masked**.
-            output_attentions (`bool`, *optional*):
-                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
-                returned tensors for more detail.
-            output_hidden_states (`bool`, *optional*):
-                Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
-                for more detail.
-            return_dict (`bool`, *optional*):
-                Whether or not to return a [`~utils.ModelOutput`] instead of a plain tuple.
-        """
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-        inputs_embeds = nn.functional.gelu(self.conv1(input_features))
-        inputs_embeds = nn.functional.gelu(self.conv2(inputs_embeds))
-
-        inputs_embeds = inputs_embeds.permute(0, 2, 1)
-        embed_pos = self.embed_positions.weight
-
-        hidden_states = inputs_embeds + embed_pos
-        hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
-
-        encoder_states = () if output_hidden_states else None
-        all_attentions = () if output_attentions else None
-
-        # check if head_mask has a correct number of layers specified if desired
-        if head_mask is not None:
-            assert head_mask.size()[0] == (
-                len(self.layers)
-            ), f"The head_mask should be specified for {len(self.layers)} layers, but it is for {head_mask.size()[0]}."
-
-        for idx, encoder_layer in enumerate(self.layers):
-            if output_hidden_states:
-                encoder_states = encoder_states + (hidden_states,)
-            # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
-            dropout_probability = random.uniform(0, 1)
-            if self.training and (dropout_probability < self.layerdrop):  # skip the layer
-                layer_outputs = (None, None)
-            else:
-                if self.gradient_checkpointing and self.training:
-
-                    def create_custom_forward(module):
-                        def custom_forward(*inputs):
-                            return module(*inputs, output_attentions)
-
-                        return custom_forward
-
-                    layer_outputs = torch.utils.checkpoint.checkpoint(
-                        create_custom_forward(encoder_layer),
-                        hidden_states,
-                        None,
-                        (head_mask[idx] if head_mask is not None else None),
-                    )
-                else:
-                    layer_outputs = encoder_layer(
-                        hidden_states,
-                        None,
-                        layer_head_mask=(head_mask[idx] if head_mask is not None else None),
-                        output_attentions=output_attentions,
-                    )
-
-                hidden_states = layer_outputs[0]
-
-            if output_attentions:
-                all_attentions = all_attentions + (layer_outputs[1],)
-
-        hidden_states = self.layer_norm(hidden_states)
-        if output_hidden_states:
-            encoder_states = encoder_states + (hidden_states,)
-
-        if not return_dict:
-            return tuple(v for v in [hidden_states, encoder_states, all_attentions] if v is not None)
-        return BaseModelOutput(
-            last_hidden_state=hidden_states, hidden_states=encoder_states, attentions=all_attentions
-        )
+class IPUWhisperPositionalEmbedding(WhisperPositionalEmbedding):
+    @classmethod
+    def from_model(cls, model: WhisperPositionalEmbedding):
+        clone = copy.deepcopy(model)
+        clone.__class__ = cls
+        clone.register_buffer("_generation_step", torch.tensor([0], dtype=torch.int32), persistent=False)
+        return clone
+
+    def to_model(self) -> WhisperPositionalEmbedding:
+        del self._generation_step
+
+        original = copy.deepcopy(self)
+        original.__class__ = WhisperPositionalEmbedding
+        return original
+
+    def forward(self, input_ids: torch.Tensor, past_key_values_length: int = 0):
+        del past_key_values_length
+
+        if input_ids.shape[-1] == 1:
+            # KV cache enabled.
+            return poptorch.dynamic_slice(self.weight, 0, self._generation_step, 1, 1)
+        else:
+            return self.weight[: input_ids.shape[-1]]
 
 
 class _WhisperDecoderWithCustomMakeCausalAndExpandMask(WhisperDecoder):
     """
     Transformer decoder consisting of *config.decoder_layers* layers. Each layer is a [`WhisperDecoderLayer`]
 
     Args:
@@ -288,242 +309,100 @@
             expanded_attn_mask = _expand_mask(attention_mask, inputs_embeds.dtype, tgt_len=input_shape[-1])
             combined_attention_mask = (
                 expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask + combined_attention_mask
             )
 
         return combined_attention_mask
 
-    def forward(
-        self,
-        input_ids=None,
-        attention_mask=None,
-        encoder_hidden_states=None,
-        head_mask=None,
-        cross_attn_head_mask=None,
-        past_key_values=None,
-        inputs_embeds=None,
-        use_cache=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        r"""
-        Args:
-            input_ids (`torch.LongTensor` of shape `(batch_size, sequence_length)`):
-                Indices of input sequence tokens in the vocabulary. Padding will be ignored by default should you
-                provide it.
-
-                Indices can be obtained using [`WhisperTokenizer`]. See [`PreTrainedTokenizer.encode`] and
-                [`PreTrainedTokenizer.__call__`] for details.
-
-                [What are input IDs?](../glossary#input-ids)
-            attention_mask (`torch.Tensor` of shape `(batch_size, sequence_length)`, *optional*):
-                Mask to avoid performing attention on padding token indices. Mask values selected in `[0, 1]`:
-
-                - 1 for tokens that are **not masked**,
-                - 0 for tokens that are **masked**.
-
-                [What are attention masks?](../glossary#attention-mask)
-            encoder_hidden_states (`torch.FloatTensor` of shape `(batch_size, encoder_sequence_length, hidden_size)`, *optional*):
-                Sequence of hidden-states at the output of the last layer of the encoder. Used in the cross-attention
-                of the decoder.
-            head_mask (`torch.Tensor` of shape `(decoder_layers, decoder_attention_heads)`, *optional*):
-                Mask to nullify selected heads of the attention modules. Mask values selected in `[0, 1]`:
-
-                - 1 indicates the head is **not masked**,
-                - 0 indicates the head is **masked**.
-
-            cross_attn_head_mask (`torch.Tensor` of shape `(decoder_layers, decoder_attention_heads)`, *optional*):
-                Mask to nullify selected heads of the attention modules in encoder to avoid performing cross-attention
-                on hidden heads. Mask values selected in `[0, 1]`:
-
-                - 1 indicates the head is **not masked**,
-                - 0 indicates the head is **masked**.
-
-            past_key_values (`tuple(tuple(torch.FloatTensor))`, *optional*, returned when `use_cache=True` is passed or when `config.use_cache=True`):
-                Tuple of `tuple(torch.FloatTensor)` of length `config.n_layers`, with each tuple having 2 tensors of
-                shape `(batch_size, num_heads, sequence_length, embed_size_per_head)`) and 2 additional tensors of
-                shape `(batch_size, num_heads, encoder_sequence_length, embed_size_per_head)`.
-
-                Contains pre-computed hidden-states (key and values in the self-attention blocks and in the
-                cross-attention blocks) that can be used (see `past_key_values` input) to speed up sequential decoding.
-
-                If `past_key_values` are used, the user can optionally input only the last `decoder_input_ids` (those
-                that don't have their past key value states given to this model) of shape `(batch_size, 1)` instead of
-                all `decoder_input_ids` of shape `(batch_size, sequence_length)`. inputs_embeds (`torch.FloatTensor` of
-                shape `(batch_size, sequence_length, hidden_size)`, *optional*): Optionally, instead of passing
-                `input_ids` you can choose to directly pass an embedded representation. This is useful if you want more
-                control over how to convert `input_ids` indices into associated vectors than the model's internal
-                embedding lookup matrix.
-                NOTE: CHANGED for static caching --- now each tuple is (None, None, cur_position, Tensor, Tensor, 0)
-            output_attentions (`bool`, *optional*):
-                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
-                returned tensors for more detail.
-            output_hidden_states (`bool`, *optional*):
-                Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
-                for more detail.
-            return_dict (`bool`, *optional*):
-                Whether or not to return a [`~utils.ModelOutput`] instead of a plain tuple.
-        """
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        # retrieve input_ids and inputs_embeds
-        if input_ids is not None and inputs_embeds is not None:
-            raise ValueError("You cannot specify both decoder_input_ids and decoder_inputs_embeds at the same time")
-        elif input_ids is not None:
-            input_shape = input_ids.size()
-            input_ids = input_ids.view(-1, input_shape[-1])
-        elif inputs_embeds is not None:
-            input_shape = inputs_embeds.size()[:-1]
-        else:
-            raise ValueError("You have to specify either decoder_input_ids or decoder_inputs_embeds")
-
-        # past_key_values_length
-        past_key_values_length = past_key_values[0][0].shape[2] if past_key_values is not None else 0
-
-        if inputs_embeds is None:
-            inputs_embeds = self.embed_tokens(input_ids)
-
-        attention_mask = self._prepare_decoder_attention_mask(
-            attention_mask, input_shape, inputs_embeds, past_key_values_length
-        )
-
-        # embed positions
-        positions = self.embed_positions(input_ids, past_key_values_length=past_key_values_length)
-
-        hidden_states = inputs_embeds + positions
-        hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
-
-        # decoder layers
-        all_hidden_states = () if output_hidden_states else None
-        all_self_attns = () if output_attentions else None
-        all_cross_attentions = () if (output_attentions and encoder_hidden_states is not None) else None
-        next_decoder_cache = () if use_cache else None
-
-        # check if head_mask/cross_attn_head_mask has a correct number of layers specified if desired
-        for attn_mask, mask_name in zip([head_mask, cross_attn_head_mask], ["head_mask", "cross_attn_head_mask"]):
-            if attn_mask is not None:
-                assert attn_mask.size()[0] == (len(self.layers)), (
-                    f"The `{mask_name}` should be specified for {len(self.layers)} layers, but it is for"
-                    f" {head_mask.size()[0]}."
-                )
-        for idx, decoder_layer in enumerate(self.layers):
-            # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
-            if output_hidden_states:
-                all_hidden_states += (hidden_states,)
-            dropout_probability = random.uniform(0, 1)
-            if self.training and (dropout_probability < self.layerdrop):
-                continue
-
-            past_key_value = past_key_values[idx] if past_key_values is not None else None
-
-            if self.gradient_checkpointing and self.training:
-                if use_cache:
-                    logger.warning(
-                        "`use_cache = True` is incompatible with gradient checkpointing. Setting `use_cache ="
-                        " False`..."
-                    )
-                    use_cache = False
-
-                def create_custom_forward(module):
-                    def custom_forward(*inputs):
-                        # None for past_key_value
-                        return module(*inputs, output_attentions, use_cache)
-
-                    return custom_forward
-
-                layer_outputs = torch.utils.checkpoint.checkpoint(
-                    create_custom_forward(decoder_layer),
-                    hidden_states,
-                    attention_mask,
-                    encoder_hidden_states,
-                    None,  # encoder attention mask
-                    head_mask[idx] if head_mask is not None else None,
-                    cross_attn_head_mask[idx] if cross_attn_head_mask is not None else None,
-                    None,  # past_key_value
-                )
-            else:
-                layer_outputs = decoder_layer(
-                    hidden_states,
-                    attention_mask=attention_mask,
-                    encoder_hidden_states=encoder_hidden_states,
-                    layer_head_mask=(head_mask[idx] if head_mask is not None else None),
-                    cross_attn_layer_head_mask=(
-                        cross_attn_head_mask[idx] if cross_attn_head_mask is not None else None
-                    ),
-                    past_key_value=past_key_value,
-                    output_attentions=output_attentions,
-                    use_cache=use_cache,
-                )
-            hidden_states = layer_outputs[0]
-
-            if use_cache:
-                next_decoder_cache += (layer_outputs[3 if output_attentions else 1],)
-
-            if output_attentions:
-                all_self_attns += (layer_outputs[1],)
-
-                if encoder_hidden_states is not None:
-                    all_cross_attentions += (layer_outputs[2],)
-
-        hidden_states = self.layer_norm(hidden_states)
-        # add hidden states from the last decoder layer
-        if output_hidden_states:
-            all_hidden_states += (hidden_states,)
-
-        next_cache = next_decoder_cache if use_cache else None
-        if not return_dict:
-            return tuple(
-                v
-                for v in [hidden_states, next_cache, all_hidden_states, all_self_attns, all_cross_attentions]
-                if v is not None
-            )
-        return BaseModelOutputWithPastAndCrossAttentions(
-            last_hidden_state=hidden_states,
-            past_key_values=next_cache,
-            hidden_states=all_hidden_states,
-            attentions=all_self_attns,
-            cross_attentions=all_cross_attentions,
-        )
-
 
+@supports_kv_cache
 @register(WhisperForConditionalGeneration)
 class PipelinedWhisperForConditionalGeneration(WhisperForConditionalGeneration, PipelineMixin, IPUGenerationMixin):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
     def change_encoder_layer_class(self, restore: bool):
         """Changes the encoder layer class to avoid the dynamic 'if'
 
         Args:
             restore: whether to restore the encoder layers to their original version or not.
         """
         for layer in self.model.encoder.layers:
             layer.__class__ = WhisperEncoderLayer if restore else _WhisperEncoderLayerClamp
 
-    def change_encoder_and_decoder_classes(self, restore: bool):
-        """Changes the encoder and decoder classes to update their forward pass so that they use our custom versions of
-        _make_causal_mask and _expand_mask.
+    def change_decoder_class(self, restore: bool):
+        """Changes the decoder class to update the _prepare_decoder_attention_mask method.
 
         Args:
-            restore: whether to restore the encoder and decoder to their original version or not.
+            restore: whether to restore the decoder to its original version or not.
         """
-        self.model.encoder.__class__ = WhisperEncoder if restore else _WhisperEncoderWithCustomExpandMask
         self.model.decoder.__class__ = WhisperDecoder if restore else _WhisperDecoderWithCustomMakeCausalAndExpandMask
 
-    def parallelize(self, for_generation=False):
+    def change_decoder_positional_embedding(self, restore: bool):
+        """Changes the decoder positional embedding to support an optional static KV cache.
+
+        Args:
+            restore: whether to restore the decoder positional embedding to their original version or not.
+        """
+        position_embedding = self.model.decoder.embed_positions
+        self.model.decoder.embed_positions = (
+            position_embedding.to_model() if restore else IPUWhisperPositionalEmbedding.from_model(position_embedding)
+        )
+
+    def change_attention_class(self, restore=False, **kwargs):
+        """Change the attention layers to support a KV cache.
+
+        Args:
+            restore: whether to restore the attention layers to their original version or not.
+        """
+        use_cache = kwargs.get("use_cache", False)
+        batch_size = kwargs.get("batch_size", 1)
+        max_length = kwargs.get("max_length", 448)
+        num_beams = kwargs.get("num_beams", 1)
+        batch_serialization_factor = kwargs.get("batch_serialization_factor", 1)
+        sequence_serialization_factor = kwargs.get("sequence_serialization_factor", 1)
+
+        for encoder_layer in self.model.encoder.layers:
+            if restore:
+                encoder_layer.self_attn = encoder_layer.self_attn.to_model(WhisperAttention)
+                continue
+
+            encoder_layer.self_attn = IPUWhisperAttention.from_model(
+                encoder_layer.self_attn,
+                use_cache=False,
+                batch_serialization_factor=batch_serialization_factor,
+                sequence_serialization_factor=sequence_serialization_factor,
+            )
+
+        for decoder_layer in self.model.decoder.layers:
+            if restore:
+                decoder_layer.self_attn = decoder_layer.self_attn.to_model(WhisperAttention)
+                decoder_layer.encoder_attn = decoder_layer.encoder_attn.to_model(WhisperAttention)
+                continue
+
+            decoder_layer.self_attn = IPUWhisperAttention.from_model(
+                decoder_layer.self_attn,
+                use_cache=use_cache,
+                batch_size=batch_size,
+                max_length=max_length,
+                num_beams=num_beams,
+                dtype=decoder_layer.self_attn.k_proj.weight.dtype,
+            )
+            decoder_layer.encoder_attn = IPUWhisperAttention.from_model(
+                decoder_layer.encoder_attn,
+                use_cache=False,
+            )
+
+    def parallelize(self, for_generation=False, use_cache=False, **kwargs):
         super().parallelize()
 
         self.change_encoder_layer_class(restore=False)
-        self.change_encoder_and_decoder_classes(restore=False)
+        self.change_decoder_class(restore=False)
+        self.change_decoder_positional_embedding(restore=False)
+        self.change_attention_class(restore=False, use_cache=use_cache and for_generation, **kwargs)
+        self.change_lm_head_to_indexed_input_linear(restore=use_cache or not for_generation)
+        self.use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
+        self.set_on_device_generation_steps(kwargs.get("on_device_generation_steps", 0))
 
         logger.info("---------- Device Allocation -----------")
         logger.info("conv1, conv2, embed_positions  --> IPU 0")
         self.model.encoder.conv1 = poptorch.BeginBlock(self.model.encoder.conv1, "Conv1", ipu_id=0)
         self.model.encoder.conv2 = poptorch.BeginBlock(self.model.encoder.conv2, "Conv2", ipu_id=0)
         self.model.encoder.embed_positions = poptorch.BeginBlock(
             self.model.encoder.embed_positions, "Embed Positions", ipu_id=0
@@ -559,25 +438,42 @@
 
         for index, (layer, ipu) in enumerate(zip(self.model.decoder.layers, decoder_layer_ipu)):
             if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
                 self._hooks.append(recomputation_checkpoint(layer))
             self.model.decoder.layers[index] = poptorch.BeginBlock(layer, f"Decoder{index}", ipu_id=ipu)
             logger.info(f"Decoder {index:<2} --> IPU {ipu}")
 
-        last_ipu = ipu
-
-        logger.info(f"Head       --> IPU {last_ipu}")
-        logger.info("---------------------------------------")
         self.model.decoder.layer_norm = poptorch.BeginBlock(
-            self.model.decoder.layer_norm, "Decoder Layer Norm", ipu_id=last_ipu
+            self.model.decoder.layer_norm, "Decoder Layer Norm", ipu_id=ipu
         )
-        self.proj_out = poptorch.BeginBlock(self.proj_out, "Output Projection", ipu_id=last_ipu)
+
+        logger.info(f"Head       --> IPU 0")
+        logger.info("---------------------------------------")
+        self.proj_out = poptorch.BeginBlock(self.proj_out, "Output Projection", ipu_id=0)
         return self
 
     def deparallelize(self):
         super().deparallelize()
 
         self.change_encoder_layer_class(restore=True)
-        self.change_encoder_and_decoder_classes(restore=True)
+        self.change_decoder_class(restore=True)
+        self.change_decoder_positional_embedding(restore=True)
+        self.change_attention_class(restore=True)
+        self.change_lm_head_to_indexed_input_linear(restore=True)
+        self.set_on_device_generation_steps(0)
 
-        if self.proj_out.__class__ == _IndexedInputLinear:
-            self.proj_out = self.lm_head.wrapped_linear
+    def prepare_inputs_for_generation(
+        self, decoder_input_ids, past=None, use_cache=None, encoder_outputs=None, attention_mask=None, **kwargs
+    ):
+        # We don't use `past` for KV caching, and rely on `use_cache` instead.
+        beam_idx = None
+        if use_cache:
+            decoder_input_ids = decoder_input_ids[:, -1:]
+            beam_idx = kwargs.get("beam_idx", torch.arange(decoder_input_ids.shape[0], dtype=torch.long))
+
+        return {
+            "encoder_outputs": encoder_outputs,
+            "past_key_values": None,
+            "decoder_input_ids": decoder_input_ids,
+            "decoder_attention_mask": None,
+            "beam_idx": beam_idx,
+        }
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/pipelines/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 from typing import Any, List, Optional, Union
 
 import torch
 
 import poptorch
 import transformers.pipelines
-from optimum.graphcore import IPUConfig
-from optimum.graphcore.generation_utils import IPUGenerationMixin
-from optimum.graphcore.modeling_utils import IncompatibleIPUConfigError, to_pipelined
+from optimum.graphcore.generation.utils import IPUGenerationMixin
+from optimum.graphcore.ipu_configuration import IncompatibleIPUConfigError, IPUConfig
+from optimum.graphcore.modeling_utils import to_pipelined
 from transformers import (
     AudioClassificationPipeline,
     AutoFeatureExtractor,
     AutomaticSpeechRecognitionPipeline,
     AutoModelForAudioClassification,
     AutoModelForCausalLM,
     AutoModelForCTC,
@@ -214,29 +214,34 @@
 
     if isinstance(ipu_config, str):
         ipu_config = IPUConfig.from_pretrained(ipu_config)
     elif isinstance(ipu_config, dict):
         ipu_config = IPUConfig.from_dict(ipu_config)
     elif not isinstance(ipu_config, IPUConfig):
         raise ValueError("ipu_config must be an IPUConfig, string, or a dictionary.")
+
+    # So that IPUConfig returns inference versions of any parameters
+    # that are different in training and inference
+    ipu_config.eval()
+
     ipu_config.inference_device_iterations = 1
     # TODO: inference_replication_factor should be adaptive, especially for batching.
     ipu_config.inference_replication_factor = 1
     if not fp16:
         ipu_config.enable_half_partials = False
     try:
         model = to_pipelined(model, ipu_config, force=False)
         if model.config.is_encoder_decoder and isinstance(model, IPUGenerationMixin):
-            model.parallelize(for_generation=True)
+            model.parallelize(for_generation=task in SUPPORTED_GENERATION_TASKS)
         else:
             model.parallelize()
     except Exception as error:
         new_message = (
             "The model and ipu_config seem to be incompatible,"
-            " please try a different IPU config or customizing it for the model."
+            " please try a different IPU config or customize it for the model."
             f" The config provided is '{ipu_config_arg}'\n"
             f"{error}"
         )
         raise IncompatibleIPUConfigError(new_message) from error
     if fp16:
         model.half()
     opts = ipu_config.to_options(for_inference=True)
@@ -246,15 +251,15 @@
     if task not in SUPPORTED_GENERATION_TASKS:
         model = poptorch.inferenceModel(model.eval(), opts)
     return model
 
 
 def check_model_type(self, supported_models: Union[List[str], dict]):
     """
-    Check if the model class is in supported by the pipeline.
+    Check if the model class is supported by the pipeline.
 
     Args:
         supported_models (`List[str]` or `dict`):
             The list of models supported by the pipeline, or a dictionary with model class values.
     """
     if not isinstance(supported_models, list):  # Create from a model mapping
         supported_models_names = []
@@ -298,17 +303,17 @@
         task : The task, see docs for ``transformers.pipeline`` for supported options.
         model : A pre-trained model, see docs for ``transformers.pipeline`` for supported options.
         ipu_config : An IPU config, can either be the path to a model from the HuggingFace Hub
             which defines a ``ipu_config.json`` or a dictionary with the same options.
         tokenizer : The tokenizer, see docs for ``transformers.pipeline`` for supported options.
         feature_extractor : The feature extractor, see docs for ``transformers.pipeline`` for supported options.
         revision : Revision of the model.
-        use_auth_token : An authorization token to use for these calls to the hub.
-        pipeline_class : Override the Pipeline class defined by the task.
-        fp16 : Whether to use Float 16 or not.
+        use_auth_token : An authorization token to use for calls to the Hub.
+        pipeline_class : Override the `Pipeline` class defined by the task.
+        fp16 : If `True`, uses float16.
 
         **kwargs: Additional keyword arguments that are passed to the ``transformers.pipeline`` function
 
     Returns:
         The pipeline object for the specified task.
     """
 
@@ -317,15 +322,15 @@
             "Impossible to instantiate a pipeline without either a task or a model "
             "being specified. "
             "Please provide a task class or a model"
         )
     if task is None and model is not None:
         if not isinstance(model, str):
             raise RuntimeError(
-                "Inferring the task automatically requires to check the hub with a model_id defined as a `str`."
+                "Inferring the task automatically requires to check the Hub with a model_id defined as a `str`."
                 f"{model} is not a valid model_id."
             )
         task = get_task(model, use_auth_token)
 
     if task in TASK_ALIASES:
         task = TASK_ALIASES[task]
 
@@ -374,15 +379,15 @@
         if feature_extractor is None and load_feature_extractor:
             raise ValueError(
                 "If you pass a model as a poptorch._poplar_executor.PoplarExecutor, you must pass a feature extractor as well"
             )
     else:
         raise ValueError(
             f"""Model {model} is not supported. Please provide a valid model either as string, PreTrainedModel or
-            poptorch._poplar_executor.PoplarExecutor. You can also provide non model then a default one will be used"""
+            poptorch._poplar_executor.PoplarExecutor. If you don't provide a model, a default model will be used."""
         )
 
     # Upstream pipeline creation does not easily support loading these when an actual model
     # is provided, so we load them here.
     if tokenizer is None and load_tokenizer:
         tokenizer = AutoTokenizer.from_pretrained(model_id)
 
@@ -434,32 +439,32 @@
     # Auto padding for some tasks
     if "max_length" in SUPPORTED_TASKS[targeted_task]["default"]:
         default_max_length = SUPPORTED_TASKS[targeted_task]["default"]["max_length"]
         if targeted_task not in SUPPORTED_GENERATION_TASKS:
             kwargs["padding"] = kwargs.get("padding", "max_length")
             if kwargs.get("max_length") is None:
                 logger.warning(
-                    f"No padding arguments specified, so pad to {default_max_length} by default. "
+                    f"No padding arguments specified, so padding to {default_max_length} by default. "
                     f"Inputs longer than {default_max_length} will be truncated."
                     " To change this behaviour, pass the `padding='max_length'` and"
-                    "`max_length=<your desired input length>` arguments to the pipeline function"
+                    "`max_length=<your desired input length>` arguments to the pipeline function."
                 )
         kwargs["max_length"] = kwargs.get("max_length", default_max_length)
 
     if targeted_task in SUPPORTED_SEQ2SEQ_GENERATION_TASKS:
         default_max_input_length = SUPPORTED_TASKS[targeted_task]["default"]["max_input_length"]
         kwargs["max_input_length"] = kwargs.get("max_input_length", default_max_input_length)
         default_truncation = SUPPORTED_TASKS[targeted_task]["default"]["truncation"]
         kwargs["truncation"] = kwargs.get("truncation", default_truncation)
 
     # question-answering already has its own default padding length `max_seq_len` defined, so we just enable padding to max length.
     if targeted_task in {"question-answering"}:
         kwargs["padding"] = kwargs.get("padding", "max_length")
         logger.warning(
-            "No padding arguments specified, so pad to 384 by default. Inputs longer than 384 will be truncated."
+            "No padding arguments specified, so padding to 384 by default. Inputs longer than 384 will be truncated."
         )
 
     # Set pad_token for models that do not have pad_token
     if model.config.model_type in {"gpt2"}:
         tokenizer.pad_token = tokenizer.eos_token
         model.config.pad_token_id = model.config.eos_token_id
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/pipelines/fill_mask.py` & `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/fill_mask.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/pipelines/text2text_generation.py` & `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/pipelines/token_classification.py` & `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/pipelines/zero_shot_classification.py` & `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/trainer.py` & `optimum-graphcore-0.6.1/optimum/graphcore/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,74 +129,83 @@
 @dataclass
 class IPUTrainerState(TrainerState):
     start_time: float = -1.0
 
 
 class IPUTrainer:
     """
-    IPUTrainer is a simple but feature-complete training and eval loop  on Graphcore IPUs for PyTorch, optimized for
-    🤗 Transformers.
+    `IPUTrainer` is a simple but feature-complete training and evaluation
+      loop on Graphcore IPUs for PyTorch, optimized for 🤗 Transformers.
 
     Args:
         model ([`transformers.PreTrainedModel`] or `torch.nn.Module`, *optional*):
-            The model to train, evaluate or use for predictions. If not provided, a `model_init` must be passed.
+            The model to train, evaluate or use for predictions. If not provided, a `model_init` function must be passed.
 
             <Tip>
 
-            [`IPUTrainer`] is optimized to work with the [`transformers.PreTrainedModel`] provided by the 🤗 Transformers
-            library. You can still use your own models defined as `torch.nn.Module` as long as they work the same way as
+            [`IPUTrainer`] is optimized to work with the [`transformers.PreTrainedModel`] class provided by the 🤗 Transformers
+            library. You can still use your own models defined as `torch.nn.Module` as long as they work in the same way as
             the 🤗 Transformers models.
 
             </Tip>
 
         args ([`IPUTrainingArguments`], *optional*):
-            The arguments to tweak for training. Will default to a basic instance of [`IPUTrainingArguments`] with the
-            `output_dir` set to a directory named *tmp_trainer* in the current directory if not provided.
+            The arguments to tweak for training. Will default to a basic
+            instance of [`IPUTrainingArguments`] with `output_dir` set to a
+            directory named *tmp_trainer* in the current directory if not
+            provided.
         data_collator ([`transformers.data.data_collator.DataCollator`], *optional*):
-            The function to use to form a batch from a list of elements of `train_dataset` or `eval_dataset`. Will
-            default to [`transformers.data.default_data_collator`] if no `tokenizer` is provided, an instance of
+            The function to use to form a batch from a list of elements of
+            `train_dataset` or `eval_dataset`. Will default to
+            [`transformers.data.default_data_collator`] if no `tokenizer` is
+            provided, or an instance of
             [`~transformers.data.DataCollatorWithPadding`] otherwise.
         train_dataset (`torch.utils.data.Dataset` or `torch.utils.data.IterableDataset`, *optional*):
-            The dataset to use for training. If it is a [`~datasets.Dataset`], columns not accepted by the
+            The dataset to use for training. If it is a [`~datasets.Dataset`]
+            dataset, the columns not accepted by the
             `model.forward()` method are automatically removed.
 
-            Note that if it's a `torch.utils.data.IterableDataset` with some randomization and you are training in a
-            distributed fashion, your iterable dataset should either use a internal attribute `generator` that is a
-            `torch.Generator` for the randomization that must be identical on all processes (and the Trainer will
-            manually set the seed of this `generator` at each epoch) or have a `set_epoch()` method that internally
-            sets the seed of the RNGs used.
+            Note that if it's a `torch.utils.data.IterableDataset` dataset with
+            some randomization and you are training in a distributed fashion,
+            your iterable dataset should either use an internal attribute
+            `generator` that is a `torch.Generator` object for the randomization that
+            must be identical on all processes (and the trainer will manually
+            set the seed of this `generator` at each epoch) or have a
+            `set_epoch()` method that internally sets the seed of the RNGs used.
         eval_dataset (Union[`torch.utils.data.Dataset`, Dict[str, `torch.utils.data.Dataset`]), *optional*):
-             The dataset to use for evaluation. If it is a [`~datasets.Dataset`], columns not accepted by the
+             The dataset to use for evaluation. If it is a [`~datasets.Dataset`] dataset, the columns not accepted by the
              `model.forward()` method are automatically removed. If it is a dictionary, it will evaluate on each
              dataset prepending the dictionary key to the metric name.
         tokenizer ([`transformers.PreTrainedTokenizerBase`], *optional*):
-            The tokenizer used to preprocess the data. If provided, will be used to automatically pad the inputs the
-            maximum length when batching inputs, and it will be saved along the model to make it easier to rerun an
-            interrupted training or reuse the fine-tuned model.
+            The tokenizer used to preprocess the data. If provided, it will be
+            used to automatically pad the inputs to the maximum length when
+            batching inputs, and it will be saved along the model to make it
+            easier to rerun an interrupted training or reuse the fine-tuned
+            model.
         model_init (`Callable[[], transformers.PreTrainedModel]`, *optional*):
             A function that instantiates the model to be used. If provided, each call to [`IPUTrainer.train`] will start
             from a new instance of the model as given by this function.
 
-            The function may have zero argument, or a single one containing the optuna/Ray Tune/SigOpt trial object, to
+            The function may have no arguments, or a single argument containing the optuna/Ray Tune/SigOpt trial object, to
             be able to choose different architectures according to hyper parameters (such as layer count, sizes of
-            inner layers, dropout probabilities etc). **Note: this feature is not supported for now.**
+            inner layers and dropout probabilities). **Note: this feature is not supported for now.**
 
         compute_metrics (`Callable[[~transformers.trainer_utils.EvalPrediction], Dict]`, *optional*):
             The function that will be used to compute metrics at evaluation. Must take a
-            [`~transformers.trainer_utils.EvalPrediction`] and return a dictionary string to metric values.
+            [`~transformers.trainer_utils.EvalPrediction`] and return a dictionary of strings to metric values.
         callbacks (List of [`transformers.trainer_callback.TrainerCallback`], *optional*):
             A list of callbacks to customize the training loop. Will add those to the list of default callbacks
             detailed in [here](callback).
 
             If you want to remove one of the default callbacks used, use the [`Trainer.remove_callback`] method.
         optimizers (`Tuple[torch.optim.Optimizer, torch.optim.lr_scheduler.LambdaLR]`, *optional*): A tuple
             containing the optimizer and the scheduler to use. Will default to an instance of `poptorch.AdamW` on your model
             and a scheduler given by [`get_linear_schedule_with_warmup`] controlled by `args`.
         preprocess_logits_for_metrics (`Callable[[torch.Tensor, torch.Tensor], torch.Tensor]`, *optional*):
-            A function that preprocess the logits right before caching them at each evaluation step. Must take two
+            A function that preprocesses the logits right before caching them at each evaluation step. Must take two
             tensors, the logits and the labels, and return the logits once processed as desired. The modifications made
             by this function will be reflected in the predictions received by `compute_metrics`.
 
             Note that the labels (second parameter) will be `None` if the dataset does not have them.
     """
 
     from transformers.trainer_pt_utils import log_metrics, metrics_format, save_metrics, save_state
@@ -238,15 +247,15 @@
         logging.set_verbosity(log_level)
 
         # force device and distributed setup init explicitly
         args._setup_devices
 
         if model is None:
             if model_init is not None:
-                raise RuntimeError("`model_init` is not supported by the `IPUTrainer` yet")
+                raise RuntimeError("`model_init` is not supported by `IPUTrainer` yet")
             else:
                 raise RuntimeError("`IPUTrainer` requires either a `model` or `model_init` argument")
         else:
             if model_init is not None:
                 warnings.warn(
                     "`IPUTrainer` requires either a `model` or `model_init` argument, but not both. "
                     "`model_init` will overwrite your model when calling the `train` method. This will become a fatal error in the next release.",
@@ -259,28 +268,36 @@
         self.data_collator = data_collator if data_collator is not None else default_collator
         # If no eval_data_collator is specified then use the train data_collator
         self.eval_data_collator = eval_data_collator if eval_data_collator is not None else self.data_collator
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.tokenizer = tokenizer
 
-        self.ipu_config = copy.deepcopy(ipu_config).for_pod_type(self.args.pod_type)
+        self.ipu_config = copy.deepcopy(ipu_config)
+        # set replication factor using n_ipu (can be overruled by ipu_config_overrides)
+        if (n_ipu := self.args.n_ipu) is not None:
+            if self.ipu_config.replication_factor > 1 or self.ipu_config.inference_replication_factor > 1:
+                warnings.warn(
+                    "IPUTrainer is overwriting the replication factors set in self.ipu_config because `--n_ipu` was provided."
+                )
+            self.ipu_config.replication_factor = n_ipu // self.ipu_config.ipus_per_replica
+            self.ipu_config.inference_replication_factor = n_ipu // self.ipu_config.inference_ipus_per_replica
         if self.ipu_config.replication_factor > 1 or self.ipu_config.inference_replication_factor > 1:
             os.environ["TOKENIZERS_PARALLELISM"] = "true"
         if args.ipu_config_overrides:
             logger.info(f"Overriding IPU config: {args.ipu_config_overrides}")
             self.ipu_config.update_from_string(args.ipu_config_overrides)
         self.ipu_config.seed = self.args.seed
         self.opts = self.ipu_config.to_options(compile_only=args.compile_only)
         self.eval_opts = self.ipu_config.to_options(for_inference=True, compile_only=args.compile_only)
 
         # If batch axis padding enabled, wrap train/eval data collators with `pad_on_batch_axis` wrapper
         if self.args.pad_on_batch_axis:
             logger.info(
-                "Padding on batch axis enabled, each batch feeded to the compiled model during training will have the proper size"
+                "Padding on batch axis enabled. Each batch fed to the compiled model during training will have the proper size"
             )
             if self.args.do_train:
                 data_collator_wrapper = pad_on_batch_axis(
                     self.args.per_device_train_batch_size * self.ipu_config.batch_size_factor()
                 )
                 self.data_collator = data_collator_wrapper(self.data_collator)
 
@@ -327,24 +344,24 @@
         if self.args.push_to_hub:
             self.init_git_repo()
 
         if self.args.should_save:
             os.makedirs(self.args.output_dir, exist_ok=True)
 
         if not callable(self.data_collator) and callable(getattr(self.data_collator, "collate_batch", None)):
-            raise ValueError("The `data_collator` should be a simple callable (function, class with `__call__`).")
+            raise ValueError("`data_collator` should be a simple callable (function, class with `__call__`).")
 
         if not callable(self.eval_data_collator) and callable(getattr(self.eval_data_collator, "collate_batch", None)):
-            raise ValueError("The `eval_data_collator` should be a simple callable (function, class with `__call__`).")
+            raise ValueError("`eval_data_collator` should be a simple callable (function, class with `__call__`).")
 
         if args.max_steps > 0:
-            logger.info("max_steps is given, it will override any value given in num_train_epochs")
+            logger.info("max_steps is given. It will override any value given in num_train_epochs")
 
         if train_dataset is not None and not isinstance(train_dataset, collections.abc.Sized) and args.max_steps <= 0:
-            raise ValueError("train_dataset does not implement __len__, max_steps has to be specified")
+            raise ValueError("train_dataset does not implement __len__. max_steps has to be specified")
 
         self._signature_columns = None
 
         # Label smoothing
         if self.args.label_smoothing_factor != 0:
             self.label_smoother = LabelSmoother(epsilon=self.args.label_smoothing_factor)
         else:
@@ -364,15 +381,14 @@
         # very last
         self._memory_tracker.stop_and_update_metrics()
 
         # If compile-only then compile and exit
         if args.compile_only:
             logger.info("Called with compile_only=True. Compiling models then exiting.")
             if args.do_train:
-                self.optimizer = self.create_optimizer()
                 train_dl = self.get_train_dataloader()
                 model = self.wrap_model(self.model)
                 self.compile_model(model, next(iter(train_dl)), log=True)
             if args.do_eval:
                 # Same thing with _wrap_and_compile_for_evaluation
                 eval_dl = self.get_eval_dataloader()
                 model = self._wrap_and_compile_model_for_evaluation(eval_dl, False)
@@ -390,18 +406,18 @@
 
         Args:
             optimizer (`torch.optim.Optimizer`):
                 The PyTorch optimizer to convert.
             model (`[transformers.PreTrainedModel]` or `torch.nn.Module`):
                 The original model the optimizer has parameter references to.
             pipelined_model (`[transformers.PreTrainedModel] or `torch.nn.Module`):
-                The pipelined version of the model, its parameters will be used by the poptorch optimizer.
+                The pipelined version of the model. Its parameters will be used by the PopTorch optimizer.
 
         Returns:
-            `poptorch.optim.Optimizer`: The converted poptorch optimizer.
+            `poptorch.optim.Optimizer`: The converted PopTorch optimizer.
         """
         first_order_type = torch.float32 if self.args.fp32 else torch.float16
         optimizer_kwargs = {
             "loss_scaling": self.args.loss_scaling,
             "accum_type": first_order_type,
             "first_order_momentum_accum_type": first_order_type,
             "second_order_momentum_accum_type": torch.float32,
@@ -414,18 +430,18 @@
             optim.Adam: (poptorch.optim.Adam, {"max_grad_norm": self.args.max_grad_norm, **optimizer_kwargs}),
             optim.AdamW: (poptorch.optim.AdamW, {"max_grad_norm": self.args.max_grad_norm, **optimizer_kwargs}),
             optim.RMSprop: (poptorch.optim.RMSprop, optimizer_kwargs),
         }
         self.args.max_grad_norm = max_grad_norm
         poptorch_optimizer_cls, kwargs = pytorch_to_poptorch_mapping.get(optimizer.__class__, (None, {}))
         if poptorch_optimizer_cls is None:
-            raise KeyError(f"Could not find a poptorch counterpart for optimizer {optimizer.__class__.__name__}")
+            raise KeyError(f"Could not find a PopTorch counterpart for optimizer {optimizer.__class__.__name__}")
 
-        # Some dummy value that should be overriden by the real value with .load_state_dict, using some absurd value to
-        # make clear if the value is not properly overriden.
+        # Some dummy value that should be overridden by the real value with .load_state_dict, using some absurd value to
+        # make clear if the value is not properly overridden.
         dummy_lr = 1e4
         poptorch_optimizer = poptorch_optimizer_cls(optimizer.param_groups, lr=dummy_lr, **kwargs)
         poptorch_optimizer.load_state_dict({"ipu_state": None, "ipu_param": None, **optimizer.state_dict()})
 
         # Currently poptorch_optimizer contains references to the original model parameters, so we need to change those
         # to references to the pipelined model parameters.
         id2name = {id(param): name for name, param in model.named_parameters()}
@@ -445,17 +461,17 @@
         """
         Compiles the model with PopTorch.
 
         Args:
             model (`poptorch.PoplarExecutor`):
                 The model to compile (already wrapped).
             sample_batch (`Dict[str, torch.Tensor]` or `Tuple[torch.Tensor]`):
-                The inputs to use the compilation, this will set the input shapes that the compiled model can accept.
+                The inputs to use for the compilation. This will set the input shapes that the compiled model can accept.
             log (`bool`, *optional*, defaults to `False`):
-                Whether to log that compilation is happening or not.
+                If `True`, logs that the compilation is in progress.
         """
         # Skipping compilation if the model was already compiled.
         if model.isCompiled():
             return
         if log:
             logger.info("Compiling Model...")
         sample_batch = self._prepare_inputs(sample_batch)
@@ -470,42 +486,42 @@
 
     def add_callback(self, callback):
         """
         Adds a callback to the current list of [`~transformer.TrainerCallback`].
 
         Args:
            callback (`type` or [`~transformer.TrainerCallback`]):
-               A [`~transformer.TrainerCallback`] class or an instance of a [`~transformer.TrainerCallback`]. In the
+               A [`~transformer.TrainerCallback`] class or an instance of [`~transformer.TrainerCallback`]. In the
                first case, will instantiate a member of that class.
         """
         self.callback_handler.add_callback(callback)
 
     def pop_callback(self, callback):
         """
         Removes a callback from the current list of [`~transformer.TrainerCallback`] and returns it.
 
         If the callback is not found, returns `None` (and no error is raised).
 
         Args:
            callback (`type` or [`~transformer.TrainerCallback`]):
-               A [`~transformer.TrainerCallback`] class or an instance of a [`~transformer.TrainerCallback`]. In the
+               A [`~transformer.TrainerCallback`] class or an instance of [`~transformer.TrainerCallback`]. In the
                first case, will pop the first member of that class found in the list of callbacks.
 
         Returns:
-            [`~transformer.TrainerCallback`]: The callback removed, if found.
+            [`~transformer.TrainerCallback`]: The callback was removed, if found.
         """
         return self.callback_handler.pop_callback(callback)
 
     def remove_callback(self, callback):
         """
         Removes a callback from the current list of [`~transformer.TrainerCallback`].
 
         Args:
            callback (`type` or [`~transformer.TrainerCallback`]):
-               A [`~transformer.TrainerCallback`] class or an instance of a [`~transformer.TrainerCallback`]. In the
+               A [`~transformer.TrainerCallback`] class or an instance of [`~transformer.TrainerCallback`]. In the
                first case, will remove the first member of that class found in the list of callbacks.
         """
         self.callback_handler.remove_callback(callback)
 
     def _set_signature_columns_if_needed(self):
         if self._signature_columns is None:
             # Inspect model forward signature to keep only the arguments it accepts.
@@ -597,15 +613,15 @@
         else:
             return RandomSampler(self.train_dataset)
 
     def get_train_dataloader(self) -> poptorch.DataLoader:
         """
         Returns the training `poptorch.DataLoader`.
 
-        Will use no sampler if `train_dataset` does not implement `__len__`, a random sampler (adapted to distributed
+        Will not use a sampler if `train_dataset` does not implement `__len__` and will use a random sampler (adapted to distributed
         training if necessary) otherwise.
 
         Subclass and override this method if you want to inject some custom behavior.
         """
         if self.train_dataset is None:
             raise ValueError("Trainer: training requires a train_dataset.")
 
@@ -661,15 +677,15 @@
         """
         Returns the evaluation `poptorch.DataLoader`.
 
         Subclass and override this method if you want to inject some custom behavior.
 
         Args:
             eval_dataset (`torch.utils.data.Dataset`, *optional*):
-                If provided, will override `self.eval_dataset`. If it is a [`~datasets.Dataset`], columns not accepted
+                If provided, will override `self.eval_dataset`. If it is a [`~datasets.Dataset`] dataset, the columns not accepted
                 by the `model.forward()` method are automatically removed. It must implement `__len__`.
         """
         poptorch_specific_kwargs = {
             "auto_distributed_partitioning": not isinstance(eval_dataset, torch.utils.data.IterableDataset),
             "mode": DataLoaderMode.Sync,
             "worker_init_fn": _WorkerInit(123),
         }
@@ -713,15 +729,15 @@
         """
         Returns the test `poptorch.DataLoader`.
 
         Subclass and override this method if you want to inject some custom behavior.
 
         Args:
             test_dataset (`torch.utils.data.Dataset`, *optional*):
-                The test dataset to use. If it is a [`~datasets.Dataset`], columns not accepted by the
+                The test dataset to use. If it is a [`~datasets.Dataset`] dataset, the columns not accepted by the
                 `model.forward()` method are automatically removed. It must implement `__len__`.
         """
         poptorch_specific_kwargs = {
             "auto_distributed_partitioning": not isinstance(test_dataset, torch.utils.data.IterableDataset),
             "mode": DataLoaderMode.Sync,
             "worker_init_fn": _WorkerInit(123),
         }
@@ -755,29 +771,29 @@
             drop_last=self.args.dataloader_drop_last,
             pin_memory=self.args.dataloader_pin_memory,
             **poptorch_specific_kwargs,
         )
 
     def create_optimizer_and_scheduler(self, num_training_steps: int):
         """
-        Setup the optimizer and the learning rate scheduler.
+        Sets up the optimizer and the learning rate scheduler.
 
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
-        Trainer's init through `optimizers`, or subclass and override this method (or `create_optimizer` and/or
+        trainer's init through `optimizers`, or subclass and override this method (or `create_optimizer` and/or
         `create_scheduler`) in a subclass.
         """
         self.create_optimizer()
         self.create_scheduler(num_training_steps=num_training_steps, optimizer=self.optimizer)
 
     def create_optimizer(self):
         """
-        Setup the optimizer.
+        Sets up the optimizer.
 
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
-        Trainer's init through `optimizers`, or subclass and override this method in a subclass.
+        trainer's init through `optimizers`, or subclass and override this method in a subclass.
         """
         if self.optimizer is None:
             decay_parameters = get_parameter_names(self.model, [nn.LayerNorm])
             decay_parameters = {name for name in decay_parameters if "bias" not in name}
             if self.args.lamb or self.args.lamb_no_bias_correction:
                 bias_parameters = {n for n, _ in self.model.named_parameters() if "bias" in n}
                 optimizer_grouped_parameters = [
@@ -840,19 +856,19 @@
 
             self.optimizer.variable_attrs.markAsConstant("weight_decay")
 
         return self.optimizer
 
     def create_scheduler(self, num_training_steps: int, optimizer: torch.optim.Optimizer = None):
         """
-        Setup the scheduler. The optimizer of the trainer must have been set up either before this method is called or
+        Sets up the scheduler. The optimizer of the trainer must have been set up either before this method is called or is
         passed as an argument.
 
         Args:
-            num_training_steps (int): The number of training steps to do.
+            num_training_steps (int): The number of training steps to execute.
         """
         optimizer = self.optimizer if optimizer is None else optimizer
         if self.lr_scheduler is None:
             self.lr_scheduler = get_scheduler(
                 self.args.lr_scheduler_type,
                 optimizer=optimizer,
                 num_warmup_steps=self.args.get_warmup_steps(num_training_steps),
@@ -861,67 +877,75 @@
             optimizer._step_count = 1
         elif isinstance(self.lr_scheduler, functools.partial):
             self.lr_scheduler = self.lr_scheduler(optimizer)
         return self.lr_scheduler
 
     def num_examples(self, dataloader: poptorch.DataLoader) -> int:
         """
-        Helper to get number of samples in a `poptorch.DataLoader` by accessing its dataset. When
-        dataloader.dataset does not exist or has no length, estimates as best it can
+        Returns the number of samples in a `poptorch.DataLoader` object by accessing its dataset. When
+        `poptorch.DataLoader.dataset` does not exist or has no length, returns the best estimate best it can.
         """
         return len(dataloader.dataset)
 
     def wrap_model(self, model: Union[PreTrainedModel, PoplarExecutor], training=True) -> PoplarExecutor:
         """
         Wraps a model for PopTorch, either for training or for inference.
 
         Args:
             model ([`transformers.PreTrainedModel`] or `poptorch.PoplarExecutor`):
                 The model to wrap.
             training (`bool`, *optional*, defaults to `True`):
-                Whether to wrap the model for training or not.
+                If `True`, wraps the model for training. If `False`, does not
+                wrap the model for training.
 
         Returns:
             `poptorch.PoplarExecutor`: The wrapped model.
 
         """
         wrapped = None
         if isinstance(model, PoplarExecutor):
             wrapped = model
         elif training:
             if self.training_model is None:
+                model.deparallelize()
+                model.ipu_config.train()
+                model.parallelize()
+                self.create_optimizer()
                 self.training_model = poptorch.trainingModel(
                     model.train(), options=self.opts, optimizer=self.optimizer
                 )
             wrapped = self.training_model
         else:
             if self.inference_model is None:
+                model.deparallelize()
+                model.ipu_config.eval()
+                model.parallelize()
                 self.inference_model = poptorch.inferenceModel(model.eval(), options=self.eval_opts)
             wrapped = self.inference_model
 
         # Attaching to device when the model that is being access was already compiled but detached from previous loop.
         if wrapped.isCompiled() and not wrapped.isAttachedToDevice():
             wrapped.attachToDevice()
         return wrapped
 
     def _detach_training_model(self):
         """
-        Detach training model from IPUs
+        Detach the training model from IPUs.
         """
         self.training_model.detachFromDevice()
 
     def _detach_inference_model(self):
         """
-        Detach inference model from IPUs
+        Detach the inference model from IPUs.
         """
         self.inference_model.detachFromDevice()
 
     def _reattach_training_model(self):
         """
-        Reattach training model from IPUs
+        Reattach the training model to IPUs.
         """
         self.training_model.attachToDevice()
 
     def train(
         self,
         resume_from_checkpoint: Optional[Union[str, bool]] = None,
         trial: Union["optuna.Trial", Dict[str, Any]] = None,
@@ -929,25 +953,28 @@
         **kwargs,
     ):
         """
         Main training entry point.
 
         Args:
             resume_from_checkpoint (`str` or `bool`, *optional*):
-                If a `str`, local path to a saved checkpoint as saved by a previous instance of [`IPUTrainer`]. If a
-                `bool` and equals `True`, load the last checkpoint in *args.output_dir* as saved by a previous instance
-                of [`Trainer`]. If present, training will resume from the model/optimizer/scheduler states loaded here.
+                Indicates that training will resume from the model, optimizer or
+                scheduler states loaded here. If `str`, local path to a saved
+                checkpoint as saved by a previous instance of [`IPUTrainer`]. If
+                `bool` and `True`, load the last checkpoint in *args.output_dir*
+                as saved by a previous instance of [`IPUTrainer`].
             trial (`optuna.Trial` or `Dict[str, Any]`, *optional*):
-                The trial run or the hyperparameter dictionary for hyperparameter search.
-                **Note**: Feature not supported for now.
+                The trial run or the hyperparameter dictionary for a
+                hyperparameter search. **Note**: Feature not supported.
             ignore_keys_for_eval (`List[str]`, *optional*)
-                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
-                gathering predictions for evaluation during the training.
+                A list of keys in the output of your model (if it is a
+                dictionary) that should be ignored when gathering predictions
+                for evaluation during the training.
             kwargs:
-                Additional keyword arguments used to hide deprecated arguments
+                Additional keyword arguments used to hide deprecated arguments.
         """
         if resume_from_checkpoint is False:
             resume_from_checkpoint = None
 
         # memory metrics - must set up as early as possible
         self._memory_tracker.start()
 
@@ -1022,24 +1049,24 @@
                 "args.max_steps must be set to a positive value if dataloader does not have a length, was"
                 f" {args.max_steps}"
             )
 
         if DebugOption.UNDERFLOW_OVERFLOW in self.args.debug:
             debug_overflow = DebugUnderflowOverflow(self.model)  # noqa
 
-        self.create_optimizer_and_scheduler(num_training_steps=max_steps)
-
         self.state = IPUTrainerState()
         if trial is not None:
             raise ValueError("Hyperparameter tuning is not supported by the IPUTrainer.")
             trial = None
         self.state.is_hyper_param_search = trial is not None
 
         self.training_model = self.wrap_model(self.model)
 
+        self.create_scheduler(num_training_steps=max_steps)
+
         # TODO: handle optimizer and scheduler creation
         # if delay_optimizer_creation:
         #     self.create_optimizer_and_scheduler(num_training_steps=max_steps)
 
         # Check if saved optimizer or scheduler states exist
         self._load_optimizer_and_scheduler(resume_from_checkpoint)
 
@@ -1049,18 +1076,20 @@
         num_examples = (
             self.num_examples(train_dataloader)
             if has_length(train_dataloader)
             else total_train_batch_size * args.max_steps
         )
         logger.info("***** Running training *****")
         logger.info(f"  Num examples = {num_examples}")
-        logger.info(f"  Num Epochs = {num_train_epochs}")
+        logger.info(f"  Num epochs = {num_train_epochs}")
         logger.info(f"  Instantaneous batch size per device = {batch_size}")
-        logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size}")
-        logger.info(f"  Gradient Accumulation steps = {self.ipu_config.gradient_accumulation_steps}")
+        logger.info(
+            f"  Total training batch size (w. parallel, distributed & accumulation) = {total_train_batch_size}"
+        )
+        logger.info(f"  Gradient accumulation steps = {self.ipu_config.gradient_accumulation_steps}")
         logger.info(f"  Total optimization steps = {max_steps}")
 
         self.state.epoch = 0
         start_time = time.time()
         epochs_trained = 0
         steps_trained_in_current_epoch = 0
         steps_trained_progress_bar = None
@@ -1257,15 +1286,15 @@
         if os.path.isfile(os.path.join(resume_from_checkpoint, CONFIG_NAME)):
             config = PretrainedConfig.from_json_file(os.path.join(resume_from_checkpoint, CONFIG_NAME))
             checkpoint_version = config.transformers_version
             if checkpoint_version is not None and checkpoint_version != __version__:
                 logger.warning(
                     f"You are resuming training from a checkpoint trained with {checkpoint_version} of "
                     f"Transformers but your current version is {__version__}. This is not recommended and could "
-                    "yield to errors or unwanted behaviors."
+                    "yield to errors or unwanted behavior."
                 )
 
         if os.path.isfile(os.path.join(resume_from_checkpoint, WEIGHTS_NAME)):
             # We load the model state dict on the CPU to avoid an OOM error.
             state_dict = torch.load(os.path.join(resume_from_checkpoint, WEIGHTS_NAME), map_location="cpu")
             # workaround for FSDP bug https://github.com/pytorch/pytorch/issues/82963
             # which takes *args instead of **kwargs
@@ -1279,15 +1308,15 @@
         best_model_path = os.path.join(self.state.best_model_checkpoint, WEIGHTS_NAME)
         if os.path.exists(best_model_path):
             # We load the model state dict on the CPU to avoid an OOM error.
             state_dict = torch.load(best_model_path, map_location="cpu")
             self._load_state_dict_in_model(state_dict)
         else:
             logger.warning(
-                f"Could not locate the best model at {best_model_path}, if you are running a distributed training "
+                f"Could not locate the best model at {best_model_path}. If you are running a distributed training "
                 "on multiple nodes, you should activate `--save_on_each_node`."
             )
 
     def _load_state_dict_in_model(self, state_dict):
         self.model.deparallelize()
         load_result = self.model.load_state_dict(state_dict, strict=False)
         self.model.parallelize()
@@ -1358,23 +1387,23 @@
 
         # TODO: validate that.
         local_rank = -1
         if local_rank != -1:
             rng_file = os.path.join(checkpoint, f"rng_state_{local_rank}.pth")
             if not os.path.isfile(os.path.join(checkpoint, rng_file)):
                 logger.info(
-                    f"Didn't find an RNG file for process {local_rank}, if you are resuming a training that "
+                    f"Didn't find an RNG file for process {local_rank}. If you are resuming a training that "
                     "wasn't launched in a distributed fashion, reproducibility is not guaranteed."
                 )
                 return
         else:
             rng_file = os.path.join(checkpoint, "rng_state.pth")
             if not os.path.isfile(rng_file):
                 logger.info(
-                    "Didn't find an RNG file, if you are resuming a training that was launched in a distributed "
+                    "Didn't find an RNG file. If you are resuming a training that was launched in a distributed "
                     "fashion, reproducibility is not guaranteed."
                 )
                 return
 
         checkpoint_rng_state = torch.load(rng_file)
         random.setstate(checkpoint_rng_state["python"])
         np.random.set_state(checkpoint_rng_state["numpy"])
@@ -1451,15 +1480,15 @@
                 self.lr_scheduler.load_state_dict(torch.load(os.path.join(checkpoint, SCHEDULER_NAME)))
             reissue_pt_warnings(caught_warnings)
 
             self.training_model.setOptimizer(self.optimizer)
 
     def log(self, logs: Dict[str, float]) -> None:
         """
-        Log `logs` on the various objects watching training.
+        Log `logs` on the various objects watching the training.
 
         Subclass and override this method to inject custom behavior.
 
         Args:
             logs (`Dict[str, float]`):
                 The values to log.
         """
@@ -1468,68 +1497,81 @@
 
         output = {**logs, **{"step": self.state.global_step}}
         self.state.log_history.append(output)
         self.control = self.callback_handler.on_log(self.args, self.state, self.control, logs)
 
     def _prepare_input(self, data: Union[torch.Tensor, Any]) -> Union[torch.Tensor, Any]:
         """
-        Prepares one `data` before feeding it to the model, be it a tensor or a nested list/dictionary of tensors.
+        Prepares a single data sample before feeding it to the model.
+
+        The data sample can be it a tensor or a nested list or dictionary of tensors.
         """
         if isinstance(data, dict):
             return type(data)(**{k: self._prepare_input(v) for k, v in data.items()})
         elif isinstance(data, (tuple, list)):
             return type(data)(self._prepare_input(v) for v in data)
         elif isinstance(data, torch.Tensor):
             return data
         return data
 
     def _prepare_inputs(self, inputs: Dict[str, Union[torch.Tensor, Any]]) -> Dict[str, Union[torch.Tensor, Any]]:
         """
-        Prepare `inputs` before feeding them to the model, converting them to tensors if they are not already and
-        handling potential state.
+        Prepares inputs before feeding them to the model.
+
+        This method converts the inputs to tensors if they are not already tensors and handles the potential state.
         """
         inputs = self._prepare_input(inputs)
         if len(inputs) == 0:
             raise ValueError(
-                "The batch received was empty, your model won't be able to train on it. Double-check that your "
-                f"training dataset contains keys expected by the model: {','.join(self._signature_columns)}."
+                "The batch received was empty. Your model won't be able to train on it. Double-check that your "
+                f"training dataset contains the keys expected by the model: {','.join(self._signature_columns)}."
             )
         if self.args.past_index >= 0 and self._past is not None:
             inputs["mems"] = self._past
 
         return inputs
 
     def training_step(
         self, model: poptorch.PoplarExecutor, inputs: Dict[str, Union[torch.Tensor, Any]]
     ) -> torch.Tensor:
         """
-        Perform a training step on a batch of inputs.
+        Performs a training step on a batch of inputs.
 
         Subclass and override to inject custom behavior.
 
         Args:
             model (`poptorch.PoplarExecutor`):
                 The model to train.
             inputs (`Dict[str, Union[torch.Tensor, Any]]`):
                 The inputs and targets of the model.
 
                 The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
                 argument `labels`. Check your model's documentation for all accepted arguments.
 
         Return:
-            `torch.Tensor`: The tensor with training loss on this batch.
+            `torch.Tensor`: The tensor with the training loss on this batch.
         """
         inputs = self._prepare_inputs(inputs)
         loss = self.compute_loss(model, inputs)
         loss = loss.mean()
         return loss
 
     def compute_loss(self, model, inputs, return_outputs=False):
         """
-        How the loss is computed by `IPUTrainer`. By default, all models return the loss in the first element.
+        Computes the loss on a batch of training inputs.
+
+        Args:
+            model:
+                The model to train.
+            inputs:
+                The inputs and targets of the model.
+            return_outputs (defaults to `False`):
+                If `True`, returns the outputs with the loss. If `False`, only returns the loss.
+
+        By default, all models return the loss in the first element.
 
         Subclass and override for custom behavior.
         """
         if self.label_smoother is not None and "labels" in inputs:
             labels = inputs.pop("labels")
         else:
             labels = None
@@ -1554,17 +1596,17 @@
 
     def is_world_process_zero(self) -> bool:
         # Needed only because log_metrics use it.
         return True
 
     def save_model(self, output_dir: Optional[str] = None, _internal_call: bool = False):
         """
-        Will save the model, so you can reload it using `from_pretrained()`.
+        Saves the model, so you can reload it using `from_pretrained()`.
 
-        Will only save from the main process.
+        Will only save the model from the main process.
         """
         if output_dir is None:
             output_dir = self.args.output_dir
 
         if self.args.should_save:
             self._save(output_dir)
 
@@ -1663,31 +1705,31 @@
     def evaluate(
         self,
         eval_dataset: Optional[Dataset] = None,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "eval",
     ) -> Dict[str, float]:
         """
-        Run evaluation and returns metrics.
+        Runs an evaluation and returns metrics.
 
-        The calling script will be responsible for providing a method to compute metrics, as they are task-dependent
+        The calling script will be responsible for providing a method to compute the metrics, as they are task-dependent
         (pass it to the init `compute_metrics` argument).
 
         You can also subclass and override this method to inject custom behavior.
 
         Args:
             eval_dataset (`Dataset`, *optional*):
-                Pass a dataset if you wish to override `self.eval_dataset`. If it is a [`~datasets.Dataset`], columns
+                Pass a dataset if you wish to override `self.eval_dataset`. If it is a [`~datasets.Dataset`] dataset, the columns
                 not accepted by the `model.forward()` method are automatically removed. It must implement the `__len__`
                 method.
             ignore_keys (`Lst[str]`, *optional*):
                 A list of keys in the output of your model (if it is a dictionary) that should be ignored when
                 gathering predictions.
             metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
-                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
+                An optional prefix to be used as the metrics key prefix. For example the metric "bleu" will be named
                 "eval_bleu" if the prefix is "eval" (default)
 
         Returns:
             A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
             dictionary also contains the epoch number which comes from the training state.
         """
         # memory metrics - must set up as early as possible
@@ -1740,43 +1782,43 @@
 
         return output.metrics
 
     def predict(
         self, test_dataset: Dataset, ignore_keys: Optional[List[str]] = None, metric_key_prefix: str = "test"
     ) -> PredictionOutput:
         """
-        Run prediction and returns predictions and potential metrics.
+        Returns predictions and potential metrics.
 
         Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
         will also return metrics, like in `evaluate()`.
 
         Args:
             test_dataset (`Dataset`):
-                Dataset to run the predictions on. If it is an `datasets.Dataset`, columns not accepted by the
+                Dataset to run the predictions on. If it is an `datasets.Dataset` dataset, the columns not accepted by the
                 `model.forward()` method are automatically removed. Has to implement the method `__len__`
             ignore_keys (`Lst[str]`, *optional*):
                 A list of keys in the output of your model (if it is a dictionary) that should be ignored when
                 gathering predictions.
             metric_key_prefix (`str`, *optional*, defaults to `"test"`):
-                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
+                An optional prefix to be used as the metrics key prefix. For example the metric "bleu" will be named
                 "test_bleu" if the prefix is "test" (default)
 
         <Tip>
 
-        If your predictions or labels have different sequence length (for instance because you're doing dynamic padding
+        If your predictions or labels have different sequence lengths (for instance because you're doing dynamic padding
         in a token classification task) the predictions will be padded (on the right) to allow for concatenation into
         one array. The padding index is -100.
 
         </Tip>
 
         Returns: *NamedTuple* A namedtuple with the following keys:
 
             - predictions (`np.ndarray`): The predictions on `test_dataset`.
             - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
-            - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
+            - metrics (`Dict[str, float]`, *optional*): The dictionary of potential metrics (if the dataset contained
               labels).
         """
         # memory metrics - must set up as early as possible
         self._memory_tracker.start()
 
         test_dataloader = self.get_test_dataloader(test_dataset)
         start_time = time.time()
@@ -1815,17 +1857,33 @@
         dataloader: poptorch.DataLoader,
         description: str,
         prediction_loss_only: Optional[bool] = None,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "eval",
     ) -> EvalLoopOutput:
         """
-        Prediction/evaluation loop, shared by `IPUTrainer.evaluate()` and `IPUTrainer.predict()`.
+        Prediction/evaluation loop, shared by [`IPUTrainer.evaluate`] and [`IPUTrainer.predict`].
 
         Works both with or without labels.
+
+        Args:
+            dataloader (`poptorch.DataLoader`):
+                The dataset to be used.
+            description (`str`):
+                The description of what is being run.
+            prediction_loss_only (`bool`):
+                If `True`, only returns the loss. If `False`, returns loss,
+                logits and labels (if present).
+            ignore_keys (`Lst[str]`, *optional*):
+                A list of keys in the output of your model (if it is a
+                dictionary) that should be ignored when gathering predictions.
+            metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
+                An optional prefix to be used as the metrics key prefix. For
+                example the metric "bleu" will be named "eval_bleu" if the
+                prefix is "eval" (default).
         """
         prediction_loss_only = (
             prediction_loss_only if prediction_loss_only is not None else self.args.prediction_loss_only
         )
 
         self.inference_model = self._wrap_and_compile_model_for_evaluation(dataloader, prediction_loss_only)
 
@@ -1962,35 +2020,38 @@
         model: poptorch.PoplarExecutor,
         inputs: Dict[str, Union[torch.Tensor, Any]],
         prediction_loss_only: bool,
         ignore_keys: Optional[List[str]] = None,
         is_last_batch: bool = False,
     ) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
         """
-        Perform an evaluation step on `model` using `inputs`.
+        Performs an evaluation step.
 
         Subclass and override to inject custom behavior.
 
         Args:
             model (`poptorch.PoplarExecutor`):
                 The model to evaluate.
             inputs (`Dict[str, Union[torch.Tensor, Any]]`):
                 The inputs and targets of the model.
 
-                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
-                argument `labels`. Check your model's documentation for all accepted arguments.
+                The dictionary will be unpacked before being fed to the model.
+                Most models expect the targets under the argument `labels`.
+                Check your model's documentation for all accepted arguments.
             prediction_loss_only (`bool`):
-                Whether or not to return the loss only.
+                If `True`, only returns the loss. If `False`, returns loss,
+                logits and labels (if present).
             ignore_keys (`Lst[str]`, *optional*):
-                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
-                gathering predictions.
+                A list of keys in the output of your model (if it is a
+                dictionary) that should be ignored when gathering predictions.
 
         Return:
-            Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]: A tuple with the loss,
-            logits and labels (each being optional).
+            Tuple[Optional[torch.Tensor], Optional[torch.Tensor],
+            Optional[torch.Tensor]]:
+                A tuple with the loss, logits and labels (each being optional).
         """
         has_labels = all(inputs.get(k) is not None for k in self.label_names)
         inputs = self._prepare_inputs(inputs)
         if ignore_keys is None:
             if hasattr(self.model, "config"):
                 ignore_keys = getattr(self.model.config, "keys_to_ignore_at_inference", [])
             else:
@@ -2004,15 +2065,15 @@
         else:
             labels = None
 
         with torch.no_grad():
             if has_labels:
                 loss, outputs = self.compute_loss(model, inputs, return_outputs=True)
                 # If last batch is incomplete, some losses might be NaN because nothing was computed on the
-                # corresponding POD, ignoring them is necessary to not mess up evaluation loss computation
+                # corresponding Pod, ignoring them is necessary to not mess up evaluation loss computation
                 if is_last_batch:
                     loss = loss[~loss.isnan()]
                 loss = loss.detach()
                 if isinstance(outputs, dict):
                     logits = tuple(v for k, v in outputs.items() if k not in ignore_keys + ["loss"])
                 else:
                     logits = outputs[1:]
@@ -2034,16 +2095,18 @@
         if len(logits) == 1:
             logits = logits[0]
 
         return (loss, logits, labels)
 
     def floating_point_ops(self, inputs: Dict[str, Union[torch.Tensor, Any]]):
         """
-        For models that inherit from [`transformers.PreTrainedModel`], uses that method to compute the number of
-        floating point operations for every backward + forward pass. If using another model, either implement such a
+        For models that inherit from [`transformers.PreTrainedModel`], uses that class's `floating_point_ops` method to compute the number of
+        floating point operations for every backward and every forward pass.
+
+        If using another model, either implement a `floating_point_ops`
         method in the model or subclass and override this method.
 
         Args:
             inputs (`Dict[str, Union[torch.Tensor, Any]]`):
                 The inputs and targets of the model.
 
         Returns:
@@ -2054,21 +2117,22 @@
         if hasattr(self.original_model, "floating_point_ops"):
             return self.original_model.floating_point_ops(inputs)
         else:
             return 0
 
     def init_git_repo(self, at_init: bool = False):
         """
-        Initializes a git repo in `self.args.hub_model_id`.
+        Initializes a Git repo in `self.args.hub_model_id`.
 
         Args:
             at_init (`bool`, *optional*, defaults to `False`):
-                Whether this function is called before any training or not. If `self.args.overwrite_output_dir` is
-                `True` and `at_init` is `True`, the path to the repo (which is `self.args.output_dir`) might be wiped
-                out.
+                If `True`, this function is called before any training. If
+                `self.args.overwrite_output_dir` is `True` and `at_init` is
+                `True`, the path to the repo (which is `self.args.output_dir`)
+                might be wiped out.
         """
         if not self.is_world_process_zero():
             return
         use_auth_token = True if self.args.hub_token is None else self.args.hub_token
         if self.args.hub_model_id is None:
             repo_name = Path(self.args.output_dir).absolute().name
         else:
@@ -2116,29 +2180,30 @@
         finetuned_from: Optional[str] = None,
         tasks: Union[str, List[str], None] = None,
         dataset_tags: Union[str, List[str], None] = None,
         dataset: Union[str, List[str], None] = None,
         dataset_args: Union[str, List[str], None] = None,
     ):
         """
-        Creates a draft of a model card using the information available to the `Trainer`.
+        Creates a draft of a model card using the information available to
+        [`IPUTrainer`].
 
         Args:
             language (`str`, *optional*):
                 The language of the model (if applicable)
             license (`str`, *optional*):
                 The license of the model. Will default to the license of the pretrained model used, if the original
-                model given to the `Trainer` comes from a repo on the Hub.
+                model given to [`IPUTrainer`] comes from a repo on the Hub.
             tags (`str` or `List[str]`, *optional*):
                 Some tags to be included in the metadata of the model card.
             model_name (`str`, *optional*):
                 The name of the model.
             finetuned_from (`str`, *optional*):
                 The name of the model used to fine-tune this one (if applicable). Will default to the name of the repo
-                of the original model given to the `Trainer` (if it comes from the Hub).
+                of the original model given to [`IPUTrainer`] (if it comes from the Hub).
             tasks (`str` or `List[str]`, *optional*):
                 One or several task identifiers, to be included in the metadata of the model card.
             dataset_tags (`str` or `List[str]`, *optional*):
                 One or several dataset tags, to be included in the metadata of the model card.
             dataset (`str` or `List[str]`, *optional*):
                 One or several dataset identifiers, to be included in the metadata of the model card.
             dataset_args (`str` or `List[str]`, *optional*):
@@ -2203,27 +2268,26 @@
         finally:
             if self.args.hub_strategy == HubStrategy.CHECKPOINT:
                 # Move back the checkpoint to its place
                 shutil.move(tmp_checkpoint, checkpoint_folder)
 
     def push_to_hub(self, commit_message: Optional[str] = "End of training", blocking: bool = True, **kwargs) -> str:
         """
-        Upload *self.model* and *self.tokenizer* to the 🤗 model hub on the repo *self.args.hub_model_id*.
+        Uploads *self.model* and *self.tokenizer* to the 🤗 Models Hub on the repo *self.args.hub_model_id*.
 
         Parameters:
             commit_message (`str`, *optional*, defaults to `"End of training"`):
-                Message to commit while pushing.
+                Message for the commit.
             blocking (`bool`, *optional*, defaults to `True`):
-                Whether the function should return only when the `git push` has finished.
+                If `True` (default), the function only returns when the `git push` command has completed. If `False`, returns immediately.
             kwargs:
                 Additional keyword arguments passed along to [`~Trainer.create_model_card`].
 
         Returns:
-            The url of the commit of your model in the given repository if `blocking=False`, a tuple with the url of
-            the commit and an object to track the progress of the commit if `blocking=True`
+            If `blocking=False`, returns the URL of the commit of your model in the given repository. If `blocking=True`, returns a tuple with the URL of the commit and an object to track the progress of the commit.
         """
         # If a user calls manually `push_to_hub` with `self.args.push_to_hub = False`, we try to create the repo but
         # it might fail.
         if not hasattr(self, "repo"):
             self.init_git_repo()
 
         if self.args.should_save:
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/trainer_pt_utils.py` & `optimum-graphcore-0.6.1/optimum/graphcore/trainer_pt_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/trainer_seq2seq.py` & `optimum-graphcore-0.6.1/optimum/graphcore/trainer_seq2seq.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,35 +16,52 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from torch import nn
 from torch.utils.data import Dataset
 
 from optimum.utils import logging
+from poptorch._impl import rewrapModelIfNecessary, unwrapModelIfNecessary
 
 from .trainer import IPUTrainer
 
 
 logger = logging.get_logger(__name__)
 
 
 class IPUSeq2SeqTrainer(IPUTrainer):
+    """
+    The [`IPUSeq2SeqTrainer`] class is used to train seq2seq models. Its behaviour is exactly the same as [`IPUTrainer`] except that it expects [`IPUSeq2SeqTrainingArguments`] instead of [`IPUTrainingArguments`].
+    """
+
     def _wrap_and_compile_model_for_evaluation(self, dataloader, prediction_loss_only):
         if prediction_loss_only:
             return super()._wrap_and_compile_model_for_evaluation(dataloader, prediction_loss_only)
 
+        # Unwrap the model, including parameter and buffer annotations and the
+        # model as a whole. This is needed to avoid issues with persistent buffers
+        # when compiling an inference model for generation
+        unwrapModelIfNecessary(self.model)
+
         # reparallelize for generation
-        self.model = self.model.deparallelize().parallelize(for_generation=True)
+        self.model.deparallelize().ipu_config.eval()
+        self.model.parallelize(for_generation=True)
 
         # let IPUGenerationMixin::_call_generate handle compilation of the model
         # note though that self.model.poptorch_decoder and self.model.poptorch_encoder
         # (attribute added by IPUGenerationMixin::_call_generate)
         # are the actual models attached to the device
         return self.model
 
+    def _rewrap_model_for_training(self):
+        self.model.deparallelize().ipu_config.train()
+        self.model.parallelize()
+        # Restores the PoptorchParameter and PoptorchBuffer annotations in the model
+        rewrapModelIfNecessary(self.model)
+
     def evaluate(
         self,
         eval_dataset: Optional[Dataset] = None,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "eval",
         max_length: Optional[int] = None,
         num_beams: Optional[int] = None,
@@ -67,101 +84,108 @@
                 gathering predictions.
             metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
                 An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
                 "eval_bleu" if the prefix is `"eval"` (default)
             max_length (`int`, *optional*):
                 The maximum target length to use when predicting with the generate method.
             num_beams (`int`, *optional*):
-                Number of beams for beam search that will be used when predicting with the generate method. 1 means no
+                Number of beams for the beam search that will be used when predicting with the generate method. 1 means no
                 beam search.
 
         Returns:
             A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
             dictionary also contains the epoch number which comes from the training state.
         """
         self._max_length = max_length if max_length is not None else self.args.generation_max_length
         self._num_beams = num_beams if num_beams is not None else self.args.generation_num_beams
-        return super().evaluate(eval_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
+        results = super().evaluate(eval_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
+        self._rewrap_model_for_training()
+        return results
 
     def predict(
         self,
         test_dataset: Dataset,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "test",
         max_length: Optional[int] = None,
         num_beams: Optional[int] = None,
     ) -> "PredictionOutput":
         """
-        Run prediction and returns predictions and potential metrics.
+        Runs prediction and returns predictions and potential metrics.
 
         Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
-        will also return metrics, like in `evaluate()`.
+        will also return metrics, like `evaluate()`.
 
         Args:
             test_dataset (`Dataset`):
-                Dataset to run the predictions on. If it is an `datasets.Dataset`, columns not accepted by the
+                Dataset to run the predictions on. If it is a `datasets.Dataset` dataset, the columns not accepted by the
                 `model.forward()` method are automatically removed. Has to implement the method `__len__`
             ignore_keys (`List[str]`, *optional*):
                 A list of keys in the output of your model (if it is a dictionary) that should be ignored when
                 gathering predictions.
             metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
                 An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
                 "eval_bleu" if the prefix is `"eval"` (default)
             max_length (`int`, *optional*):
                 The maximum target length to use when predicting with the generate method.
             num_beams (`int`, *optional*):
-                Number of beams for beam search that will be used when predicting with the generate method. 1 means no
+                Number of beams for the beam search that will be used when predicting with the generate method. 1 means no
                 beam search.
 
         <Tip>
 
         If your predictions or labels have different sequence lengths (for instance because you're doing dynamic
         padding in a token classification task) the predictions will be padded (on the right) to allow for
         concatenation into one array. The padding index is -100.
 
         </Tip>
 
         Returns: *NamedTuple* A namedtuple with the following keys:
 
-            - predictions (`np.ndarray`): The predictions on `test_dataset`.
-            - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
-            - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
-              labels).
+            - predictions (`np.ndarray`):
+                The predictions on `test_dataset`.
+            - label_ids (`np.ndarray`, *optional*):
+                The labels (if the dataset contained some).
+            - metrics (`Dict[str, float]`, *optional*):
+                The potential dictionary of metrics (if the dataset contained
+                labels).
         """
         self._max_length = max_length if max_length is not None else self.args.generation_max_length
         self._num_beams = num_beams if num_beams is not None else self.args.generation_num_beams
-        return super().predict(test_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
+        results = super().predict(test_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
+        self._rewrap_model_for_training()
+        return results
 
     def prediction_step(
         self,
         model: nn.Module,
         inputs: Dict[str, Union[torch.Tensor, Any]],
         prediction_loss_only: bool,
         ignore_keys: Optional[List[str]] = None,
         is_last_batch: bool = False,
     ) -> Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
         """
-        Perform an evaluation step on `model` using `inputs`.
+        Performs an evaluation step on a model using the inputs.
 
         Subclass and override to inject custom behavior.
 
         Args:
             model (`nn.Module`):
                 The model to evaluate.
             inputs (`Dict[str, Union[torch.Tensor, Any]]`):
                 The inputs and targets of the model.
 
                 The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
                 argument `labels`. Check your model's documentation for all accepted arguments.
             prediction_loss_only (`bool`):
-                Whether or not to return the loss only.
+                If `True`, only returns the loss.
 
         Return:
-            Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]: A tuple with the loss, logits and
-            labels (each being optional).
+            Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
+                A tuple with the loss, logits and labels (each being optional).
         """
 
         if not self.args.predict_with_generate or prediction_loss_only:
             return super().prediction_step(
                 model,
                 inputs,
                 prediction_loss_only=prediction_loss_only,
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/trainer_utils.py` & `optimum-graphcore-0.6.1/optimum/graphcore/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/training_args.py` & `optimum-graphcore-0.6.1/optimum/graphcore/training_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 from poptorch import DataLoaderMode
 from transformers.debug_utils import DebugOption
 from transformers.file_utils import cached_property, get_full_repo_name, is_torch_available, torch_required
 from transformers.trainer_utils import EvaluationStrategy, HubStrategy, IntervalStrategy, SchedulerType
 from transformers.training_args import default_logdir
 from transformers.utils import ExplicitEnum
 
-from .ipu_configuration import ALLOWED_POD_TYPES
-
 
 logger = logging.get_logger(__name__)
 log_levels = logging.get_log_levels_dict().copy()
 trainer_log_levels = dict(**log_levels, passive=-1)
 
+ALLOWED_N_IPU = [2**i for i in range(7)]
+
 
 class ParallelMode(Enum):
     IPU = "ipu"
 
 
 class OptimizerNames(ExplicitEnum):
     """
-    Stores the acceptable string identifiers for optimizers.
+    Stores the allowed string identifiers for optimizers.
     """
 
     ADAMW_HF = "adamw_hf"
     ADAMW_TORCH = "adamw_torch"
     ADAMW_TORCH_XLA = "adamw_torch_xla"
     ADAMW_APEX_FUSED = "adamw_apex_fused"
     ADAFACTOR = "adafactor"
@@ -58,180 +58,180 @@
     SGD = "sgd"
     ADAGRAD = "adagrad"
 
 
 @dataclass
 class IPUTrainingArguments:
     """
-    `IPUTrainingArguments` is the subset of the arguments we use in our example scripts **which relate to the training loop
-    itself**.
+    `IPUTrainingArguments` is the class that contains the subset of the input
+    arguments **which relate to the training loop itself**.
 
     Using [`transformers.HfArgumentParser`] we can turn this class into
-    [argparse](https://docs.python.org/3/library/argparse#module-argparse) arguments that can be specified on the
-    command line.
+    [argparse](https://docs.python.org/3/library/argparse#module-argparse)
+    arguments that can be specified on the command line.
 
     Parameters:
         output_dir (`str`):
             The output directory where the model predictions and checkpoints will be written.
         overwrite_output_dir (`bool`, *optional*, defaults to `False`):
-            If `True`, overwrite the content of the output directory. Use this to continue training if `output_dir`
-            points to a checkpoint directory.
+            If `True`, overwrites the contents of the output directory. Use this
+            to continue training if `output_dir` points to a checkpoint
+            directory.
         do_train (`bool`, *optional*, defaults to `False`):
-            Whether to run training or not. This argument is not directly used by [`Trainer`], it's intended to be used
+            If `True`, runs training. This argument is not directly used by [`Trainer`]. It's intended to be used
             by your training/evaluation scripts instead. See the [example
             scripts](https://github.com/huggingface/transformers/tree/main/examples) for more details.
         do_eval (`bool`, *optional*):
-            Whether to run evaluation on the validation set or not. Will be set to `True` if `evaluation_strategy` is
-            different from `"no"`. This argument is not directly used by [`Trainer`], it's intended to be used by your
+            If `True`, runs evaluation on the validation set. Will be set to `True` if `evaluation_strategy` is
+            different from `"no"`. This argument is not directly used by [`Trainer`]. It's intended to be used by your
             training/evaluation scripts instead. See the [example
             scripts](https://github.com/huggingface/transformers/tree/main/examples) for more details.
         do_predict (`bool`, *optional*, defaults to `False`):
-            Whether to run predictions on the test set or not. This argument is not directly used by [`Trainer`], it's
+            If `True`, runs predictions on the test set. This argument is not directly used by [`Trainer`]. It's
             intended to be used by your training/evaluation scripts instead. See the [example
             scripts](https://github.com/huggingface/transformers/tree/main/examples) for more details.
         evaluation_strategy (`str` or [`~trainer_utils.IntervalStrategy`], *optional*, defaults to `"no"`):
             The evaluation strategy to adopt during training. Possible values are:
 
                 - `"no"`: No evaluation is done during training.
                 - `"steps"`: Evaluation is done (and logged) every `eval_steps`.
                 - `"epoch"`: Evaluation is done at the end of each epoch.
 
         prediction_loss_only (`bool`, *optional*, defaults to `False`):
-            When performing evaluation and generating predictions, only returns the loss.
+            If `True`, only returns the loss, when performing evaluation and generating predictions.
         per_device_train_batch_size (`int`, *optional*, defaults to 1):
             The batch size per IPU for training.
         per_device_eval_batch_size (`int`, *optional*, defaults to 1):
             The batch size per IPU for evaluation.
         gradient_accumulation_steps (`int`, *optional*, defaults to 1):
             Number of updates steps to accumulate the gradients for, before performing a backward/update pass.
 
             <Tip warning={true}>
 
-            When using gradient accumulation, one step is counted as one step with backward pass. Therefore, logging,
-            evaluation, save will be conducted every `gradient_accumulation_steps * xxx_step` training examples.
+            When using gradient accumulation, one step is counted as one step with a backward pass. Therefore, logging,
+            evaluation and saving will be conducted every `gradient_accumulation_steps * xxx_step` training examples.
 
             </Tip>
 
         eval_delay (`float`, *optional*):
+            The number of epochs or steps to wait before the first evaluation can be performed, depending on the evaluation strategy.
         adam_beta1 (`float`, *optional*, defaults to 0.9):
             The beta1 hyperparameter for the [`AdamW`] optimizer.
         adam_beta2 (`float`, *optional*, defaults to 0.999):
             The beta2 hyperparameter for the [`AdamW`] optimizer.
         adam_epsilon (`float`, *optional*, defaults to 1e-8):
             The epsilon hyperparameter for the [`AdamW`] optimizer.
         max_grad_norm (`float`, *optional*, defaults to 1.0):
             Maximum gradient norm (for gradient clipping).
         num_train_epochs(`float`, *optional*, defaults to 3.0):
-            Total number of training epochs to perform (if not an integer, will perform the decimal part percents of
-            the last epoch before stopping training).
+            Total number of training epochs to perform (if not an integer, training will continue for the indicated fraction of the last epoch before stopping).
         max_steps (`int`, *optional*, defaults to -1):
             If set to a positive number, the total number of training steps to perform. Overrides `num_train_epochs`.
-            In case of using a finite iterable dataset the training may stop before reaching the set number of steps
+            In the case of using a finite iterable dataset, the training may stop before reaching the set number of steps
             when all data is exhausted
         lr_scheduler_type (`str` or [`SchedulerType`], *optional*, defaults to `"linear"`):
-            The scheduler type to use. See the documentation of [`SchedulerType`] for all possible values.
+            The type of scheduler to use. See the documentation of [`SchedulerType`] for all possible values.
         warmup_ratio (`float`, *optional*, defaults to 0.0):
-            Ratio of total training steps used for a linear warmup from 0 to `learning_rate`.
+            The fraction of total steps to be used to linear warmup. Ranges from 0 to `learning_rate`.
         warmup_steps (`int`, *optional*, defaults to 0):
-            Number of steps used for a linear warmup from 0 to `learning_rate`. Overrides any effect of `warmup_ratio`.
+            Number of steps used for a linear warmup. Ranges from 0 to `learning_rate`*total steps. Overrides any effect of `warmup_ratio`.
         log_level (`str`, *optional*, defaults to `passive`):
             Logger log level to use on the main process. Possible choices are the log levels as strings: 'debug',
-            'info', 'warning', 'error' and 'critical', plus a 'passive' level which doesn't set anything and lets the
-            application set the level.
+            'info', 'warning', 'error' and 'critical', plus a 'passive' level which lets the application set the level.
         logging_dir (`str`, *optional*):
             [TensorBoard](https://www.tensorflow.org/tensorboard) log directory. Will default to
             *output_dir/runs/**CURRENT_DATETIME_HOSTNAME***.
         logging_strategy (`str` or [`~trainer_utils.IntervalStrategy`], *optional*, defaults to `"steps"`):
             The logging strategy to adopt during training. Possible values are:
 
                 - `"no"`: No logging is done during training.
                 - `"epoch"`: Logging is done at the end of each epoch.
                 - `"steps"`: Logging is done every `logging_steps`.
 
         logging_first_step (`bool`, *optional*, defaults to `False`):
-            Whether to log and evaluate the first `global_step` or not.
+            If `True`, logs and evaluates the first `global_step`.
         logging_steps (`int`, *optional*, defaults to 500):
             Number of update steps between two logs if `logging_strategy="steps"`.
         logging_nan_inf_filter (`bool`, *optional*, defaults to `True`):
-            Whether to filter `nan` and `inf` losses for logging. If set to `True` the loss of every step that is `nan`
+            If `True`, the loss of every step that is `nan`
             or `inf` is filtered and the average loss of the current logging window is taken instead.
 
             <Tip>
 
-            `logging_nan_inf_filter` only influences the logging of loss values, it does not change the behavior the
-            gradient is computed or applied to the model.
+            `logging_nan_inf_filter` only influences the logging of loss values
+            and it does not change the behavior of how the gradient is computed
+            or applied to the model.
 
             </Tip>
 
         save_strategy (`str` or [`~trainer_utils.IntervalStrategy`], *optional*, defaults to `"steps"`):
             The checkpoint save strategy to adopt during training. Possible values are:
 
-                - `"no"`: No save is done during training.
-                - `"epoch"`: Save is done at the end of each epoch.
-                - `"steps"`: Save is done every `save_steps`.
+                - `"no"`: No save during training.
+                - `"epoch"`: Save at the end of each epoch.
+                - `"steps"`: Save every `save_steps`.
         save_steps (`int`, *optional*, defaults to 500):
-            Number of updates steps before two checkpoint saves if `save_strategy="steps"`.
+            Number of update steps before two checkpoint saves if `save_strategy="steps"`.
         save_total_limit (`int`, *optional*):
-            If a value is passed, will limit the total amount of checkpoints. Deletes the older checkpoints in
+            If a value is passed, will limit the total number of checkpoints. Deletes the older checkpoints in
             `output_dir`.
         seed (`int`, *optional*, defaults to 42):
             Random seed that will be set at the beginning of training. To ensure reproducibility across runs, use the
             [`~Trainer.model_init`] function to instantiate the model if it has some randomly initialized parameters.
         data_seed (`int`, *optional*):
             Random seed to be used with data samplers. If not set, random generators for data sampling will use the
             same seed as `seed`. This can be used to ensure reproducibility of data sampling, independent of the model
             seed.
         dataloader_drop_last (`bool`, *optional*, defaults to `False`):
-            Whether to drop the last incomplete batch (if the length of the dataset is not divisible by the batch size)
-            or not.
+            If `True`, drops the last incomplete batch (if the length of the dataset is not divisible by the batch size).
         eval_steps (`int`, *optional*):
             Number of update steps between two evaluations if `evaluation_strategy="steps"`. Will default to the same
             value as `logging_steps` if not set.
         dataloader_num_workers (`int`, *optional*, defaults to 0):
             Number of subprocesses to use for data loading (PyTorch only). 0 means that the data will be loaded in the
             main process.
         past_index (`int`, *optional*, defaults to -1):
             Some models like [TransformerXL](../model_doc/transformerxl) or [XLNet](../model_doc/xlnet) can make use of
-            the past hidden states for their predictions. If this argument is set to a positive int, the `Trainer` will
+            past hidden states for their predictions. If this argument is set to a positive int, `Trainer` will
             use the corresponding output (usually index 2) as the past state and feed it to the model at the next
             training step under the keyword argument `mems`.
         run_name (`str`, *optional*):
-            A descriptor for the run. Typically used for [wandb](https://www.wandb.com/) and
-            [mlflow](https://www.mlflow.org/) logging.
+            A descriptor for the run. Typically used for [WandB](https://www.wandb.com/) and
+            [MLflow](https://www.mlflow.org/) logging.
         disable_tqdm (`bool`, *optional*):
-            Whether or not to disable the tqdm progress bars and table of metrics produced by
+            If `True`, disables the tqdm progress bars and table of metrics produced by
             [`~notebook.NotebookTrainingTracker`] in Jupyter Notebooks. Will default to `True` if the logging level is
             set to warn or lower (default), `False` otherwise.
         remove_unused_columns (`bool`, *optional*, defaults to `True`):
-            Whether or not to automatically remove the columns unused by the model forward method.
+            If `True`, automatically removes the columns unused by the model forward method.
         label_names (`List[str]`, *optional*):
             The list of keys in your dictionary of inputs that correspond to the labels.
 
             Will eventually default to `["labels"]` except if the model used is one of the `XxxForQuestionAnswering` in
             which case it will default to `["start_positions", "end_positions"]`.
         load_best_model_at_end (`bool`, *optional*, defaults to `False`):
-            Whether or not to load the best model found during training at the end of training.
+            If `True`, loads the best model found during training at the end of training.
 
             <Tip>
 
-            When set to `True`, the parameters `save_strategy` needs to be the same as `evaluation_strategy`, and in
+            When set to `True`, the parameter `save_strategy` needs to be the same as `evaluation_strategy`, and in
             the case it is "steps", `save_steps` must be a round multiple of `eval_steps`.
 
             </Tip>
 
         metric_for_best_model (`str`, *optional*):
-            Use in conjunction with `load_best_model_at_end` to specify the metric to use to compare two different
+            Use in conjunction with `load_best_model_at_end` to specify the metric for comparing two different
             models. Must be the name of a metric returned by the evaluation with or without the prefix `"eval_"`. Will
             default to `"loss"` if unspecified and `load_best_model_at_end=True` (to use the evaluation loss).
 
-            If you set this value, `greater_is_better` will default to `True`. Don't forget to set it to `False` if
+            If you set this parameter, `greater_is_better` will default to `True`. Don't forget to set it to `False` if
             your metric is better when lower.
         greater_is_better (`bool`, *optional*):
             Use in conjunction with `load_best_model_at_end` and `metric_for_best_model` to specify if better models
-            should have a greater metric or not. Will default to:
+            should have a higher metric or not. Will default to:
 
             - `True` if `metric_for_best_model` is set to a value that isn't `"loss"` or `"eval_loss"`.
             - `False` if `metric_for_best_model` is not set, or set to `"loss"` or `"eval_loss"`.
         ignore_data_skip (`bool`, *optional*, defaults to `False`):
             When resuming training, whether or not to skip the epochs and batches to get the data loading at the same
             stage as in the previous training. If set to `True`, the training will begin faster (as that skipping step
             can take a long time) but will not yield the same results as the interrupted training would have.
@@ -248,211 +248,209 @@
               the event
 
             The options should be separated by whitespaces.
         optim (`str` or [`training_args.OptimizerNames`], *optional*, defaults to `"adamw_hf"`):
             The optimizer to use: adamw_hf, adamw_torch, adamw_apex_fused, or adafactor.
             **Note**: currently not supported.
         lamb (`bool`, *optional*, defaults to `False`):
-            Whether or not to replace AdamW by LAMB.
+            If `True`, replaces AdamW with LAMB.
         lamb_no_bias_correction (`bool`, *optional*, defaults to `False`):
-            Whether or not to replace AdamW by LAMB without bias correction.
+            If `True`, replaces AdamW with LAMB without bias correction.
         group_by_length (`bool`, *optional*, defaults to `False`):
-            Whether or not to group together samples of roughly the same length in the training dataset (to minimize
+            If `True`, groups together samples of roughly the same length in the training dataset (to minimize
             padding applied and be more efficient). Only useful if applying dynamic padding.
         length_column_name (`str`, *optional*, defaults to `"length"`):
-            Column name for precomputed lengths. If the column exists, grouping by length will use these values rather
-            than computing them on train startup. Ignored unless `group_by_length` is `True` and the dataset is an
+            The column name for precomputed lengths. If the column exists, grouping by length will use these values rather
+            than computing them on training startup. Ignored unless `group_by_length` is `True` and the dataset is an
             instance of `Dataset`.
         report_to (`str` or `List[str]`, *optional*, defaults to `"all"`):
             The list of integrations to report the results and logs to. Supported platforms are `"azure_ml"`,
             `"comet_ml"`, `"mlflow"`, `"neptune"`, `"tensorboard"` and `"wandb"`. Use `"all"` to report to all
             integrations installed, `"none"` for no integrations.
         dataloader_pin_memory (`bool`, *optional*, defaults to `True`):
-            Whether you want to pin memory in data loaders or not. Will default to `True`.
+            If `True`, pins memory in data loaders. Will default to `True`.
         skip_memory_metrics (`bool`, *optional*, defaults to `True`):
-            Whether to skip adding of memory profiler reports to metrics. This is skipped by default because it slows
-            down the training and evaluation speed.
+            If `True`, skips adding of memory profiler reports to metrics. This is skipped by default because it slows down the training and evaluation.
         push_to_hub (`bool`, *optional*, defaults to `False`):
-            Whether or not to push the model to the Hub every time the model is saved. If this is activated,
-            `output_dir` will begin a git directory synced with the repo (determined by `hub_model_id`) and the content
+            If `True`, pushes the model to the Hub every time the model is saved. If this is activated,
+            `output_dir` will begin a Git directory synced with the repo (determined by `hub_model_id`) and the content
             will be pushed each time a save is triggered (depending on your `save_strategy`). Calling
             [`~Trainer.save_model`] will also trigger a push.
 
             <Tip warning={true}>
 
-            If `output_dir` exists, it needs to be a local clone of the repository to which the [`Trainer`] will be
+            If `output_dir` exists, it needs to be a local clone of the repository to which the [`Trainer`] instance will be
             pushed.
 
             </Tip>
 
         resume_from_checkpoint (`str`, *optional*):
             The path to a folder with a valid checkpoint for your model. This argument is not directly used by
-            [`Trainer`], it's intended to be used by your training/evaluation scripts instead. See the [example
+            [`Trainer`]. It's intended to be used by your training/evaluation scripts instead. See the [example
             scripts](https://github.com/huggingface/transformers/tree/main/examples) for more details.
         hub_model_id (`str`, *optional*):
             The name of the repository to keep in sync with the local *output_dir*. It can be a simple model ID in
             which case the model will be pushed in your namespace. Otherwise it should be the whole repository name,
             for instance `"user_name/model"`, which allows you to push to an organization you are a member of with
             `"organization_name/model"`. Will default to `user_name/output_dir_name` with *output_dir_name* being the
             name of `output_dir`.
 
             Will default to the name of `output_dir`.
         hub_strategy (`str` or [`~trainer_utils.HubStrategy`], *optional*, defaults to `"every_save"`):
             Defines the scope of what is pushed to the Hub and when. Possible values are:
 
-            - `"end"`: push the model, its configuration, the tokenizer (if passed along to the [`Trainer`]) and a
+            - `"end"`: push the model, its configuration, the tokenizer (if passed along to [`Trainer`]) and a
               draft of a model card when the [`~Trainer.save_model`] method is called.
-            - `"every_save"`: push the model, its configuration, the tokenizer (if passed along to the [`Trainer`]) and
+            - `"every_save"`: push the model, its configuration, the tokenizer (if passed along to [`Trainer`]) and
               a draft of a model card each time there is a model save. The pushes are asynchronous to not block
-              training, and in case the save are very frequent, a new push is only attempted if the previous one is
-              finished. A last push is made with the final model at the end of training.
+              training, and if the saves are very frequent, a new push is only attempted if the previous push has completed. A last push is made with the final model at the end of training.
             - `"checkpoint"`: like `"every_save"` but the latest checkpoint is also pushed in a subfolder named
               last-checkpoint, allowing you to resume training easily with
               `trainer.train(resume_from_checkpoint="last-checkpoint")`.
             - `"all_checkpoints"`: like `"checkpoint"` but all checkpoints are pushed like they appear in the output
               folder (so you will get one checkpoint folder per folder in your final repository)
 
         hub_token (`str`, *optional*):
             The token to use to push the model to the Hub. Will default to the token in the cache folder obtained with
             `huggingface-cli login`.
         hub_private_repo (`bool`, *optional*, defaults to `False`):
-            If True, the Hub repo will be set to private.
+            If `True`, the Hub repo will be set to private.
         gradient_checkpointing (`bool`, *optional*, defaults to `False`):
-            If True, use gradient checkpointing to save memory at the expense of slower backward pass.
+            If `True`, use gradient checkpointing to save memory at the expense of slower backward pass.
         include_inputs_for_metrics (`bool`, *optional*, defaults to `False`):
-            Whether or not the inputs will be passed to the `compute_metrics` function. This is intended for metrics
-            that need inputs, predictions and references for scoring calculation in Metric class.
+            If `True`, the inputs will be passed to the `compute_metrics` function. This is intended for metrics
+            that need inputs, predictions and references for scoring calculation in the `Metric` class.
             **Note**: currently not supported.
         ipu_config_name (`str`, *optional*):
             The pretrained IPU config name or path if not the same as the model name or path.
-        pod_type (`str`, *optional*):
-            The targeted pod type (POD4, POD8, POD16, ...)
+        n_ipu (`int`, *optional*):
+            The number of IPUs to use. Must be a power of 2 and a multiple of the number of IPUs required by your model.
         fp32 (`bool`, *optional*, defaults to `False`):
-            Whether to use 32-bit (full) precision instead of 16-bit
+            If `True`, uses 32-bit (full) precision instead of 16-bit.
         loss_scaling (`float`, *optional*):
             The loss scaling factor (using a power of 2 is recommended). If using automatic loss scaling, this value will
             be the initial value.
         auto_loss_scaling (`bool`, *optional*, defaults to `False`):
-            Enables automatic lauss scaling for half precision training.
+            If `True`, enables automatic loss scaling for half precision training.
             **Note**: this feature is experimental.
         dataloader_mode (`str`, *optional*, defaults to `"sync"`):
-            The way data should be accessed. Possible values:
+            The way in which data should be accessed. Possible values:
 
             - sync
             - async
             - async_rebatched
 
         compile_only (`bool`, *optional*, defaults to `False`):
-            If `True`, the [`IPUTrainer`] will only perform model compilation and stop.
+            If `True`, the [`IPUTrainer`] instance will only perform model compilation and stop.
         ipu_config_overrides (`str`, *optional*):
             Overrides some existing IPU config settings.
             Example: `device_iterations=4,gradient_accumulation_steps=64`
         pad_on_batch_axis (`bool`, *optional*, defaults to `False`):
             Will pad each batch up to a fixed size. This ensures that the compiled model will have an input with the
-            proper shape, and allows to not use `dataloader_drop_last` during training.
+            proper shape, and means that `dataloader_drop_last` will not have to be used during training.
     """
 
     output_dir: str = field(
         metadata={"help": "The output directory where the model predictions and checkpoints will be written."},
     )
     overwrite_output_dir: bool = field(
         default=False,
         metadata={
             "help": (
-                "Overwrite the content of the output directory. "
+                "If `True`, overwrites the contents of the output directory. "
                 "Use this to continue training if output_dir points to a checkpoint directory."
             )
         },
     )
 
-    do_train: bool = field(default=False, metadata={"help": "Whether to run training."})
-    do_eval: bool = field(default=False, metadata={"help": "Whether to run eval on the dev set."})
-    do_predict: bool = field(default=False, metadata={"help": "Whether to run predictions on the test set."})
+    do_train: bool = field(default=False, metadata={"help": "If `True`, run training."})
+    do_eval: bool = field(default=False, metadata={"help": "If `True`, run evaluation on the development set."})
+    do_predict: bool = field(default=False, metadata={"help": "If `True`, run predictions on the test set."})
     evaluation_strategy: IntervalStrategy = field(
         default="no",
         metadata={"help": "The evaluation strategy to use."},
     )
     prediction_loss_only: bool = field(
         default=False,
-        metadata={"help": "When performing evaluation and predictions, only returns the loss."},
+        metadata={"help": "If `True`, only return the loss when performing evaluation and predictions."},
     )
 
     per_device_train_batch_size: int = field(default=1, metadata={"help": "Batch size per IPU for training."})
     per_device_eval_batch_size: int = field(default=1, metadata={"help": "Batch size per IPU for evaluation."})
 
     gradient_accumulation_steps: int = field(
         default=None,
-        metadata={"help": "Number of updates steps to accumulate before performing a backward/update pass."},
+        metadata={"help": "Number of update steps to accumulate before performing a backward/update pass."},
     )
     eval_delay: Optional[float] = field(
         default=0,
         metadata={
-            "help": "Number of epochs or steps to wait for before the first evaluation can be performed, depending on the evaluation_strategy."
+            "help": "Number of epochs or steps to wait before the first evaluation can be performed. Depends on the evaluation strategy."
         },
     )
     learning_rate: float = field(default=5e-5, metadata={"help": "The initial learning rate for AdamW."})
     weight_decay: float = field(default=0.0, metadata={"help": "Weight decay for AdamW if we apply some."})
     adam_beta1: float = field(default=0.9, metadata={"help": "Beta1 for AdamW optimizer"})
     adam_beta2: float = field(default=0.999, metadata={"help": "Beta2 for AdamW optimizer"})
     adam_epsilon: float = field(default=1e-8, metadata={"help": "Epsilon for AdamW optimizer."})
     max_grad_norm: float = field(default=1.0, metadata={"help": "Max gradient norm."})
 
     num_train_epochs: float = field(default=3.0, metadata={"help": "Total number of training epochs to perform."})
     max_steps: int = field(
         default=-1,
-        metadata={"help": "If > 0: set total number of training steps to perform. Override num_train_epochs."},
+        metadata={"help": "If > 0, set total number of training steps to perform. Overrides num_train_epochs."},
     )
     lr_scheduler_type: SchedulerType = field(
         default="linear",
-        metadata={"help": "The scheduler type to use."},
+        metadata={"help": "The scheduler type to use. Defaults to 'linear'."},
     )
     warmup_ratio: float = field(
-        default=0.0, metadata={"help": "Linear warmup over warmup_ratio fraction of total steps."}
+        default=0.0, metadata={"help": "The fraction of total steps to be used to linear warmup."}
     )
-    warmup_steps: int = field(default=0, metadata={"help": "Linear warmup over warmup_steps."})
+    warmup_steps: int = field(default=0, metadata={"help": "The number of steps to be used for linear warmup."})
 
     log_level: Optional[str] = field(
         default="passive",
         metadata={
             "help": (
-                "Logger log level to use on the main node. Possible choices are the log levels as strings: 'debug',"
-                " 'info', 'warning', 'error' and 'critical', plus a 'passive' level which doesn't set anything and"
+                "Logger log level to use on the main node. Possible choices are: 'debug',"
+                " 'info', 'warning', 'error' and 'critical', plus a 'passive' level which"
                 " lets the application set the level. Defaults to 'passive'."
             ),
             "choices": trainer_log_levels.keys(),
         },
     )
-    logging_dir: Optional[str] = field(default=None, metadata={"help": "Tensorboard log dir."})
+    logging_dir: Optional[str] = field(default=None, metadata={"help": "TensorBoard log dir."})
     logging_strategy: IntervalStrategy = field(
         default="steps",
         metadata={"help": "The logging strategy to use."},
     )
-    logging_first_step: bool = field(default=False, metadata={"help": "Log the first global_step"})
+    logging_first_step: bool = field(default=False, metadata={"help": "Log the first global_step."})
     logging_steps: int = field(default=500, metadata={"help": "Log every X updates steps."})
     logging_nan_inf_filter: bool = field(default=False, metadata={"help": "Filter nan and inf losses for logging."})
     save_strategy: IntervalStrategy = field(
         default="steps",
         metadata={"help": "The checkpoint save strategy to use."},
     )
     save_steps: int = field(default=500, metadata={"help": "Save checkpoint every X updates steps."})
     save_total_limit: Optional[int] = field(
         default=None,
         metadata={
             "help": (
-                "Limit the total amount of checkpoints. "
-                "Deletes the older checkpoints in the output_dir. Default is unlimited checkpoints"
+                "Limit the total number of checkpoints. "
+                "Deletes the older checkpoints in the output directory. Default is unlimited checkpoints."
             )
         },
     )
     seed: int = field(default=42, metadata={"help": "Random seed that will be set at the beginning of training."})
     data_seed: Optional[int] = field(default=None, metadata={"help": "Random seed to be used with data samplers."})
     debug: str = field(
         default="",
         metadata={
-            "help": "Whether or not to enable debug mode. Current options: "
+            "help": "Select whether or not to enable debug mode. Current options: "
             "`underflow_overflow` (Detect underflow and overflow in activations and weights), "
         },
     )
 
     dataloader_drop_last: bool = field(
         default=False, metadata={"help": "Drop the last incomplete batch if it is not divisible by the batch size."}
     )
@@ -465,153 +463,166 @@
     )
     past_index: int = field(
         default=-1,
         metadata={"help": "If >=0, uses the corresponding part of the output as the past state for next step."},
     )
 
     run_name: Optional[str] = field(
-        default=None, metadata={"help": "An optional descriptor for the run. Notably used for wandb logging."}
+        default=None, metadata={"help": "An optional descriptor for the run. Notably used for WandB logging."}
     )
     disable_tqdm: Optional[bool] = field(
         default=None, metadata={"help": "Whether or not to disable the tqdm progress bars."}
     )
 
     remove_unused_columns: Optional[bool] = field(
         default=True, metadata={"help": "Remove columns not required by the model when using an nlp.Dataset."}
     )
     label_names: Optional[List[str]] = field(
         default=None, metadata={"help": "The list of keys in your dictionary of inputs that correspond to the labels."}
     )
 
     load_best_model_at_end: Optional[bool] = field(
         default=False,
-        metadata={"help": "Whether or not to load the best model found during training at the end of training."},
+        metadata={"help": "If `True`, loads the best model found during training at the end of training."},
     )
     metric_for_best_model: Optional[str] = field(
         default=None, metadata={"help": "The metric to use to compare two different models."}
     )
     greater_is_better: Optional[bool] = field(
-        default=None, metadata={"help": "Whether the `metric_for_best_model` should be maximized or not."}
+        default=None, metadata={"help": "If `True`, maximizes `metric_for_best_model`."}
     )
     ignore_data_skip: bool = field(
         default=False,
         metadata={
-            "help": "When resuming training, whether or not to skip the first epochs and batches to get to the same training data."
+            "help": "If `True`, skips the first epochs and batches to get to the same training data, when resuming training. Default: False."
         },
     )
     label_smoothing_factor: float = field(
-        default=0.0, metadata={"help": "The label smoothing epsilon to apply (zero means no label smoothing)."}
+        default=0.0, metadata={"help": "The label smoothing epsilon to apply. 0 (default) means no label smoothing."}
     )
     # TODO: support this.
     # Type annotation not supported in transformers 4.20.1
     # optim: Union[OptimizerNames, str] = field(
     #    default="adamw_hf",
     #    metadata={"help": "The optimizer to use."},
     # )
     group_by_length: bool = field(
         default=False,
-        metadata={"help": "Whether or not to group samples of roughly the same length together when batching."},
+        metadata={
+            "help": "If `True`, groups samples of roughly the same length together when batching. Default: False."
+        },
     )
     length_column_name: Optional[str] = field(
         default="length",
-        metadata={"help": "Column name with precomputed lengths to use when grouping by length."},
+        metadata={
+            "help": "The column name with precomputed lengths to use when grouping by length. Default: 'length'"
+        },
     )
     report_to: Optional[List[str]] = field(
         default="none", metadata={"help": "The list of integrations to report the results and logs to."}
     )
     dataloader_pin_memory: bool = field(
-        default=True, metadata={"help": "Whether or not to pin memory for DataLoader."}
+        default=True, metadata={"help": "If `True`, pins memory for DataLoader. Default: True."}
     )
     skip_memory_metrics: bool = field(
-        default=True, metadata={"help": "Whether or not to skip adding of memory profiler reports to metrics."}
+        default=True, metadata={"help": "If `True`, skips adding of memory profiler reports to metrics."}
     )
     push_to_hub: bool = field(
-        default=False, metadata={"help": "Whether or not to upload the trained model to the model hub after training."}
+        default=False,
+        metadata={
+            "help": "If `True`, Whether or not to upload the trained model to the model hub after training. Default: False."
+        },
     )
     resume_from_checkpoint: Optional[str] = field(
         default=None,
         metadata={"help": "The path to a folder with a valid checkpoint for your model."},
     )
     hub_model_id: str = field(
         default=None, metadata={"help": "The name of the repository to keep in sync with the local `output_dir`."}
     )
     hub_strategy: HubStrategy = field(
         default="every_save",
-        metadata={"help": "The hub strategy to use when `--push_to_hub` is activated."},
+        metadata={"help": "The Hub strategy to use when `--push_to_hub` is activated."},
     )
     hub_token: str = field(default=None, metadata={"help": "The token to use to push to the Model Hub."})
-    hub_private_repo: bool = field(default=False, metadata={"help": "Whether the model repository is private or not."})
+    hub_private_repo: bool = field(
+        default=False, metadata={"help": "If `True`, indicates that the Hub Model repository is private."}
+    )
     gradient_checkpointing: bool = field(
         default=False,
         metadata={
-            "help": "If True, use gradient checkpointing to save memory at the expense of slower backward pass."
+            "help": "If `True`, use gradient checkpointing to save memory at the expense of slower backward pass. Default: False."
         },
     )
     # TODO: support this.
     include_inputs_for_metrics: bool = field(
-        default=False, metadata={"help": "Whether or not the inputs will be passed to the `compute_metrics` function."}
+        default=False,
+        metadata={"help": "If `True`, pass the inputs to the `compute_metrics` function. Default: False."},
     )
 
     # Deprecated arguments
     push_to_hub_model_id: str = field(
-        default=None, metadata={"help": "The name of the repository to which push the `Trainer`."}
+        default=None, metadata={"help": "The name of the repository to which push `Trainer` to."}
     )
     push_to_hub_organization: str = field(
-        default=None, metadata={"help": "The name of the organization in with to which push the `Trainer`."}
+        default=None, metadata={"help": "The name of the organization to use when pushing `Trainer`."}
     )
     push_to_hub_token: str = field(default=None, metadata={"help": "The token to use to push to the Model Hub."})
-
+    pod_type: Optional[str] = field(
+        default=None,
+        metadata={"help": "The POD type to run the `Trainer` on."},
+    )
     # IPU Specific arguments
     ipu_config_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained IPU config name or path if not the same as model_name."}
+        default=None, metadata={"help": "Pre-trained IPU config name or path if not the same as model_name."}
     )
-    pod_type: Optional[str] = field(
+    n_ipu: Optional[int] = field(
         default=None,
-        metadata={"help": "The POD type to run the `Trainer` on.", "choices": ALLOWED_POD_TYPES},
+        metadata={"help": "The number of IPUs to run the `Trainer` on.", "choices": ALLOWED_N_IPU},
     )
     fp32: bool = field(
         default=False,
-        metadata={"help": "Whether to use 32-bit (full) precision instead of 16-bit"},
+        metadata={"help": "If `True`, use 32-bit (full) precision instead of 16-bit."},
     )
-    lamb: bool = field(default=False, metadata={"help": "Whether or not to replace AdamW by LAMB."})
+    lamb: bool = field(default=False, metadata={"help": "If `True`, replace AdamW with LAMB. Default: False."})
     lamb_no_bias_correction: bool = field(
-        default=False, metadata={"help": "Whether or not to replace AdamW by LAMB without bias correction."}
+        default=False, metadata={"help": "If `True`, replace AdamW with LAMB without bias correction."}
     )
     loss_scaling: Optional[float] = field(
         default=None,
         metadata={
             "help": "Loss scaling factor (recommend using powers of 2)"
             "If using automatic loss scaling, this value will be the initial value."
         },
     )
     auto_loss_scaling: bool = field(
         default=False,
         metadata={
-            "help": "Enable automatic loss scaling for half precision training. Note that this is an experimental feature."
+            "help": "If `True`, enable automatic loss scaling for half precision training. Note that this is an experimental feature."
         },
     )
     dataloader_mode: str = field(
         default="sync",
         metadata={"help": "The way data should be accessed.", "choices": ["sync", "async", "async_rebatched"]},
     )
     compile_only: bool = field(
-        default=False, metadata={"help": "If True, the `IPUTrainer` will only perform model compilation and stop."}
+        default=False, metadata={"help": "If `True`, `IPUTrainer` will only perform model compilation and stop."}
     )
     ipu_config_overrides: Optional[str] = field(
         default=None,
         metadata={
-            "help": "Override some existing ipu config settings. Example: device_iterations=4,gradient_accumulation_steps=64"
+            "help": "Override some existing IPU config settings. Example: device_iterations=4,gradient_accumulation_steps=64"
         },
     )
     pad_on_batch_axis: bool = field(
         default=False,
         metadata={
             "help": (
                 "Will pad each batch up to a fixed size. This ensures that the compiled model will have an input with",
-                " the proper shape, and allows to not use drop_last during training.",
+                " the proper shape. This means drop_last doesn't have to be used during training.",
             ),
         },
     )
 
     def __post_init__(self):
         # convert to int
         self.log_level = trainer_log_levels[self.log_level]
@@ -628,15 +639,15 @@
             self.logging_dir = os.path.expanduser(self.logging_dir)
 
         if self.disable_tqdm is None:
             self.disable_tqdm = logger.getEffectiveLevel() > logging.WARN
 
         if isinstance(self.evaluation_strategy, EvaluationStrategy):
             warnings.warn(
-                "using `EvaluationStrategy` for `evaluation_strategy` is deprecated and will be removed in version 5 of 🤗 Transformers. Use `IntervalStrategy` instead",
+                "Using `EvaluationStrategy` for `evaluation_strategy` is deprecated and will be removed in version 5 of 🤗 Transformers. Use `IntervalStrategy` instead",
                 FutureWarning,
             )
             # Go back to the underlying string or we won't be able to instantiate `IntervalStrategy` on it.
             self.evaluation_strategy = self.evaluation_strategy.value
 
         self.evaluation_strategy = IntervalStrategy(self.evaluation_strategy)
         self.logging_strategy = IntervalStrategy(self.logging_strategy)
@@ -646,24 +657,24 @@
         self.lr_scheduler_type = SchedulerType(self.lr_scheduler_type)
         if self.do_eval is False and self.evaluation_strategy != IntervalStrategy.NO:
             self.do_eval = True
 
         # eval_steps has to be defined and non-zero, fallbacks to logging_steps if the latter is non-zero
         if self.evaluation_strategy == IntervalStrategy.STEPS and (self.eval_steps is None or self.eval_steps == 0):
             if self.logging_steps > 0:
-                logger.info(f"using `logging_steps` to initialize `eval_steps` to {self.logging_steps}")
+                logger.info(f"Using `logging_steps` to initialize `eval_steps` to {self.logging_steps}")
                 self.eval_steps = self.logging_steps
             else:
                 raise ValueError(
-                    f"evaluation strategy {self.evaluation_strategy} requires either non-zero --eval_steps or --logging_steps"
+                    f"Evaluation strategy {self.evaluation_strategy} requires either non-zero --eval_steps or --logging_steps"
                 )
 
         # logging_steps must be non-zero for logging_strategy that is other than 'no'
         if self.logging_strategy == IntervalStrategy.STEPS and self.logging_steps == 0:
-            raise ValueError(f"logging strategy {self.logging_strategy} requires non-zero --logging_steps")
+            raise ValueError(f"Logging strategy {self.logging_strategy} requires non-zero --logging_steps")
 
         # Sanity checks for load_best_model_at_end: we require save and eval strategies to be compatible.
         if self.load_best_model_at_end:
             if self.evaluation_strategy != self.save_strategy:
                 raise ValueError(
                     "--load_best_model_at_end requires the save and eval strategy to match, but found\n- Evaluation "
                     f"strategy: {self.evaluation_strategy}\n- Save strategy: {self.save_strategy}"
@@ -691,15 +702,15 @@
         elif not isinstance(self.report_to, list):
             self.report_to = [self.report_to]
 
         if self.warmup_ratio < 0 or self.warmup_ratio > 1:
             raise ValueError("warmup_ratio must lie in range [0,1]")
         elif self.warmup_ratio > 0 and self.warmup_steps > 0:
             logger.info(
-                "Both warmup_ratio and warmup_steps given, warmup_steps will override any effect of warmup_ratio during training"
+                "Both warmup_ratio and warmup_steps given, warmup_steps will override any effect of warmup_ratio during training."
             )
 
         if isinstance(self.debug, str):
             self.debug = [DebugOption(s) for s in self.debug.split()]
 
         if self.push_to_hub_token is not None:
             warnings.warn(
@@ -732,14 +743,22 @@
             warnings.warn(
                 "`--push_to_hub_organization` is deprecated and will be removed in version 5 of 🤗 Transformers. Use "
                 "`--hub_model_id` instead and pass the full repo name to this argument (in this case "
                 f"{self.hub_model_id}).",
                 FutureWarning,
             )
 
+        if self.pod_type is not None:
+            warnings.warn(
+                "`pod_type` is deprecated and will be removed in the next release of Optimum Graphcore. Use `n_ipu` "
+                "instead to specify how many IPUs you would like the Trainer to use.",
+                FutureWarning,
+            )
+            self.n_ipu = int(self.pod_type.strip("pod"))
+
         # IPU specific
         dataloader_mode_mapping = {"sync": 0, "async": 1, "async_rebatched": 2}
         self.dataloader_mode = DataLoaderMode(dataloader_mode_mapping[self.dataloader_mode])
 
         override_str = []
         if self.gradient_accumulation_steps is not None:
             override_str.append(f"gradient_accumulation_steps={self.gradient_accumulation_steps}")
@@ -772,70 +791,72 @@
         The device used by this process.
         """
         return self._setup_devices
 
     @property
     def should_save(self):
         """
-        Whether or not the current process should write to disk, e.g., to save models and checkpoints.
+        Returns whether the current process should write to disk or not, for example, to save models and checkpoints.
         """
         return True
 
     def get_process_log_level(self):
         """
-        Returns the log level to be used depending on whether this process is the main process of node 0, main process
+        Returns the log level to be used depending on whether this process is the main process of node 0, the main process
         of node non-0, or a non-main process.
 
-        For the main process the log level defaults to ``logging.INFO`` unless overridden by ``log_level`` argument.
+        For the main process, the log level defaults to ``logging.INFO`` unless overridden by the ``log_level`` argument.
 
-        For the replica processes the log level defaults to ``logging.WARNING`` unless overridden by
+        For the replica processes, the log level defaults to ``logging.WARNING`` unless overridden by the
         ``log_level_replica`` argument.
 
         The choice between the main and replica process settings is made according to the return value of
         ``should_log``.
         """
         log_level_main_node = logging.INFO if self.log_level == -1 else self.log_level
         return log_level_main_node
 
     @contextlib.contextmanager
     def main_process_first(self, local=True, desc="work"):
         """
-            A context manager for torch distributed environment where on needs to do something on the main process,
-            while blocking replicas, and when it's finished releasing the replicas.
-
-            One such use is for ``datasets``'s ``map`` feature which to be efficient should be run once on the main
-            process, which upon completion saves a cached version of results and which then automatically gets loaded
-            by the replicas.
+            A context manager for a `torch` distributed environment where one
+            needs to run a task on the main process, while blocking replicas,
+            and when the task is finished to release the replicas.
+
+            An example is for the ``datasets`` ``map`` feature which, to be
+            efficient, should be run once on the main process. Upon completion,
+            it saves a cached version of results and which then automatically
+            gets loaded by the replicas.
 
         Args:
             local (:obj:`bool`, `optional`, defaults to :obj:`True`):
                 if :obj:`True` first means process of rank 0 of each node if :obj:`False` first means process of rank 0
                 of node rank 0 In multi-node environment with a shared filesystem you most likely will want to use
                 ``local=False`` so that only the main process of the first node will do the processing. If however, the
                 filesystem is not shared, then the main process of each node will need to do the processing, which is
                 the default behavior.
             desc (:obj:`str`, `optional`, defaults to ``"work"``):
-                a work description to be used in debug logs
+                A work description to be used in debug logs
 
         """
         # Not useful, kept to save us from having to edit all the examples.
         yield
 
     def get_warmup_steps(self, num_training_steps: int):
         """
-        Get number of steps used for a linear warmup.
+        Get the number of steps used for a linear warmup.
         """
         warmup_steps = (
             self.warmup_steps if self.warmup_steps > 0 else math.ceil(num_training_steps * self.warmup_ratio)
         )
         return warmup_steps
 
     def to_dict(self):
         """
-        Serializes this instance while replace `Enum` by their values (for JSON serialization support). It obfuscates
+        Serializes this instance while replacing the `Enum` with their values (for JSON serialization support). It obfuscates
         the token values by removing their value.
         """
         d = asdict(self)
         for k, v in d.items():
             if isinstance(v, Enum):
                 d[k] = v.value
             if isinstance(v, list) and len(v) > 0 and isinstance(v[0], Enum):
@@ -848,15 +869,15 @@
         """
         Serializes this instance to a JSON string.
         """
         return json.dumps(self.to_dict(), indent=2)
 
     def to_sanitized_dict(self) -> Dict[str, Any]:
         """
-        Sanitized serialization to use with TensorBoard’s hparams
+        Sanitized serialization to use with TensorBoard HParams.
         """
         d = self.to_dict()
         d = {**d, **{"train_batch_size": self.train_batch_size, "eval_batch_size": self.eval_batch_size}}
 
         valid_types = [bool, int, float, str]
         if is_torch_available():
             valid_types.append(torch.Tensor)
```

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/training_args_seq2seq.py` & `optimum-graphcore-0.6.1/optimum/graphcore/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/utils/__init__.py` & `optimum-graphcore-0.6.1/optimum/graphcore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/optimum/graphcore/version.py` & `optimum-graphcore-0.6.1/optimum/graphcore/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `optimum-graphcore-0.6.0/optimum_graphcore.egg-info/PKG-INFO` & `optimum-graphcore-0.6.1/optimum_graphcore.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-graphcore
-Version: 0.6.0
+Version: 0.6.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://huggingface.co/hardware
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,training,ipu
 Classifier: Development Status :: 3 - Alpha
@@ -17,33 +17,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: quality
 License-File: LICENSE
 
+[![examples](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-examples.yml/badge.svg)](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-examples.yml) [![pipelines](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-pipelines.yml/badge.svg)](https://github.com/huggingface/optimum-graphcore/actions/workflows/test-pipelines.yml)
+
 <p align="center">
     <img src="readme_logo.png" />
 </p>
 
 # Optimum Graphcore
 
 🤗 Optimum Graphcore is the interface between the 🤗 Transformers library and [Graphcore IPUs](https://www.graphcore.ai/products/ipu).
-It provides a set of tools enabling model parallelization and loading on IPUs, training and fine-tuning on all the tasks already supported by Transformers while being compatible with the Hugging Face Hub and every model available on it out of the box.
+It provides a set of tools enabling model parallelization and loading on IPUs, training, fine-tuning and inference on all the tasks already supported by 🤗 Transformers while being compatible with the 🤗 Hub and every model available on it out of the box.
 
 ## What is an Intelligence Processing Unit (IPU)?
 Quote from the Hugging Face [blog post](https://huggingface.co/blog/graphcore#what-is-an-intelligence-processing-unit):
 >IPUs are the processors that power Graphcore’s IPU-POD datacenter compute systems. This new type of processor is designed to support the very specific computational requirements of AI and machine learning. Characteristics such as fine-grained parallelism, low precision arithmetic, and the ability to handle sparsity have been built into our silicon.
 
 > Instead of adopting a SIMD/SIMT architecture like GPUs, Graphcore’s IPU uses a massively parallel, MIMD architecture, with ultra-high bandwidth memory placed adjacent to the processor cores, right on the silicon die.
 
 > This design delivers high performance and new levels of efficiency, whether running today’s most popular models, such as BERT and EfficientNet, or exploring next-generation AI applications.
 
 ## Poplar SDK setup
-A Poplar SDK environment needs to be enabled to use this library. Please refer to Graphcore's [Getting Started](https://docs.graphcore.ai/en/latest/getting-started.html) guide.
+A Poplar SDK environment needs to be enabled to use this library. Please refer to Graphcore's [Getting Started](https://docs.graphcore.ai/en/latest/getting-started.html) guides.
 
 ## Install
 To install the latest release of this package:
 
 `pip install optimum-graphcore`
 
 Optimum Graphcore is a fast-moving project, and you may want to install from source.
@@ -71,17 +73,17 @@
 Please install the requirements for every example:
 
 ```
 cd <example-folder>
 pip install -r requirements.txt
 ```
 
-## How to use it?
+## How to use Optimum Graphcore
 🤗 Optimum Graphcore was designed with one goal in mind: **make training and evaluation straightforward for any 🤗 Transformers user while leveraging the complete power of IPUs.**
-It requires minimal compared to using 🤗 Transformers.
+It requires minimal changes if you are already using 🤗 Transformers.
 
 To immediately use a model on a given input (text, image, audio, ...), we support the `pipeline` API:
 
 ```diff
 ->>> from transformers import pipeline
 +>>> from optimum.graphcore import pipeline
 
@@ -117,28 +119,30 @@
      model=model,
 +    ipu_config=ipu_config,
      args=training_args,
      train_dataset=train_dataset if training_args.do_train else None,
      ...  # Other arguments
 ```
 
-For more information, check our [documentation](https://huggingface.co/docs/optimum/graphcore_index)
+For more information, refer to the full [🤗 Optimum Graphcore documentation](https://huggingface.co/docs/optimum/graphcore_index).
 
-## Supported Models
+## Supported models
 The following model architectures and tasks are currently supported by 🤗 Optimum Graphcore:
-|            | Pre-Training | Masked LM | Causal LM | Seq2Seq LM (Summarization, Translation, etc) | Text Classification | Token Classification | Question Answering | Multiple Choice | Image Classification |
-|------------|--------------|-----------|-----------|----------------------------------------------|-------------------------|----------------------|--------------------|-----------------|----------------------|
-| BART       | ✅            |           | ❌         | ✅                                            | ✅                       |                      | ❌                  |                 |                      |
-| BERT       | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| ConvNeXt   | ✅            |           |           |                                              |                         |                      |                    |                 | ✅                    |
-| DeBERTa    | ✅            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  |                 |                      |
-| DistilBERT | ❌            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| GPT-2      | ✅            |           | ✅         |                                              | ✅                       | ✅                    |                    |                 |                      |
-| [GroupBERT](https://arxiv.org/abs/2106.05822)   | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| HuBERT     | ❌            |           |           |                                              | ✅                       |                      |                    |                 |                      |
-| LXMERT     | ❌            |           |           |                                              |                         |                      | ✅                  |                 |                      |
-| RoBERTa    | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |
-| T5         | ✅            |           |           | ✅                                            |                         |                      |                    |                 |                      |
-| ViT        | ❌            |           |           |                                              |                         |                      |                    |                 | ✅                    |
-| Wav2Vec2   | ✅            |           |           |                                              |                         |                      |                    |                 |                      |
+|            | Pre-Training | Masked LM | Causal LM | Seq2Seq LM (Summarization, Translation, etc) | Sequence Classification | Token Classification | Question Answering | Multiple Choice | Image Classification | CTC |
+|------------|--------------|-----------|-----------|----------------------------------------------|-------------------------|----------------------|--------------------|-----------------|----------------------| ------------ |
+| BART       | ✅            |           | ❌         | ✅                                            | ✅                       |                      | ❌                  |                 |                      |             |
+| BERT       | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| ConvNeXt   | ✅            |           |           |                                              |                         |                      |                    |                 | ✅                    |             |
+| DeBERTa    | ✅            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  |                 |                      |             |
+| DistilBERT | ❌            | ✅         |           |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| GPT-2      | ✅            |           | ✅         |                                              | ✅                       | ✅                    |                    |                 |                      |             |
+| [GroupBERT](https://arxiv.org/abs/2106.05822)   | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| HuBERT     | ❌            |           |           |                                              | ✅                       |                      |                    |                 |                      |       ✅      |
+| LXMERT     | ❌            |           |           |                                              |                         |                      | ✅                  |                 |                      |             |
+| RoBERTa    | ✅            | ✅         | ❌         |                                              | ✅                       | ✅                    | ✅                  | ✅               |                      |             |
+| T5         | ✅            |           |           | ✅                                            |                         |                      |                    |                 |                      |             |
+| ViT        | ❌            |           |           |                                              |                         |                      |                    |                 | ✅                    |             |
+| Wav2Vec2   | ✅            |           |           |                                              |                         |                      |                    |                 |                      |      ✅        |
+| Whisper   |    ❌          |           |           |                    ✅                           |                          |                      |                    |                 |                      |              |
+
 
 If you find any issue while using those, please open an issue or a pull request.
```

### Comparing `optimum-graphcore-0.6.0/optimum_graphcore.egg-info/SOURCES.txt` & `optimum-graphcore-0.6.1/optimum_graphcore.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 optimum/graphcore/__init__.py
-optimum/graphcore/generation_utils.py
 optimum/graphcore/ipu_configuration.py
 optimum/graphcore/modelcard.py
 optimum/graphcore/modeling_utils.py
 optimum/graphcore/trainer.py
 optimum/graphcore/trainer_pt_utils.py
 optimum/graphcore/trainer_seq2seq.py
 optimum/graphcore/trainer_utils.py
@@ -23,14 +22,19 @@
 optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
 optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
 optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
 optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
 optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
 optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
 optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
+optimum/graphcore/generation/__init__.py
+optimum/graphcore/generation/attention_mixin.py
+optimum/graphcore/generation/logits_process.py
+optimum/graphcore/generation/on_device_generation.py
+optimum/graphcore/generation/utils.py
 optimum/graphcore/models/__init__.py
 optimum/graphcore/models/bart/__init__.py
 optimum/graphcore/models/bart/modeling_bart.py
 optimum/graphcore/models/bert/__init__.py
 optimum/graphcore/models/bert/bert_fused_attention.py
 optimum/graphcore/models/bert/modeling_bert.py
 optimum/graphcore/models/convnext/__init__.py
@@ -49,26 +53,30 @@
 optimum/graphcore/models/groupbert/groupbert_ffn.py
 optimum/graphcore/models/groupbert/modeling_groupbert.py
 optimum/graphcore/models/hubert/__init__.py
 optimum/graphcore/models/hubert/ipu_layer_drop.py
 optimum/graphcore/models/hubert/modeling_hubert.py
 optimum/graphcore/models/lxmert/__init__.py
 optimum/graphcore/models/lxmert/modeling_lxmert.py
+optimum/graphcore/models/mt5/__init__.py
+optimum/graphcore/models/mt5/modeling_mt5.py
 optimum/graphcore/models/roberta/__init__.py
 optimum/graphcore/models/roberta/modeling_roberta.py
 optimum/graphcore/models/t5/__init__.py
 optimum/graphcore/models/t5/modeling_t5.py
 optimum/graphcore/models/vit/__init__.py
 optimum/graphcore/models/vit/modeling_vit.py
 optimum/graphcore/models/wav2vec2/__init__.py
 optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
 optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
 optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
 optimum/graphcore/models/whisper/__init__.py
+optimum/graphcore/models/whisper/feature_extraction_whisper.py
 optimum/graphcore/models/whisper/modeling_whisper.py
+optimum/graphcore/models/whisper/processing_whisper.py
 optimum/graphcore/pipelines/__init__.py
 optimum/graphcore/pipelines/fill_mask.py
 optimum/graphcore/pipelines/text2text_generation.py
 optimum/graphcore/pipelines/token_classification.py
 optimum/graphcore/pipelines/zero_shot_classification.py
 optimum/graphcore/utils/__init__.py
 optimum_graphcore.egg-info/PKG-INFO
@@ -77,9 +85,10 @@
 optimum_graphcore.egg-info/not-zip-safe
 optimum_graphcore.egg-info/requires.txt
 optimum_graphcore.egg-info/top_level.txt
 tests/test_examples.py
 tests/test_examples_match_transformers.py
 tests/test_ipu_configuration.py
 tests/test_modeling_common.py
+tests/test_modeling_utils.py
 tests/test_pipelined_models.py
 tests/test_trainer.py
```

### Comparing `optimum-graphcore-0.6.0/pyproject.toml` & `optimum-graphcore-0.6.1/optimum/graphcore/generation/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-#  Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-[tool.black]
-line-length = 119
-target-version = ['py38']
+from .attention_mixin import IPUAttentionMixin
+from .utils import IPUGenerationMixin, supports_kv_cache
```

### Comparing `optimum-graphcore-0.6.0/setup.cfg` & `optimum-graphcore-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/setup.py` & `optimum-graphcore-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 INSTALL_REQUIRES = [
     "transformers==4.25.1",
     "optimum==1.6.1",
     "diffusers[torch]==0.12.1",
     "datasets",
     "tokenizers",
-    "torch",
+    "typeguard",
     "sentencepiece",
     "scipy",
     "pillow",
 ]
 
 QUALITY_REQUIRES = [
     "black",
```

### Comparing `optimum-graphcore-0.6.0/tests/test_examples.py` & `optimum-graphcore-0.6.1/tests/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     NUM_EPOCHS = 1
     LEARNING_RATE = 1e-4
     TRAIN_BATCH_SIZE = 2
     EVAL_BATCH_SIZE = 2
     INFERENCE_DEVICE_ITERATIONS = 4
     GRADIENT_ACCUMULATION_STEPS = 64
     EXTRA_COMMAND_LINE_ARGUMENTS = None
-    POD_TYPE = "pod8"
+    N_IPU = 8
 
     def setUp(self):
         self._create_venv()
 
     def tearDown(self):
         self._remove_venv()
 
@@ -282,15 +282,15 @@
             f"--ipu_config_overrides {ipu_config_overrides}",
             f" --num_train_epochs {num_epochs}",
             "--dataloader_num_workers 16",
             "--pad_on_batch_axis",
             "--save_steps -1",
             "--save_total_limit 1",
             "--report_to none",
-            f"--pod_type {self.POD_TYPE}",
+            f"--n_ipu {self.N_IPU}",
         ]
         if dataset_config_name is not None:
             cmd_line.append(f"--dataset_config_name {dataset_config_name}")
 
         if extra_command_line_arguments is not None:
             cmd_line += extra_command_line_arguments
 
@@ -548,24 +548,25 @@
 
 class SpeechRecognitionExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_speech_recognition_ctc"
 ):
     TASK_NAME = "common_voice"
     DATASET_CONFIG_NAME = "tr"
     TRAIN_BATCH_SIZE = 1
-    GRADIENT_ACCUMULATION_STEPS = 8
+    GRADIENT_ACCUMULATION_STEPS = 32
     EVAL_BATCH_SIZE = 1
-    NUM_EPOCHS = 15
+    NUM_EPOCHS = 20
     # Here we are evaluating against the loss because it can take a long time to have wer < 1.0
     SCORE_NAME = "eval_loss"
-    EVAL_SCORE_THRESHOLD = 4
+    EVAL_SCORE_THRESHOLD = 6
     EVAL_SCORE_GREATER_IS_BETTER = False
     EXTRA_COMMAND_LINE_ARGUMENTS = [
-        "--learning_rate 3e-4",
+        "--learning_rate 1e-4",
         "--warmup_steps 400",
         "--mask_time_prob 0.0",
         "--layerdrop 0.0",
+        "--weight_decay 0.005",
         "--freeze_feature_encoder",
         "--text_column_name sentence",
         "--length_column_name input_length",
         '--chars_to_ignore , ? . ! - \\; \\: \\" “ % ‘ ” � ',
     ]
```

### Comparing `optimum-graphcore-0.6.0/tests/test_examples_match_transformers.py` & `optimum-graphcore-0.6.1/tests/test_examples_match_transformers.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/tests/test_ipu_configuration.py` & `optimum-graphcore-0.6.1/tests/test_ipu_configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,112 +10,85 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import random
+import re
 import string
 import unittest
 from collections.abc import Iterable
 from typing import Any, Dict, Optional, Set
 
 import pytest
 
 from optimum.graphcore import IPUConfig
-from optimum.graphcore.ipu_configuration import ALLOWED_POD_TYPES
-from optimum.graphcore.modeling_utils import (
-    IncompatibleIPUConfigError,
-    get_layer_ipu,
-    split_encoder_decoder_ipu_config,
-)
+from optimum.graphcore.ipu_configuration import IncompatibleIPUConfigError
+from optimum.graphcore.modeling_utils import get_layer_ipu, split_encoder_decoder_ipu_config
+from parameterized import parameterized
 from poptorch import OutputMode
 
 
-def random_value_from_initial_value(initial_value):
-    if isinstance(initial_value, bool):
-        return bool(random.randint(0, 1))
-    elif isinstance(initial_value, int):
-        return random.randint(1, 10)
-    elif isinstance(initial_value, float):
-        return random.random()
-    elif isinstance(initial_value, str):
-        return "".join(random.choices(string.ascii_lowercase, k=len(initial_value)))
-    elif isinstance(initial_value, Iterable):
-        return type(initial_value)([random_value_from_initial_value(x) for x in initial_value])
-    elif initial_value is None:
-        return None
-    else:
-        raise TypeError(f"cannot create random value from initial value of type {type(initial_value)}")
-
-
-def create_pod_specific_attribute(
-    initial_value: Any, add_default_value: bool = False, remove_pod_types: Optional[Set[str]] = None
-) -> Dict[str, Any]:
-    p = random.random()
-    if p < 0.5:
-        return initial_value
-    if remove_pod_types is None:
-        remove_pod_types = set()
-    values = {k: random_value_from_initial_value(initial_value) for k in set(ALLOWED_POD_TYPES) - remove_pod_types}
-    if add_default_value:
-        values["default"] = random_value_from_initial_value(initial_value)
-    return values
-
-
-def create_ipu_config(with_default_values: bool = False, remove_pod_types: Optional[Set[str]] = None) -> IPUConfig:
+def create_ipu_config() -> IPUConfig:
     initial_dict = IPUConfig().to_dict()
-    initial_dict = {
-        k: create_pod_specific_attribute(v, add_default_value=with_default_values, remove_pod_types=remove_pod_types)
-        for k, v in initial_dict.items()
-    }
     allowed_output_modes = ["all", "sum", "final"]
-    if isinstance(initial_dict["output_mode"], dict):
-        initial_dict["output_mode"] = {k: random.choice(allowed_output_modes) for k in initial_dict["output_mode"]}
-    else:
-        initial_dict["output_mode"] = random.choice(allowed_output_modes)
+    initial_dict["output_mode"] = random.choice(allowed_output_modes)
     # Setting this setting to False as it is currently not supported and will throw an error.
     initial_dict["execute_encoder_on_cpu_for_generation"] = False
-    # Edge case where replication_factor=1 and replicated_tensor_sharding=True which will get overriden to
-    # replicated_tensor_sharding=False.
-    if isinstance(initial_dict["replication_factor"], dict) and isinstance(
-        initial_dict["replicated_tensor_sharding"], dict
-    ):
-        for pod_type in initial_dict["replication_factor"].keys():
-            if initial_dict["replication_factor"][pod_type] == 1:
-                initial_dict["replicated_tensor_sharding"][pod_type] = False
     return IPUConfig.from_dict(initial_dict)
 
 
+def create_mode_ipu_config(test_attributes: Dict[str, Any], mode):
+    helper_config = IPUConfig()
+    helper_config.mode = mode
+    ipu_config = IPUConfig(
+        **{helper_config._get_managed_attr_mode_name(attr): value for attr, value in test_attributes.items()}
+    )
+    ipu_config.mode = mode
+    return ipu_config
+
+
 class IPUConfigTester(unittest.TestCase):
-    def test_for_pod_type(self):
-        ipu_config = create_ipu_config()
-        for pod_type in ALLOWED_POD_TYPES:
-            pod_type_dict = {k: v[pod_type] if isinstance(v, dict) else v for k, v in ipu_config.to_dict().items()}
-            ipu_config_for_pod_type = ipu_config.for_pod_type(pod_type)
-            self.assertEqual(pod_type_dict, ipu_config_for_pod_type.to_dict())
-
-    def test_for_pod_type_with_default(self):
-        ipu_config = create_ipu_config(with_default_values=True)
-        pod_type_dict = {k: v["default"] if isinstance(v, dict) else v for k, v in ipu_config.to_dict().items()}
-        ipu_config_for_pod_type = ipu_config.for_pod_type()
-        print(pod_type_dict)
-        print(ipu_config_for_pod_type.to_dict())
-        self.assertEqual(pod_type_dict, ipu_config_for_pod_type.to_dict())
+    def test_attribute_default_values(self):
+        # ipus_per_replica should equal to len(layers_per_ipu) if not provided
+        ipu_config = IPUConfig(layers_per_ipu=[1, 2, 3])
+        self.assertEqual(ipu_config.ipus_per_replica, 3)
+
+        # inference_matmul_proportion not specified but matmul_proportion is
+        ipu_config = IPUConfig(
+            layers_per_ipu=[1, 2, 3, 4],
+            matmul_proportion=[0.1, 0.2, 0.3, 0.4],
+        )
+        self.assertEqual(ipu_config.inference_matmul_proportion, [0.1, 0.2, 0.3, 0.4])
 
-    def test_for_pod_type_with_unallowed_pod_type(self):
-        ipu_config = create_ipu_config()
-        with pytest.raises(ValueError):
-            ipu_config.for_pod_type("blablabla")
+        # inference_matmul_proportion not specified but inference_layers_per_ipu != len(matmul_proportion)
+        ipu_config = IPUConfig(
+            layers_per_ipu=[1, 2, 3, 4], matmul_proportion=[0.1, 0.2, 0.3, 0.4], inference_layers_per_ipu=[3, 7]
+        )
+        self.assertEqual(ipu_config.inference_matmul_proportion, 0.2)
+
+        # inference_ipus_per_replica not specified but ipus_per_replica is
+        ipu_config = IPUConfig(
+            ipus_per_replica=10,
+        )
+        self.assertEqual(ipu_config.inference_ipus_per_replica, 10)
 
-    def test_for_pod_type_not_in_config_attribute(self):
-        pod_type_to_remove = random.choice(ALLOWED_POD_TYPES)
-        ipu_config = create_ipu_config(remove_pod_types={pod_type_to_remove})
-        with pytest.raises(KeyError):
-            ipu_config.for_pod_type(pod_type_to_remove)
+        # inference_ipus_per_replica not specified but inference_layers_per_ipu is
+        ipu_config = IPUConfig(ipus_per_replica=10, inference_layers_per_ipu=[1, 2, 3])
+        self.assertEqual(ipu_config.inference_ipus_per_replica, 3)
+
+        # If the user has not provided either {projection/embedding}_serialization_factor
+        # or serialized_{projection/embedding}_splits_per_ipu, {projection/embedding}_serialization_factor}
+        # should default to 1
+        ipu_config = IPUConfig()
+        self.assertEqual(ipu_config.projection_serialization_factor, 1)
+        self.assertEqual(ipu_config.inference_projection_serialization_factor, 1)
+        self.assertEqual(ipu_config.embedding_serialization_factor, 1)
+        self.assertEqual(ipu_config.inference_embedding_serialization_factor, 1)
 
     def _test_to_options(self, for_inference: bool):
         def make_poptorch_options_comparable_to_ipu_config(options_dict):
             options_dict = copy.deepcopy(options_dict)
             # mapping specifies how to transform an options dict entry to something that can be compared to an IPUConfig.
             # It maps a string to either another string or a function:
             #   1. String -> string: it specifies how to align values for attribute names that differ between
@@ -163,65 +136,49 @@
         def intersection_of_dicts(d1, d2):
             d1 = copy.deepcopy(d1)
             d2 = copy.deepcopy(d2)
             d1 = {k: v for k, v in d1.items() if k in d2}
             d2 = {k: v for k, v in d2.items() if k in d1}
             return d1, d2
 
-        pod_type = random.choice(ALLOWED_POD_TYPES)
-        # Case 1: the IPUConfig is not "specialized" and contains values for many pod types.
         ipu_config = create_ipu_config()
-        options = ipu_config.to_options(for_inference=for_inference, pod_type=pod_type)
-        ipu_config_dict = ipu_config.for_pod_type(pod_type).to_dict()
-        if for_inference:
-            ipu_config_dict["replication_factor"] = ipu_config_dict["inference_replication_factor"]
-            ipu_config_dict["device_iterations"] = ipu_config_dict["inference_device_iterations"]
-            ipu_config_dict["gradient_accumulation_steps"] = 1
-            ipu_config_dict["output_mode"] = "all"
-        ipu_config_dict, options_dict = intersection_of_dicts(
-            ipu_config_dict, make_poptorch_options_comparable_to_ipu_config(options.toDict())
-        )
-        self.assertEqual(ipu_config_dict, options_dict)
-        # Case 2: the IPUConfig is specialized, no pod type needs to be specified to create the poptorch.Options.
-        ipu_config = create_ipu_config().for_pod_type(pod_type)
         options = ipu_config.to_options(for_inference=for_inference)
         ipu_config_dict = ipu_config.to_dict()
         if for_inference:
             ipu_config_dict["replication_factor"] = ipu_config_dict["inference_replication_factor"]
             ipu_config_dict["device_iterations"] = ipu_config_dict["inference_device_iterations"]
+            ipu_config_dict["matmul_proportion"] = ipu_config_dict["inference_matmul_proportion"]
             ipu_config_dict["gradient_accumulation_steps"] = 1
             ipu_config_dict["output_mode"] = "all"
         ipu_config_dict, options_dict = intersection_of_dicts(
             ipu_config_dict, make_poptorch_options_comparable_to_ipu_config(options.toDict())
         )
         self.assertEqual(ipu_config_dict, options_dict)
 
     def test_to_options(self):
         return self._test_to_options(False)
 
     def test_to_options_for_inference(self):
         return self._test_to_options(True)
 
     def _test_batch_size_factor(self, for_inference: bool):
-        pod_type = random.choice(ALLOWED_POD_TYPES)
         # Case 1: the IPUConfig is not "specialized" and contains values for many pod types.
         ipu_config = create_ipu_config()
-        batch_size_factor = ipu_config.batch_size_factor(for_inference=for_inference, pod_type=pod_type)
-        ipu_config = ipu_config.for_pod_type(pod_type)
+        batch_size_factor = ipu_config.batch_size_factor(for_inference=for_inference)
         replication_factor = (
             ipu_config.inference_replication_factor if for_inference else ipu_config.replication_factor
         )
         gradient_accumulation_steps = 1 if for_inference else ipu_config.gradient_accumulation_steps
         device_iterations = ipu_config.inference_device_iterations if for_inference else ipu_config.device_iterations
         self.assertEqual(
             replication_factor * gradient_accumulation_steps * device_iterations,
             batch_size_factor,
         )
         # Case 2: the IPUConfig is specialized, no pod type needs to be specified to compute the batch size factor.
-        ipu_config = create_ipu_config().for_pod_type(pod_type)
+        ipu_config = create_ipu_config()
         batch_size_factor = ipu_config.batch_size_factor(for_inference=for_inference)
         replication_factor = (
             ipu_config.inference_replication_factor if for_inference else ipu_config.replication_factor
         )
         gradient_accumulation_steps = 1 if for_inference else ipu_config.gradient_accumulation_steps
         device_iterations = ipu_config.inference_device_iterations if for_inference else ipu_config.device_iterations
         self.assertEqual(
@@ -263,24 +220,18 @@
         with pytest.raises(
             IncompatibleIPUConfigError,
             match="layers_per_ipu does not define the correct number of layers for the current model",
         ):
             layer_ipu = get_layer_ipu(ipu_config, 4)
 
         # layers_per_ipu and ipus_per_replica mismatch raises
-        ipu_config = IPUConfig(layers_per_ipu=[1, 2], ipus_per_replica=4)
-        with pytest.raises(
-            IncompatibleIPUConfigError,
-            match=r"layers_per_ipu has non-default value set, but its length does not match ipus_per_replica",
-        ):
-            layer_ipu = get_layer_ipu(ipu_config, 3)
         ipu_config = IPUConfig(layers_per_ipu=[1, -1], ipus_per_replica=4)
         with pytest.raises(
             IncompatibleIPUConfigError,
-            match=r"layers_per_ipu has non-default value set, but its length does not match ipus_per_replica",
+            match=r"layers_per_ipu has a non-default value set, but its length does not match ipus_per_replica",
         ):
             layer_ipu = get_layer_ipu(ipu_config, 3)
 
         # Default config everything should be on single IPU
         ipu_config = IPUConfig()
         layer_ipu = get_layer_ipu(ipu_config, 9)
         self.assertEqual(layer_ipu, [0] * 9)
@@ -299,22 +250,14 @@
         ipu_config = IPUConfig(layers_per_ipu=[-1, 2])
         layer_ipu = get_layer_ipu(ipu_config, 6)
         self.assertEqual(layer_ipu, [0, 0, 0, 0, 1, 1])
         ipu_config = IPUConfig(layers_per_ipu=[-1, 2, -1, 2])
         layer_ipu = get_layer_ipu(ipu_config, 7)
         self.assertEqual(layer_ipu, [0, 1, 1, 2, 2, 3, 3])
 
-        # Invalid values
-        ipu_config = IPUConfig(layers_per_ipu=[2, -2])
-        with pytest.raises(IncompatibleIPUConfigError, match=r"Invalid values in layers_per_ipu"):
-            layer_ipu = get_layer_ipu(ipu_config, 6)
-        ipu_config = IPUConfig(ipus_per_replica=0)
-        with pytest.raises(IncompatibleIPUConfigError, match=r"Invalid value for ipus_per_replica"):
-            layer_ipu = get_layer_ipu(ipu_config, 6)
-
     def test_split_encoder_decoder_ipu_config(self):
         # Test splitting two IPUs
         ipu_config = IPUConfig(layers_per_ipu=[1, 2])
         e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 1, 2)
         self.assertEqual(e_ipu_config.layers_per_ipu, [1])
         self.assertEqual(e_ipu_config.ipus_per_replica, 1)
         self.assertEqual(d_ipu_config.layers_per_ipu, [2])
@@ -322,22 +265,40 @@
 
         # Test splitting matmul_proportion
         ipu_config = IPUConfig(layers_per_ipu=[2, 2, 2, 2], matmul_proportion=[0.1, 0.2, 0.3, 0.4])
         e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 4, 4)
         self.assertEqual(e_ipu_config.matmul_proportion, [0.1, 0.2])
         self.assertEqual(d_ipu_config.matmul_proportion, [0.3, 0.4])
 
+        # For generation using encoder decoder models and layers `SplitProjection`
+        # and `SerializedEmbedding` placed on different IPUs, cannot
+        # have serialized_{linear/embedding}_splits_per_ipu present in
+        # both the encoder and decoder
+        with pytest.raises(ValueError, match=f"must have all splits placed on the"):
+            failing_ipu_config = IPUConfig(
+                layers_per_ipu=[0, 2, 2, 0], serialized_projection_splits_per_ipu=[0, 2, 2, 0]
+            )
+            split_encoder_decoder_ipu_config(failing_ipu_config, 2, 2)
+
+        with pytest.raises(ValueError, match=f"must have all splits placed on the"):
+            failing_ipu_config = IPUConfig(
+                layers_per_ipu=[0, 2, 2, 0], serialized_embedding_splits_per_ipu=[0, 2, 2, 0]
+            )
+            split_encoder_decoder_ipu_config(failing_ipu_config, 2, 2)
+
         # Test that all the other values from the original ipu_config are intact
         ipu_config = ipu_config.to_dict()
         e_ipu_config = e_ipu_config.to_dict()
         d_ipu_config = d_ipu_config.to_dict()
+        skip = {"layers_per_ipu", "ipus_per_replica", "matmul_proportion"}
         for k in ipu_config.keys():
-            if k not in {"layers_per_ipu", "ipus_per_replica", "matmul_proportion"}:
-                self.assertEqual(ipu_config[k], e_ipu_config[k])
-                self.assertEqual(ipu_config[k], d_ipu_config[k])
+            if re.search("|".join(skip), k):
+                continue
+            self.assertEqual(ipu_config[k], e_ipu_config[k], k)
+            self.assertEqual(ipu_config[k], d_ipu_config[k], k)
 
         # Test that wildcards work
         ipu_config = IPUConfig(layers_per_ipu=[-1, -1])
         e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 2, 3)
         self.assertEqual(e_ipu_config.layers_per_ipu, [2])
         self.assertEqual(d_ipu_config.layers_per_ipu, [3])
 
@@ -348,23 +309,23 @@
             match=r"layers_per_ipu does not define the correct number of layers for the current model",
         ):
             e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 2, 2)
 
         # Encoder and decoder layers defined on same IPU should raise an exception
         ipu_config = IPUConfig(layers_per_ipu=[4, 3])
         with pytest.raises(
-            IncompatibleIPUConfigError, match=r"Unable to find valid split of ipu_config.layers_per_ipu"
+            IncompatibleIPUConfigError, match=r"Unable to find a valid split of ipu_config.layers_per_ipu"
         ):
             e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 3, 4)
 
         # If ipu_config only has 1 IPU then it should raise and exception
         ipu_config = IPUConfig(layers_per_ipu=[4])
         with pytest.raises(
             IncompatibleIPUConfigError,
-            match=r"Need ipus_per_replica of at least 2 to split ipu_config into encoder and decoder configs",
+            match=r"Need ipus_per_replica to be at least 2 to split ipu_config into encoder and decoder configs",
         ):
             e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 2, 2)
 
         # Handle empty IPU in last stage of encoder
         ipu_config = IPUConfig(layers_per_ipu=[1, 2, 3, 0, 5, 6, 7, 8])
         e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 6, 26)
         self.assertEqual(e_ipu_config.layers_per_ipu, [1, 2, 3, 0])
@@ -383,7 +344,192 @@
         # Split where there are many zeros
         ipu_config = IPUConfig(layers_per_ipu=[3, 0, 3, 0, 0, 7])
         e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 6, 7)
         self.assertEqual(e_ipu_config.layers_per_ipu, [3, 0, 3, 0])
         self.assertEqual(e_ipu_config.ipus_per_replica, 4)
         self.assertEqual(d_ipu_config.layers_per_ipu, [0, 7])
         self.assertEqual(d_ipu_config.ipus_per_replica, 2)
+
+
+class IPUConfigExecutionModeTester(unittest.TestCase):
+    def test_mode_set(self):
+        # Default mode should be training
+        config = IPUConfig()
+        self.assertEqual(config.mode, "training")
+
+        # Set with convenience methods
+        config.train()
+        self.assertEqual(config.mode, "training")
+        config.eval()
+        self.assertEqual(config.mode, "inference")
+
+        # Set with invalid mode value
+        with pytest.raises(ValueError, match="`IPUConfig` mode can only take"):
+            config.mode = "invalid"
+
+    @parameterized.expand(
+        (
+            (attr, test_value, mode)
+            for mode in IPUConfig.modes
+            for attr, test_value in {
+                "layers_per_ipu": [1, 2, 3, 4],
+                "matmul_proportion": 0.6,
+                "ipus_per_replica": 4,
+                "serialized_projection_splits_per_ipu": [4],
+                "serialized_embedding_splits_per_ipu": [4],
+                "projection_serialization_factor": 4,
+                "embedding_serialization_factor": 4,
+            }.items()
+        )
+    )
+    def test_attr_mode_retrieval(self, attr, value, mode):
+        ipu_config = create_mode_ipu_config({attr: value}, mode)
+        self.assertEqual(getattr(ipu_config, f"_{attr}"), value)
+
+    @parameterized.expand((mode for mode in IPUConfig.modes))
+    def test_layers_per_ipu_wildcard(self, mode):
+        ipu_config = create_mode_ipu_config({"ipus_per_replica": 4, "layers_per_ipu": [-1]}, mode=mode)
+        layer_ipu = get_layer_ipu(ipu_config, 8)
+        self.assertEqual(ipu_config._ipus_per_replica, 4)
+        self.assertEqual(layer_ipu, [0, 0, 1, 1, 2, 2, 3, 3])
+
+    @parameterized.expand((mode for mode in IPUConfig.modes))
+    def test_split_encoder_decoder_ipu_config(self, mode):
+        ipu_config = create_mode_ipu_config(
+            {
+                "layers_per_ipu": [1, 2, 3, 4],
+                "matmul_proportion": [0.1, 0.2, 0.3, 0.4],
+                "ipus_per_replica": 4,
+                "serialized_projection_splits_per_ipu": [0, 0, 2, 2],
+                "serialized_embedding_splits_per_ipu": [2, 2, 0, 0],
+            },
+            mode,
+        )
+
+        e_ipu_config, d_ipu_config = split_encoder_decoder_ipu_config(ipu_config, 3, 7)
+
+        self.assertEqual(e_ipu_config._layers_per_ipu, [1, 2])
+        self.assertEqual(e_ipu_config._ipus_per_replica, 2)
+        self.assertEqual(e_ipu_config._matmul_proportion, [0.1, 0.2])
+        self.assertEqual(e_ipu_config._serialized_projection_splits_per_ipu, None)
+        self.assertEqual(e_ipu_config._serialized_embedding_splits_per_ipu, [2, 2])
+
+        self.assertEqual(d_ipu_config._layers_per_ipu, [3, 4])
+        self.assertEqual(d_ipu_config._ipus_per_replica, 2)
+        self.assertEqual(d_ipu_config._matmul_proportion, [0.3, 0.4])
+        self.assertEqual(d_ipu_config._serialized_projection_splits_per_ipu, [2, 2])
+        self.assertEqual(d_ipu_config._serialized_embedding_splits_per_ipu, None)
+
+
+class IPUConfigAttributeValidationTester(unittest.TestCase):
+    @parameterized.expand(
+        (
+            (attr, test_value, mode)
+            for mode in IPUConfig.modes
+            for attr, test_value in {
+                "layers_per_ipu": [-1],
+                "matmul_proportion": [0.2, 0.3, 0.0, 0.4],
+                "replication_factor": 1,
+                "gradient_accumulation_steps": 1,
+                "ipus_per_replica": 1,
+                "embedding_serialization_factor": 1,
+                "device_iterations": 1,
+                "projection_serialization_factor": 1,
+                "embedding_serialization_factor": 1,
+            }.items()
+        )
+    )
+    def test_contents_geq_value_validator(self, attr, value, mode):
+        ipu_config = IPUConfig()
+        ipu_config.mode = mode
+        attr = ipu_config._get_managed_attr_mode_name(attr)
+        setattr(ipu_config, attr, value)
+
+        with pytest.raises(ValueError, match=f"`IPUConfig` attribute `{attr}` must .* >="):
+            if isinstance(value, list):
+                argmin = min(enumerate(value), key=lambda x: x[1])[0]
+                value[argmin] -= 1
+            else:
+                value -= 1
+            setattr(ipu_config, attr, value)
+
+    def test_output_mode_validator(self):
+        with pytest.raises(ValueError):
+            IPUConfig(output_mode="invalid")
+        # should not raise
+        allowed_output_modes = ("all", "sum", "final", "default")
+        for output_mode in allowed_output_modes:
+            with self.subTest(output_mode=output_mode):
+                IPUConfig(output_mode=output_mode)
+
+    @parameterized.expand(
+        (serialized_layer, mode) for mode in IPUConfig.modes for serialized_layer in ("projection", "embedding")
+    )
+    def test_serialized_splits_per_ipu_validator(self, layer, mode):
+        # Must be of type List[int>=0]
+        ipu_config = IPUConfig()
+        ipu_config.mode = mode
+        serialized_mode_layer = ipu_config._get_managed_attr_mode_name(f"serialized_{layer}_splits_per_ipu")
+        with pytest.raises(ValueError, match=f"`IPUConfig` attribute `{serialized_mode_layer}` must .* >="):
+            setattr(ipu_config, serialized_mode_layer, [0, 2, 2, -1])
+
+        # Must have atleast 1 split if the pipeline is provided
+        with pytest.raises(
+            ValueError,
+            match=re.escape(f"`IPUConfig` attribute `{serialized_mode_layer}=[0, 0]` must have atleast 1 split"),
+        ):
+            setattr(ipu_config, serialized_mode_layer, [0, 0])
+
+        # Splits should be on consecutive IPUs
+        with pytest.raises(
+            ValueError,
+            match=re.escape(f"`IPUConfig` attribute `{serialized_mode_layer}=[0, 3, 0, 2]` must have its splits on"),
+        ):
+            setattr(ipu_config, serialized_mode_layer, [0, 3, 0, 2])
+
+    @parameterized.expand((mode for mode in IPUConfig.modes))
+    def test_validate_ipu_config(self, mode):
+        with self.subTest(
+            "if *matmul_proportion is a List[float], it must use the same number of IPUs as *ipus_per_replica"
+        ):
+            ipus_per_replica = 4
+            matmul_proportion = [0.2] * (ipus_per_replica + 1)
+            with pytest.raises(
+                IncompatibleIPUConfigError,
+                match=re.escape(f"matmul_proportion={matmul_proportion} should use the same number"),
+            ):
+                create_mode_ipu_config(
+                    {"ipus_per_replica": ipus_per_replica, "matmul_proportion": matmul_proportion}, mode
+                )
+                IPUConfig(ipus_per_replica=ipus_per_replica, matmul_proportion=matmul_proportion)
+
+        with self.subTest(
+            "If there are no wildcards in *layers_per_ipu, the pipeline length should equal *ipus_per_replica"
+        ):
+            layers_per_ipu = [2] * (ipus_per_replica + 1)
+            with pytest.raises(
+                IncompatibleIPUConfigError,
+                match=re.escape(f"layers_per_ipu={layers_per_ipu} should use the same number"),
+            ):
+                create_mode_ipu_config({"ipus_per_replica": ipus_per_replica, "layers_per_ipu": layers_per_ipu}, mode)
+
+        # The user cannot provide both {projection/embedding}_serialization_factor and
+        # serialized_{projection/embedding}_splits_per_ipu
+        for layer in ("projection", "embedding"):
+            with self.subTest(
+                f"The user cannot provide both {layer}_serialization_factor" f" and serialized_{layer}_splits_per_ipu."
+            ):
+                with pytest.raises(ValueError, match=f"Only one of .*{layer}.*"):
+                    create_mode_ipu_config(
+                        {f"{layer}_serialization_factor": 2, f"serialized_{layer}_splits_per_ipu": [1, 1]}, mode
+                    )
+
+            with self.subTest(
+                f"The pipeline length of serialized_{layer}_splits_per_ipu must equal"
+                " the number of IPUs specified by IPUs per replica."
+            ):
+                with pytest.raises(
+                    ValueError, match=f".*{layer}.*=\\[0, 0, 1, 1\\] should use the same number of IPUs as"
+                ):
+                    create_mode_ipu_config(
+                        {"ipus_per_replica": 8, f"serialized_{layer}_splits_per_ipu": [0, 0, 1, 1]}, mode
+                    )
```

### Comparing `optimum-graphcore-0.6.0/tests/test_modeling_common.py` & `optimum-graphcore-0.6.1/tests/test_modeling_common.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.0/tests/test_pipelined_models.py` & `optimum-graphcore-0.6.1/tests/test_pipelined_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     def _generate_input_for_model_class(self, model_name_or_path, model_class):
         # TODO: add support for labels.
         inputs = None
         extractor = None
         if model_class in [
             *MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING.values(),
             *MODEL_FOR_AUDIO_CLASSIFICATION_MAPPING.values(),
+            *MODEL_FOR_CTC_MAPPING.values(),
         ]:
             extractor = AutoFeatureExtractor.from_pretrained(model_name_or_path)
         else:
             extractor = AutoTokenizer.from_pretrained(model_name_or_path)
         if model_class in MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING.values():
             encoder_input_text = "This is the text that is going to be fed to the encoder."
             decoder_input_text = "This is part, on the other end, will be fed to the decoder."
```

### Comparing `optimum-graphcore-0.6.0/tests/test_trainer.py` & `optimum-graphcore-0.6.1/tests/test_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import tempfile
 import unittest
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 
-from huggingface_hub import HfFolder, Repository, delete_repo, set_access_token
+from huggingface_hub import HfFolder, Repository, delete_repo
 from optimum.graphcore import IPUConfig, IPUTrainingArguments
 from optimum.utils import logging
 from requests.exceptions import HTTPError
 from transformers import AutoTokenizer, IntervalStrategy, PretrainedConfig, is_torch_available
 from transformers.file_utils import WEIGHTS_NAME
 from transformers.testing_utils import (
     ENDPOINT_STAGING,
@@ -576,15 +576,15 @@
         trainer.train()
         # Setting fp32 to True because that is what is being done in get_regression_trainer.
         args = IPUTrainingArguments("./regression", report_to=[], fp32=True)
         dict1, dict2 = args.to_dict(), trainer.args.to_dict()
         for key in dict1.keys():
             # Logging dir can be slightly different as they default to something with the time.
             if key != "logging_dir":
-                self.assertEqual(dict1[key], dict2[key])
+                self.assertEqual(dict1[key], dict2[key], f"{key=}: {dict1[key]=} != {dict2[key]=}")
 
     def test_number_of_steps_in_training(self):
         # Regular training has n_epochs * len(train_dl) steps
         trainer = get_regression_trainer(learning_rate=0.1)
         train_output = trainer.train()
         combined_batch_size = get_ipu_config().batch_size_factor() * self.batch_size
         self.assertEqual(train_output.global_step, self.n_epochs * TRAIN_LEN / combined_batch_size)
@@ -1308,15 +1308,14 @@
 
 @require_torch
 @is_staging_test
 class IPUTrainerIntegrationWithHubTester(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls._token = TOKEN
-        set_access_token(TOKEN)
         HfFolder.save_token(TOKEN)
 
     @classmethod
     def tearDownClass(cls):
         for model in ["test-trainer", "test-trainer-epoch", "test-trainer-step"]:
             try:
                 delete_repo(token=cls._token, name=model)
```

