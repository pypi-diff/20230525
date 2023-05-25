# Comparing `tmp/penn-0.0.7.tar.gz` & `tmp/penn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penn-0.0.7.tar", last modified: Thu Apr 27 12:33:40 2023, max compression
+gzip compressed data, was "penn-0.0.8.tar", last modified: Thu May 25 18:20:02 2023, max compression
```

## Comparing `penn-0.0.7.tar` & `penn-0.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.198188 penn-0.0.7/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1078 2023-04-24 20:20:15.000000 penn-0.0.7/LICENSE
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10415 2023-04-27 12:33:40.198188 penn-0.0.7/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9968 2023-04-24 20:20:15.000000 penn-0.0.7/README.md
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.190188 penn-0.0.7/penn/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      988 2023-04-24 20:20:15.000000 penn-0.0.7/penn/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2343 2023-04-24 20:20:15.000000 penn-0.0.7/penn/__main__.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.190188 penn-0.0.7/penn/assets/
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.190188 penn-0.0.7/penn/assets/partitions/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4204 2023-04-24 20:20:15.000000 penn-0.0.7/penn/assets/partitions/mdb.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    84988 2023-04-24 20:20:15.000000 penn-0.0.7/penn/assets/partitions/ptdb.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2293 2023-04-24 20:20:15.000000 penn-0.0.7/penn/checkpoint.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/config/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-24 20:20:15.000000 penn-0.0.7/penn/config/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4082 2023-04-24 20:20:15.000000 penn-0.0.7/penn/config/defaults.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1385 2023-04-24 20:20:15.000000 penn-0.0.7/penn/config/static.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2207 2023-04-24 20:20:15.000000 penn-0.0.7/penn/convert.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    14526 2023-04-24 20:20:15.000000 penn-0.0.7/penn/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/data/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      133 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     6876 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/dataset.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/data/download/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/download/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      561 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/download/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1851 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/download/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1022 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/loader.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/data/preprocess/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/preprocess/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      580 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/preprocess/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     6918 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/preprocess/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2790 2023-04-24 20:20:15.000000 penn-0.0.7/penn/data/sampler.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4886 2023-04-24 20:20:15.000000 penn-0.0.7/penn/decode.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/dsp/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       37 2023-04-24 20:20:15.000000 penn-0.0.7/penn/dsp/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2944 2023-04-24 20:20:15.000000 penn-0.0.7/penn/dsp/dio.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8978 2023-04-24 20:20:15.000000 penn-0.0.7/penn/dsp/pyin.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/evaluate/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       85 2023-04-24 20:20:15.000000 penn-0.0.7/penn/evaluate/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      874 2023-04-24 20:20:15.000000 penn-0.0.7/penn/evaluate/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    18545 2023-04-24 20:20:15.000000 penn-0.0.7/penn/evaluate/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     7562 2023-04-24 20:20:15.000000 penn-0.0.7/penn/evaluate/metrics.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      366 2023-04-24 20:20:15.000000 penn-0.0.7/penn/load.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/model/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      361 2023-04-24 20:20:15.000000 penn-0.0.7/penn/model/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      234 2023-04-24 20:20:15.000000 penn-0.0.7/penn/model/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2681 2023-04-24 20:20:15.000000 penn-0.0.7/penn/model/crepe.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2969 2023-04-24 20:20:15.000000 penn-0.0.7/penn/model/deepf0.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1747 2023-04-24 20:20:15.000000 penn-0.0.7/penn/model/fcnf0.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/partition/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/partition/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      562 2023-04-24 20:20:15.000000 penn-0.0.7/penn/partition/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      956 2023-04-24 20:20:15.000000 penn-0.0.7/penn/partition/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1177 2023-04-24 20:20:15.000000 penn-0.0.7/penn/periodicity.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/plot/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       67 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/__init__.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/plot/density/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/density/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1016 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/density/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3485 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/density/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/plot/logits/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/logits/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1029 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/logits/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2881 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/logits/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.194188 penn-0.0.7/penn/plot/threshold/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/threshold/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      926 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/threshold/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1948 2023-04-24 20:20:15.000000 penn-0.0.7/penn/plot/threshold/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1262 2023-04-24 20:20:15.000000 penn-0.0.7/penn/time.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.198188 penn-0.0.7/penn/train/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-24 20:20:15.000000 penn-0.0.7/penn/train/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1274 2023-04-24 20:20:15.000000 penn-0.0.7/penn/train/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9864 2023-04-24 20:20:15.000000 penn-0.0.7/penn/train/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1029 2023-04-25 13:15:56.000000 penn-0.0.7/penn/voicing.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1449 2023-04-24 20:20:15.000000 penn-0.0.7/penn/write.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.190188 penn-0.0.7/penn.egg-info/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10415 2023-04-27 12:33:40.000000 penn-0.0.7/penn.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1440 2023-04-27 12:33:40.000000 penn-0.0.7/penn.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-04-27 12:33:40.000000 penn-0.0.7/penn.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       63 2023-04-27 12:33:40.000000 penn-0.0.7/penn.egg-info/requires.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        5 2023-04-27 12:33:40.000000 penn-0.0.7/penn.egg-info/top_level.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-04-27 12:33:40.198188 penn-0.0.7/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1024 2023-04-27 12:31:52.000000 penn-0.0.7/setup.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-27 12:33:40.198188 penn-0.0.7/test/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      448 2023-04-24 20:20:15.000000 penn-0.0.7/test/test_core.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.447732 penn-0.0.8/
+-rw-r--r--   0 max       (1007) max       (1007)     1078 2023-02-08 13:51:26.000000 penn-0.0.8/LICENSE
+-rw-r--r--   0 max       (1007) max       (1007)    10415 2023-05-25 18:20:02.447732 penn-0.0.8/PKG-INFO
+-rw-r--r--   0 max       (1007) max       (1007)     9968 2023-02-08 13:51:26.000000 penn-0.0.8/README.md
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/
+-rw-r--r--   0 max       (1007) max       (1007)      988 2023-02-08 13:51:26.000000 penn-0.0.8/penn/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     2343 2023-02-08 13:51:26.000000 penn-0.0.8/penn/__main__.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.439732 penn-0.0.8/penn/assets/
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/assets/partitions/
+-rw-r--r--   0 max       (1007) max       (1007)     4204 2023-05-17 21:13:15.000000 penn-0.0.8/penn/assets/partitions/mdb.json
+-rw-r--r--   0 max       (1007) max       (1007)    84988 2023-05-17 21:13:15.000000 penn-0.0.8/penn/assets/partitions/ptdb.json
+-rw-r--r--   0 max       (1007) max       (1007)     2293 2023-02-08 13:51:26.000000 penn-0.0.8/penn/checkpoint.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/config/
+-rw-r--r--   0 max       (1007) max       (1007)        0 2023-02-08 13:51:26.000000 penn-0.0.8/penn/config/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     4088 2023-05-17 20:39:52.000000 penn-0.0.8/penn/config/defaults.py
+-rw-r--r--   0 max       (1007) max       (1007)     1385 2023-02-08 13:51:26.000000 penn-0.0.8/penn/config/static.py
+-rw-r--r--   0 max       (1007) max       (1007)     2207 2023-02-08 13:51:26.000000 penn-0.0.8/penn/convert.py
+-rw-r--r--   0 max       (1007) max       (1007)    14538 2023-05-17 20:39:52.000000 penn-0.0.8/penn/core.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/data/
+-rw-r--r--   0 max       (1007) max       (1007)      133 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     6876 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/dataset.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/data/download/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/download/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)      561 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/download/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)     1851 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/download/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     1022 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/loader.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/data/preprocess/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/preprocess/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)      580 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/preprocess/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)     6918 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/preprocess/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     2790 2023-02-08 13:51:26.000000 penn-0.0.8/penn/data/sampler.py
+-rw-r--r--   0 max       (1007) max       (1007)     4982 2023-05-17 20:41:21.000000 penn-0.0.8/penn/decode.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/dsp/
+-rw-r--r--   0 max       (1007) max       (1007)       37 2023-02-08 13:51:26.000000 penn-0.0.8/penn/dsp/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     2944 2023-02-08 13:51:26.000000 penn-0.0.8/penn/dsp/dio.py
+-rw-r--r--   0 max       (1007) max       (1007)     8978 2023-02-08 13:51:26.000000 penn-0.0.8/penn/dsp/pyin.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/evaluate/
+-rw-r--r--   0 max       (1007) max       (1007)       85 2023-02-08 13:51:26.000000 penn-0.0.8/penn/evaluate/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)      874 2023-02-08 13:51:26.000000 penn-0.0.8/penn/evaluate/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)    18545 2023-02-08 13:51:26.000000 penn-0.0.8/penn/evaluate/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     7562 2023-02-08 13:51:26.000000 penn-0.0.8/penn/evaluate/metrics.py
+-rw-r--r--   0 max       (1007) max       (1007)      366 2023-02-08 13:51:26.000000 penn-0.0.8/penn/load.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/model/
+-rw-r--r--   0 max       (1007) max       (1007)      361 2023-02-08 13:51:26.000000 penn-0.0.8/penn/model/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)      234 2023-02-08 13:51:26.000000 penn-0.0.8/penn/model/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     2681 2023-02-08 13:51:26.000000 penn-0.0.8/penn/model/crepe.py
+-rw-r--r--   0 max       (1007) max       (1007)     2969 2023-02-08 13:51:26.000000 penn-0.0.8/penn/model/deepf0.py
+-rw-r--r--   0 max       (1007) max       (1007)     1747 2023-02-08 13:51:26.000000 penn-0.0.8/penn/model/fcnf0.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/partition/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/partition/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)      562 2023-02-08 13:51:26.000000 penn-0.0.8/penn/partition/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)      956 2023-02-08 13:51:26.000000 penn-0.0.8/penn/partition/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     1177 2023-02-08 13:51:26.000000 penn-0.0.8/penn/periodicity.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/plot/
+-rw-r--r--   0 max       (1007) max       (1007)       67 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/__init__.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/plot/density/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/density/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     1016 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/density/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)     3506 2023-05-21 15:43:04.000000 penn-0.0.8/penn/plot/density/core.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn/plot/logits/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/logits/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     1029 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/logits/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)     2881 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/logits/core.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.447732 penn-0.0.8/penn/plot/threshold/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/threshold/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)      926 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/threshold/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)     1948 2023-02-08 13:51:26.000000 penn-0.0.8/penn/plot/threshold/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     1262 2023-02-08 13:51:26.000000 penn-0.0.8/penn/time.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.447732 penn-0.0.8/penn/train/
+-rw-r--r--   0 max       (1007) max       (1007)       20 2023-02-08 13:51:26.000000 penn-0.0.8/penn/train/__init__.py
+-rw-r--r--   0 max       (1007) max       (1007)     1274 2023-02-08 13:51:26.000000 penn-0.0.8/penn/train/__main__.py
+-rw-r--r--   0 max       (1007) max       (1007)     9864 2023-02-08 13:51:26.000000 penn-0.0.8/penn/train/core.py
+-rw-r--r--   0 max       (1007) max       (1007)     1029 2023-05-17 20:38:35.000000 penn-0.0.8/penn/voicing.py
+-rw-r--r--   0 max       (1007) max       (1007)     1449 2023-02-08 13:51:26.000000 penn-0.0.8/penn/write.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.443732 penn-0.0.8/penn.egg-info/
+-rw-r--r--   0 max       (1007) max       (1007)    10415 2023-05-25 18:20:02.000000 penn-0.0.8/penn.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1007) max       (1007)     1440 2023-05-25 18:20:02.000000 penn-0.0.8/penn.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1007) max       (1007)        1 2023-05-25 18:20:02.000000 penn-0.0.8/penn.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1007) max       (1007)       63 2023-05-25 18:20:02.000000 penn-0.0.8/penn.egg-info/requires.txt
+-rw-r--r--   0 max       (1007) max       (1007)        5 2023-05-25 18:20:02.000000 penn-0.0.8/penn.egg-info/top_level.txt
+-rw-r--r--   0 max       (1007) max       (1007)       38 2023-05-25 18:20:02.447732 penn-0.0.8/setup.cfg
+-rw-r--r--   0 max       (1007) max       (1007)     1024 2023-05-25 18:18:09.000000 penn-0.0.8/setup.py
+drwxr-xr-x   0 max       (1007) max       (1007)        0 2023-05-25 18:20:02.447732 penn-0.0.8/test/
+-rw-r--r--   0 max       (1007) max       (1007)      448 2023-02-08 13:51:26.000000 penn-0.0.8/test/test_core.py
```

### Comparing `penn-0.0.7/LICENSE` & `penn-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/PKG-INFO` & `penn-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penn
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pitch Estimating Neural Networks (PENN)
 Home-page: https://github.com/interactiveaudiolab/penn
 Author: Max Morrison, Caedon Hsieh, Nathan Pruyne, and Bryan Pardo
 Author-email: interactiveaudiolab@gmail.com
 License: MIT
 Keywords: audio,frequency,music,periodicity,pitch,speech
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `penn-0.0.7/README.md` & `penn-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/__init__.py` & `penn-0.0.8/penn/__init__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/__main__.py` & `penn-0.0.8/penn/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/assets/partitions/mdb.json` & `penn-0.0.8/penn/assets/partitions/mdb.json`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/assets/partitions/ptdb.json` & `penn-0.0.8/penn/assets/partitions/ptdb.json`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/checkpoint.py` & `penn-0.0.8/penn/checkpoint.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/config/defaults.py` & `penn-0.0.8/penn/config/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 ###############################################################################
 # Model parameters
 ###############################################################################
 
 
 # The decoder to use for postprocessing
-DECODER = 'locally_normal'
+DECODER = 'local_expected_value'
 
 # The dropout rate. Set to None to turn off dropout.
 DROPOUT = None
 
 # The name of the model to use for training
 MODEL = 'fcnf0'
```

