# Comparing `tmp/qermit-0.3.0.tar.gz` & `tmp/qermit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qermit-0.3.0.tar", last modified: Fri Mar 10 15:13:12 2023, max compression
+gzip compressed data, was "qermit-0.4.0.tar", last modified: Thu May 25 09:33:02 2023, max compression
```

## Comparing `qermit-0.3.0.tar` & `qermit-0.4.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.181567 qermit-0.3.0/
--rw-r--r--   0 danielmills   (501) staff       (20)    10172 2022-09-29 03:19:21.000000 qermit-0.3.0/LICENSE
--rw-r--r--   0 danielmills   (501) staff       (20)       20 2021-05-27 11:23:58.000000 qermit-0.3.0/MANIFEST.in
--rw-r--r--   0 danielmills   (501) staff       (20)     2888 2023-03-10 15:13:12.180912 qermit-0.3.0/PKG-INFO
--rw-r--r--   0 danielmills   (501) staff       (20)     2120 2023-03-10 15:10:41.000000 qermit-0.3.0/README.md
--rw-r--r--   0 danielmills   (501) staff       (20)       22 2023-03-10 15:10:41.000000 qermit-0.3.0/_version.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.108957 qermit-0.3.0/qermit/
--rw-r--r--   0 danielmills   (501) staff       (20)     1327 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/__init__.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.118543 qermit-0.3.0/qermit/clifford_noise_characterisation/
--rw-r--r--   0 danielmills   (501) staff       (20)      868 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/clifford_noise_characterisation/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)    25982 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/clifford_noise_characterisation/ccl.py
--rw-r--r--   0 danielmills   (501) staff       (20)    10368 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/clifford_noise_characterisation/cdr_post.py
--rw-r--r--   0 danielmills   (501) staff       (20)    15897 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/clifford_noise_characterisation/dfsc.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.120434 qermit-0.3.0/qermit/frame_randomisation/
--rw-r--r--   0 danielmills   (501) staff       (20)      860 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/frame_randomisation/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)     7784 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/frame_randomisation/frame_randomisation.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.123265 qermit-0.3.0/qermit/probabilistic_error_cancellation/
--rw-r--r--   0 danielmills   (501) staff       (20)      854 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/probabilistic_error_cancellation/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)     9481 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/probabilistic_error_cancellation/cliff_circuit_gen.py
--rw-r--r--   0 danielmills   (501) staff       (20)    45528 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/probabilistic_error_cancellation/pec_learning_based.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.136377 qermit-0.3.0/qermit/spam/
--rw-r--r--   0 danielmills   (501) staff       (20)     1000 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spam/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)     8458 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spam/full_spam_correction.py
--rw-r--r--   0 danielmills   (501) staff       (20)    23307 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spam/full_transition_tomography.py
--rw-r--r--   0 danielmills   (501) staff       (20)     1944 2022-12-12 17:19:07.000000 qermit-0.3.0/qermit/spam/nn_data_generation.py
--rw-r--r--   0 danielmills   (501) staff       (20)     2440 2022-12-12 17:19:07.000000 qermit-0.3.0/qermit/spam/nn_spam.py
--rw-r--r--   0 danielmills   (501) staff       (20)     5408 2022-12-12 17:19:08.000000 qermit-0.3.0/qermit/spam/nn_spam_probability_distribution.py
--rw-r--r--   0 danielmills   (501) staff       (20)     4014 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spam/spam_mitres.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.146766 qermit-0.3.0/qermit/spectral_filtering/
--rw-r--r--   0 danielmills   (501) staff       (20)      899 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spectral_filtering/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)     1594 2022-12-12 17:19:07.000000 qermit-0.3.0/qermit/spectral_filtering/characterisation_cache.py
--rw-r--r--   0 danielmills   (501) staff       (20)     2093 2022-12-12 17:19:08.000000 qermit-0.3.0/qermit/spectral_filtering/results_cache.py
--rw-r--r--   0 danielmills   (501) staff       (20)     1378 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spectral_filtering/signal_filter.py
--rw-r--r--   0 danielmills   (501) staff       (20)    24923 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/spectral_filtering/spectral_filtering.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.154716 qermit-0.3.0/qermit/taskgraph/
--rw-r--r--   0 danielmills   (501) staff       (20)     1472 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)     5271 2022-09-29 03:19:21.000000 qermit-0.3.0/qermit/taskgraph/graphviz.py
--rw-r--r--   0 danielmills   (501) staff       (20)     5308 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/measurement_reduction.py
--rw-r--r--   0 danielmills   (501) staff       (20)    21227 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/mitex.py
--rw-r--r--   0 danielmills   (501) staff       (20)    17448 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/mitres.py
--rw-r--r--   0 danielmills   (501) staff       (20)     4121 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/mittask.py
--rw-r--r--   0 danielmills   (501) staff       (20)    18982 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/task_graph.py
--rw-r--r--   0 danielmills   (501) staff       (20)    17909 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/taskgraph/utils.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.156918 qermit-0.3.0/qermit/zero_noise_extrapolation/
--rw-r--r--   0 danielmills   (501) staff       (20)      810 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/zero_noise_extrapolation/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)    41562 2023-03-10 15:10:41.000000 qermit-0.3.0/qermit/zero_noise_extrapolation/zne.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.114631 qermit-0.3.0/qermit.egg-info/
--rw-r--r--   0 danielmills   (501) staff       (20)     2888 2023-03-10 15:13:11.000000 qermit-0.3.0/qermit.egg-info/PKG-INFO
--rw-r--r--   0 danielmills   (501) staff       (20)     1858 2023-03-10 15:13:11.000000 qermit-0.3.0/qermit.egg-info/SOURCES.txt
--rw-r--r--   0 danielmills   (501) staff       (20)        1 2023-03-10 15:13:11.000000 qermit-0.3.0/qermit.egg-info/dependency_links.txt
--rw-r--r--   0 danielmills   (501) staff       (20)        1 2021-05-27 17:47:58.000000 qermit-0.3.0/qermit.egg-info/not-zip-safe
--rw-r--r--   0 danielmills   (501) staff       (20)       33 2023-03-10 15:13:11.000000 qermit-0.3.0/qermit.egg-info/requires.txt
--rw-r--r--   0 danielmills   (501) staff       (20)       13 2023-03-10 15:13:11.000000 qermit-0.3.0/qermit.egg-info/top_level.txt
--rw-r--r--   0 danielmills   (501) staff       (20)       38 2023-03-10 15:13:12.181722 qermit-0.3.0/setup.cfg
--rw-r--r--   0 danielmills   (501) staff       (20)     1121 2023-03-10 15:10:41.000000 qermit-0.3.0/setup.py
-drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-03-10 15:13:12.178597 qermit-0.3.0/tests/
--rw-r--r--   0 danielmills   (501) staff       (20)        0 2023-03-06 15:04:40.000000 qermit-0.3.0/tests/__init__.py
--rw-r--r--   0 danielmills   (501) staff       (20)    10808 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/ccl_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     5710 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/cdr_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)    12159 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/dfsc_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     3190 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/frame_randomisation_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     4927 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/full_spam_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     4248 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/measurement_reduction_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)    10651 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/mitex_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     4836 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/mitres_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)    19697 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/pec_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     2371 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/spam_methods_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)    18817 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/spectral_filtering_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     6335 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/taskgraph_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     7586 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/tomography_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)     9036 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/utils_test.py
--rw-r--r--   0 danielmills   (501) staff       (20)    21368 2023-03-10 15:10:41.000000 qermit-0.3.0/tests/zne_test.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.093831 qermit-0.4.0/
+-rw-r--r--   0 danielmills   (501) staff       (20)    10172 2022-09-29 03:19:21.000000 qermit-0.4.0/LICENSE
+-rw-r--r--   0 danielmills   (501) staff       (20)       20 2021-05-27 11:23:58.000000 qermit-0.4.0/MANIFEST.in
+-rw-r--r--   0 danielmills   (501) staff       (20)     2892 2023-05-25 09:33:02.093476 qermit-0.4.0/PKG-INFO
+-rw-r--r--   0 danielmills   (501) staff       (20)     2124 2023-05-25 09:32:48.000000 qermit-0.4.0/README.md
+-rw-r--r--   0 danielmills   (501) staff       (20)       22 2023-05-25 09:32:48.000000 qermit-0.4.0/_version.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:01.986549 qermit-0.4.0/qermit/
+-rw-r--r--   0 danielmills   (501) staff       (20)     1390 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/__init__.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:01.993856 qermit-0.4.0/qermit/clifford_noise_characterisation/
+-rw-r--r--   0 danielmills   (501) staff       (20)      894 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/clifford_noise_characterisation/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    25981 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/clifford_noise_characterisation/ccl.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    10367 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/clifford_noise_characterisation/cdr_post.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    15897 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/clifford_noise_characterisation/dfsc.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.013468 qermit-0.4.0/qermit/frame_randomisation/
+-rw-r--r--   0 danielmills   (501) staff       (20)      873 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/frame_randomisation/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     7783 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/frame_randomisation/frame_randomisation.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.014938 qermit-0.4.0/qermit/mock_backend/
+-rw-r--r--   0 danielmills   (501) staff       (20)      793 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/mock_backend/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     7165 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/mock_backend/mock_quantinuum_backend.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.017312 qermit-0.4.0/qermit/probabilistic_error_cancellation/
+-rw-r--r--   0 danielmills   (501) staff       (20)      867 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/probabilistic_error_cancellation/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     9481 2023-03-31 09:34:34.000000 qermit-0.4.0/qermit/probabilistic_error_cancellation/cliff_circuit_gen.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    45527 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/probabilistic_error_cancellation/pec_learning_based.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.027374 qermit-0.4.0/qermit/spam/
+-rw-r--r--   0 danielmills   (501) staff       (20)     1025 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/spam/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     8457 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/spam/full_spam_correction.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    23439 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/spam/full_transition_tomography.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     1944 2022-12-12 17:19:07.000000 qermit-0.4.0/qermit/spam/nn_data_generation.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     2440 2022-12-12 17:19:07.000000 qermit-0.4.0/qermit/spam/nn_spam.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     5408 2022-12-12 17:19:08.000000 qermit-0.4.0/qermit/spam/nn_spam_probability_distribution.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     4220 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/spam/spam_mitres.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.043486 qermit-0.4.0/qermit/spectral_filtering/
+-rw-r--r--   0 danielmills   (501) staff       (20)      899 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/spectral_filtering/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     1594 2022-12-12 17:19:07.000000 qermit-0.4.0/qermit/spectral_filtering/characterisation_cache.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     2093 2022-12-12 17:19:08.000000 qermit-0.4.0/qermit/spectral_filtering/results_cache.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     1378 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/spectral_filtering/signal_filter.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    24923 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/spectral_filtering/spectral_filtering.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.070976 qermit-0.4.0/qermit/taskgraph/
+-rw-r--r--   0 danielmills   (501) staff       (20)     1550 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/taskgraph/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     5271 2022-09-29 03:19:21.000000 qermit-0.4.0/qermit/taskgraph/graphviz.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     5308 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/taskgraph/measurement_reduction.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    21227 2023-03-22 17:39:07.000000 qermit-0.4.0/qermit/taskgraph/mitex.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    17448 2023-03-22 17:39:01.000000 qermit-0.4.0/qermit/taskgraph/mitres.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     4121 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/taskgraph/mittask.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    18934 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/taskgraph/task_graph.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    17909 2023-03-10 15:10:41.000000 qermit-0.4.0/qermit/taskgraph/utils.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.073264 qermit-0.4.0/qermit/zero_noise_extrapolation/
+-rw-r--r--   0 danielmills   (501) staff       (20)      822 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/zero_noise_extrapolation/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    41803 2023-05-25 09:32:48.000000 qermit-0.4.0/qermit/zero_noise_extrapolation/zne.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:01.990255 qermit-0.4.0/qermit.egg-info/
+-rw-r--r--   0 danielmills   (501) staff       (20)     2892 2023-05-25 09:33:01.000000 qermit-0.4.0/qermit.egg-info/PKG-INFO
+-rw-r--r--   0 danielmills   (501) staff       (20)     1937 2023-05-25 09:33:01.000000 qermit-0.4.0/qermit.egg-info/SOURCES.txt
+-rw-r--r--   0 danielmills   (501) staff       (20)        1 2023-05-25 09:33:01.000000 qermit-0.4.0/qermit.egg-info/dependency_links.txt
+-rw-r--r--   0 danielmills   (501) staff       (20)        1 2021-05-27 17:47:58.000000 qermit-0.4.0/qermit.egg-info/not-zip-safe
+-rw-r--r--   0 danielmills   (501) staff       (20)       33 2023-05-25 09:33:01.000000 qermit-0.4.0/qermit.egg-info/requires.txt
+-rw-r--r--   0 danielmills   (501) staff       (20)       13 2023-05-25 09:33:01.000000 qermit-0.4.0/qermit.egg-info/top_level.txt
+-rw-r--r--   0 danielmills   (501) staff       (20)       38 2023-05-25 09:33:02.093962 qermit-0.4.0/setup.cfg
+-rw-r--r--   0 danielmills   (501) staff       (20)     1121 2023-04-11 21:04:28.000000 qermit-0.4.0/setup.py
+drwxr-xr-x   0 danielmills   (501) staff       (20)        0 2023-05-25 09:33:02.091791 qermit-0.4.0/tests/
+-rw-r--r--   0 danielmills   (501) staff       (20)        0 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/__init__.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    10808 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/ccl_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     5710 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/cdr_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    12159 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/dfsc_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     3190 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/frame_randomisation_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     4927 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/full_spam_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     4228 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/measurement_reduction_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    10651 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/mitex_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     4836 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/mitres_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    19697 2023-05-25 09:32:39.000000 qermit-0.4.0/tests/pec_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     2833 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/spam_methods_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    18769 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/spectral_filtering_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     6335 2023-03-10 15:10:41.000000 qermit-0.4.0/tests/taskgraph_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     7833 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/tomography_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)     9037 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/utils_test.py
+-rw-r--r--   0 danielmills   (501) staff       (20)    22163 2023-05-25 09:32:48.000000 qermit-0.4.0/tests/zne_test.py
```

### Comparing `qermit-0.3.0/LICENSE` & `qermit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/PKG-INFO` & `qermit-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qermit
-Version: 0.3.0
+Version: 0.4.0
 Summary: error-mitigation framework, an extension to pytket
 License: CQC Non-Commercial Use Software Licence
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Other/Proprietary License
@@ -54,16 +54,16 @@
 changes on the `main` branch, and open a PR from your fork. If it passes
 tests and is accepted after review, it will be merged in.
 
 ### Code style
 
 #### Formatting
 
