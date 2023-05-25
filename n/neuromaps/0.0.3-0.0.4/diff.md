# Comparing `tmp/neuromaps-0.0.3.tar.gz` & `tmp/neuromaps-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuromaps-0.0.3.tar", last modified: Thu Oct  6 20:15:36 2022, max compression
+gzip compressed data, was "neuromaps-0.0.4.tar", last modified: Thu May 25 16:38:43 2023, max compression
```

## Comparing `neuromaps-0.0.3.tar` & `neuromaps-0.0.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    20849 2022-10-06 20:07:39.000000 neuromaps-0.0.3/LICENSE
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      140 2022-10-06 20:07:39.000000 neuromaps-0.0.3/MANIFEST.in
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     2661 2022-10-06 20:15:36.672188 neuromaps-0.0.3/PKG-INFO
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1753 2022-10-06 20:07:39.000000 neuromaps-0.0.3/README.rst
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.676188 neuromaps-0.0.3/neuromaps/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      234 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/__init__.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      497 2022-10-06 20:15:36.676188 neuromaps-0.0.3/neuromaps/_version.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     4486 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/caret.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     3583 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/civet.py
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps/datasets/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      854 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/__init__.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    12925 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/_osf.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     8050 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/annotations.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     9416 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/atlases.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     7838 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/contributions.py
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps/datasets/data/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    70781 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/data/osf.json
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps/datasets/tests/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/tests/__init__.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      971 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/tests/test__osf.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      689 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/tests/test_annotations.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1185 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/tests/test_atlases.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      811 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/tests/test_utils.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     4572 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/datasets/utils.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    18635 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/images.py
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps/nulls/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      347 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/__init__.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     5351 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/burt.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    25105 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/nulls.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    27669 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/spins.py
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps/nulls/tests/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/tests/__init__.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      530 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/tests/test_burt.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      695 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/tests/test_nulls.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      814 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/nulls/tests/test_spins.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     9633 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/parcellate.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     4529 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/plotting.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    15007 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/points.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    10475 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/resampling.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     9378 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/stats.py
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps/tests/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/__init__.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      320 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/conftest.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      413 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_caret.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      289 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_civet.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1436 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_images.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      288 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_parcellate.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      161 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_plotting.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1045 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_points.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      968 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_resampling.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1456 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_stats.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1458 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_transforms.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      467 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/tests/test_utils.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    22321 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/transforms.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     3543 2022-10-06 20:07:39.000000 neuromaps-0.0.3/neuromaps/utils.py
-drwxrwxr-x   0 zqliu     (1000) zqliu     (1001)        0 2022-10-06 20:15:36.672188 neuromaps-0.0.3/neuromaps.egg-info/
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     2661 2022-10-06 20:15:36.000000 neuromaps-0.0.3/neuromaps.egg-info/PKG-INFO
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1583 2022-10-06 20:15:36.000000 neuromaps-0.0.3/neuromaps.egg-info/SOURCES.txt
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)        1 2022-10-06 20:15:36.000000 neuromaps-0.0.3/neuromaps.egg-info/dependency_links.txt
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)        1 2022-10-06 20:15:36.000000 neuromaps-0.0.3/neuromaps.egg-info/not-zip-safe
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      309 2022-10-06 20:15:36.000000 neuromaps-0.0.3/neuromaps.egg-info/requires.txt
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)       10 2022-10-06 20:15:36.000000 neuromaps-0.0.3/neuromaps.egg-info/top_level.txt
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      118 2022-10-06 20:07:39.000000 neuromaps-0.0.3/pyproject.toml
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)       83 2022-10-06 20:07:39.000000 neuromaps-0.0.3/requirements.txt
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)     1727 2022-10-06 20:15:36.676188 neuromaps-0.0.3/setup.cfg
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)      276 2022-10-06 20:07:39.000000 neuromaps-0.0.3/setup.py
--rw-rw-r--   0 zqliu     (1000) zqliu     (1001)    70144 2022-10-06 20:07:39.000000 neuromaps-0.0.3/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.379939 neuromaps-0.0.4/
+-rw-rw-rw-   0        0        0    20849 2023-05-25 16:36:18.000000 neuromaps-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      140 2023-05-25 16:36:18.000000 neuromaps-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2742 2023-05-25 16:38:43.380442 neuromaps-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1753 2023-05-25 16:36:18.000000 neuromaps-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.383159 neuromaps-0.0.4/neuromaps/
+-rw-rw-rw-   0        0        0      234 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-25 16:38:43.383159 neuromaps-0.0.4/neuromaps/_version.py
+-rw-rw-rw-   0        0        0     4486 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/caret.py
+-rw-rw-rw-   0        0        0     3583 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/civet.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.208543 neuromaps-0.0.4/neuromaps/datasets/
+-rw-rw-rw-   0        0        0      854 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/__init__.py
+-rw-rw-rw-   0        0        0    12925 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/_osf.py
+-rw-rw-rw-   0        0        0     8689 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/annotations.py
+-rw-rw-rw-   0        0        0     9416 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/atlases.py
+-rw-rw-rw-   0        0        0     7838 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/contributions.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.214583 neuromaps-0.0.4/neuromaps/datasets/data/
+-rw-rw-rw-   0        0        0    78949 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/data/osf.json
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.244493 neuromaps-0.0.4/neuromaps/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/tests/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/tests/test__osf.py
+-rw-rw-rw-   0        0        0      689 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/tests/test_annotations.py
+-rw-rw-rw-   0        0        0     1185 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/tests/test_atlases.py
+-rw-rw-rw-   0        0        0      811 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/tests/test_utils.py
+-rw-rw-rw-   0        0        0     4572 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/datasets/utils.py
+-rw-rw-rw-   0        0        0    18635 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/images.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.278446 neuromaps-0.0.4/neuromaps/nulls/
+-rw-rw-rw-   0        0        0      347 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/__init__.py
+-rw-rw-rw-   0        0        0     5351 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/burt.py
+-rw-rw-rw-   0        0        0    25481 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/nulls.py
+-rw-rw-rw-   0        0        0    27681 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/spins.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.304037 neuromaps-0.0.4/neuromaps/nulls/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/tests/__init__.py
+-rw-rw-rw-   0        0        0      530 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/tests/test_burt.py
+-rw-rw-rw-   0        0        0      695 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/tests/test_nulls.py
+-rw-rw-rw-   0        0        0      814 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/nulls/tests/test_spins.py
+-rw-rw-rw-   0        0        0     9633 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/parcellate.py
+-rw-rw-rw-   0        0        0     4529 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/plotting.py
+-rw-rw-rw-   0        0        0    15007 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/points.py
+-rw-rw-rw-   0        0        0    10475 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/resampling.py
+-rw-rw-rw-   0        0        0    10661 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.379318 neuromaps-0.0.4/neuromaps/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/__init__.py
+-rw-rw-rw-   0        0        0      320 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/conftest.py
+-rw-rw-rw-   0        0        0      413 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_caret.py
+-rw-rw-rw-   0        0        0      289 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_civet.py
+-rw-rw-rw-   0        0        0     1436 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_images.py
+-rw-rw-rw-   0        0        0      288 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_parcellate.py
+-rw-rw-rw-   0        0        0      161 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     1045 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_points.py
+-rw-rw-rw-   0        0        0      968 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_resampling.py
+-rw-rw-rw-   0        0        0     1456 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_stats.py
+-rw-rw-rw-   0        0        0     1458 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_transforms.py
+-rw-rw-rw-   0        0        0      467 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/tests/test_utils.py
+-rw-rw-rw-   0        0        0    22321 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/transforms.py
+-rw-rw-rw-   0        0        0     3543 2023-05-25 16:36:18.000000 neuromaps-0.0.4/neuromaps/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:38:43.153029 neuromaps-0.0.4/neuromaps.egg-info/
+-rw-rw-rw-   0        0        0     2742 2023-05-25 16:38:42.000000 neuromaps-0.0.4/neuromaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1583 2023-05-25 16:38:43.000000 neuromaps-0.0.4/neuromaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:38:42.000000 neuromaps-0.0.4/neuromaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 16:38:42.000000 neuromaps-0.0.4/neuromaps.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      309 2023-05-25 16:38:42.000000 neuromaps-0.0.4/neuromaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 16:38:42.000000 neuromaps-0.0.4/neuromaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-05-25 16:36:18.000000 neuromaps-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       83 2023-05-25 16:36:18.000000 neuromaps-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0     1820 2023-05-25 16:38:43.382606 neuromaps-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      276 2023-05-25 16:36:18.000000 neuromaps-0.0.4/setup.py
+-rw-rw-rw-   0        0        0    70144 2023-05-25 16:36:18.000000 neuromaps-0.0.4/versioneer.py
```

### Comparing `neuromaps-0.0.3/LICENSE` & `neuromaps-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/PKG-INFO` & `neuromaps-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: neuromaps
-Version: 0.0.3
-Summary: A toolbox for projecting, resampling, and comparing brain maps
-Home-page: https://github.com/netneurolab/neuromaps
-Download-URL: https://github.com/netneurolab/neuromaps
-Author: Network Neuroscience Lab
-Maintainer: Network Neuroscience Lab
-Maintainer-email: rossmarkello+coding@gmail.com
-License: BSD-3
-Platform: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides: neuromaps
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: doc
-Provides-Extra: nulls
-Provides-Extra: style
-Provides-Extra: test
-Provides-Extra: all
-License-File: LICENSE
-
-.. image:: neuromaps_logo.png
-
-The ``neuromaps`` toolbox is designed to help researchers make easy,
-statistically-rigorous comparisons between brain maps (or brain annotations).
-
-The accompanying paper is published in `Nature Methods <https://www.nature.com/articles/s41592-022-01625-w>`_.
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5842499.svg
-   :target: https://doi.org/10.5281/zenodo.5842499
-
-Installation requirements
--------------------------
-
-Currently, ``neuromaps`` works with Python 3.7+ and requires a few
-dependencies:
-
-- matplotlib
-- nibabel (>=3.0)
-- nilearn (>=0.7)
-- numpy (>=1.14)
-- scikit-learn (>=0.17)
-- scipy
-
-You can get started by installing ``neuromaps`` from the source repository
-with:
-
-.. code-block:: bash
-
-    git clone https://github.com/netneurolab/neuromaps
-    cd neuromaps
-    pip install .
-
-You will also need to have `Connectome Workbench <https://www.humanconnectome.
-org/software/connectome-workbench>`_ installed and available on your path in
-order to use most of the transformation / resampling functionality of
-``neuromaps``.
-
-.. _installation:
-
-Citation
---------
-
-If you use the ``neuromaps`` toolbox, please cite our `paper <https://www.nature.com/articles/s41592-022-01625-w>`_.
-If you use data included in the ``neuromaps`` repository, be sure to cite the original paper that published this data.
-A table with references for each brain map can be found in the Wiki.
-
-License information
--------------------
-
-This work is licensed under a
-Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ``cc-by-nc-sa``.
-The full license can be found in the
-`LICENSE <https://github.com/netneurolab/neuromaps/blob/main/neuromaps
-/LICENSE>`_ file in the ``neuromaps`` distribution.
+Metadata-Version: 2.1
+Name: neuromaps
+Version: 0.0.4
+Summary: A toolbox for projecting, resampling, and comparing brain maps
+Home-page: https://github.com/netneurolab/neuromaps
+Download-URL: https://github.com/netneurolab/neuromaps
+Author: Network Neuroscience Lab
+Maintainer: Network Neuroscience Lab
+Maintainer-email: rossmarkello+coding@gmail.com
+License: BSD-3
+Platform: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides: neuromaps
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: doc
+Provides-Extra: nulls
+Provides-Extra: style
+Provides-Extra: test
+Provides-Extra: all
+License-File: LICENSE
+
+.. image:: neuromaps_logo.png
+
+The ``neuromaps`` toolbox is designed to help researchers make easy,
+statistically-rigorous comparisons between brain maps (or brain annotations).
+
+The accompanying paper is published in `Nature Methods <https://www.nature.com/articles/s41592-022-01625-w>`_.
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5842499.svg
+   :target: https://doi.org/10.5281/zenodo.5842499
+
+Installation requirements
+-------------------------
+
+Currently, ``neuromaps`` works with Python 3.7+ and requires a few
+dependencies:
+
+- matplotlib
+- nibabel (>=3.0)
+- nilearn (>=0.7)
+- numpy (>=1.14)
+- scikit-learn (>=0.17)
+- scipy
+
+You can get started by installing ``neuromaps`` from the source repository
+with:
+
+.. code-block:: bash
+
+    git clone https://github.com/netneurolab/neuromaps
+    cd neuromaps
+    pip install .
+
+You will also need to have `Connectome Workbench <https://www.humanconnectome.
+org/software/connectome-workbench>`_ installed and available on your path in
+order to use most of the transformation / resampling functionality of
+``neuromaps``.
+
+.. _installation:
+
+Citation
+--------
+
+If you use the ``neuromaps`` toolbox, please cite our `paper <https://www.nature.com/articles/s41592-022-01625-w>`_.
+If you use data included in the ``neuromaps`` repository, be sure to cite the original paper that published this data.
+A table with references for each brain map can be found in the Wiki.
+
+License information
+-------------------
+
+This work is licensed under a
+Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ``cc-by-nc-sa``.
+The full license can be found in the
+`LICENSE <https://github.com/netneurolab/neuromaps/blob/main/neuromaps
+/LICENSE>`_ file in the ``neuromaps`` distribution.
```

### Comparing `neuromaps-0.0.3/README.rst` & `neuromaps-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/caret.py` & `neuromaps-0.0.4/neuromaps/caret.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/civet.py` & `neuromaps-0.0.4/neuromaps/civet.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/__init__.py` & `neuromaps-0.0.4/neuromaps/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/_osf.py` & `neuromaps-0.0.4/neuromaps/datasets/_osf.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/annotations.py` & `neuromaps-0.0.4/neuromaps/datasets/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Functions for fetching annotations (from the internet, if necessary)
 """
 
 from collections import defaultdict
 from pathlib import Path
 import re
 import shutil
+import numpy as np
+import warnings
 
 from nilearn.datasets.utils import _fetch_file
 
 from neuromaps.datasets.utils import (get_data_dir, get_dataset_info,
                                       _get_token, _get_session)
 
 MATCH = re.compile(
@@ -224,8 +226,18 @@
         fn = Path(data_dir) / 'annotations' / dset['rel_path'] / dset['fname']
         if not fn.exists():
             dl_file = _fetch_file(dset['url'], str(fn.parent), verbose=verbose,
                                   md5sum=dset['checksum'], session=session)
             shutil.move(dl_file, fn)
         data.append(str(fn))
 
+    # warning for specific maps
+    warn = [np.logical_and(np.logical_or(dset['source'] == 'beliveau2017',
+                                         dset['source'] == 'norgaard2021'),
+                           dset['space'] == 'MNI152') for dset in info]
+    if any(warn):
+        warnings.warn('Data from beliveau2017 and norgaard2021 is best used in'
+                      ' the provided fsaverage space '
+                      '(e.g. source=\'beliveau2017\', space=\'fsaverage\', '
+                      'den=\'164k\'). MNI152 maps should only be used for '
+                      'subcortical data.')
     return _groupby_match(data, return_single=return_single)
```

### Comparing `neuromaps-0.0.3/neuromaps/datasets/atlases.py` & `neuromaps-0.0.4/neuromaps/datasets/atlases.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/contributions.py` & `neuromaps-0.0.4/neuromaps/datasets/contributions.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/data/osf.json` & `neuromaps-0.0.4/neuromaps/datasets/data/osf.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9825705803615286%*

 * *Differences: {"'annotations'": "{44: {'url': {insert: [(1, '6130fe34af610c0217dfe61a')], delete: [1]}}, 78: "*

 * *                  "{'source': 'norgaard2021', 'fname': "*

 * *                  "'source-norgaard2021_desc-flumazenil_space-MNI152_res-1mm_feature.nii.gz', "*

 * *                  "'rel_path': 'norgaard2021/flumazenil/MNI152/', 'url': {insert: [(1, "*

 * *                  "'6385541b228a5a18da7bd628')], delete: [1]}}, insert: [(6, "*

 * *                  "OrderedDict([('source', 'beliveau2017'), ('desc', 'az10419369'), ('space',  […]*

```diff
@@ -140,14 +140,56 @@
             "title": null,
             "url": [
                 "4mw3a",
                 "6196cb28bbe37803c059ee6d"
             ]
         },
         {
+            "checksum": "23501cf62b1e7c2881d830cdf4d0ebff",
+            "den": "164k",
+            "desc": "az10419369",
+            "fname": "source-beliveau2017_desc-az10419369_space-fsaverage_den-164k_hemi-L_feature.func.gii",
+            "format": "surface",
+            "hemi": "L",
+            "redir": null,
+            "rel_path": "beliveau2017/az10419369/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638543b0723a11190518c8a6"
+            ]
+        },
+        {
+            "checksum": "df01756cd50af0e9ebcc2c6df0405135",
+            "den": "164k",
+            "desc": "az10419369",
+            "fname": "source-beliveau2017_desc-az10419369_space-fsaverage_den-164k_hemi-R_feature.func.gii",
+            "format": "surface",
+            "hemi": "R",
+            "redir": null,
+            "rel_path": "beliveau2017/az10419369/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638543a2c86e2818da88f993"
+            ]
+        },
+        {
             "checksum": "7f0f2aa3d4132d7365e3cf12e3d3c0df",
             "desc": "cimbi36",
             "fname": "source-beliveau2017_desc-cimbi36_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
             "redir": null,
             "rel_path": "beliveau2017/cimbi36/MNI152/",
             "res": "1mm",
@@ -160,14 +202,56 @@
             "title": null,
             "url": [
                 "4mw3a",
                 "6196cb34bbe37803bd59f194"
             ]
         },
         {
+            "checksum": "2dcf2c82b5fb96ac6921d560a3416e64",
+            "den": "164k",
+            "desc": "cimbi36",
+            "fname": "source-beliveau2017_desc-cimbi36_space-fsaverage_den-164k_hemi-L_feature.func.gii",
+            "format": "surface",
+            "hemi": "L",
+            "redir": null,
+            "rel_path": "beliveau2017/cimbi36/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638543bf228a5a18987bc2c1"
+            ]
+        },
+        {
+            "checksum": "d31200bc45b31953f6d8c3632b5d7044",
+            "den": "164k",
+            "desc": "cimbi36",
+            "fname": "source-beliveau2017_desc-cimbi36_space-fsaverage_den-164k_hemi-R_feature.func.gii",
+            "format": "surface",
+            "hemi": "R",
+            "redir": null,
+            "rel_path": "beliveau2017/cimbi36/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638543cdc86e2818da88f9e7"
+            ]
+        },
+        {
             "checksum": "5d1284e2a9e3401ac82c3f1c425cffb1",
             "desc": "cumi101",
             "fname": "source-beliveau2017_desc-cumi101_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
             "redir": null,
             "rel_path": "beliveau2017/cumi101/MNI152/",
             "res": "1mm",
@@ -180,14 +264,56 @@
             "title": null,
             "url": [
                 "4mw3a",
                 "6196cb3f0b0c1e03d87fbf65"
             ]
         },
         {
+            "checksum": "e76c623cb51a28f2105d26dab0f2ebe0",
+            "den": "164k",
+            "desc": "cumi101",
+            "fname": "source-beliveau2017_desc-cumi101_space-fsaverage_den-164k_hemi-L_feature.func.gii",
+            "format": "surface",
+            "hemi": "L",
+            "redir": null,
+            "rel_path": "beliveau2017/cumi101/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638543ea1daa6b183975935a"
+            ]
+        },
+        {
+            "checksum": "7b5bab02f7edbdc255b5c72c93189d4e",
+            "den": "164k",
+            "desc": "cumi101",
+            "fname": "source-beliveau2017_desc-cumi101_space-fsaverage_den-164k_hemi-R_feature.func.gii",
+            "format": "surface",
+            "hemi": "R",
+            "redir": null,
+            "rel_path": "beliveau2017/cumi101/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638543dbc86e2818d988f7ea"
+            ]
+        },
+        {
             "checksum": "7ccea5d10ff4421b88ce859159039057",
             "desc": "dasb",
             "fname": "source-beliveau2017_desc-dasb_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
             "redir": null,
             "rel_path": "beliveau2017/dasb/MNI152/",
             "res": "1mm",
@@ -200,14 +326,56 @@
             "title": null,
             "url": [
                 "4mw3a",
                 "6196cb1c0b0c1e03ca7fd263"
             ]
         },
         {
+            "checksum": "21fb41e524fbb5cdf2d60a3ffdd49712",
+            "den": "164k",
+            "desc": "dasb",
+            "fname": "source-beliveau2017_desc-dasb_space-fsaverage_den-164k_hemi-L_feature.func.gii",
+            "format": "surface",
+            "hemi": "L",
+            "redir": null,
+            "rel_path": "beliveau2017/dasb/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "63854394228a5a18987bc26e"
+            ]
+        },
+        {
+            "checksum": "e4921dcc6da907318ef47d7b15250b84",
+            "den": "164k",
+            "desc": "dasb",
+            "fname": "source-beliveau2017_desc-dasb_space-fsaverage_den-164k_hemi-R_feature.func.gii",
+            "format": "surface",
+            "hemi": "R",
+            "redir": null,
+            "rel_path": "beliveau2017/dasb/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "63854385c86e2818da88f94b"
+            ]
+        },
+        {
             "checksum": "a9195d94a8ae80b617bd232ac890f17d",
             "desc": "sb207145",
             "fname": "source-beliveau2017_desc-sb207145_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
             "redir": null,
             "rel_path": "beliveau2017/sb207145/MNI152/",
             "res": "1mm",
@@ -220,14 +388,56 @@
             "title": null,
             "url": [
                 "4mw3a",
                 "6196cb10bbe37803b559fe58"
             ]
         },
         {
+            "checksum": "5520fb0ed11a4037b22de7b63fa9704b",
+            "den": "164k",
+            "desc": "sb207145",
+            "fname": "source-beliveau2017_desc-sb207145_space-fsaverage_den-164k_hemi-L_feature.func.gii",
+            "format": "space",
+            "hemi": "L",
+            "redir": null,
+            "rel_path": "beliveau2017/sb207145/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638542c2c86e2818d588f461"
+            ]
+        },
+        {
+            "checksum": "4bb6b0f54f2cdf3b3dba9e63cf3daa8d",
+            "den": "164k",
+            "desc": "sb207145",
+            "fname": "source-beliveau2017_desc-sb207145_space-fsaverage_den-164k_hemi-R_feature.func.gii",
+            "format": "space",
+            "hemi": "R",
+            "redir": null,
+            "rel_path": "beliveau2017/sb207145/fsaverage/",
+            "source": "beliveau2017",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638542b2a98e5f1ac2103866"
+            ]
+        },
+        {
             "checksum": "10333676136be9ebe19c299ec9cb1170",
             "desc": "mrb",
             "fname": "source-ding2010_desc-mrb_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
             "redir": null,
             "rel_path": "ding2010/mrb/MNI152/",
             "res": "1mm",
@@ -732,15 +942,15 @@
             "tags": [
                 "structural",
                 "MRI"
             ],
             "title": null,
             "url": [
                 "4mw3a",
-                "6130fe40ab8bca0225edc458"
+                "6130fe34af610c0217dfe61a"
             ]
         },
         {
             "checksum": "1bdc330c2e87cb06766dbe5dac8ee043",
             "den": "32k",
             "desc": "thickness",
             "fname": "source-hcps1200_desc-thickness_space-fsLR_den-32k_hemi-R_feature.func.gii",
@@ -1448,29 +1658,71 @@
                 "4mw3a",
                 "60c22953f3ce9401fa24e651"
             ]
         },
         {
             "checksum": "e4eab79ed371d7362741f66bb44388d8",
             "desc": "flumazenil",
-            "fname": "source-norgaard2020_desc-flumazenil_space-MNI152_res-1mm_feature.nii.gz",
+            "fname": "source-norgaard2021_desc-flumazenil_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
             "redir": null,
-            "rel_path": "norgaard2020/flumazenil/MNI152/",
+            "rel_path": "norgaard2021/flumazenil/MNI152/",
             "res": "1mm",
-            "source": "norgaard2020",
+            "source": "norgaard2021",
             "space": "MNI152",
             "tags": [
                 "receptors",
                 "PET"
             ],
             "title": null,
             "url": [
                 "4mw3a",
-                "6196caeb0b0c1e03bf7fdd23"
+                "6385541b228a5a18da7bd628"
+            ]
+        },
+        {
+            "checksum": "3735d34649c932a9eecce57ff688030c",
+            "den": "164k",
+            "desc": "flumazenil",
+            "fname": "source-norgaard2021_desc-flumazenil_space-fsaverage_den-164k_hemi-L_feature.func.gii",
+            "format": "surface",
+            "hemi": "L",
+            "redir": null,
+            "rel_path": "norgaard2021/flumazenil/fsaverage/",
+            "source": "norgaard2021",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "638553fe228a5a18d67bcac8"
+            ]
+        },
+        {
+            "checksum": "4f711daa3327499295fb7e9b13552197",
+            "den": "164k",
+            "desc": "flumazenil",
+            "fname": "source-norgaard2021_desc-flumazenil_space-fsaverage_den-164k_hemi-R_feature.func.gii",
+            "format": "surface",
+            "hemi": "R",
+            "redir": null,
+            "rel_path": "norgaard2021/flumazenil/fsaverage/",
+            "source": "norgaard2021",
+            "space": "fsaverage",
+            "tags": [
+                "receptors",
+                "PET"
+            ],
+            "title": null,
+            "url": [
+                "4mw3a",
+                "6385540d228a5a18d67bcadd"
             ]
         },
         {
             "checksum": "df9b898b4f1c012410148e7196003c95",
             "desc": "omar",
             "fname": "source-normandin2015_desc-omar_space-MNI152_res-1mm_feature.nii.gz",
             "format": "volume",
@@ -2212,25 +2464,25 @@
             "md5": "7932b4418f63d28935b5adf67150b16f",
             "url": [
                 "4mw3a",
                 "60b684b53a6df1021bd4df2d"
             ]
         },
         "4k": {
-            "md5": "b7ba3039b3fff65c9f396e2eb1b064c8",
+            "md5": "72b7b17d389a04774ca6fd4ca28b4087",
             "url": [
                 "4mw3a",
-                "60b684b19096b7020e6424b1"
+                "63eadf00cb544b03fa9e6f00"
             ]
         },
         "8k": {
-            "md5": "3879107951b1543654b9a689b485fc44",
+            "md5": "a1226aee262475e23d2cc37b84ef261d",
             "url": [
                 "4mw3a",
-                "60b684b39096b7021b63cf7f"
+                "63eadef9b3fed60444e3434f"
             ]
         }
     },
     "fsaverage": {
         "10k": {
             "md5": "c61384c271ee2e6b5449222281137414",
             "url": [
```

### Comparing `neuromaps-0.0.3/neuromaps/datasets/tests/test__osf.py` & `neuromaps-0.0.4/neuromaps/datasets/tests/test__osf.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/tests/test_annotations.py` & `neuromaps-0.0.4/neuromaps/datasets/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/tests/test_atlases.py` & `neuromaps-0.0.4/neuromaps/datasets/tests/test_atlases.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/tests/test_utils.py` & `neuromaps-0.0.4/neuromaps/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/datasets/utils.py` & `neuromaps-0.0.4/neuromaps/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/images.py` & `neuromaps-0.0.4/neuromaps/images.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/nulls/burt.py` & `neuromaps-0.0.4/neuromaps/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/nulls/nulls.py` & `neuromaps-0.0.4/neuromaps/nulls/nulls.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,14 +527,18 @@
     darr = load_data(data)
     surrogates = np.full((darr.shape) + (n_perm,), np.nan)
     genfunc = _vol_surrogates if atlas == 'MNI152' else _surf_surrogates
     for hdata, hdist, hind, hsl in genfunc(data, atlas, density,
                                            parcellation, distmat,
                                            n_proc=n_proc):
         if method == 'burt2018':
+            if parcellation is None:
+                if hind is not None:
+                    hdist = np.take_along_axis(
+                        hdist, np.argsort(hind, axis=-1), axis=-1)
             hdata += np.abs(np.nanmin(darr)) + 0.1
             hsurr = batch_surrogates(hdist, hdata, n_surr=n_perm, seed=seed)
         elif method == 'burt2020':
             if parcellation is None:
                 if hind is None:
                     hind = np.argsort(hdist, axis=-1)
                     hdist = np.sort(hdist, axis=-1)
@@ -548,20 +552,24 @@
             if hasattr(hdist, 'filename'):
                 hdist._mmap.close()
                 hind._mmap.close()
                 os.unlink(hdist.filename)
                 os.unlink(hind.filename)
                 del hdist, hind
         elif method == 'moran':
+            if parcellation is None:
+                if hind is not None:
+                    hdist = np.take_along_axis(
+                        hdist, np.argsort(hind, axis=-1), axis=-1)
             dist = hdist.astype('float64')
             np.fill_diagonal(dist, 1)
             dist **= -1
             opts = dict(joint=True, tol=1e-6, n_rep=n_perm, random_state=seed)
             opts.update(**kwargs)
-            mrs = MoranRandomization(**kwargs)
+            mrs = MoranRandomization(**opts)
             hsurr = mrs.fit(dist).randomize(hdata).T
 
         surrogates[hsl] = hsurr
 
     return surrogates
```

### Comparing `neuromaps-0.0.3/neuromaps/nulls/spins.py` & `neuromaps-0.0.4/neuromaps/nulls/spins.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         parcellation = (None, None)
 
     centroids, hemiid = [], []
     for n, (parc, surf) in enumerate(zip(parcellation, surfaces)):
         vertices, faces = load_gifti(surf).agg_data()
         if parc is not None:
             labels = load_gifti(parc).agg_data()
-            labeltable = parc.labeltable.get_labels_as_dict()
+            labeltable = load_gifti(parc).labeltable.get_labels_as_dict()
 
             for lab in np.unique(labels):
                 if labeltable.get(lab) in drop:
                     continue
 
                 mask = labels == lab
                 if method in ('average', 'surface'):
```

### Comparing `neuromaps-0.0.3/neuromaps/nulls/tests/test_burt.py` & `neuromaps-0.0.4/neuromaps/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/nulls/tests/test_nulls.py` & `neuromaps-0.0.4/neuromaps/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/nulls/tests/test_spins.py` & `neuromaps-0.0.4/neuromaps/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/parcellate.py` & `neuromaps-0.0.4/neuromaps/parcellate.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/plotting.py` & `neuromaps-0.0.4/neuromaps/plotting.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/points.py` & `neuromaps-0.0.4/neuromaps/points.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/resampling.py` & `neuromaps-0.0.4/neuromaps/resampling.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/stats.py` & `neuromaps-0.0.4/neuromaps/stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from scipy.stats.stats import _chk2_asarray  # scipy < 1.8.0
 from sklearn.utils.validation import check_random_state
 
 from neuromaps.images import load_data
 
 
 def compare_images(src, trg, metric='pearsonr', ignore_zero=True, nulls=None,
-                   nan_policy='omit'):
+                   nan_policy='omit', return_nulls=False):
     """
     Compares images `src` and `trg`
 
     If `src` and `trg` represent data from multiple hemispheres the data are
     concatenated across hemispheres prior to comparison
 
     Parameters
