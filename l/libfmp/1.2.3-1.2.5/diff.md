# Comparing `tmp/libfmp-1.2.3.tar.gz` & `tmp/libfmp-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libfmp-1.2.3.tar", last modified: Wed Jul 27 12:10:07 2022, max compression
+gzip compressed data, was "dist/libfmp-1.2.5.tar", last modified: Thu May 25 14:43:53 2023, max compression
```

## Comparing `libfmp-1.2.3.tar` & `libfmp-1.2.5.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp.egg-info/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     1623 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp.egg-info/SOURCES.txt
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     6389 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp.egg-info/PKG-INFO
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)        1 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp.egg-info/dependency_links.txt
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)        7 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp.egg-info/top_level.txt
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)      247 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp.egg-info/requires.txt
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)       38 2022-07-27 12:10:07.000000 libfmp-1.2.3/setup.cfg
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     6389 2022-07-27 12:10:07.000000 libfmp-1.2.3/PKG-INFO
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     5156 2022-07-27 12:09:01.000000 libfmp-1.2.3/README.md
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/b/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     3710 2021-07-14 10:10:05.000000 libfmp-1.2.3/libfmp/b/b_annotation.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    27114 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/b/b_plot.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)      979 2020-10-19 10:42:34.000000 libfmp-1.2.3/libfmp/b/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)      665 2021-04-22 08:27:28.000000 libfmp-1.2.3/libfmp/b/b_test_module.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2503 2021-07-14 10:09:50.000000 libfmp-1.2.3/libfmp/b/b_audio.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     9980 2021-07-14 10:12:15.000000 libfmp-1.2.3/libfmp/b/b_sonification.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2007 2021-07-14 09:53:56.000000 libfmp-1.2.3/libfmp/b/b_layout.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c4/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2850 2021-04-21 13:23:16.000000 libfmp-1.2.3/libfmp/c4/c4s4_novelty_kernel.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    15239 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c4/c4s2_ssm.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     4350 2021-05-11 12:14:22.000000 libfmp-1.2.3/libfmp/c4/c4s2_threshold.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    11133 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c4/c4s5_evaluation.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     4415 2021-07-14 10:17:16.000000 libfmp-1.2.3/libfmp/c4/c4s1_annotation.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    20094 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c4/c4s3_thumbnail.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)     1541 2021-05-11 11:23:30.000000 libfmp-1.2.3/libfmp/c4/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2525 2021-04-22 08:37:15.000000 libfmp-1.2.3/libfmp/c4/c4s2_synthetic_ssm.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     3456 2021-04-22 09:42:02.000000 libfmp-1.2.3/libfmp/c4/c4s4_structure_feature.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c8/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    17348 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c8/c8s2_f0.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    11425 2021-05-11 11:27:58.000000 libfmp-1.2.3/libfmp/c8/c8s1_hps.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    11614 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c8/c8s3_nmf.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)     1098 2020-10-19 12:37:52.000000 libfmp-1.2.3/libfmp/c8/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    10439 2021-05-11 12:26:31.000000 libfmp-1.2.3/libfmp/c8/c8s2_salience.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c5/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     1792 2021-04-21 15:28:54.000000 libfmp-1.2.3/libfmp/c5/c5s1_basic_theory_harmony.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    12876 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c5/c5s3_chord_rec_hmm.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    13417 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c5/c5s2_chord_rec_template.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)      734 2020-10-19 11:42:19.000000 libfmp-1.2.3/libfmp/c5/__init__.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c3/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     4532 2021-04-21 09:00:58.000000 libfmp-1.2.3/libfmp/c3/c3s1_post_processing.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     7612 2021-05-11 12:06:18.000000 libfmp-1.2.3/libfmp/c3/c3s1_transposition_tuning.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     3771 2021-04-22 08:35:31.000000 libfmp-1.2.3/libfmp/c3/c3s2_dtw.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     1429 2021-04-21 12:55:18.000000 libfmp-1.2.3/libfmp/c3/c3s2_dtw_plot.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)      945 2020-10-19 08:41:11.000000 libfmp-1.2.3/libfmp/c3/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2990 2021-04-22 08:46:27.000000 libfmp-1.2.3/libfmp/c3/c3s1_audio_feature.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     8234 2021-06-29 06:58:04.000000 libfmp-1.2.3/libfmp/c3/c3s3_tempo_curve.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)        0 2020-10-16 15:51:10.000000 libfmp-1.2.3/libfmp/__init__.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c2/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    10420 2021-04-21 08:08:52.000000 libfmp-1.2.3/libfmp/c2/c2_fourier.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     1456 2021-04-22 08:32:28.000000 libfmp-1.2.3/libfmp/c2/c2_complex.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2022 2021-04-22 08:34:00.000000 libfmp-1.2.3/libfmp/c2/c2_interpolation.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     2141 2021-05-11 11:37:46.000000 libfmp-1.2.3/libfmp/c2/c2_interference.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)      749 2020-10-19 08:30:07.000000 libfmp-1.2.3/libfmp/c2/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     8441 2021-04-23 06:21:50.000000 libfmp-1.2.3/libfmp/c2/c2_digitization.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c1/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     6420 2021-07-14 10:14:08.000000 libfmp-1.2.3/libfmp/c1/c1s2_symbolic_rep.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    12683 2021-04-21 06:40:50.000000 libfmp-1.2.3/libfmp/c1/c1s3_audio_rep.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)      651 2020-10-19 08:18:22.000000 libfmp-1.2.3/libfmp/c1/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     3835 2021-04-22 08:28:43.000000 libfmp-1.2.3/libfmp/c1/c1s1_sheet_music.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c7/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    15049 2021-06-29 06:58:17.000000 libfmp-1.2.3/libfmp/c7/c7s2_audio_matching.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     6610 2021-11-23 15:52:32.000000 libfmp-1.2.3/libfmp/c7/c7s1_audio_id.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)     1032 2020-10-20 06:47:43.000000 libfmp-1.2.3/libfmp/c7/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     8803 2021-04-22 06:26:58.000000 libfmp-1.2.3/libfmp/c7/c7s3_version_id.py
-drwxrwxr-x   0 swpffm    (1000) swpffm    (1000)        0 2022-07-27 12:10:07.000000 libfmp-1.2.3/libfmp/c6/
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    12774 2021-05-11 12:15:53.000000 libfmp-1.2.3/libfmp/c6/c6s2_tempo_analysis.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     4229 2021-04-22 10:50:56.000000 libfmp-1.2.3/libfmp/c6/c6s3_adaptive_windowing.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    11025 2021-06-29 06:58:12.000000 libfmp-1.2.3/libfmp/c6/c6s1_onset_detection.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     4287 2021-05-11 11:45:51.000000 libfmp-1.2.3/libfmp/c6/c6s3_beat_tracking.py
--rw-r--r--   0 swpffm    (1000) swpffm    (1000)      979 2021-04-14 16:54:02.000000 libfmp-1.2.3/libfmp/c6/__init__.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)    10175 2021-05-11 11:48:56.000000 libfmp-1.2.3/libfmp/c6/c6s1_peak_picking.py
--rw-rw-r--   0 swpffm    (1000) swpffm    (1000)     1496 2022-07-27 12:09:01.000000 libfmp-1.2.3/setup.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     5872 2023-05-25 14:43:53.000000 libfmp-1.2.5/PKG-INFO
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1476 2023-05-25 14:41:35.000000 libfmp-1.2.5/LICENSE
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp.egg-info/
+-rwx------   0 zal      (1043591436) staff       (20)     5872 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp.egg-info/PKG-INFO
+-rwx------   0 zal      (1043591436) staff       (20)     1631 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp.egg-info/SOURCES.txt
+-rwx------   0 zal      (1043591436) staff       (20)      248 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp.egg-info/requires.txt
+-rwx------   0 zal      (1043591436) staff       (20)        7 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp.egg-info/top_level.txt
+-rwx------   0 zal      (1043591436) staff       (20)        1 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp.egg-info/dependency_links.txt
+-rw-r--r--   0 zal      (1043591436) staff       (20)     5156 2023-05-25 14:41:35.000000 libfmp-1.2.5/README.md
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1497 2023-05-25 14:41:35.000000 libfmp-1.2.5/setup.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c7/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     8803 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c7/c7s3_version_id.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1032 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c7/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     6610 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c7/c7s1_audio_id.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    15049 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c7/c7s2_audio_matching.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c8/
+-rw-r--r--   0 zal      (1043591436) staff       (20)    11425 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c8/c8s1_hps.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    11614 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c8/c8s3_nmf.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    17348 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c8/c8s2_f0.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1098 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c8/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    10439 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c8/c8s2_salience.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c1/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     3835 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c1/c1s1_sheet_music.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)      651 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c1/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     6420 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c1/c1s2_symbolic_rep.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    12680 2023-03-07 13:11:39.000000 libfmp-1.2.5/libfmp/c1/c1s3_audio_rep.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c6/
+-rw-r--r--   0 zal      (1043591436) staff       (20)    10175 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c6/c6s1_peak_picking.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)      979 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c6/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     4288 2023-05-25 07:34:45.000000 libfmp-1.2.5/libfmp/c6/c6s3_beat_tracking.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    11016 2023-03-07 13:12:00.000000 libfmp-1.2.5/libfmp/c6/c6s1_onset_detection.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    12774 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c6/c6s2_tempo_analysis.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     4229 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c6/c6s3_adaptive_windowing.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)        0 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/__init__.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c3/
+-rw-r--r--   0 zal      (1043591436) staff       (20)      945 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     4532 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/c3s1_post_processing.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     3771 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/c3s2_dtw.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     7612 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/c3s1_transposition_tuning.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     8234 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/c3s3_tempo_curve.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1429 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/c3s2_dtw_plot.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2990 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c3/c3s1_audio_feature.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c4/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     4415 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s1_annotation.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2850 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s4_novelty_kernel.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     3456 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s4_structure_feature.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    11133 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s5_evaluation.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1541 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    20094 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s3_thumbnail.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2525 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s2_synthetic_ssm.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     4350 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s2_threshold.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    15239 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c4/c4s2_ssm.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c5/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1792 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c5/c5s1_basic_theory_harmony.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)      734 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c5/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    12876 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c5/c5s3_chord_rec_hmm.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    13418 2023-01-13 12:53:52.000000 libfmp-1.2.5/libfmp/c5/c5s2_chord_rec_template.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/c2/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     1456 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c2/c2_complex.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    10420 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c2/c2_fourier.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     8441 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c2/c2_digitization.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)      749 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c2/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2022 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c2/c2_interpolation.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2141 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/c2/c2_interference.py
+drwxr-xr-x   0 zal      (1043591436) staff       (20)        0 2023-05-25 14:43:53.000000 libfmp-1.2.5/libfmp/b/
+-rw-r--r--   0 zal      (1043591436) staff       (20)     3710 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/b_annotation.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)      979 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/__init__.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)    27114 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/b_plot.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)      665 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/b_test_module.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2007 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/b_layout.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     2503 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/b_audio.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)     9980 2022-07-18 06:16:19.000000 libfmp-1.2.5/libfmp/b/b_sonification.py
+-rw-r--r--   0 zal      (1043591436) staff       (20)       38 2023-05-25 14:43:53.000000 libfmp-1.2.5/setup.cfg
```

### Comparing `libfmp-1.2.3/libfmp.egg-info/SOURCES.txt` & `libfmp-1.2.5/libfmp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 libfmp/__init__.py
 libfmp.egg-info/PKG-INFO
 libfmp.egg-info/SOURCES.txt
 libfmp.egg-info/dependency_links.txt
 libfmp.egg-info/requires.txt
