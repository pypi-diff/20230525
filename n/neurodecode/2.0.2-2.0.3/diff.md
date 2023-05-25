# Comparing `tmp/neurodecode-2.0.2.tar.gz` & `tmp/neurodecode-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurodecode-2.0.2.tar", last modified: Fri Jan 20 09:19:12 2023, max compression
+gzip compressed data, was "neurodecode-2.0.3.tar", last modified: Thu May 25 04:03:26 2023, max compression
```

## Comparing `neurodecode-2.0.2.tar` & `neurodecode-2.0.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.622729 neurodecode-2.0.2/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9930 2023-01-20 09:19:12.622729 neurodecode-2.0.2/PKG-INFO
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9597 2022-11-04 09:26:38.000000 neurodecode-2.0.2/README.md
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     4422 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/__init__.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/analysis/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/analysis/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     7563 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/analysis/feature_importances_topo.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     6449 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/analysis/parse_features.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    12560 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/analysis/tfr_export.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     4928 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/analysis/tfr_export_each_file.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     4350 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/colorer.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/decoder/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/decoder/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    29810 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/decoder/decoder.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    19602 2023-01-19 16:02:04.000000 neurodecode-2.0.2/neurodecode/decoder/features.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3235 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/decoder/rlda.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    27572 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/decoder/trainer.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/glass/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/glass/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     5437 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/glass/bgi_client.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/protocols/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        1 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/protocols/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    20725 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/protocols/feedback.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    22921 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/protocols/feedback_fes.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     7022 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/protocols/viz_bars.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9395 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/protocols/viz_images.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2958 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/pycnbi_config.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/stream_player/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_player/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     5868 2023-01-19 15:39:29.000000 neurodecode-2.0.2/neurodecode/stream_player/stream_player.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/stream_receiver/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_receiver/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    22404 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_receiver/stream_receiver.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/stream_recorder/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_recorder/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     6840 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_recorder/stream_recorder.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/stream_viewer/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_viewer/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1502 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_viewer/scope_settings.ini
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    40740 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_viewer/stream_viewer.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    25369 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/stream_viewer/ui_mainwindow_Viewer.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode/triggers/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/triggers/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    10620 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/triggers/pyLptControl.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2156 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/triggers/trigger_def.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.622729 neurodecode-2.0.2/neurodecode/utils/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     5949 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/Motionstim8.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2472 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/ScalerMad.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2250 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/add_lsl_events.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1044 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/benchmark_decoder.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1185 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/benchmark_multitaper.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    19412 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/convert2fif.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2809 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/epochs2mat.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2370 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/epochs2txt.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1664 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/fif2mat.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1199 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/fif_info.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1505 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/fif_resample.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1455 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/fix_channel_names.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3687 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/hdf5_to_python.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1414 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/images2pkl.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      684 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/list_trigger_pins.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2061 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/mat2fif.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2305 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/merge_events.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2772 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/nd_lsl.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      853 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/parse_online_results.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3705 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/psd_visualizer.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    24294 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/pycnbi_utils.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    24367 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/q_common.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3897 2022-11-04 09:26:38.000000 neurodecode-2.0.2/neurodecode/utils/raw2psd.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-01-20 09:19:12.618729 neurodecode-2.0.2/neurodecode.egg-info/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9930 2023-01-20 09:19:12.000000 neurodecode-2.0.2/neurodecode.egg-info/PKG-INFO
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2245 2023-01-20 09:19:12.000000 neurodecode-2.0.2/neurodecode.egg-info/SOURCES.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        1 2023-01-20 09:19:12.000000 neurodecode-2.0.2/neurodecode.egg-info/dependency_links.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      850 2023-01-20 09:19:12.000000 neurodecode-2.0.2/neurodecode.egg-info/entry_points.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      299 2023-01-20 09:19:12.000000 neurodecode-2.0.2/neurodecode.egg-info/requires.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)       12 2023-01-20 09:19:12.000000 neurodecode-2.0.2/neurodecode.egg-info/top_level.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)       38 2023-01-20 09:19:12.622729 neurodecode-2.0.2/setup.cfg
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2429 2023-01-20 09:18:52.000000 neurodecode-2.0.2/setup.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.939749 neurodecode-2.0.3/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     9930 2023-05-25 04:03:26.939749 neurodecode-2.0.3/PKG-INFO
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     9597 2022-11-04 09:26:38.000000 neurodecode-2.0.3/README.md
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     4422 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/__init__.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/analysis/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/analysis/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     7563 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/analysis/feature_importances_topo.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     6449 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/analysis/parse_features.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    12560 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/analysis/tfr_export.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     4928 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/analysis/tfr_export_each_file.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     4350 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/colorer.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/decoder/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/decoder/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    29797 2023-01-20 12:47:05.000000 neurodecode-2.0.3/neurodecode/decoder/decoder.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    19602 2023-01-19 16:02:04.000000 neurodecode-2.0.3/neurodecode/decoder/features.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     3235 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/decoder/rlda.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    27572 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/decoder/trainer.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/glass/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/glass/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     5437 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/glass/bgi_client.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/protocols/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        1 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/protocols/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    20725 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/protocols/feedback.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    22921 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/protocols/feedback_fes.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     7022 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/protocols/viz_bars.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     9395 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/protocols/viz_images.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2958 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/pycnbi_config.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/stream_player/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_player/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     5868 2023-01-19 15:39:29.000000 neurodecode-2.0.3/neurodecode/stream_player/stream_player.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/stream_receiver/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_receiver/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    22404 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_receiver/stream_receiver.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/stream_recorder/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_recorder/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     6840 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_recorder/stream_recorder.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode/stream_viewer/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_viewer/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1502 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_viewer/scope_settings.ini
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    40740 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_viewer/stream_viewer.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    25369 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/stream_viewer/ui_mainwindow_Viewer.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.939749 neurodecode-2.0.3/neurodecode/triggers/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/triggers/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    10620 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/triggers/pyLptControl.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2156 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/triggers/trigger_def.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.939749 neurodecode-2.0.3/neurodecode/utils/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     5949 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/Motionstim8.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2472 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/ScalerMad.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/__init__.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2250 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/add_lsl_events.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1044 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/benchmark_decoder.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1185 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/benchmark_multitaper.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    19412 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/convert2fif.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2809 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/epochs2mat.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2370 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/epochs2txt.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1664 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/fif2mat.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1199 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/fif_info.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1505 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/fif_resample.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1455 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/fix_channel_names.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     3687 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/hdf5_to_python.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     1414 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/images2pkl.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)      684 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/list_trigger_pins.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2061 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/mat2fif.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2305 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/merge_events.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2772 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/nd_lsl.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)      853 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/parse_online_results.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     3705 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/psd_visualizer.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    24294 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/pycnbi_utils.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)    24367 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/q_common.py
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     3897 2022-11-04 09:26:38.000000 neurodecode-2.0.3/neurodecode/utils/raw2psd.py
+drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:03:26.935749 neurodecode-2.0.3/neurodecode.egg-info/
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     9930 2023-05-25 04:03:26.000000 neurodecode-2.0.3/neurodecode.egg-info/PKG-INFO
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2245 2023-05-25 04:03:26.000000 neurodecode-2.0.3/neurodecode.egg-info/SOURCES.txt
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)        1 2023-05-25 04:03:26.000000 neurodecode-2.0.3/neurodecode.egg-info/dependency_links.txt
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)      853 2023-05-25 04:03:26.000000 neurodecode-2.0.3/neurodecode.egg-info/entry_points.txt
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)      299 2023-05-25 04:03:26.000000 neurodecode-2.0.3/neurodecode.egg-info/requires.txt
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)       12 2023-05-25 04:03:26.000000 neurodecode-2.0.3/neurodecode.egg-info/top_level.txt
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)       38 2023-05-25 04:03:26.939749 neurodecode-2.0.3/setup.cfg
+-rw-rw-r--   0 leeq      (1000) leeq      (1000)     2432 2023-05-25 04:02:55.000000 neurodecode-2.0.3/setup.py
```

### Comparing `neurodecode-2.0.2/PKG-INFO` & `neurodecode-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurodecode
-Version: 2.0.2
+Version: 2.0.3
 Summary: Real-time brain signal decoding framework
 Home-page: https://github.com/dbdq/neurodecode/
 Author: Kyuhwa Lee, Arnaud Desvachez
 Author-email: lee.kyuh@gmail.com, arnaud.desvachez@gmail.com
 License: The GNU General Public License
 Description-Content-Type: text/markdown