@@ -36,65 +36,81 @@
     ignore_zero : bool, optional
         Whether to perform comparisons ignoring all zero values in `src` and
         `trg` data. Default: True
     nulls : array_like, optional
         Null data for `src` to use in generating a non-parametric p-value.
         If not specified a parameteric p-value is generated. Default: None
     nan_policy : {'propagate', 'raise', 'omit'}, optional
-        Defines how to handle when input contains nan. 'propagate' returns nan,
-        'raise' throws an error, 'omit' performs the calculations ignoring nan
-        values. Default: 'omit'
+        Defines how to handle when input contains nan. 'propagate' propagates
+        the nan values to the callable metric (will return nan if the metric
+        is `spearmanr` `or pearsonr`), 'raise' throws an error, 'omit' performs
+        the calculations ignoring nan values. Default: 'omit'
+    return_nulls : bool, optional
+        Whether to return the null distribution of comparisons. Can only be set
+        to `True` if `nulls` is not None. Default: False
 
     Returns
     -------
     similarity : float
          Comparison metric between `src` and `trg`
     pvalue : float
         The p-value of `similarity`, if `nulls` is not None
+    nulls : (n_perm, ) array_like
+        Null distribution of similarity metrics. Only returned if
+        `return_nulls` is True.
     """
 
     methods = ('pearsonr', 'spearmanr')
     if metric not in methods:
         if not callable(metric):
             raise ValueError(f'Invalid `metric`: {metric}')
         else:
             if not isinstance(metric([1, 1], [1, 1]), float):
                 raise ValueError('Provided callable `metric` must accept two '
                                  'inputs and return single value.')
 
+    if return_nulls and nulls is None:
+        raise ValueError('`return_nulls` cannot be True when `nulls` is None.')
+
     srcdata, trgdata = load_data(src), load_data(trg)
 
-    mask = np.zeros(len(srcdata), dtype=bool)
+    # drop NaNs (if nan_policy==`omit`) and zeros (if ignore_zero=True)
+    zeromask = np.zeros(len(srcdata), dtype=bool)
     if ignore_zero:
-        mask = np.logical_or(np.isclose(srcdata, 0), np.isclose(trgdata, 0))
-
-    # drop NaNs
+        zeromask = np.logical_or(np.isclose(srcdata, 0),
+                                 np.isclose(trgdata, 0))
     nanmask = np.logical_or(np.isnan(srcdata), np.isnan(trgdata))
-    if np.any(nanmask) and nan_policy == 'raise':
-        raise ValueError('Inputs contain nan')
-    mask = np.logical_and(np.logical_not(mask), np.logical_not(nanmask))
+    if nan_policy == 'raise':
+        if np.any(nanmask):
+            raise ValueError('Inputs contain nan')
+    elif nan_policy == 'omit':
+        mask = np.logical_and(np.logical_not(zeromask),
+                              np.logical_not(nanmask))
+    elif nan_policy == 'propagate':
+        mask = np.logical_not(zeromask)
     srcdata, trgdata = srcdata[mask], trgdata[mask]
 
     if metric in methods:
         if metric == 'spearmanr':
             srcdata = sstats.rankdata(srcdata)
             trgdata = sstats.rankdata(trgdata)
         metric = partial(efficient_pearsonr, return_pval=False)
 
     if nulls is not None:
         n_perm = nulls.shape[-1]
         nulls = nulls[mask]
         return permtest_metric(srcdata, trgdata, metric, n_perm=n_perm,
-                               nulls=nulls, nan_policy=nan_policy)
+                               nulls=nulls, nan_policy=nan_policy,
+                               return_nulls=return_nulls)
 
     return metric(srcdata, trgdata)
 
 
 def permtest_metric(a, b, metric='pearsonr', n_perm=1000, seed=0, nulls=None,
-                    nan_policy='propagate'):
+                    nan_policy='propagate', return_nulls=False):
     """
     Generates non-parameteric p-value of `a` and `b` for `metric`
 
     Calculates two-tailed p-value for hypothesis of whether samples `a` and `b`
     are related using permutation tests
 
     Parameters