### Comparing `penn-0.0.7/penn/config/static.py` & `penn-0.0.8/penn/config/static.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/convert.py` & `penn-0.0.8/penn/convert.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/core.py` & `penn-0.0.8/penn/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,16 +284,16 @@
         logits[:, maxidx:] = -float('inf')
 
         # Decode pitch from logits
         if penn.DECODER == 'argmax':
             bins, pitch = penn.decode.argmax(logits)
         elif penn.DECODER.startswith('viterbi'):
             bins, pitch = penn.decode.viterbi(logits)
-        elif penn.DECODER == 'locally_normal':
-            bins, pitch = penn.decode.locally_normal(logits)
+        elif penn.DECODER == 'local_expected_value':
+            bins, pitch = penn.decode.local_expected_value(logits)
         else:
             raise ValueError(f'Decoder method {penn.DECODER} is not defined')
 
         # Decode periodicity from logits
         if penn.PERIODICITY == 'entropy':
             periodicity = penn.periodicity.entropy(logits)
         elif penn.PERIODICITY == 'max':
```

### Comparing `penn-0.0.7/penn/data/dataset.py` & `penn-0.0.8/penn/data/dataset.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/data/download/__main__.py` & `penn-0.0.8/penn/data/download/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/data/download/core.py` & `penn-0.0.8/penn/data/download/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/data/loader.py` & `penn-0.0.8/penn/data/loader.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/data/preprocess/__main__.py` & `penn-0.0.8/penn/data/preprocess/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/data/preprocess/core.py` & `penn-0.0.8/penn/data/preprocess/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/data/sampler.py` & `penn-0.0.8/penn/data/sampler.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/decode.py` & `penn-0.0.8/penn/decode.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,18 @@
             (torch.exp(logits.permute(2, 1, 0)), unvoiced[None]),
             dim=1).numpy()
     else:
 
         # Viterbi REQUIRES a categorical distribution, even if the loss was BCE
         distributions = torch.nn.functional.softmax(logits, dim=1)
         distributions = distributions.permute(2, 1, 0)