-All code should be formatted using
-[black](https://black.readthedocs.io/en/stable/), with default options. 
+All code should adhere to [flake8](https://flake8.pycqa.org/en/latest/)
+formatting, ignoring only E501 and W503
 
 #### Type annotation
 
 On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
 type checker and all submissions must pass its checks. You should therefore run
 `mypy` locally on any changed files before submitting a PR.
```

### Comparing `qermit-0.3.0/README.md` & `qermit-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 changes on the `main` branch, and open a PR from your fork. If it passes
 tests and is accepted after review, it will be merged in.
 
 ### Code style
 
 #### Formatting
 
-All code should be formatted using
-[black](https://black.readthedocs.io/en/stable/), with default options. 
+All code should adhere to [flake8](https://flake8.pycqa.org/en/latest/)
+formatting, ignoring only E501 and W503
 
 #### Type annotation
 
 On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
 type checker and all submissions must pass its checks. You should therefore run
 `mypy` locally on any changed files before submitting a PR.
```

### Comparing `qermit-0.3.0/qermit/__init__.py` & `qermit-0.4.0/qermit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
-qermit provides tools for running and composing error-mitigation methods. Error 
-mitigation methods are split into two types, those which in some manner modify the set 
+qermit provides tools for running and composing error-mitigation methods. Error
+mitigation methods are split into two types, those which in some manner modify the set
 of shots returned when running quantum circuits on quantum devices (MitRes), and those which
 modify the expectation value of some observable (MitEx).
 """
-from qermit.taskgraph.task_graph import TaskGraph
-from qermit.taskgraph.mittask import (
+from qermit.taskgraph.task_graph import TaskGraph  # noqa:F401
+from qermit.taskgraph.mittask import (  # noqa:F401
     MitTask,
     AnsatzCircuit,
     CircuitShots,
     ObservableExperiment,
 )
-from qermit.taskgraph.mitres import MitRes
-from qermit.taskgraph.mitex import MitEx
-from qermit.taskgraph.utils import SymbolsDict, MeasurementCircuit, ObservableTracker
+from qermit.taskgraph.mitres import MitRes  # noqa:F401
+from qermit.taskgraph.mitex import MitEx  # noqa:F401
+from qermit.taskgraph.utils import SymbolsDict, MeasurementCircuit, ObservableTracker  # noqa:F401
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)  # type: ignore
```

### Comparing `qermit-0.3.0/qermit/clifford_noise_characterisation/__init__.py` & `qermit-0.4.0/qermit/spam/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
-The clifford_noise_characterisation module provides generator methods for producing MitEx
-objects that automatically characterise and correct some device noise using
-characterisation via Clifford circuits.
+The spam module defines tasks for completing SPAM Mitigation methods, and generator
+functions for producing MitRes objects that automatically characterise and apply SPAM
+Mitigation methods to experiment results.
 """
-from .ccl import (
-    gen_CDR_MitEx,
+from .spam_mitres import (  # noqa:F401
+    gen_FullyCorrelated_SPAM_MitRes,
+    gen_UnCorrelated_SPAM_MitRes,
+    CorrectionMethod,
 )
-from .dfsc import gen_DFSC_MitEx
+from .full_transition_tomography import FullCorrelatedNoiseCharacterisation  # noqa:F401
```

### Comparing `qermit-0.3.0/qermit/clifford_noise_characterisation/ccl.py` & `qermit-0.4.0/qermit/clifford_noise_characterisation/ccl.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         if len(noisy_exp) != len(exact_exp):
             raise RuntimeError(
                 "Batching task should receive identical number of Simulated and Device run results."
             )
 
         zipped = list(zip(noisy_exp, exact_exp))
         chunked_zipped = [
-            zipped[i : i + n_state_circuits]
+            zipped[i: i + n_state_circuits]
             for i in range(0, len(zipped), n_state_circuits)
         ]
         return (chunked_zipped,)
 
     return MitTask(
         _label="CCLBatchResults", _n_in_wires=2, _n_out_wires=1, _method=task
     )
```

### Comparing `qermit-0.3.0/qermit/clifford_noise_characterisation/cdr_post.py` & `qermit-0.4.0/qermit/clifford_noise_characterisation/cdr_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from abc import ABC, abstractmethod
 from typing import List, Tuple, cast, Dict, Union
 
-import numpy as np  #  type: ignore
+import numpy as np  # type: ignore
 from pytket.utils import QubitPauliOperator
 from pytket.pauli import QubitPauliString  # type: ignore
 from qermit import MitTask
 from copy import copy
 import math
 import warnings
 from sympy.core.expr import Expr
```

### Comparing `qermit-0.3.0/qermit/clifford_noise_characterisation/dfsc.py` & `qermit-0.4.0/qermit/clifford_noise_characterisation/dfsc.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/frame_randomisation/__init__.py` & `qermit-0.4.0/qermit/frame_randomisation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 """
 The frame_randomisation module provides generator methods for producing MitRes objects
 that automatically run frame randomisation protocols (a generalisation of randomised
 compilation).
 """
 
-from .frame_randomisation import FrameRandomisation, gen_Frame_Randomisation_MitRes
+from .frame_randomisation import FrameRandomisation, gen_Frame_Randomisation_MitRes  # noqa:F401
```

### Comparing `qermit-0.3.0/qermit/frame_randomisation/frame_randomisation.py` & `qermit-0.4.0/qermit/frame_randomisation/frame_randomisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         :param all_fr_results: A list of BackendResult objects for all frame randomisations for all experiment circuits.
         :type: all_fr_results: List[BackendResult]
 
         :return: Collated BackendResult objects, reflecting frame randomisation procedure
         :rtype: Tuple[List[BackendResult]]
         """
         chunked_results = [
-            all_fr_results[i : i + samples]
+            all_fr_results[i: i + samples]
             for i in range(0, len(all_fr_results), samples)
         ]
         results = []
         for chunk in chunked_results:
             all_counts = [result.get_counts() for result in chunk]
             combined_counts = reduce(operator.add, all_counts)
             outcome_array = {
```

### Comparing `qermit-0.3.0/qermit/probabilistic_error_cancellation/__init__.py` & `qermit-0.4.0/qermit/probabilistic_error_cancellation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 
 """
 The probabilistic_error_cancellation module provides generator methods for producing
 MitEx objects that automatically characterise and correct device noise via
 Probabilistic Error Cancellation.
 """
 
-from .pec_learning_based import (
+from .pec_learning_based import (  # noqa:F401
     gen_PEC_learning_based_MitEx,
 )
```

### Comparing `qermit-0.3.0/qermit/probabilistic_error_cancellation/cliff_circuit_gen.py` & `qermit-0.4.0/qermit/probabilistic_error_cancellation/cliff_circuit_gen.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/probabilistic_error_cancellation/pec_learning_based.py` & `qermit-0.4.0/qermit/probabilistic_error_cancellation/pec_learning_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         # of quasi probabilities. Each inner list now consists of results
         # corresponding to one ideal circuit.
         first = 0
         for experiment in prob_list:
             # The number of noisy circuits corresponding to one ideal.
             last = len(experiment[0])
             # Append portion of the list of noisy results that relate to one circuit.
-            circ_results_list.append(noisy_circ_results[first : first + last])
+            circ_results_list.append(noisy_circ_results[first: first + last])
             first += last
 
         # Create new list with mitigated results
         em_expect_list = []
         for circuit_results, circuit_prob in zip(circ_results_list, prob_list):
             em_expect = {}
             for i, qps in enumerate(circuit_results[0]._dict):
```

### Comparing `qermit-0.3.0/qermit/spam/__init__.py` & `qermit-0.4.0/qermit/zero_noise_extrapolation/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
-The spam module defines tasks for completing SPAM Mitigation methods, and generator
-functions for producing MitRes objects that automatically characterise and apply SPAM 
-Mitigation methods to experiment results.
+The zero_noise_extrapolation module provides generator methods for producing MitEx
+objects that automatically run digital zero noise extrapolation protocols.
 """
-from .spam_mitres import (
-    gen_FullyCorrelated_SPAM_MitRes,
-    gen_UnCorrelated_SPAM_MitRes,
-    CorrectionMethod,
+from .zne import (  # noqa:F401
+    gen_ZNE_MitEx,
+    Folding,
+    Fit,
 )
-from .full_transition_tomography import FullCorrelatedNoiseCharacterisation
```

### Comparing `qermit-0.3.0/qermit/spam/full_spam_correction.py` & `qermit-0.4.0/qermit/spam/full_spam_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
                 is qubit_subsets
             ):
                 return (wire, [], [])
 
         process_circuit = Circuit(
             len([qb for subset in qubit_subsets for qb in subset])
         )
-
         tomo_circuit_states = get_full_transition_tomography_circuits(
             process_circuit, backend, qubit_subsets
         )
 
         tomo_circuit_shots = [
             CircuitShots(Circuit=c, Shots=shots) for c in tomo_circuit_states[0]
         ]
```

### Comparing `qermit-0.3.0/qermit/spam/full_transition_tomography.py` & `qermit-0.4.0/qermit/spam/full_transition_tomography.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 FullCorrelatedNoiseCharacterisation = namedtuple(
     "FullCorrelatedNoiseCharacterisation",
     ["CorrelatedNodes", "NodeToIntDict", "CharacterisationMatrices"],
 )
 
 StateInfo = namedtuple("StateInfo", ["PreparedStates", "QubitBitMaps"])
 
+
 # Helper methods for holding basis states
 @lru_cache(maxsize=128)
 def binary_to_int(bintuple: Tuple[int]) -> int:
     """Convert a binary tuple to corresponding integer, with most significant bit as the
     first element of tuple.
 
     :param bintuple: Binary tuple
@@ -81,21 +82,19 @@
         provide a single list.  The qubits in `correlations` must be nodes in the
         backend's associated `Device`.
     :type correlations: List[List[Node]]
     :return: A list of calibration circuits to be run on the machine. The circuits
         should be processed without compilation.
     :rtype: List[Circuit]
     """
-
     subsets_matrix_map = OrderedDict.fromkeys(
         sorted(map(tuple, correlations), key=len, reverse=True)
     )
     # ordered from largest to smallest via OrderedDict & sorted
     subset_dimensions = [len(subset) for subset in subsets_matrix_map]
-
     major_state_dimensions = subset_dimensions[0]
     n_circuits = 1 << major_state_dimensions
     all_qubits = [qb for subset in correlations for qb in subset]
 
     if len(process_circuit.qubits) != len(all_qubits):
         raise ValueError(
             "Process being characterised has {} qubits, correlations only specify {} qubits.".format(
@@ -108,17 +107,22 @@
     state_infos = []
 
     # set up CircBox of X gate for preparing basis states
     xcirc = Circuit(1).X(0)
     xcirc = backend.get_compiled_circuit(xcirc)
     FlattenRegisters().apply(xcirc)
     xbox = CircBox(xcirc)
-
     # need to be default register to add as box suitably
+
+    n_qubits_pre_compile = process_circuit.n_qubits
     process_circuit = backend.get_compiled_circuit(process_circuit)
+
+    while process_circuit.n_qubits < n_qubits_pre_compile:
+        process_circuit.add_qubit(Qubit("temp_q", process_circuit.n_qubits))
+
     rename_map_pc = {}
     for index, qb in enumerate(process_circuit.qubits):
         rename_map_pc[qb] = Qubit(index)
     process_circuit.rename_units(rename_map_pc)
     pbox = CircBox(process_circuit)
 
     # set up base circuit for appending xbox to
@@ -143,14 +147,15 @@
             # add state to prepared states
             new_state_dicts[qubits] = major_state[:dim]
             # find only qubits that are expected to be in 1 state, add xbox to given qubits
             for flipped_qb in itertools.compress(qubits, major_state[:dim]):
                 state_circuit.add_circbox(xbox, [flipped_qb])
         # Decompose boxes, add barriers to preserve circuit, add measures
         state_circuit.add_barrier(all_qubits)
+
         # add process circuit to measure
         state_circuit.add_circbox(pbox, state_circuit.qubits)
         DecomposeBoxes().apply(state_circuit)
         state_circuit.add_barrier(all_qubits)
         for q in measures:
             state_circuit.Measure(q, measures[q])
         # add to returned types
@@ -217,22 +222,21 @@
     # normalise everything
     normalised_mats = [mat / np.sum(mat, axis=0) for mat in subsets_matrix_map.values()]  # type: ignore
     return FullCorrelatedNoiseCharacterisation(
         correlations, node_index_dict, normalised_mats
     )
 
 
-#########################################
-### _compute_dot and helper functions ###
-###
-### With thanks to
-### https://math.stackexchange.com/a/3423910
-### and especially
-### https://gist.github.com/ahwillia/f65bc70cb30206d4eadec857b98c4065
-### on which this code is based.
+# _compute_dot and helper functions #
+#
+# With thanks to
+# https://math.stackexchange.com/a/3423910
+# and especially
+# https://gist.github.com/ahwillia/f65bc70cb30206d4eadec857b98c4065
+# on which this code is based.
 def _unfold(tens: np.ndarray, mode: int, dims: List[int]) -> np.ndarray:
     """
     Unfolds tensor into matrix.
 
     :param tens: Tensor with shape equivalent to dimensions
     :type tens: np.ndarray
     :param mode: Specifies axis move to front of matrix in unfolding of tensor
```

### Comparing `qermit-0.3.0/qermit/spam/nn_data_generation.py` & `qermit-0.4.0/qermit/spam/nn_data_generation.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spam/nn_spam.py` & `qermit-0.4.0/qermit/spam/nn_spam.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spam/nn_spam_probability_distribution.py` & `qermit-0.4.0/qermit/spam/nn_spam_probability_distribution.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spam/spam_mitres.py` & `qermit-0.4.0/qermit/spam/spam_mitres.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,11 +97,16 @@
     :param backend: Default Backend characterisation and experiment are executed on.
     :type backend: Backend
     :param calibration_shots: Number of shots required for each characterisation circuit
     :type calibration_shots: int
     """
     if backend.backend_info is None:
         raise ValueError("Backend has no backend_info attribute.")
+    if len(backend.backend_info.architecture.nodes) == 0:
+        raise ValueError(
+            "Backend Architecture has no specified Nodes, please use a Backend with a specified Architecture."
+        )
     correlations = [[n] for n in backend.backend_info.architecture.nodes]
+
     return gen_FullyCorrelated_SPAM_MitRes(
         backend, calibration_shots, correlations, **kwargs
     )
```

### Comparing `qermit-0.3.0/qermit/spectral_filtering/__init__.py` & `qermit-0.4.0/qermit/spectral_filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spectral_filtering/characterisation_cache.py` & `qermit-0.4.0/qermit/spectral_filtering/characterisation_cache.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spectral_filtering/results_cache.py` & `qermit-0.4.0/qermit/spectral_filtering/results_cache.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spectral_filtering/signal_filter.py` & `qermit-0.4.0/qermit/spectral_filtering/signal_filter.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/spectral_filtering/spectral_filtering.py` & `qermit-0.4.0/qermit/spectral_filtering/spectral_filtering.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/taskgraph/__init__.py` & `qermit-0.4.0/qermit/taskgraph/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,37 +13,37 @@
 # limitations under the License.
 
 
 """
 The taskgraph module defines the TaskGraph, MitRes and MitTask objects, through which
 mitigated experiments are run.
 """
-from .task_graph import TaskGraph
-from .mittask import (
+from .task_graph import TaskGraph  # noqa:F401
+from .mittask import (  # noqa:F401
     MitTask,
     IOTask,
     CircuitShots,
     Wire,
     duplicate_wire_task_gen,
     AnsatzCircuit,
     ObservableExperiment,
 )
-from .mitres import (
+from .mitres import (  # noqa:F401
     MitRes,
     backend_compile_circuit_shots_task_gen,
     backend_handle_task_gen,
     backend_res_task_gen,
     split_shots_task_gen,
     group_shots_task_gen,
     gen_shot_split_MitRes,
 )
-from .mitex import (
+from .mitex import (  # noqa:F401
     MitEx,
     gen_compiled_MitRes,
     filter_observable_tracker_task_gen,
     collate_circuit_shots_task_gen,
     split_results_task_gen,
     get_expectations_task_gen,
     gen_compiled_shot_split_MitRes,
 )
-from .utils import SymbolsDict, MeasurementCircuit, ObservableTracker
-from .measurement_reduction import gen_MeasurementReduction_MitEx
+from .utils import SymbolsDict, MeasurementCircuit, ObservableTracker  # noqa:F401
+from .measurement_reduction import gen_MeasurementReduction_MitEx  # noqa:F401
```

### Comparing `qermit-0.3.0/qermit/taskgraph/graphviz.py` & `qermit-0.4.0/qermit/taskgraph/graphviz.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/taskgraph/measurement_reduction.py` & `qermit-0.4.0/qermit/taskgraph/measurement_reduction.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/taskgraph/mitex.py` & `qermit-0.4.0/qermit/taskgraph/mitex.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/taskgraph/mitres.py` & `qermit-0.4.0/qermit/taskgraph/mitres.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/taskgraph/mittask.py` & `qermit-0.4.0/qermit/taskgraph/mittask.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/taskgraph/task_graph.py` & `qermit-0.4.0/qermit/taskgraph/task_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
     def decompose_TaskGraph_nodes(self):
         """
         For each node in self._task_graph, if node is a TaskGraph object, substitutes that node
         with the _task_graph structure held inside the node.
         """
         check_for_decompose = True
-        while check_for_decompose == True:
+        while check_for_decompose:
             # get all nodes and iterate through them
             check_for_decompose = False
             node_list = list(nx.topological_sort(self._task_graph))
             for task in node_list:
                 # => TaskGraph object with _task_graph attribute for decomposition
                 if hasattr(task, "_task_graph"):
                     # relabel task names for ease of viewing wit visualisation methods
@@ -247,16 +247,15 @@
                     )
 
                     if (
                         len(
                             set(task_input_out_edges).intersection(
                                 set(task_output_in_edges)
                             )
-                        )
-                        > 0
+                        ) > 0
                     ):
                         raise ValueError(
                             "Decomposition of TaskGraph node {}, not permitted: TaskGraph to be decomposed has edge between input and output vertices.".format(
                                 task
                             )
                         )
 
@@ -374,15 +373,15 @@
         # topological_sort fixes any dependency issues so can iterate and assume
         # input wires all realised before a task is reached
         node_list = list(nx.topological_sort(self._task_graph))
 
         self.characterisation.update(characterisation)
         # clear cache of held data if required
         # also check that all mittask label are unique else dict will fail
-        if cache == True:
+        if cache:
             unique_labels = set()
             for task in node_list:
                 if task not in (self._i, self._o):
                     unique_labels.add(task._label)
             if len(unique_labels) != len(self._task_graph) - 2:
                 raise ValueError(
                     "Cache can't store all information as not all MitTask labels are unique."
@@ -400,15 +399,15 @@
             inputs = [None] * len(in_edges)
             for _, _, ports, i_data in in_edges:
                 assert i_data["data"] is not None
                 inputs[ports[1]] = i_data["data"]
             # run held task
             outputs = task(inputs)
             self.characterisation.update(task.characterisation)
-            if cache == True:
+            if cache:
                 self._cache[task._label] = (task, outputs)
             # assign outputs ot out_edges of task
             out_edges = self._task_graph.out_edges(task, data=True, keys=True)
             assert len(out_edges) == len(outputs)
             for _, _, ports, o_data in out_edges:
                 o_data["data"] = outputs[ports[0]]
```

### Comparing `qermit-0.3.0/qermit/taskgraph/utils.py` & `qermit-0.4.0/qermit/taskgraph/utils.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/qermit/zero_noise_extrapolation/__init__.py` & `qermit-0.4.0/qermit/clifford_noise_characterisation/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
-The zero_noise_extrapolation module provides generator methods for producing MitEx 
-objects that automatically run digital zero noise extrapolation protocols.
+The clifford_noise_characterisation module provides generator methods for producing MitEx
+objects that automatically characterise and correct some device noise using
+characterisation via Clifford circuits.
 """
-from .zne import (
-    gen_ZNE_MitEx,
-    Folding,
-    Fit,
+from .ccl import (  # noqa:F401
+    gen_CDR_MitEx,
 )
+from .dfsc import gen_DFSC_MitEx  # noqa:F401
```

### Comparing `qermit-0.3.0/qermit/zero_noise_extrapolation/zne.py` & `qermit-0.4.0/qermit/zero_noise_extrapolation/zne.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         # odd integer less than noise_scaling.
         num_folds_dict = {
             i: (int(noise_scaling - 1) // 2)
             for i, cmd in enumerate(circ.get_commands())
             if (
                 not (cmd.op.type == OpType.Barrier)
                 and not (cmd.op.type in box_types)
-                and len(cmd.qubits) == 2
+                and (len(cmd.qubits) == 2)
             )
         }
 
         if len(num_folds_dict) == 0:
             raise RuntimeError(
                 "There are no valid q qubits gates in this circuit to fold. "
                 "Your circuit should include 2 qubit gates other than "
@@ -895,38 +895,40 @@
     :type backend: Backend
     :param optimisation_level: level of default compiler, defaults to 1
     :type optimisation_level: int, optional
     """
 
     def task(
         obj, wire: List[ObservableExperiment]
-    ) -> Tuple[List[ObservableExperiment], Dict[Node, Node]]:
+    ) -> Tuple[List[ObservableExperiment], List[Dict[Node, Node]]]:
         """Performs initial compilation before folding. This is to ensure minimal compilation
         after folding, as this could disrupt by how much the noise is increased.
 
         :param wire: List of experiments
         :type wire: List[ObservableExperiment]
         :return: List of experiments compiled to run on the inputted backend.
-        Additionally a dictionary describing how the nodes have been mapped
-        by compilation.
-        :rtype: Tuple[List[ObservableExperiment], Dict[Node, Node]]
+            Additionally a list of dictionaries describing how the nodes have
+            been mapped by compilation.
+        :rtype: Tuple[List[ObservableExperiment], List[Dict[Node, Node]]]
         """
 
         mapped_wire = []
+        node_map_list = []
 
         for obs_exp in wire:
             # Perform default compilation, tracking to which physical
             # qubits the initial qubits are mapped
             compiled_circ = obs_exp.AnsatzCircuit.Circuit.copy()
 
             cu = CompilationUnit(compiled_circ)
             backend.default_compilation_pass(
                 optimisation_level=optimisation_level
             ).apply(cu)
             node_map = cu.final_map
+            node_map_list.append(node_map)
 
             # Alter the qubit pauli operator so that it maps to the new physical qubits.
             qpo = obs_exp[1]._qubit_pauli_operator
             new_qpo = qpo_node_relabel(qpo, node_map)
 
             # Construct new list of experiments, but with compiled circuits.
             mapped_wire.append(
@@ -938,15 +940,15 @@
                     ),
                     ObservableTracker=ObservableTracker(new_qpo),
                 )
             )
 
         return (
             mapped_wire,
-            node_map,
+            node_map_list,
         )
 
     return MitTask(
         _label="CompileToBackend",
         _n_out_wires=2,
         _n_in_wires=1,
         _method=task,
@@ -958,30 +960,34 @@
     This should follow gen_initial_compilation_task
 
     :return: Task performing relabelling.
     :rtype: MitTask
     """
 
     def task(
-        obj, qpo_list: List[QubitPauliOperator], compilation_map: Dict[Node, Node]
+        obj, qpo_list: List[QubitPauliOperator], compilation_map_list: List[Dict[Node, Node]]
     ) -> Tuple[List[QubitPauliOperator]]:
         """Use node map returned by compilation unit to undo the relabelling
         performed by gen_initial_compilation_task
 
         :param qpo_list: List of QubitPauliOperator
         :type qpo_list: List[QubitPauliOperator]
-        :param compilation_map: Dictionary mapping nodes as returned by
-        gen_initial_compilation_task task
-        :type compilation_map: Dict[Node, Node]
+        :param compilation_map_list: List of Dictionaries mapping nodes as
+            returned by gen_initial_compilation_task task
+        :type compilation_map_list: List[Dict[Node, Node]]
         :return: List of QubitPauliOperator with relabeled nodes.
         :rtype: Tuple[List[QubitPauliOperator]]
         """
 
-        node_map = {value: key for key, value in compilation_map.items()}
-        new_qpo_list = [qpo_node_relabel(qpo, node_map) for qpo in qpo_list]
+        new_qpo_list = []
+
+        for compilation_map, qpo in zip(compilation_map_list, qpo_list):
+
+            node_map = {value: key for key, value in compilation_map.items()}
+            new_qpo_list.append(qpo_node_relabel(qpo, node_map))
 
         return (new_qpo_list,)
 
     return MitTask(
         _label="RelabelQubits",
         _n_out_wires=1,
         _n_in_wires=2,
```

### Comparing `qermit-0.3.0/qermit.egg-info/PKG-INFO` & `qermit-0.4.0/qermit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qermit
-Version: 0.3.0
+Version: 0.4.0
 Summary: error-mitigation framework, an extension to pytket
 License: CQC Non-Commercial Use Software Licence
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Other/Proprietary License
@@ -54,16 +54,16 @@
 changes on the `main` branch, and open a PR from your fork. If it passes
 tests and is accepted after review, it will be merged in.
 
 ### Code style
 
 #### Formatting
 
-All code should be formatted using
-[black](https://black.readthedocs.io/en/stable/), with default options. 
+All code should adhere to [flake8](https://flake8.pycqa.org/en/latest/)
+formatting, ignoring only E501 and W503
 
 #### Type annotation
 
 On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
 type checker and all submissions must pass its checks. You should therefore run
 `mypy` locally on any changed files before submitting a PR.
```

### Comparing `qermit-0.3.0/qermit.egg-info/SOURCES.txt` & `qermit-0.4.0/qermit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 qermit.egg-info/top_level.txt
 qermit/clifford_noise_characterisation/__init__.py
 qermit/clifford_noise_characterisation/ccl.py
 qermit/clifford_noise_characterisation/cdr_post.py
 qermit/clifford_noise_characterisation/dfsc.py
 qermit/frame_randomisation/__init__.py
 qermit/frame_randomisation/frame_randomisation.py
+qermit/mock_backend/__init__.py
+qermit/mock_backend/mock_quantinuum_backend.py
 qermit/probabilistic_error_cancellation/__init__.py
 qermit/probabilistic_error_cancellation/cliff_circuit_gen.py
 qermit/probabilistic_error_cancellation/pec_learning_based.py
 qermit/spam/__init__.py
 qermit/spam/full_spam_correction.py
 qermit/spam/full_transition_tomography.py
 qermit/spam/nn_data_generation.py
```

### Comparing `qermit-0.3.0/setup.py` & `qermit-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/ccl_test.py` & `qermit-0.4.0/tests/ccl_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/cdr_test.py` & `qermit-0.4.0/tests/cdr_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/dfsc_test.py` & `qermit-0.4.0/tests/dfsc_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/frame_randomisation_test.py` & `qermit-0.4.0/tests/frame_randomisation_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/full_spam_test.py` & `qermit-0.4.0/tests/full_spam_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/measurement_reduction_test.py` & `qermit-0.4.0/tests/measurement_reduction_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,18 +73,18 @@
     assert info11[0][0] == 0
     # check bits are correct
     assert [Bit(1), Bit(2)] == info00[0][1]
     assert [Bit(0), Bit(1)] == info01[0][1]
     assert [Bit(0), Bit(1), Bit(2)] == info10[0][1]
     assert [Bit(0), Bit(1)] == info11[0][1]
     # check no result expects inversion of expectation
-    assert info00[0][2] == False
-    assert info01[0][2] == False
-    assert info10[0][2] == False
-    assert info11[0][2] == False
+    assert not info00[0][2]
+    assert not info01[0][2]
+    assert not info10[0][2]
+    assert not info11[0][2]
 
 
 def test_gen_me_MitEx():
     # set up experiment with guaranteed expectations
     # confirm that despite measurement reduction reducing the number
     # of circuits simulated, the expectation value is still correct
     me = gen_MeasurementReduction_MitEx(AerBackend())
```

### Comparing `qermit-0.3.0/tests/mitex_test.py` & `qermit-0.4.0/tests/mitex_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/mitres_test.py` & `qermit-0.4.0/tests/mitres_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/pec_test.py` & `qermit-0.4.0/tests/pec_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/spam_methods_test.py` & `qermit-0.4.0/tests/spam_methods_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,29 @@
 from pytket.circuit import Node  # type: ignore
 from pytket.architecture import Architecture  # type: ignore
 from qermit.spam import (  # type: ignore
     gen_FullyCorrelated_SPAM_MitRes,
     gen_UnCorrelated_SPAM_MitRes,
     CorrectionMethod,
 )
-from qermit.taskgraph import CircuitShots  # type: ignore
+from qermit import CircuitShots
+from qermit.mock_backend import MockQuantinuumBackend  # type: ignore
+
+
+def test_mock_quantinuum_all_qubits() -> None:
+
+    circuit = Circuit(2).X(0).X(1).measure_all()
+    circ_shots = CircuitShots(circuit, 1000)
+    noisy_backend = MockQuantinuumBackend()
+
+    spam_mitres = gen_UnCorrelated_SPAM_MitRes(
+        backend=noisy_backend,
+        calibration_shots=1000,
+    )
+    assert (1, 1) in spam_mitres.run([circ_shots])[0].get_counts().keys()
 
 
 def gen_test_wire():
     c0 = Circuit(4).X(0).X(2).measure_all()
     c1 = Circuit(5).X(1).X(3).measure_all()
     return [CircuitShots(c0.copy(), 20), CircuitShots(c1.copy(), 20)]
 
@@ -69,7 +83,8 @@
     assert res[0].get_counts()[(1, 0, 1, 0)] == 20
     assert res[1].get_counts()[(0, 1, 0, 1, 0)] == 20
 
 
 if __name__ == "__main__":
     test_gen_FC_mr()
     test_gen_UC_mr()
+    test_mock_quantinuum_all_qubits()
```

### Comparing `qermit-0.3.0/tests/spectral_filtering_test.py` & `qermit-0.4.0/tests/spectral_filtering_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from qermit.spectral_filtering.spectral_filtering import (
-    gen_fft_task,
     gen_result_extraction_task,
     gen_wire_copy_task,
     gen_inv_fft_task,
     gen_mitigation_task,
     gen_fft_task,
     gen_flatten_task,
     gen_reshape_task,
@@ -17,15 +16,14 @@
 import numpy as np
 from pytket.utils import QubitPauliOperator
 import math
 from pytket import Circuit, Qubit
 from pytket.pauli import QubitPauliString, Pauli
 from qermit import AnsatzCircuit, SymbolsDict, ObservableExperiment, ObservableTracker
 from sympy import Symbol
-from qermit import TaskGraph
 import scipy.fft
 from pytket.extensions.qiskit import AerBackend
 
 
 def generate_sine_wave(freq, sample_rate, duration):
     x = np.linspace(0, duration, sample_rate * duration, endpoint=False)
     y = np.sin((2 * np.pi) * x * freq)
@@ -314,15 +312,15 @@
     in_wire = (grid_list,)
     out_wire = flatten_task(in_wire)
 
     assert len(out_wire[0]) == 35
 
     assert out_wire[1] == length_list
     assert out_wire[0][: length_list[0]] == grid_0_flattened
-    assert out_wire[0][length_list[0] : length_list[0] + length_list[1]] == [
+    assert out_wire[0][length_list[0]: length_list[0] + length_list[1]] == [
         1,
         2,
         3,
         4,
         5,
         6,
         7,
```

### Comparing `qermit-0.3.0/tests/taskgraph_test.py` & `qermit-0.4.0/tests/taskgraph_test.py`

 * *Files identical despite different names*

### Comparing `qermit-0.3.0/tests/tomography_test.py` & `qermit-0.4.0/tests/tomography_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,20 @@
     calculate_correlation_matrices,
     correct_transition_noise,
     CorrectionMethod,
     reduce_matrix,
     reduce_matrices,
 )
 
-from pytket import Circuit, Bit
+from pytket import Circuit, Bit, Qubit
 from pytket.extensions.qiskit import AerBackend  # type: ignore
 import qiskit.providers.aer.noise as noise  # type: ignore
 import numpy as np  # type: ignore
 
+
 # set up basic readout error noise model backend for tests
 def get_noisy_backend(n_qubits, prob_ro):
     noise_model = noise.NoiseModel()
     probabilities = [[1 - prob_ro, prob_ro], [prob_ro, 1 - prob_ro]]
     error_ro = noise.ReadoutError(probabilities)
     for i in range(n_qubits):
         noise_model.add_readout_error(error_ro, [i])
@@ -41,14 +42,23 @@
 
 def test_binary_int_methods():
     test_int = 2
     converted_binary = int_to_binary(test_int, 5)
     assert binary_to_int(converted_binary) == test_int
 
 
+def test_wire_adding():
+    c = Circuit(10).CX(0, 1)
+    n_qubits = c.n_qubits
+    c.remove_blank_wires()
+    while c.n_qubits < n_qubits:
+        c.add_qubit(Qubit("temp", c.n_qubits))
+    assert c.n_qubits == 10
+
+
 def test_get_transition_tomography_circuits():
     backend = get_noisy_backend(4, 0.1)
     pc = Circuit(4).CX(0, 1)
     nodes = backend.backend_info.architecture.nodes
     correlations = [[nodes[0], nodes[1]], [nodes[2], nodes[3]]]
     # get tomography circuits
     output = get_full_transition_tomography_circuits(pc, backend, correlations)
@@ -198,7 +208,8 @@
 
 if __name__ == "__main__":
     test_binary_int_methods()
     test_get_transition_tomography_circuits()
     test_calculate_correlation_matrices()
     test_correct_transition_noise()
     test_reduce_matrices()
+    test_wire_adding()
```

### Comparing `qermit-0.3.0/tests/utils_test.py` & `qermit-0.4.0/tests/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 )
 
 from pytket.circuit import Circuit, fresh_symbol, Qubit, Bit  # type: ignore
 from pytket.pauli import QubitPauliString, Pauli  # type: ignore
 from pytket.utils import QubitPauliOperator
 from pytket.extensions.qiskit import AerBackend  # type: ignore
 
+
 # tests for SymbolsDict class in utils
 def test_SymbolsDict_circuit_constructor() -> None:
     test_circuit = Circuit(4)
     symbols = []
     for i in range(4):
         sym = fresh_symbol("a" + str(i))
         test_circuit.Ry(sym, i)
```

### Comparing `qermit-0.3.0/tests/zne_test.py` & `qermit-0.4.0/tests/zne_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 import numpy as np  # type: ignore
 from qermit import AnsatzCircuit, ObservableExperiment  # type: ignore
 import qiskit.providers.aer.noise as noise  # type: ignore
 from pytket.circuit import OpType  # type: ignore
 from qiskit import IBMQ  # type: ignore
 import pytest
 from pytket.circuit import Node  # type: ignore
+from qermit.mock_backend import MockQuantinuumBackend  # type: ignore
 
 n_qubits = 2
 
 prob_1 = 0.005
 prob_2 = 0.02
 
 noise_model = noise.NoiseModel()
@@ -103,15 +104,15 @@
     assert task.n_out_wires == 1
 
     qubit_pauli_string = QubitPauliString(
         [Qubit(0), Qubit(1), Qubit(2)], [Pauli.Z, Pauli.Z, Pauli.Z]
     )
     qubit_pauli_operator = QubitPauliOperator({qubit_pauli_string: 1.0})
 
-    compilation_map = {Node(0): Qubit(0), Node(1): Qubit(1), Node(2): Qubit(2)}
+    compilation_map = [{Node(0): Qubit(0), Node(1): Qubit(1), Node(2): Qubit(2)}]
 
     relabeled_qubit_pauli_string = QubitPauliString(
         [Node(0), Node(1), Node(2)], [Pauli.Z, Pauli.Z, Pauli.Z]
     )
     relabeled_qubit_pauli_operator = QubitPauliOperator(
         {relabeled_qubit_pauli_string: 1.0}
     )
@@ -126,21 +127,21 @@
 
     task = gen_initial_compilation_task(be, optimisation_level=1)
 
     assert task.n_in_wires == 1
     assert task.n_out_wires == 2
 
     c_1 = Circuit(2).CZ(0, 1).T(1)
-    c_2 = Circuit(2).CZ(0, 1).T(0).X(1)
+    c_2 = Circuit(1).T(0).X(0)
 
     ac_1 = AnsatzCircuit(c_1, 10000, {})
     ac_2 = AnsatzCircuit(c_2, 10000, {})
 
-    qpo_1 = QubitPauliOperator({QubitPauliString([Qubit(0)], [Pauli.Z]): 1})
-    qpo_2 = QubitPauliOperator({QubitPauliString([Qubit(1)], [Pauli.Z]): 1})
+    qpo_1 = QubitPauliOperator({QubitPauliString([Qubit(1)], [Pauli.Z]): 1})
+    qpo_2 = QubitPauliOperator({QubitPauliString([Qubit(0)], [Pauli.Z]): 1})
 
     experiment_1 = ObservableExperiment(ac_1, ObservableTracker(qpo_1))
     experiment_2 = ObservableExperiment(ac_2, ObservableTracker(qpo_2))
 
     result = task([[experiment_1, experiment_2]])
 
     compiled_experiment_1 = result[0][0]
@@ -150,14 +151,37 @@
     compiled_c_2 = compiled_experiment_2[0][0]
 
     # Check that the compiled circuits are indeed valid
     assert be.valid_circuit(compiled_c_1)
     assert be.valid_circuit(compiled_c_2)
 
 
+def test_gen_initial_compilation_task_quantinuum_qubit_names():
+    be = MockQuantinuumBackend()
+
+    task = gen_initial_compilation_task(be, optimisation_level=0)
+
+    assert task.n_in_wires == 1
+    assert task.n_out_wires == 2
+
+    c = Circuit(2).X(0).X(1)
+
+    ac = AnsatzCircuit(c, 10000, {})
+
+    qpo = QubitPauliOperator({QubitPauliString([Qubit(0)], [Pauli.Z]): 1})
+
+    experiment = ObservableExperiment(ac, ObservableTracker(qpo))
+
+    result = task([[experiment]])
+
+    c_qubits = set(result[0][0].AnsatzCircuit.Circuit.qubits)
+    qpo_qubits = result[0][0].ObservableTracker._qubit_pauli_operator.all_qubits
+    assert qpo_qubits.issubset(c_qubits)
+
+
 def test_gen_duplication_task():
 
     n_dups = 2
 
     task = gen_duplication_task(n_dups)
 
     assert task.n_in_wires == 1
@@ -438,41 +462,41 @@
         _label="TestZNEMitEx",
         optimisation_level=0,
         folding_type=Folding.gate,
         show_fit=False,
     )
 
     c_1 = Circuit(2).CZ(0, 1).T(1)
-    c_2 = Circuit(2).CZ(0, 1).T(0).X(1)
+    c_2 = Circuit(1).T(0).X(0)
     ac_1 = AnsatzCircuit(c_1, 10000, SymbolsDict())
     ac_2 = AnsatzCircuit(c_2, 10000, SymbolsDict())
     circ_list = []
     circ_list.append(
         ObservableExperiment(
             ac_1,
             ObservableTracker(
-                QubitPauliOperator({QubitPauliString([Qubit(0)], [Pauli.Z]): 1})
+                QubitPauliOperator({QubitPauliString([Qubit(1)], [Pauli.Z]): 1})
             ),
         )
     )
     circ_list.append(
         ObservableExperiment(
             ac_2,
             ObservableTracker(
-                QubitPauliOperator({QubitPauliString([Qubit(1)], [Pauli.Z]): 1})
+                QubitPauliOperator({QubitPauliString([Qubit(0)], [Pauli.Z]): 1})
             ),
         )
     )
 
     result = me.run(circ_list)
     expectation_1 = result[0]
     expectation_2 = result[1]
 
-    res1 = expectation_1[QubitPauliString([Qubit(0)], [Pauli.Z])]
-    res2 = expectation_2[QubitPauliString([Qubit(1)], [Pauli.Z])]
+    res1 = expectation_1[QubitPauliString([Qubit(1)], [Pauli.Z])]
+    res2 = expectation_2[QubitPauliString([Qubit(0)], [Pauli.Z])]
 
     assert round(float(res1)) == 1.0
     assert round(float(res2)) == -1.0
 
 
 def test_circuit_folding_TK1():
 
@@ -550,25 +574,25 @@
     assert task_1.n_in_wires == 1
     assert task_1.n_out_wires == 1
     assert task_2.n_in_wires == 1
     assert task_2.n_out_wires == 1
     assert task_invalid.n_in_wires == 1
     assert task_invalid.n_out_wires == 1
 
-    c_1 = Circuit(2).Rz(0.3,0).ZZPhase(0.3,1,0)
+    c_1 = Circuit(2).Rz(0.3, 0).ZZPhase(0.3, 1, 0)
     # This is to ensure that the barrier is not folded, even though it
     # acts on 2 qubits
-    c_2 = Circuit(3).Rz(0.3,2).CZ(1,2).add_barrier([0,1]).CX(0,1).X(0)
-    c_3 = Circuit(3).CZ(0,1).CZ(1,2).CZ(0,2)
+    c_2 = Circuit(3).Rz(0.3, 2).CZ(1, 2).add_barrier([0, 1]).CX(0, 1).X(0)
+    c_3 = Circuit(3).CZ(0, 1).CZ(1, 2).CZ(0, 2)
 
     circ_box = CircBox(c_1)
     # Tests that circuits with nothing to fold will raise an error.
-    c_gate_set_invalid_1 = Circuit(2).add_circbox(circ_box, [0,1])
+    c_gate_set_invalid_1 = Circuit(2).add_circbox(circ_box, [0, 1])
     # Tests that circuits with CircBox will raise an error.
-    c_gate_set_invalid_2 = Circuit(2).add_circbox(circ_box, [0,1]).CZ(0,1)
+    c_gate_set_invalid_2 = Circuit(2).add_circbox(circ_box, [0, 1]).CZ(0, 1)
 
     ac_1 = AnsatzCircuit(c_1, 10000, {})
     ac_2 = AnsatzCircuit(c_2, 10000, {})
     ac_3 = AnsatzCircuit(c_3, 10000, {})
     ac_gate_set_invalid_1 = AnsatzCircuit(c_gate_set_invalid_1, 10000, {})
     ac_gate_set_invalid_2 = AnsatzCircuit(c_gate_set_invalid_2, 10000, {})
 
@@ -583,47 +607,47 @@
     experiment_gate_set_invalid_2 = ObservableExperiment(
         ac_gate_set_invalid_2, ObservableTracker(qpo_1)
     )
 
     with pytest.raises(ValueError):
         task_invalid([[experiment_1, experiment_2]])
 
-    with  pytest.raises(RuntimeError):
+    with pytest.raises(RuntimeError):
         task_1([[experiment_gate_set_invalid_1]])
 
-    with  pytest.raises(RuntimeError):
+    with pytest.raises(RuntimeError):
         task_1([[experiment_gate_set_invalid_2]])
-    
+
     folded_experiment_1 = task_1([[experiment_1, experiment_2]])[0]
     folded_experiment_2 = task_2([[experiment_3]])[0]
 
     folded_c_1 = folded_experiment_1[0].AnsatzCircuit.Circuit
     folded_c_2 = folded_experiment_1[1].AnsatzCircuit.Circuit
     folded_c_3 = folded_experiment_2[0].AnsatzCircuit.Circuit
 
     ideal_folded_c_1 = Circuit(2)
-    ideal_folded_c_1.Rz(0.3,0)
-    ideal_folded_c_1.ZZPhase(0.3,1,0)
-    ideal_folded_c_1.add_barrier([1,0])
-    ideal_folded_c_1.ZZPhase(3.7,1,0)
-    ideal_folded_c_1.add_barrier([1,0])
-    ideal_folded_c_1.ZZPhase(0.3,1,0)
+    ideal_folded_c_1.Rz(0.3, 0)
+    ideal_folded_c_1.ZZPhase(0.3, 1, 0)
+    ideal_folded_c_1.add_barrier([1, 0])
+    ideal_folded_c_1.ZZPhase(3.7, 1, 0)
+    ideal_folded_c_1.add_barrier([1, 0])
+    ideal_folded_c_1.ZZPhase(0.3, 1, 0)
 
     assert folded_c_1 == ideal_folded_c_1
 
     assert GateSetPredicate(be.backend_info.gate_set).verify(folded_c_1)
     assert GateSetPredicate(be.backend_info.gate_set).verify(folded_c_2)
     assert GateSetPredicate(be.backend_info.gate_set).verify(folded_c_3)
 
     # Note that in both cases barriers are added. This is why there is the
     # n_folds_i - 1 term at the end.
     assert folded_c_1.n_gates == c_1.n_gates + 2 * c_1.n_2qb_gates() * (n_folds_1 - 1)
     assert folded_c_2.n_gates == c_2.n_gates + 2 * c_2.n_2qb_gates() * (n_folds_1 - 1)
     # note that this gives an nose scaling = 17/3 = 5.6 which is a little smaller than 5.8
-    assert folded_c_3.n_2qb_gates() == 17 
+    assert folded_c_3.n_2qb_gates() == 17
 
     c_1_unitary = c_1.get_unitary()
     c_2_unitary = c_2.get_unitary()
     c_3_unitary = c_3.get_unitary()
     folded_c_1_unitary = folded_c_1.get_unitary()
     folded_c_2_unitary = folded_c_2.get_unitary()
     folded_c_3_unitary = folded_c_3.get_unitary()
@@ -641,7 +665,8 @@
     test_gen_initial_compilation_task()
     test_zne_identity()
     test_simple_run_end_to_end()
     test_odd_gate_folding()
     test_circuit_folding_TK1()
     test_gen_qubit_relabel_task()
     test_two_qubit_gate_folding()
+    test_gen_initial_compilation_task_quantinuum_qubit_names()
```