@@ -118,21 +134,26 @@
         and `b`. Providing this will override the value supplied to `n_perm`.
         When not specified a standard permutation is used to shuffle `a`.
         Default: None
     nan_policy : {'propagate', 'raise', 'omit'}, optional
         Defines how to handle when inputs contain nan. 'propagate' returns nan,
         'raise' throws an error, 'omit' performs the calculations ignoring nan
         values. Default: 'propagate'
+    return_nulls : bool, optional
+        Whether to return the null distribution of comparisons. Default: False
 
     Returns
     -------
     similarity : float
         Similarity metric
     pvalue : float
         Non-parametric p-value
+    nulls : (n_perm, ) array_like
+        Null distribution of similarity metrics. Only returned if
+        `return_nulls` is True.
 
     Notes
     -----
     The lowest p-value that can be returned by this function is equal to 1 /
     (`n_perm` + 1).
     """
 
@@ -166,23 +187,27 @@
         n_perm = nulls.shape[-1]
 
     # divide by one forces coercion to float if ndim = 0
     true_sim = compfunc(a, b, nan_policy=nan_policy) / 1
     abs_true = np.abs(true_sim)
 
     permutations = np.ones(true_sim.shape)
+    nulldist = np.zeros(((n_perm, ) + true_sim.shape))
     for perm in range(n_perm):
         # permute `a` and determine whether correlations exceed original
         ap = a[rs.permutation(len(a))] if nulls is None else nulls[:, perm]
-        permutations += np.abs(
-            compfunc(ap, b, nan_policy=nan_policy)
-        ) >= abs_true
+        nullcomp = compfunc(ap, b, nan_policy=nan_policy)
+        permutations += np.abs(nullcomp) >= abs_true
+        nulldist[perm] = nullcomp
 
     pvals = permutations / (n_perm + 1)  # + 1 in denom accounts for true_sim
 
+    if return_nulls:
+        return true_sim, pvals, nulldist
+
     return true_sim, pvals
 
 
 def efficient_pearsonr(a, b, ddof=1, nan_policy='propagate', return_pval=True):
     """
     Computes correlation of matching columns in `a` and `b`