```

### Comparing `libfmp-1.2.3/libfmp.egg-info/PKG-INFO` & `libfmp-1.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 Metadata-Version: 2.1
 Name: libfmp
-Version: 1.2.3
+Version: 1.2.5
 Summary: Python module for fundamentals of music processing
 Home-page: http://audiolabs-erlangen.de/FMP
 Author: Meinard Müller and Frank Zalkow
 Author-email: meinard.mueller@audiolabs-erlangen.de
 License: MIT
 Download-URL: https://github.com/meinardmueller/libfmp
-Description: # libfmp
-        
-        This repository contains the Python package libfmp. This package goes hand in hand with the FMP Notebooks, a collection of educational material for teaching and learning Fundamentals of Music Processing (FMP) with a particular focus on the audio domain. For detailed explanations and example appliciations of the libfmp-functions we refer to the FMP Notebooks:
-        
-        https://audiolabs-erlangen.de/FMP
-        
-        The FMP notebooks also contain a dedicated notebook for libfmp:
-        
-        https://www.audiolabs-erlangen.de/resources/MIR/FMP/B/B_libfmp.html
-        
-        There is also an API documentation for libfmp:
-        
-        https://meinardmueller.github.io/libfmp
-        
-        If you use the package libfmp, please consider the following references.
-        
-        ## References
-        
-        Meinard Müller and Frank Zalkow. [libfmp: A Python Package for Fundamentals of Music Processing.](https://joss.theoj.org/papers/10.21105/joss.03326) Journal of Open Source Software (JOSS), 6(63), 2021.
-        
-        Meinard Müller and Frank Zalkow. [FMP Notebooks: Educational Material for Teaching and Learning Fundamentals of Music Processing.](https://archives.ismir.net/ismir2019/paper/000069.pdf) Proceedings of the International Conference on Music Information Retrieval (ISMIR), pp. 573&ndash;580, Delft, The Netherlands, 2019.
-        
-        Meinard Müller. [Fundamentals of Music Processing &ndash; Using Python and Jupyter Notebooks.](http://www.music-processing.de/) Springer Verlag, 2nd edition, 2021.
-        
-        Meinard Müller. [An Educational Guide Through the FMP Notebooks for Teaching and Learning Fundamentals of Music Processing.](https://www.mdpi.com/2624-6120/2/2/18) Signals, 2(2): 245&ndash;285, 2021.
-        
-        ## Statement of Need
-        
-        The libfmp package bundles core concepts from the music information retrieval (MIR) field in the form of well-documented and easy-to-use Python functions. It is designed to aid students with the transition from being learners (e.g., studying the FMP notebooks) to becoming researchers by providing proper software support for building and experimenting with complex MIR pipelines. Going beyond and complementing existing Python packages (such as librosa), the libfmp package contains (previously unpublished) reference implementations of MIR algorithms from the literature and new Python implementations of previously published MATLAB toolboxes. The functionality of libfmp addresses diverse MIR tasks such as tuning estimation, music structure analysis, audio thumbnailing, chord recognition, tempo estimation, beat and local pulse tracking, fragment-level music retrieval, and audio decomposition.
-        
-        ## Installing
-        
-        With Python >= 3.6, you can install libfmp using the Python package manager pip:
-        
-        ```
-        pip install libfmp
-        ```
-        
-        ## Contributing
-        
-        The libfmp-package has been developed in the context of the FMP notebooks. Being an integral part, all libfmp-functions need to manually synchronized with text passages, explanations, and the code in the FMP notebooks. Of course, we are happy for suggestions and contributions. However, to facilitate the synchronization, we would be grateful for either directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating [an issue](https://github.com/meinardmueller/libfmp/issues) in our GitHub repository. Please do not submit a pull request without prior consultation with us.
-        
-        If you want to report an issue with libfmp or seek support, please use the same communication channels (email or GitHub issue).
-        
-        ## Tests
-        
-        The functions of libmfp are also covered in the [FMP notebooks](https://audiolabs-erlangen.de/FMP). There, you find several test cases for the functions, showing typical input-output behaviors. Beyond these tests, the FMP notebooks offer extensive explanations of these functions. Thus, we consider FMP as a replacement for conventional unit tests.
-        
-        Furthermore, we provide a small script that tests one function of each subpackage from libfmp. Rather than covering the full functionality of libfmp, it only verifies the correct import structure within the libfmp package.
-        
-        There are two options for executing the test script. The first is just to run the script, which results in no output if there are no errors.
-        
-        ```
-        python test_examples.py
-        ```
-        
-        The second option is to use [pytest](https://pytest.org), which results in a more instructive output. pytest is available when installing libfmp with the extra requirements for testing.
-        
-        ```
-        pip install 'libfmp[tests]'
-        pytest test_examples.py
-        ```
-        
-        ## Acknowledgements
-        
-        The main authors of libfmp, Meinard Müller and Frank Zalkow, are associated with the International Audio Laboratories Erlangen, which are a joint institution of the Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU) and Fraunhofer Institute for Integrated Circuits IIS. We thank the German Research Foundation (DFG) for various research grants that allow us for conducting fundamental research in music processing. Furthermore, we thank the various people who have contributed to libfmp with code and suggestions. In particular, we want to thank (in alphabetic order) Stefan Balke, Michael Krause, Patricio Lopez-Serrano, Julian Reck, Sebastian Rosenzweig, Angel Villar-Corrales, Christof Weiß, and Tim Zunner.
-        
 Keywords: audio music sound
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+License-File: LICENSE
+
+# libfmp
+
+This repository contains the Python package libfmp. This package goes hand in hand with the FMP Notebooks, a collection of educational material for teaching and learning Fundamentals of Music Processing (FMP) with a particular focus on the audio domain. For detailed explanations and example appliciations of the libfmp-functions we refer to the FMP Notebooks:
+
+https://audiolabs-erlangen.de/FMP
+
+The FMP notebooks also contain a dedicated notebook for libfmp:
+
+https://www.audiolabs-erlangen.de/resources/MIR/FMP/B/B_libfmp.html
+
+There is also an API documentation for libfmp:
+
+https://meinardmueller.github.io/libfmp
+
+If you use the package libfmp, please consider the following references.
+
+## References
+
+Meinard Müller and Frank Zalkow. [libfmp: A Python Package for Fundamentals of Music Processing.](https://joss.theoj.org/papers/10.21105/joss.03326) Journal of Open Source Software (JOSS), 6(63), 2021.
+
+Meinard Müller and Frank Zalkow. [FMP Notebooks: Educational Material for Teaching and Learning Fundamentals of Music Processing.](https://archives.ismir.net/ismir2019/paper/000069.pdf) Proceedings of the International Conference on Music Information Retrieval (ISMIR), pp. 573&ndash;580, Delft, The Netherlands, 2019.
+
+Meinard Müller. [Fundamentals of Music Processing &ndash; Using Python and Jupyter Notebooks.](http://www.music-processing.de/) Springer Verlag, 2nd edition, 2021.
+
+Meinard Müller. [An Educational Guide Through the FMP Notebooks for Teaching and Learning Fundamentals of Music Processing.](https://www.mdpi.com/2624-6120/2/2/18) Signals, 2(2): 245&ndash;285, 2021.
+
+## Statement of Need
+
+The libfmp package bundles core concepts from the music information retrieval (MIR) field in the form of well-documented and easy-to-use Python functions. It is designed to aid students with the transition from being learners (e.g., studying the FMP notebooks) to becoming researchers by providing proper software support for building and experimenting with complex MIR pipelines. Going beyond and complementing existing Python packages (such as librosa), the libfmp package contains (previously unpublished) reference implementations of MIR algorithms from the literature and new Python implementations of previously published MATLAB toolboxes. The functionality of libfmp addresses diverse MIR tasks such as tuning estimation, music structure analysis, audio thumbnailing, chord recognition, tempo estimation, beat and local pulse tracking, fragment-level music retrieval, and audio decomposition.
+
+## Installing
+
+With Python >= 3.6, you can install libfmp using the Python package manager pip:
+
+```
+pip install libfmp
+```
+
+## Contributing
+
+The libfmp-package has been developed in the context of the FMP notebooks. Being an integral part, all libfmp-functions need to manually synchronized with text passages, explanations, and the code in the FMP notebooks. Of course, we are happy for suggestions and contributions. However, to facilitate the synchronization, we would be grateful for either directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating [an issue](https://github.com/meinardmueller/libfmp/issues) in our GitHub repository. Please do not submit a pull request without prior consultation with us.
+
+If you want to report an issue with libfmp or seek support, please use the same communication channels (email or GitHub issue).
+
+## Tests
+
+The functions of libmfp are also covered in the [FMP notebooks](https://audiolabs-erlangen.de/FMP). There, you find several test cases for the functions, showing typical input-output behaviors. Beyond these tests, the FMP notebooks offer extensive explanations of these functions. Thus, we consider FMP as a replacement for conventional unit tests.
+
+Furthermore, we provide a small script that tests one function of each subpackage from libfmp. Rather than covering the full functionality of libfmp, it only verifies the correct import structure within the libfmp package.
+
+There are two options for executing the test script. The first is just to run the script, which results in no output if there are no errors.
+
+```
+python test_examples.py
+```
+
+The second option is to use [pytest](https://pytest.org), which results in a more instructive output. pytest is available when installing libfmp with the extra requirements for testing.
+
+```
+pip install 'libfmp[tests]'
+pytest test_examples.py
+```
+
+## Acknowledgements
+
+The main authors of libfmp, Meinard Müller and Frank Zalkow, are associated with the International Audio Laboratories Erlangen, which are a joint institution of the Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU) and Fraunhofer Institute for Integrated Circuits IIS. We thank the German Research Foundation (DFG) for various research grants that allow us for conducting fundamental research in music processing. Furthermore, we thank the various people who have contributed to libfmp with code and suggestions. In particular, we want to thank (in alphabetic order) Stefan Balke, Michael Krause, Patricio Lopez-Serrano, Julian Reck, Sebastian Rosenzweig, Angel Villar-Corrales, Christof Weiß, and Tim Zunner.
+
+
```

### Comparing `libfmp-1.2.3/PKG-INFO` & `libfmp-1.2.5/libfmp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 Metadata-Version: 2.1
 Name: libfmp
-Version: 1.2.3
+Version: 1.2.5
 Summary: Python module for fundamentals of music processing
 Home-page: http://audiolabs-erlangen.de/FMP
 Author: Meinard Müller and Frank Zalkow
 Author-email: meinard.mueller@audiolabs-erlangen.de
 License: MIT
 Download-URL: https://github.com/meinardmueller/libfmp
-Description: # libfmp
-        
-        This repository contains the Python package libfmp. This package goes hand in hand with the FMP Notebooks, a collection of educational material for teaching and learning Fundamentals of Music Processing (FMP) with a particular focus on the audio domain. For detailed explanations and example appliciations of the libfmp-functions we refer to the FMP Notebooks:
-        
-        https://audiolabs-erlangen.de/FMP
-        
-        The FMP notebooks also contain a dedicated notebook for libfmp:
-        
-        https://www.audiolabs-erlangen.de/resources/MIR/FMP/B/B_libfmp.html
-        
-        There is also an API documentation for libfmp:
-        
-        https://meinardmueller.github.io/libfmp
-        
-        If you use the package libfmp, please consider the following references.
-        
-        ## References
-        
-        Meinard Müller and Frank Zalkow. [libfmp: A Python Package for Fundamentals of Music Processing.](https://joss.theoj.org/papers/10.21105/joss.03326) Journal of Open Source Software (JOSS), 6(63), 2021.
-        
-        Meinard Müller and Frank Zalkow. [FMP Notebooks: Educational Material for Teaching and Learning Fundamentals of Music Processing.](https://archives.ismir.net/ismir2019/paper/000069.pdf) Proceedings of the International Conference on Music Information Retrieval (ISMIR), pp. 573&ndash;580, Delft, The Netherlands, 2019.
-        
-        Meinard Müller. [Fundamentals of Music Processing &ndash; Using Python and Jupyter Notebooks.](http://www.music-processing.de/) Springer Verlag, 2nd edition, 2021.
-        
-        Meinard Müller. [An Educational Guide Through the FMP Notebooks for Teaching and Learning Fundamentals of Music Processing.](https://www.mdpi.com/2624-6120/2/2/18) Signals, 2(2): 245&ndash;285, 2021.
-        
-        ## Statement of Need
-        
-        The libfmp package bundles core concepts from the music information retrieval (MIR) field in the form of well-documented and easy-to-use Python functions. It is designed to aid students with the transition from being learners (e.g., studying the FMP notebooks) to becoming researchers by providing proper software support for building and experimenting with complex MIR pipelines. Going beyond and complementing existing Python packages (such as librosa), the libfmp package contains (previously unpublished) reference implementations of MIR algorithms from the literature and new Python implementations of previously published MATLAB toolboxes. The functionality of libfmp addresses diverse MIR tasks such as tuning estimation, music structure analysis, audio thumbnailing, chord recognition, tempo estimation, beat and local pulse tracking, fragment-level music retrieval, and audio decomposition.
-        
-        ## Installing
-        
-        With Python >= 3.6, you can install libfmp using the Python package manager pip:
-        
-        ```
-        pip install libfmp
-        ```
-        
-        ## Contributing
-        
-        The libfmp-package has been developed in the context of the FMP notebooks. Being an integral part, all libfmp-functions need to manually synchronized with text passages, explanations, and the code in the FMP notebooks. Of course, we are happy for suggestions and contributions. However, to facilitate the synchronization, we would be grateful for either directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating [an issue](https://github.com/meinardmueller/libfmp/issues) in our GitHub repository. Please do not submit a pull request without prior consultation with us.
-        
-        If you want to report an issue with libfmp or seek support, please use the same communication channels (email or GitHub issue).
-        
-        ## Tests
-        
-        The functions of libmfp are also covered in the [FMP notebooks](https://audiolabs-erlangen.de/FMP). There, you find several test cases for the functions, showing typical input-output behaviors. Beyond these tests, the FMP notebooks offer extensive explanations of these functions. Thus, we consider FMP as a replacement for conventional unit tests.
-        
-        Furthermore, we provide a small script that tests one function of each subpackage from libfmp. Rather than covering the full functionality of libfmp, it only verifies the correct import structure within the libfmp package.
-        
-        There are two options for executing the test script. The first is just to run the script, which results in no output if there are no errors.
-        
-        ```
-        python test_examples.py
-        ```
-        
-        The second option is to use [pytest](https://pytest.org), which results in a more instructive output. pytest is available when installing libfmp with the extra requirements for testing.
-        
-        ```
-        pip install 'libfmp[tests]'
-        pytest test_examples.py
-        ```
-        
-        ## Acknowledgements
-        
-        The main authors of libfmp, Meinard Müller and Frank Zalkow, are associated with the International Audio Laboratories Erlangen, which are a joint institution of the Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU) and Fraunhofer Institute for Integrated Circuits IIS. We thank the German Research Foundation (DFG) for various research grants that allow us for conducting fundamental research in music processing. Furthermore, we thank the various people who have contributed to libfmp with code and suggestions. In particular, we want to thank (in alphabetic order) Stefan Balke, Michael Krause, Patricio Lopez-Serrano, Julian Reck, Sebastian Rosenzweig, Angel Villar-Corrales, Christof Weiß, and Tim Zunner.
-        
 Keywords: audio music sound
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+License-File: LICENSE
+
+# libfmp
+
+This repository contains the Python package libfmp. This package goes hand in hand with the FMP Notebooks, a collection of educational material for teaching and learning Fundamentals of Music Processing (FMP) with a particular focus on the audio domain. For detailed explanations and example appliciations of the libfmp-functions we refer to the FMP Notebooks:
+
+https://audiolabs-erlangen.de/FMP
+
+The FMP notebooks also contain a dedicated notebook for libfmp:
+
+https://www.audiolabs-erlangen.de/resources/MIR/FMP/B/B_libfmp.html
+
+There is also an API documentation for libfmp:
+
+https://meinardmueller.github.io/libfmp
+
+If you use the package libfmp, please consider the following references.
+
+## References
+
+Meinard Müller and Frank Zalkow. [libfmp: A Python Package for Fundamentals of Music Processing.](https://joss.theoj.org/papers/10.21105/joss.03326) Journal of Open Source Software (JOSS), 6(63), 2021.
+
+Meinard Müller and Frank Zalkow. [FMP Notebooks: Educational Material for Teaching and Learning Fundamentals of Music Processing.](https://archives.ismir.net/ismir2019/paper/000069.pdf) Proceedings of the International Conference on Music Information Retrieval (ISMIR), pp. 573&ndash;580, Delft, The Netherlands, 2019.
+
+Meinard Müller. [Fundamentals of Music Processing &ndash; Using Python and Jupyter Notebooks.](http://www.music-processing.de/) Springer Verlag, 2nd edition, 2021.
+
+Meinard Müller. [An Educational Guide Through the FMP Notebooks for Teaching and Learning Fundamentals of Music Processing.](https://www.mdpi.com/2624-6120/2/2/18) Signals, 2(2): 245&ndash;285, 2021.
+
+## Statement of Need
+
+The libfmp package bundles core concepts from the music information retrieval (MIR) field in the form of well-documented and easy-to-use Python functions. It is designed to aid students with the transition from being learners (e.g., studying the FMP notebooks) to becoming researchers by providing proper software support for building and experimenting with complex MIR pipelines. Going beyond and complementing existing Python packages (such as librosa), the libfmp package contains (previously unpublished) reference implementations of MIR algorithms from the literature and new Python implementations of previously published MATLAB toolboxes. The functionality of libfmp addresses diverse MIR tasks such as tuning estimation, music structure analysis, audio thumbnailing, chord recognition, tempo estimation, beat and local pulse tracking, fragment-level music retrieval, and audio decomposition.
+
+## Installing
+
+With Python >= 3.6, you can install libfmp using the Python package manager pip:
+
+```
+pip install libfmp
+```
+
+## Contributing
+
+The libfmp-package has been developed in the context of the FMP notebooks. Being an integral part, all libfmp-functions need to manually synchronized with text passages, explanations, and the code in the FMP notebooks. Of course, we are happy for suggestions and contributions. However, to facilitate the synchronization, we would be grateful for either directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating [an issue](https://github.com/meinardmueller/libfmp/issues) in our GitHub repository. Please do not submit a pull request without prior consultation with us.
+
+If you want to report an issue with libfmp or seek support, please use the same communication channels (email or GitHub issue).
+
+## Tests
+
+The functions of libmfp are also covered in the [FMP notebooks](https://audiolabs-erlangen.de/FMP). There, you find several test cases for the functions, showing typical input-output behaviors. Beyond these tests, the FMP notebooks offer extensive explanations of these functions. Thus, we consider FMP as a replacement for conventional unit tests.
+
+Furthermore, we provide a small script that tests one function of each subpackage from libfmp. Rather than covering the full functionality of libfmp, it only verifies the correct import structure within the libfmp package.
+
+There are two options for executing the test script. The first is just to run the script, which results in no output if there are no errors.
+
+```
+python test_examples.py
+```
+
+The second option is to use [pytest](https://pytest.org), which results in a more instructive output. pytest is available when installing libfmp with the extra requirements for testing.
+
+```
+pip install 'libfmp[tests]'
+pytest test_examples.py
+```
+
+## Acknowledgements
+
+The main authors of libfmp, Meinard Müller and Frank Zalkow, are associated with the International Audio Laboratories Erlangen, which are a joint institution of the Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU) and Fraunhofer Institute for Integrated Circuits IIS. We thank the German Research Foundation (DFG) for various research grants that allow us for conducting fundamental research in music processing. Furthermore, we thank the various people who have contributed to libfmp with code and suggestions. In particular, we want to thank (in alphabetic order) Stefan Balke, Michael Krause, Patricio Lopez-Serrano, Julian Reck, Sebastian Rosenzweig, Angel Villar-Corrales, Christof Weiß, and Tim Zunner.
+
+
```

### Comparing `libfmp-1.2.3/README.md` & `libfmp-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/b_annotation.py` & `libfmp-1.2.5/libfmp/b/b_annotation.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/b_plot.py` & `libfmp-1.2.5/libfmp/b/b_plot.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/__init__.py` & `libfmp-1.2.5/libfmp/b/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/b_test_module.py` & `libfmp-1.2.5/libfmp/b/b_test_module.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/b_audio.py` & `libfmp-1.2.5/libfmp/b/b_audio.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/b_sonification.py` & `libfmp-1.2.5/libfmp/b/b_sonification.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/b/b_layout.py` & `libfmp-1.2.5/libfmp/b/b_layout.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s4_novelty_kernel.py` & `libfmp-1.2.5/libfmp/c4/c4s4_novelty_kernel.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s2_ssm.py` & `libfmp-1.2.5/libfmp/c4/c4s2_ssm.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s2_threshold.py` & `libfmp-1.2.5/libfmp/c4/c4s2_threshold.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s5_evaluation.py` & `libfmp-1.2.5/libfmp/c4/c4s5_evaluation.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s1_annotation.py` & `libfmp-1.2.5/libfmp/c4/c4s1_annotation.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s3_thumbnail.py` & `libfmp-1.2.5/libfmp/c4/c4s3_thumbnail.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/__init__.py` & `libfmp-1.2.5/libfmp/c4/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s2_synthetic_ssm.py` & `libfmp-1.2.5/libfmp/c4/c4s2_synthetic_ssm.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c4/c4s4_structure_feature.py` & `libfmp-1.2.5/libfmp/c4/c4s4_structure_feature.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c8/c8s2_f0.py` & `libfmp-1.2.5/libfmp/c8/c8s2_f0.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c8/c8s1_hps.py` & `libfmp-1.2.5/libfmp/c8/c8s1_hps.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c8/c8s3_nmf.py` & `libfmp-1.2.5/libfmp/c8/c8s3_nmf.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c8/__init__.py` & `libfmp-1.2.5/libfmp/c8/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c8/c8s2_salience.py` & `libfmp-1.2.5/libfmp/c8/c8s2_salience.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c5/c5s1_basic_theory_harmony.py` & `libfmp-1.2.5/libfmp/c5/c5s1_basic_theory_harmony.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c5/c5s3_chord_rec_hmm.py` & `libfmp-1.2.5/libfmp/c5/c5s3_chord_rec_hmm.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c5/c5s2_chord_rec_template.py` & `libfmp-1.2.5/libfmp/c5/c5s2_chord_rec_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         # Compute chroma features with filter bank (using IIR elliptic filter)
         X = librosa.iirt(y=x, sr=Fs, win_length=N, hop_length=H, center=True, tuning=0.0)
         if gamma is not None:
             X = np.log(1.0 + gamma * X)
         X = librosa.feature.chroma_cqt(C=X, bins_per_octave=12, n_octaves=7,
                                        fmin=librosa.midi_to_hz(24), norm=None)
     if norm is not None:
-        X = libfmp.c3.normalize_feature_sequence(X, norm='2')
+        X = libfmp.c3.normalize_feature_sequence(X, norm=norm)
     Fs_X = Fs / H
     return X, Fs_X, x, Fs, x_dur
 
 
 def plot_chromagram_annotation(ax, X, Fs_X, ann, color_ann, x_dur, cmap='gray_r', title=''):
     """Plot chromagram and annotation
```

### Comparing `libfmp-1.2.3/libfmp/c5/__init__.py` & `libfmp-1.2.5/libfmp/c5/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/c3s1_post_processing.py` & `libfmp-1.2.5/libfmp/c3/c3s1_post_processing.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/c3s1_transposition_tuning.py` & `libfmp-1.2.5/libfmp/c3/c3s1_transposition_tuning.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/c3s2_dtw.py` & `libfmp-1.2.5/libfmp/c3/c3s2_dtw.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/c3s2_dtw_plot.py` & `libfmp-1.2.5/libfmp/c3/c3s2_dtw_plot.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/__init__.py` & `libfmp-1.2.5/libfmp/c3/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/c3s1_audio_feature.py` & `libfmp-1.2.5/libfmp/c3/c3s1_audio_feature.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c3/c3s3_tempo_curve.py` & `libfmp-1.2.5/libfmp/c3/c3s3_tempo_curve.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c2/c2_fourier.py` & `libfmp-1.2.5/libfmp/c2/c2_fourier.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c2/c2_complex.py` & `libfmp-1.2.5/libfmp/c2/c2_complex.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c2/c2_interpolation.py` & `libfmp-1.2.5/libfmp/c2/c2_interpolation.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c2/c2_interference.py` & `libfmp-1.2.5/libfmp/c2/c2_interference.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c2/__init__.py` & `libfmp-1.2.5/libfmp/c2/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c2/c2_digitization.py` & `libfmp-1.2.5/libfmp/c2/c2_digitization.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c1/c1s2_symbolic_rep.py` & `libfmp-1.2.5/libfmp/c1/c1s2_symbolic_rep.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c1/c1s3_audio_rep.py` & `libfmp-1.2.5/libfmp/c1/c1s3_audio_rep.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         Fs: Sampling rate (Default value = 11025)
         N: FFT length (Default value = 4096)
         H: Hopsize (Default value = 2048)
         figsize: Size of the figure (Default value = (4, 2))
 
     """
     N, H = 2048, 1024
-    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hanning')
+    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hann')
     Y = np.abs(X)
     plt.figure(figsize=figsize)
     librosa.display.specshow(librosa.amplitude_to_db(Y, ref=np.max),
                              y_axis='linear', x_axis='time', sr=Fs, hop_length=H, cmap='gray_r')
     plt.ylim([0, 3000])
     # plt.colorbar(format='%+2.0f dB')
     plt.xlabel('Time (seconds)')
```

### Comparing `libfmp-1.2.3/libfmp/c1/__init__.py` & `libfmp-1.2.5/libfmp/c1/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c1/c1s1_sheet_music.py` & `libfmp-1.2.5/libfmp/c1/c1s1_sheet_music.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c7/c7s2_audio_matching.py` & `libfmp-1.2.5/libfmp/c7/c7s2_audio_matching.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c7/c7s1_audio_id.py` & `libfmp-1.2.5/libfmp/c7/c7s1_audio_id.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c7/__init__.py` & `libfmp-1.2.5/libfmp/c7/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c7/c7s3_version_id.py` & `libfmp-1.2.5/libfmp/c7/c7s3_version_id.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c6/c6s2_tempo_analysis.py` & `libfmp-1.2.5/libfmp/c6/c6s2_tempo_analysis.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c6/c6s3_adaptive_windowing.py` & `libfmp-1.2.5/libfmp/c6/c6s3_adaptive_windowing.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c6/c6s1_onset_detection.py` & `libfmp-1.2.5/libfmp/c6/c6s1_onset_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         M (int): Size (frames) of local average (Default value = 10)
         norm (bool): Apply max norm (if norm==True) (Default value = True)
 
     Returns:
         novelty_spectrum (np.ndarray): Energy-based novelty function
         Fs_feature (scalar): Feature rate
     """
-    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hanning')
+    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hann')
     Fs_feature = Fs / H
     Y = np.log(1 + gamma * np.abs(X))
     Y_diff = np.diff(Y)
     Y_diff[Y_diff < 0] = 0
     novelty_spectrum = np.sum(Y_diff, axis=0)
     novelty_spectrum = np.concatenate((novelty_spectrum, np.array([0.0])))
     if M > 0:
@@ -165,15 +165,15 @@
         M (int): Determines size (2M+1) in samples of centric window  used for local average (Default value = 40)
         norm (bool): Apply max norm (if norm==True) (Default value = True)
 
     Returns:
         novelty_phase (np.ndarray): Energy-based novelty function
         Fs_feature (scalar): Feature rate
     """
-    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hanning')
+    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hann')
     Fs_feature = Fs / H
     phase = np.angle(X) / (2*np.pi)
     phase_diff = principal_argument(np.diff(phase, axis=1))
     phase_diff2 = principal_argument(np.diff(phase_diff, axis=1))
     novelty_phase = np.sum(np.abs(phase_diff2), axis=0)
     novelty_phase = np.concatenate((novelty_phase, np.array([0, 0])))
     if M > 0:
@@ -201,15 +201,15 @@
         M (int): Determines size (2M+1) in samples of centric window used for local average (Default value = 40)
         norm (bool): Apply max norm (if norm==True) (Default value = True)
 
     Returns:
         novelty_complex (np.ndarray): Energy-based novelty function
         Fs_feature (scalar): Feature rate
     """
-    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hanning')
+    X = librosa.stft(x, n_fft=N, hop_length=H, win_length=N, window='hann')
     Fs_feature = Fs / H
     mag = np.abs(X)
     if gamma > 0:
         mag = np.log(1 + gamma * mag)
     phase = np.angle(X) / (2*np.pi)
     phase_diff = np.diff(phase, axis=1)
     phase_diff = np.concatenate((phase_diff, np.zeros((phase.shape[0], 1))), axis=1)
```

### Comparing `libfmp-1.2.3/libfmp/c6/c6s3_beat_tracking.py` & `libfmp-1.2.5/libfmp/c6/c6s3_beat_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         tempo (float): Tempo (BPM)
     """
     tempo = 60 / (beat / Fs)
     return tempo
 
 
 def compute_plot_sonify_beat(x, Fs, nov, Fs_nov, beat_ref, factor, title=None, figsize=(6, 2)):
-    """Compute, plot, and sonfy beat sequence from novelty function [FMP, Section 6.3.2]
+    """Compute, plot, and sonify beat sequence from novelty function [FMP, Section 6.3.2]
 
     Notebook: C6/C6S3_BeatTracking.ipynb
 
     Args:
         x: Novelty function
         Fs: Sample rate
         nov: Novelty function
```

### Comparing `libfmp-1.2.3/libfmp/c6/__init__.py` & `libfmp-1.2.5/libfmp/c6/__init__.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/libfmp/c6/c6s1_peak_picking.py` & `libfmp-1.2.5/libfmp/c6/c6s1_peak_picking.py`

 * *Files identical despite different names*

### Comparing `libfmp-1.2.3/setup.py` & `libfmp-1.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as fdesc:
     long_description = fdesc.read()
 
 setup(
     name='libfmp',
-    version='1.2.3',
+    version='1.2.5',
     description='Python module for fundamentals of music processing',
     author='Meinard Müller and Frank Zalkow',
     author_email='meinard.mueller@audiolabs-erlangen.de',
     url='http://audiolabs-erlangen.de/FMP',
     download_url='https://github.com/meinardmueller/libfmp',
     packages=find_packages(),
     long_description=long_description,
@@ -20,22 +20,22 @@
         "Programming Language :: Python",
         "Intended Audience :: Developers",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         "Programming Language :: Python :: 3",
     ],
     keywords='audio music sound',
     license='MIT',
-    install_requires=['ipython >= 7.8.0, < 8.0.0',
+    install_requires=['ipython >= 7.10.0, < 8.0.0',
                       'librosa >= 0.8.0, < 1.0.0',
-                      'matplotlib >= 3.1.0, < 4.0.0',
+                      'matplotlib >= 3.3.0, < 4.0.0',
                       'music21 >= 5.7.0, < 6.0.0',
-                      'numba >= 0.51.0, < 1.0.0',
-                      'numpy >= 1.17.0, < 2.0.0',
-                      'pandas >= 1.0.0, < 2.0.0',
+                      'numba >= 0.56.0, < 1.0.0',
+                      'numpy >= 1.19.0, < 2.0.0',
+                      'pandas >= 1.1.0, < 2.0.0',
                       'pretty_midi >= 0.2.0, < 1.0.0',
                       'soundfile >= 0.9.0, < 1.0.0',
-                      'scipy >= 1.3.0, < 2.0.0'],
-    python_requires='>=3.6',
+                      'scipy >= 1.5.0, < 2.0.0'],
+    python_requires='>=3.8',
     extras_require={
         'tests': ['pytest == 6.2.*']
     }
 )
```