```

### Comparing `neurodecode-2.0.2/README.md` & `neurodecode-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/__init__.py` & `neurodecode-2.0.3/neurodecode/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/analysis/feature_importances_topo.py` & `neurodecode-2.0.3/neurodecode/analysis/feature_importances_topo.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/analysis/parse_features.py` & `neurodecode-2.0.3/neurodecode/analysis/parse_features.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/analysis/tfr_export.py` & `neurodecode-2.0.3/neurodecode/analysis/tfr_export.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/analysis/tfr_export_each_file.py` & `neurodecode-2.0.3/neurodecode/analysis/tfr_export_each_file.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/colorer.py` & `neurodecode-2.0.3/neurodecode/colorer.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/decoder/decoder.py` & `neurodecode-2.0.3/neurodecode/decoder/decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
             # debug: show min-max stats
             # c=1; print( '### %d: %.1f - %.1f = %.1f'% ( self.picks[c], max(w[c]), min(w[c]), max(w[c])-min(w[c]) ) )
 
             # psd = channels x freqs
             psd = self.psde.transform(w.reshape((1, w.shape[0], w.shape[1])))
 
-            # make a feautre vector and classify
+            # make a feature vector
             feats = np.concatenate(psd[0]).reshape(1, -1)
 
             # compute likelihoods
             probs = self.cls.predict_proba(feats)[0]
 
             # update psd buffer ( < 1 msec overhead )
             '''
```

### Comparing `neurodecode-2.0.2/neurodecode/decoder/features.py` & `neurodecode-2.0.3/neurodecode/decoder/features.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/decoder/rlda.py` & `neurodecode-2.0.3/neurodecode/decoder/rlda.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/decoder/trainer.py` & `neurodecode-2.0.3/neurodecode/decoder/trainer.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/glass/bgi_client.py` & `neurodecode-2.0.3/neurodecode/glass/bgi_client.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/protocols/feedback.py` & `neurodecode-2.0.3/neurodecode/protocols/feedback.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/protocols/feedback_fes.py` & `neurodecode-2.0.3/neurodecode/protocols/feedback_fes.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/protocols/viz_bars.py` & `neurodecode-2.0.3/neurodecode/protocols/viz_bars.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/protocols/viz_images.py` & `neurodecode-2.0.3/neurodecode/protocols/viz_images.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/pycnbi_config.py` & `neurodecode-2.0.3/neurodecode/pycnbi_config.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/stream_player/stream_player.py` & `neurodecode-2.0.3/neurodecode/stream_player/stream_player.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/stream_receiver/stream_receiver.py` & `neurodecode-2.0.3/neurodecode/stream_receiver/stream_receiver.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/stream_recorder/stream_recorder.py` & `neurodecode-2.0.3/neurodecode/stream_recorder/stream_recorder.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/stream_viewer/scope_settings.ini` & `neurodecode-2.0.3/neurodecode/stream_viewer/scope_settings.ini`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/stream_viewer/stream_viewer.py` & `neurodecode-2.0.3/neurodecode/stream_viewer/stream_viewer.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/stream_viewer/ui_mainwindow_Viewer.py` & `neurodecode-2.0.3/neurodecode/stream_viewer/ui_mainwindow_Viewer.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/triggers/pyLptControl.py` & `neurodecode-2.0.3/neurodecode/triggers/pyLptControl.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/triggers/trigger_def.py` & `neurodecode-2.0.3/neurodecode/triggers/trigger_def.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/Motionstim8.py` & `neurodecode-2.0.3/neurodecode/utils/Motionstim8.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/ScalerMad.py` & `neurodecode-2.0.3/neurodecode/utils/ScalerMad.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/add_lsl_events.py` & `neurodecode-2.0.3/neurodecode/utils/add_lsl_events.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/benchmark_decoder.py` & `neurodecode-2.0.3/neurodecode/utils/benchmark_decoder.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/benchmark_multitaper.py` & `neurodecode-2.0.3/neurodecode/utils/benchmark_multitaper.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/convert2fif.py` & `neurodecode-2.0.3/neurodecode/utils/convert2fif.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/epochs2mat.py` & `neurodecode-2.0.3/neurodecode/utils/epochs2mat.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/epochs2txt.py` & `neurodecode-2.0.3/neurodecode/utils/epochs2txt.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/fif2mat.py` & `neurodecode-2.0.3/neurodecode/utils/fif2mat.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/fif_info.py` & `neurodecode-2.0.3/neurodecode/utils/fif_info.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/fif_resample.py` & `neurodecode-2.0.3/neurodecode/utils/fif_resample.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/fix_channel_names.py` & `neurodecode-2.0.3/neurodecode/utils/fix_channel_names.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/hdf5_to_python.py` & `neurodecode-2.0.3/neurodecode/utils/hdf5_to_python.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/images2pkl.py` & `neurodecode-2.0.3/neurodecode/utils/images2pkl.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/list_trigger_pins.py` & `neurodecode-2.0.3/neurodecode/utils/list_trigger_pins.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/mat2fif.py` & `neurodecode-2.0.3/neurodecode/utils/mat2fif.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/merge_events.py` & `neurodecode-2.0.3/neurodecode/utils/merge_events.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/nd_lsl.py` & `neurodecode-2.0.3/neurodecode/utils/nd_lsl.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/parse_online_results.py` & `neurodecode-2.0.3/neurodecode/utils/parse_online_results.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/psd_visualizer.py` & `neurodecode-2.0.3/neurodecode/utils/psd_visualizer.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/pycnbi_utils.py` & `neurodecode-2.0.3/neurodecode/utils/pycnbi_utils.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/q_common.py` & `neurodecode-2.0.3/neurodecode/utils/q_common.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode/utils/raw2psd.py` & `neurodecode-2.0.3/neurodecode/utils/raw2psd.py`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode.egg-info/PKG-INFO` & `neurodecode-2.0.3/neurodecode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurodecode
-Version: 2.0.2
+Version: 2.0.3
 Summary: Real-time brain signal decoding framework
 Home-page: https://github.com/dbdq/neurodecode/
 Author: Kyuhwa Lee, Arnaud Desvachez
 Author-email: lee.kyuh@gmail.com, arnaud.desvachez@gmail.com
 License: The GNU General Public License
 Description-Content-Type: text/markdown
```

### Comparing `neurodecode-2.0.2/neurodecode.egg-info/SOURCES.txt` & `neurodecode-2.0.3/neurodecode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.2/neurodecode.egg-info/entry_points.txt` & `neurodecode-2.0.3/neurodecode.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [console_scripts]
 nd_add_lsl_events = neurodecode.utils.add_lsl_events:main
 nd_convert2fif = neurodecode.utils.convert2fif:main
 nd_decoder = neurodecode.decoder.decoder:main
 nd_fif2mat = neurodecode.utils.fif2mat:main
 nd_fif_info = neurodecode.utils.fif_info:main
 nd_fif_resample = neurodecode.utils.fif_resample:main
-nd_parse_features = neurodecode.utils.parse_features:main
+nd_parse_features = neurodecode.analysis.parse_features:main
 nd_stream_player = neurodecode.stream_player.stream_player:main
 nd_stream_recorder = neurodecode.stream_recorder.stream_recorder:main
 nd_stream_viewer = neurodecode.stream_viewer.stream_viewer:main
 nd_test_mi = neurodecode.protocols.mi.test_mi:main
 nd_tfr_export = neurodecode.analysis.tfr_export:main
 nd_tfr_export_each_file = neurodecode.analysis.tfr_export_each_file:main
 nd_train_mi = neurodecode.protocols.mi.train_mi:main
```

### Comparing `neurodecode-2.0.2/setup.py` & `neurodecode-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         os.system('mklink pycnbi neurodecode /J')
     else:
         os.symlink('./neurodecode', './pycnbi', True)
 '''
 
 setup(
     name='neurodecode',
-    version='2.0.2',
+    version='2.0.3',
     author='Kyuhwa Lee, Arnaud Desvachez',
     author_email='lee.kyuh@gmail.com, arnaud.desvachez@gmail.com',
     license='The GNU General Public License',
     url='https://github.com/dbdq/neurodecode/',
     description='Real-time brain signal decoding framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
@@ -50,15 +50,15 @@
     ],
     entry_points = {'console_scripts':[
         'nd_stream_viewer=neurodecode.stream_viewer.stream_viewer:main',
         'nd_fif_info=neurodecode.utils.fif_info:main',
         'nd_fif_resample=neurodecode.utils.fif_resample:main',
         'nd_fif2mat=neurodecode.utils.fif2mat:main',
         'nd_add_lsl_events=neurodecode.utils.add_lsl_events:main',
-        'nd_parse_features=neurodecode.utils.parse_features:main',
+        'nd_parse_features=neurodecode.analysis.parse_features:main',
         'nd_convert2fif=neurodecode.utils.convert2fif:main',
         'nd_train_mi=neurodecode.protocols.mi.train_mi:main',
         'nd_test_mi=neurodecode.protocols.mi.test_mi:main',
         'nd_stream_player=neurodecode.stream_player.stream_player:main',
         'nd_stream_recorder=neurodecode.stream_recorder.stream_recorder:main',
         'nd_tfr_export=neurodecode.analysis.tfr_export:main',
         'nd_tfr_export_each_file=neurodecode.analysis.tfr_export_each_file:main',
```