```

### Comparing `neuromaps-0.0.3/neuromaps/tests/test_images.py` & `neuromaps-0.0.4/neuromaps/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/tests/test_points.py` & `neuromaps-0.0.4/neuromaps/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/tests/test_resampling.py` & `neuromaps-0.0.4/neuromaps/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/tests/test_stats.py` & `neuromaps-0.0.4/neuromaps/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/tests/test_transforms.py` & `neuromaps-0.0.4/neuromaps/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/transforms.py` & `neuromaps-0.0.4/neuromaps/transforms.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps/utils.py` & `neuromaps-0.0.4/neuromaps/utils.py`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/neuromaps.egg-info/PKG-INFO` & `neuromaps-0.0.4/neuromaps.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: neuromaps
-Version: 0.0.3
-Summary: A toolbox for projecting, resampling, and comparing brain maps
-Home-page: https://github.com/netneurolab/neuromaps
-Download-URL: https://github.com/netneurolab/neuromaps
-Author: Network Neuroscience Lab
-Maintainer: Network Neuroscience Lab
-Maintainer-email: rossmarkello+coding@gmail.com
-License: BSD-3
-Platform: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides: neuromaps
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: doc
-Provides-Extra: nulls
-Provides-Extra: style
-Provides-Extra: test
-Provides-Extra: all
-License-File: LICENSE
-
-.. image:: neuromaps_logo.png
-
-The ``neuromaps`` toolbox is designed to help researchers make easy,
-statistically-rigorous comparisons between brain maps (or brain annotations).
-
-The accompanying paper is published in `Nature Methods <https://www.nature.com/articles/s41592-022-01625-w>`_.
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5842499.svg
-   :target: https://doi.org/10.5281/zenodo.5842499
-
-Installation requirements
--------------------------
-
-Currently, ``neuromaps`` works with Python 3.7+ and requires a few
-dependencies:
-
-- matplotlib
-- nibabel (>=3.0)
-- nilearn (>=0.7)
-- numpy (>=1.14)
-- scikit-learn (>=0.17)
-- scipy
-
-You can get started by installing ``neuromaps`` from the source repository
-with:
-
-.. code-block:: bash
-
-    git clone https://github.com/netneurolab/neuromaps
-    cd neuromaps
-    pip install .
-
-You will also need to have `Connectome Workbench <https://www.humanconnectome.
-org/software/connectome-workbench>`_ installed and available on your path in
-order to use most of the transformation / resampling functionality of
-``neuromaps``.
-
-.. _installation:
-
-Citation
---------
-
-If you use the ``neuromaps`` toolbox, please cite our `paper <https://www.nature.com/articles/s41592-022-01625-w>`_.
-If you use data included in the ``neuromaps`` repository, be sure to cite the original paper that published this data.
-A table with references for each brain map can be found in the Wiki.
-
-License information
--------------------
-
-This work is licensed under a
-Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ``cc-by-nc-sa``.
-The full license can be found in the
-`LICENSE <https://github.com/netneurolab/neuromaps/blob/main/neuromaps
-/LICENSE>`_ file in the ``neuromaps`` distribution.
+Metadata-Version: 2.1
+Name: neuromaps
+Version: 0.0.4
+Summary: A toolbox for projecting, resampling, and comparing brain maps
+Home-page: https://github.com/netneurolab/neuromaps
+Download-URL: https://github.com/netneurolab/neuromaps
+Author: Network Neuroscience Lab
+Maintainer: Network Neuroscience Lab
+Maintainer-email: rossmarkello+coding@gmail.com
+License: BSD-3
+Platform: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides: neuromaps
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: doc
+Provides-Extra: nulls
+Provides-Extra: style
+Provides-Extra: test
+Provides-Extra: all
+License-File: LICENSE
+
+.. image:: neuromaps_logo.png
+
+The ``neuromaps`` toolbox is designed to help researchers make easy,
+statistically-rigorous comparisons between brain maps (or brain annotations).
+
+The accompanying paper is published in `Nature Methods <https://www.nature.com/articles/s41592-022-01625-w>`_.
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5842499.svg
+   :target: https://doi.org/10.5281/zenodo.5842499
+
+Installation requirements
+-------------------------
+
+Currently, ``neuromaps`` works with Python 3.7+ and requires a few
+dependencies:
+
+- matplotlib
+- nibabel (>=3.0)
+- nilearn (>=0.7)
+- numpy (>=1.14)
+- scikit-learn (>=0.17)
+- scipy
+
+You can get started by installing ``neuromaps`` from the source repository
+with:
+
+.. code-block:: bash
+
+    git clone https://github.com/netneurolab/neuromaps
+    cd neuromaps
+    pip install .
+
+You will also need to have `Connectome Workbench <https://www.humanconnectome.
+org/software/connectome-workbench>`_ installed and available on your path in
+order to use most of the transformation / resampling functionality of
+``neuromaps``.
+
+.. _installation:
+
+Citation
+--------
+
+If you use the ``neuromaps`` toolbox, please cite our `paper <https://www.nature.com/articles/s41592-022-01625-w>`_.
+If you use data included in the ``neuromaps`` repository, be sure to cite the original paper that published this data.
+A table with references for each brain map can be found in the Wiki.
+
+License information
+-------------------
+
+This work is licensed under a
+Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ``cc-by-nc-sa``.
+The full license can be found in the
+`LICENSE <https://github.com/netneurolab/neuromaps/blob/main/neuromaps
+/LICENSE>`_ file in the ``neuromaps`` distribution.
```

### Comparing `neuromaps-0.0.3/neuromaps.egg-info/SOURCES.txt` & `neuromaps-0.0.4/neuromaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuromaps-0.0.3/setup.cfg` & `neuromaps-0.0.4/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6e65 7572 6f6d 6170 730a 7572 6c20  = neuromaps.url 
-00000020: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000030: 2e63 6f6d 2f6e 6574 6e65 7572 6f6c 6162  .com/netneurolab
-00000040: 2f6e 6575 726f 6d61 7073 0a64 6f77 6e6c  /neuromaps.downl
-00000050: 6f61 645f 7572 6c20 3d20 6874 7470 733a  oad_url = https:
-00000060: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6574  //github.com/net
-00000070: 6e65 7572 6f6c 6162 2f6e 6575 726f 6d61  neurolab/neuroma
-00000080: 7073 0a61 7574 686f 7220 3d20 4e65 7477  ps.author = Netw
-00000090: 6f72 6b20 4e65 7572 6f73 6369 656e 6365  ork Neuroscience
-000000a0: 204c 6162 0a6d 6169 6e74 6169 6e65 7220   Lab.maintainer 
-000000b0: 3d20 4e65 7477 6f72 6b20 4e65 7572 6f73  = Network Neuros
-000000c0: 6369 656e 6365 204c 6162 0a6d 6169 6e74  cience Lab.maint
-000000d0: 6169 6e65 725f 656d 6169 6c20 3d20 726f  ainer_email = ro
-000000e0: 7373 6d61 726b 656c 6c6f 2b63 6f64 696e  ssmarkello+codin
-000000f0: 6740 676d 6169 6c2e 636f 6d0a 636c 6173  g@gmail.com.clas
-00000100: 7369 6669 6572 7320 3d20 0a09 4465 7665  sifiers = ..Deve
-00000110: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000120: 3a20 3320 2d20 416c 7068 610a 0949 6e74  : 3 - Alpha..Int
-00000130: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000140: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000150: 6368 0a09 4c69 6365 6e73 6520 3a3a 204f  ch..License :: O
-00000160: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
-00000170: 5344 204c 6963 656e 7365 0a09 5072 6f67  SD License..Prog
-00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001a0: 370a 0950 726f 6772 616d 6d69 6e67 204c  7..Programming L
-000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001c0: 6e20 3a3a 2033 2e38 0a09 5072 6f67 7261  n :: 3.8..Progra
-000001d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001e0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-000001f0: 6c69 6365 6e73 6520 3d20 4253 442d 330a  license = BSD-3.
-00000200: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
-00000210: 746f 6f6c 626f 7820 666f 7220 7072 6f6a  toolbox for proj
-00000220: 6563 7469 6e67 2c20 7265 7361 6d70 6c69  ecting, resampli
-00000230: 6e67 2c20 616e 6420 636f 6d70 6172 696e  ng, and comparin
-00000240: 6720 6272 6169 6e20 6d61 7073 0a6c 6f6e  g brain maps.lon
-00000250: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000260: 6669 6c65 3a52 4541 444d 452e 7273 740a  file:README.rst.
-00000270: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000280: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000290: 7465 7874 2f78 2d72 7374 3b20 6368 6172  text/x-rst; char
-000002a0: 7365 743d 5554 462d 380a 706c 6174 666f  set=UTF-8.platfo
-000002b0: 726d 7320 3d20 4f53 2049 6e64 6570 656e  rms = OS Indepen
-000002c0: 6465 6e74 0a70 726f 7669 6465 7320 3d20  dent.provides = 
-000002d0: 0a09 6e65 7572 6f6d 6170 730a 0a5b 6f70  ..neuromaps..[op
-000002e0: 7469 6f6e 735d 0a70 7974 686f 6e5f 7265  tions].python_re
-000002f0: 7175 6972 6573 203d 203e 3d33 2e37 0a69  quires = >=3.7.i
-00000300: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000310: 3d20 0a09 6d61 7470 6c6f 746c 6962 0a09  = ..matplotlib..
-00000320: 6e69 6261 6265 6c20 3e3d 332e 302e 300a  nibabel >=3.0.0.
-00000330: 096e 696c 6561 726e 0a09 6e75 6d70 7920  .nilearn..numpy 
-00000340: 3e3d 312e 3134 2e30 0a09 7363 696b 6974  >=1.14.0..scikit
-00000350: 2d6c 6561 726e 0a09 7363 6970 7920 3e3d  -learn..scipy >=
-00000360: 302e 3137 0a7a 6970 5f73 6166 6520 3d20  0.17.zip_safe = 
-00000370: 4661 6c73 650a 7061 636b 6167 6573 203d  False.packages =
-00000380: 2066 696e 643a 0a0a 5b6f 7074 696f 6e73   find:..[options
-00000390: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-000003a0: 0a64 6f63 203d 200a 0973 7068 696e 7820  .doc = ..sphinx 
-000003b0: 3e3d 322e 300a 0973 7068 696e 785f 7274  >=2.0..sphinx_rt
-000003c0: 645f 7468 656d 650a 6e75 6c6c 7320 3d20  d_theme.nulls = 
-000003d0: 0a09 6272 6169 6e73 6d61 7368 203e 3d30  ..brainsmash >=0
-000003e0: 2e31 302e 300a 0962 7261 696e 7370 6163  .10.0..brainspac
-000003f0: 650a 7374 796c 6520 3d20 0a09 666c 616b  e.style = ..flak
-00000400: 6538 0a74 6573 7420 3d20 0a09 636f 7665  e8.test = ..cove
-00000410: 7261 6765 0a09 7079 7465 7374 203e 3d33  rage..pytest >=3
-00000420: 2e36 0a09 7079 7465 7374 2d63 6f76 0a61  .6..pytest-cov.a
-00000430: 6c6c 203d 200a 0925 2864 6f63 2973 0a09  ll = ..%(doc)s..
-00000440: 2528 6e75 6c6c 7329 730a 0925 2873 7479  %(nulls)s..%(sty
-00000450: 6c65 2973 0a09 2528 7465 7374 2973 0a0a  le)s..%(test)s..
-00000460: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000470: 5f64 6174 615d 0a6e 6575 726f 6d61 7073  _data].neuromaps
-00000480: 203d 200a 0964 6174 612f 2a0a 0964 6174   = ..data/*..dat
-00000490: 6173 6574 732f 6461 7461 2f2a 0a0a 5b62  asets/data/*..[b
-000004a0: 6469 7374 5f77 6865 656c 5d0a 756e 6976  dist_wheel].univ
-000004b0: 6572 7361 6c20 3d20 310a 0a5b 636f 7665  ersal = 1..[cove
-000004c0: 7261 6765 3a72 756e 5d0a 6f6d 6974 203d  rage:run].omit =
-000004d0: 200a 096e 6575 726f 6d61 7073 2f5f 7665   ..neuromaps/_ve
-000004e0: 7273 696f 6e2e 7079 0a0a 5b66 6c61 6b65  rsion.py..[flake
-000004f0: 385d 0a64 6f63 7465 7374 7320 3d20 5472  8].doctests = Tr
-00000500: 7565 0a65 7863 6c75 6465 203d 200a 092a  ue.exclude = ..*
-00000510: 6275 696c 642f 0a09 2a73 7068 696e 782a  build/..*sphinx*
-00000520: 0a09 2a2f 5f5f 696e 6974 5f5f 2e70 790a  ..*/__init__.py.
-00000530: 6967 6e6f 7265 203d 2057 3530 332c 2045  ignore = W503, E
-00000540: 3430 320a 6d61 782d 6c69 6e65 2d6c 656e  402.max-line-len
-00000550: 6774 6820 3d20 3739 0a0a 5b74 6f6f 6c3a  gth = 79..[tool:
-00000560: 7079 7465 7374 5d0a 646f 6374 6573 745f  pytest].doctest_
-00000570: 6f70 7469 6f6e 666c 6167 7320 3d20 4e4f  optionflags = NO
-00000580: 524d 414c 495a 455f 5748 4954 4553 5041  RMALIZE_WHITESPA
-00000590: 4345 0a78 6661 696c 5f73 7472 6963 7420  CE.xfail_strict 
-000005a0: 3d20 7472 7565 0a61 6464 6f70 7473 203d  = true.addopts =
-000005b0: 202d 7278 0a6d 6172 6b65 7273 203d 200a   -rx.markers = .
-000005c0: 0977 6f72 6b62 656e 6368 3a20 6d61 726b  .workbench: mark
-000005d0: 2061 2074 6573 7420 6173 2072 6571 7569   a test as requi
-000005e0: 7269 6e67 2063 6f6e 6e65 6374 6f6d 6520  ring connectome 
-000005f0: 776f 726b 6265 6e63 680a 0a5b 7665 7273  workbench..[vers
-00000600: 696f 6e65 6572 5d0a 5643 5320 3d20 6769  ioneer].VCS = gi
-00000610: 740a 7374 796c 6520 3d20 7065 7034 3430  t.style = pep440
-00000620: 0a76 6572 7369 6f6e 6669 6c65 5f73 6f75  .versionfile_sou
-00000630: 7263 6520 3d20 6e65 7572 6f6d 6170 732f  rce = neuromaps/
-00000640: 5f76 6572 7369 6f6e 2e70 790a 7665 7273  _version.py.vers
-00000650: 696f 6e66 696c 655f 6275 696c 6420 3d20  ionfile_build = 
-00000660: 6e65 7572 6f6d 6170 732f 5f76 6572 7369  neuromaps/_versi
-00000670: 6f6e 2e70 790a 7461 675f 7072 6566 6978  on.py.tag_prefix
-00000680: 203d 200a 7061 7265 6e74 6469 725f 7072   = .parentdir_pr
-00000690: 6566 6978 203d 200a 0a5b 6567 675f 696e  efix = ..[egg_in
-000006a0: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
-000006b0: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206e 6575 726f 6d61 7073 0d0a 7572   = neuromaps..ur
+00000020: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000030: 7562 2e63 6f6d 2f6e 6574 6e65 7572 6f6c  ub.com/netneurol
+00000040: 6162 2f6e 6575 726f 6d61 7073 0d0a 646f  ab/neuromaps..do
+00000050: 776e 6c6f 6164 5f75 726c 203d 2068 7474  wnload_url = htt
+00000060: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000070: 6e65 746e 6575 726f 6c61 622f 6e65 7572  netneurolab/neur
+00000080: 6f6d 6170 730d 0a61 7574 686f 7220 3d20  omaps..author = 
+00000090: 4e65 7477 6f72 6b20 4e65 7572 6f73 6369  Network Neurosci
+000000a0: 656e 6365 204c 6162 0d0a 6d61 696e 7461  ence Lab..mainta
+000000b0: 696e 6572 203d 204e 6574 776f 726b 204e  iner = Network N
+000000c0: 6575 726f 7363 6965 6e63 6520 4c61 620d  euroscience Lab.
+000000d0: 0a6d 6169 6e74 6169 6e65 725f 656d 6169  .maintainer_emai
+000000e0: 6c20 3d20 726f 7373 6d61 726b 656c 6c6f  l = rossmarkello
+000000f0: 2b63 6f64 696e 6740 676d 6169 6c2e 636f  +coding@gmail.co
+00000100: 6d0d 0a63 6c61 7373 6966 6965 7273 203d  m..classifiers =
+00000110: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
+00000120: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
+00000130: 7068 610d 0a09 496e 7465 6e64 6564 2041  pha...Intended A
+00000140: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
+00000150: 6365 2f52 6573 6561 7263 680d 0a09 4c69  ce/Research...Li
+00000160: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000170: 726f 7665 6420 3a3a 2042 5344 204c 6963  roved :: BSD Lic
+00000180: 656e 7365 0d0a 0950 726f 6772 616d 6d69  ense...Programmi
+00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001a0: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0950  ython :: 3.7...P
+000001b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001d0: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 2e39 0d0a 6c69  ython :: 3.9..li
+00000200: 6365 6e73 6520 3d20 4253 442d 330d 0a64  cense = BSD-3..d
+00000210: 6573 6372 6970 7469 6f6e 203d 2041 2074  escription = A t
+00000220: 6f6f 6c62 6f78 2066 6f72 2070 726f 6a65  oolbox for proje
+00000230: 6374 696e 672c 2072 6573 616d 706c 696e  cting, resamplin
+00000240: 672c 2061 6e64 2063 6f6d 7061 7269 6e67  g, and comparing
+00000250: 2062 7261 696e 206d 6170 730d 0a6c 6f6e   brain maps..lon
+00000260: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+00000270: 6669 6c65 3a52 4541 444d 452e 7273 740d  file:README.rst.
+00000280: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000290: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+000002a0: 2074 6578 742f 782d 7273 743b 2063 6861   text/x-rst; cha
+000002b0: 7273 6574 3d55 5446 2d38 0d0a 706c 6174  rset=UTF-8..plat
+000002c0: 666f 726d 7320 3d20 4f53 2049 6e64 6570  forms = OS Indep
+000002d0: 656e 6465 6e74 0d0a 7072 6f76 6964 6573  endent..provides
+000002e0: 203d 200d 0a09 6e65 7572 6f6d 6170 730d   = ...neuromaps.
+000002f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
+00000300: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000310: 3e3d 332e 370d 0a69 6e73 7461 6c6c 5f72  >=3.7..install_r
+00000320: 6571 7569 7265 7320 3d20 0d0a 096d 6174  equires = ...mat
+00000330: 706c 6f74 6c69 620d 0a09 6e69 6261 6265  plotlib...nibabe
+00000340: 6c20 3e3d 332e 302e 300d 0a09 6e69 6c65  l >=3.0.0...nile
+00000350: 6172 6e0d 0a09 6e75 6d70 7920 3e3d 312e  arn...numpy >=1.
+00000360: 3134 2e30 0d0a 0973 6369 6b69 742d 6c65  14.0...scikit-le
+00000370: 6172 6e0d 0a09 7363 6970 7920 3e3d 302e  arn...scipy >=0.
+00000380: 3137 0d0a 7a69 705f 7361 6665 203d 2046  17..zip_safe = F
+00000390: 616c 7365 0d0a 7061 636b 6167 6573 203d  alse..packages =
+000003a0: 2066 696e 643a 0d0a 0d0a 5b6f 7074 696f   find:....[optio
+000003b0: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
+000003c0: 655d 0d0a 646f 6320 3d20 0d0a 0973 7068  e]..doc = ...sph
+000003d0: 696e 7820 3e3d 322e 300d 0a09 7370 6869  inx >=2.0...sphi
+000003e0: 6e78 5f72 7464 5f74 6865 6d65 0d0a 6e75  nx_rtd_theme..nu
+000003f0: 6c6c 7320 3d20 0d0a 0962 7261 696e 736d  lls = ...brainsm
+00000400: 6173 6820 3e3d 302e 3130 2e30 0d0a 0962  ash >=0.10.0...b
+00000410: 7261 696e 7370 6163 650d 0a73 7479 6c65  rainspace..style
+00000420: 203d 200d 0a09 666c 616b 6538 0d0a 7465   = ...flake8..te
+00000430: 7374 203d 200d 0a09 636f 7665 7261 6765  st = ...coverage
+00000440: 0d0a 0970 7974 6573 7420 3e3d 332e 360d  ...pytest >=3.6.
+00000450: 0a09 7079 7465 7374 2d63 6f76 0d0a 616c  ..pytest-cov..al
+00000460: 6c20 3d20 0d0a 0925 2864 6f63 2973 0d0a  l = ...%(doc)s..
+00000470: 0925 286e 756c 6c73 2973 0d0a 0925 2873  .%(nulls)s...%(s
+00000480: 7479 6c65 2973 0d0a 0925 2874 6573 7429  tyle)s...%(test)
+00000490: 730d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  s....[options.pa
+000004a0: 636b 6167 655f 6461 7461 5d0d 0a6e 6575  ckage_data]..neu
+000004b0: 726f 6d61 7073 203d 200d 0a09 6461 7461  romaps = ...data
+000004c0: 2f2a 0d0a 0964 6174 6173 6574 732f 6461  /*...datasets/da
+000004d0: 7461 2f2a 0d0a 0d0a 5b62 6469 7374 5f77  ta/*....[bdist_w
+000004e0: 6865 656c 5d0d 0a75 6e69 7665 7273 616c  heel]..universal
+000004f0: 203d 2031 0d0a 0d0a 5b63 6f76 6572 6167   = 1....[coverag
+00000500: 653a 7275 6e5d 0d0a 6f6d 6974 203d 200d  e:run]..omit = .
+00000510: 0a09 6e65 7572 6f6d 6170 732f 5f76 6572  ..neuromaps/_ver
+00000520: 7369 6f6e 2e70 790d 0a0d 0a5b 666c 616b  sion.py....[flak
+00000530: 6538 5d0d 0a64 6f63 7465 7374 7320 3d20  e8]..doctests = 
+00000540: 5472 7565 0d0a 6578 636c 7564 6520 3d20  True..exclude = 
+00000550: 0d0a 092a 6275 696c 642f 0d0a 092a 7370  ...*build/...*sp
+00000560: 6869 6e78 2a0d 0a09 2a2f 5f5f 696e 6974  hinx*...*/__init
+00000570: 5f5f 2e70 790d 0a69 676e 6f72 6520 3d20  __.py..ignore = 
+00000580: 5735 3033 2c20 4534 3032 0d0a 6d61 782d  W503, E402..max-
+00000590: 6c69 6e65 2d6c 656e 6774 6820 3d20 3739  line-length = 79
+000005a0: 0d0a 0d0a 5b74 6f6f 6c3a 7079 7465 7374  ....[tool:pytest
+000005b0: 5d0d 0a64 6f63 7465 7374 5f6f 7074 696f  ]..doctest_optio
+000005c0: 6e66 6c61 6773 203d 204e 4f52 4d41 4c49  nflags = NORMALI
+000005d0: 5a45 5f57 4849 5445 5350 4143 450d 0a78  ZE_WHITESPACE..x
+000005e0: 6661 696c 5f73 7472 6963 7420 3d20 7472  fail_strict = tr
+000005f0: 7565 0d0a 6164 646f 7074 7320 3d20 2d72  ue..addopts = -r
+00000600: 780d 0a6d 6172 6b65 7273 203d 200d 0a09  x..markers = ...
+00000610: 776f 726b 6265 6e63 683a 206d 6172 6b20  workbench: mark 
+00000620: 6120 7465 7374 2061 7320 7265 7175 6972  a test as requir
+00000630: 696e 6720 636f 6e6e 6563 746f 6d65 2077  ing connectome w
+00000640: 6f72 6b62 656e 6368 0d0a 0d0a 5b76 6572  orkbench....[ver
+00000650: 7369 6f6e 6565 725d 0d0a 5643 5320 3d20  sioneer]..VCS = 
+00000660: 6769 740d 0a73 7479 6c65 203d 2070 6570  git..style = pep
+00000670: 3434 300d 0a76 6572 7369 6f6e 6669 6c65  440..versionfile
+00000680: 5f73 6f75 7263 6520 3d20 6e65 7572 6f6d  _source = neurom
+00000690: 6170 732f 5f76 6572 7369 6f6e 2e70 790d  aps/_version.py.
+000006a0: 0a76 6572 7369 6f6e 6669 6c65 5f62 7569  .versionfile_bui
+000006b0: 6c64 203d 206e 6575 726f 6d61 7073 2f5f  ld = neuromaps/_
+000006c0: 7665 7273 696f 6e2e 7079 0d0a 7461 675f  version.py..tag_
+000006d0: 7072 6566 6978 203d 200d 0a70 6172 656e  prefix = ..paren
+000006e0: 7464 6972 5f70 7265 6669 7820 3d20 0d0a  tdir_prefix = ..
+000006f0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000700: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000710: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `neuromaps-0.0.3/versioneer.py` & `neuromaps-0.0.4/versioneer.py`

 * *Files identical despite different names*