-        distributions = distributions.to(device=torch.device('cpu'), dtype=torch.float32).numpy()
+        distributions = distributions.to(
+            device=torch.device('cpu'),
+            dtype=torch.float32
+        ).numpy()
 
     # Cache viterbi probabilities
     if not hasattr(viterbi, 'transition'):
         # Get number of bins per frame
         bins_per_octave = penn.OCTAVE / penn.CENTS_PER_BIN
         max_octaves_per_frame = \
             penn.MAX_OCTAVES_PER_SECOND * penn.HOPSIZE / penn.SAMPLE_RATE
@@ -77,15 +80,17 @@
         p_init=viterbi.initial)
     bins = torch.from_numpy(bins.astype(np.int32))
 
     # Convert to frequency in Hz
     if penn.DECODER.endswith('normal'):
 
         # Decode using an assumption of normality around to the viterbi path
-        pitch = locally_normal_from_bins(bins.T.to(logits.device), logits).T
+        pitch = local_expected_value_from_bins(
+            bins.T.to(logits.device),
+            logits).T
 
     else:
 
         # Argmax decoding
         pitch = penn.convert.bins_to_frequency(bins)
 
     if penn.METHOD == 'pyin':
@@ -94,20 +99,20 @@
         pitch[bins >= penn.PITCH_BINS] = 0
         pitch = penn.data.preprocess.interpolate_unvoiced(pitch.numpy())[0]
         pitch = torch.from_numpy(pitch)
 
     return bins.T, pitch.T
 
 
-def locally_normal(logits, window=penn.LOCAL_PITCH_WINDOW_SIZE):
+def local_expected_value(logits, window=penn.LOCAL_PITCH_WINDOW_SIZE):
     """Decode pitch using a normal assumption around the argmax"""
     # Get center bins
     bins = logits.argmax(dim=1)
 
-    return bins, locally_normal_from_bins(bins, logits, window)
+    return bins, local_expected_value_from_bins(bins, logits, window)
 
 
 ###############################################################################
 # Utilities
 ###############################################################################
 
 
@@ -128,15 +133,18 @@
     if penn.LOSS == 'binary_cross_entropy':
         pitch = pitch / distributions.sum(dim=1)
 
     # Convert to hz
     return penn.convert.cents_to_frequency(pitch)
 
 
-def locally_normal_from_bins(bins, logits, window=penn.LOCAL_PITCH_WINDOW_SIZE):
+def local_expected_value_from_bins(
+    bins,
+    logits,
+    window=penn.LOCAL_PITCH_WINDOW_SIZE):
     """Decode pitch using normal assumption around argmax from bin indices"""
     # Pad
     padded = torch.nn.functional.pad(
         logits.squeeze(2),
         (window // 2, window // 2),
         value=-float('inf'))
```

### Comparing `penn-0.0.7/penn/dsp/dio.py` & `penn-0.0.8/penn/dsp/dio.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/dsp/pyin.py` & `penn-0.0.8/penn/dsp/pyin.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/evaluate/__main__.py` & `penn-0.0.8/penn/evaluate/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/evaluate/core.py` & `penn-0.0.8/penn/evaluate/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/evaluate/metrics.py` & `penn-0.0.8/penn/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/model/crepe.py` & `penn-0.0.8/penn/model/crepe.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/model/deepf0.py` & `penn-0.0.8/penn/model/deepf0.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/model/fcnf0.py` & `penn-0.0.8/penn/model/fcnf0.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/partition/__main__.py` & `penn-0.0.8/penn/partition/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/partition/core.py` & `penn-0.0.8/penn/partition/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/periodicity.py` & `penn-0.0.8/penn/periodicity.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/plot/density/__main__.py` & `penn-0.0.8/penn/plot/density/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/plot/density/core.py` & `penn-0.0.8/penn/plot/density/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,32 +32,32 @@
     # Plot true data density
     x = torch.arange(0, penn.PITCH_BINS, DOWNSAMPLE_RATE)
     y_true, y_pred = histograms(datasets, checkpoint, gpu)
     y_true = y_true.reshape(-1, DOWNSAMPLE_RATE).sum(-1)
     axis.bar(
         x,
         y_true,
-        width=DOWNSAMPLE_RATE,
+        width=1.05 * DOWNSAMPLE_RATE,
         label=f'Data distribution')
 
     # Plot our guesses
     y_pred = y_pred.reshape(-1, DOWNSAMPLE_RATE).sum(-1)
     axis.bar(
         x,
         y_pred,
-        width=DOWNSAMPLE_RATE,
+        width=1.05 * DOWNSAMPLE_RATE,
         label='Inferred distribution')
 
     # Plot overlap
     overlap = torch.minimum(y_true, y_pred)
     axis.bar(
         x,
         overlap,
         color='gray',
-        width=DOWNSAMPLE_RATE,
+        width=1.05 * DOWNSAMPLE_RATE,
         label='Overlap')
 
     # Add legend
     axis.legend(frameon=False, prop={'size': 10})
 
     # Save plot
     figure.savefig(output_file, bbox_inches='tight', pad_inches=0, dpi=300)
```

### Comparing `penn-0.0.7/penn/plot/logits/__main__.py` & `penn-0.0.8/penn/plot/logits/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/plot/logits/core.py` & `penn-0.0.8/penn/plot/logits/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/plot/threshold/__main__.py` & `penn-0.0.8/penn/plot/threshold/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/plot/threshold/core.py` & `penn-0.0.8/penn/plot/threshold/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/time.py` & `penn-0.0.8/penn/time.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/train/__main__.py` & `penn-0.0.8/penn/train/__main__.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/train/core.py` & `penn-0.0.8/penn/train/core.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/voicing.py` & `penn-0.0.8/penn/voicing.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn/write.py` & `penn-0.0.8/penn/write.py`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/penn.egg-info/PKG-INFO` & `penn-0.0.8/penn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penn
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pitch Estimating Neural Networks (PENN)
 Home-page: https://github.com/interactiveaudiolab/penn
 Author: Max Morrison, Caedon Hsieh, Nathan Pruyne, and Bryan Pardo
 Author-email: interactiveaudiolab@gmail.com
 License: MIT
 Keywords: audio,frequency,music,periodicity,pitch,speech
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `penn-0.0.7/penn.egg-info/SOURCES.txt` & `penn-0.0.8/penn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `penn-0.0.7/setup.py` & `penn-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md') as file:
     long_description = file.read()
 
 
 setup(
     name='penn',
     description='Pitch Estimating Neural Networks (PENN)',
-    version='0.0.7',
+    version='0.0.8',
     author='Max Morrison, Caedon Hsieh, Nathan Pruyne, and Bryan Pardo',
     author_email='interactiveaudiolab@gmail.com',
     url='https://github.com/interactiveaudiolab/penn',
     install_requires=[
         'huggingface_hub', # 0.11.1
         'numpy',           # 1.23.4
         'tensorboard',     # 2.11.0
```

