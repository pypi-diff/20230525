# Comparing `tmp/scipion-em-tomo-3.1.8.tar.gz` & `tmp/scipion-em-tomo-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomo-3.1.8.tar", last modified: Mon Apr 24 13:02:54 2023, max compression
+gzip compressed data, was "scipion-em-tomo-3.1.9.tar", last modified: Thu May 25 10:20:11 2023, max compression
```

## Comparing `scipion-em-tomo-3.1.8.tar` & `scipion-em-tomo-3.1.9.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.024696 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.024696 scipion-em-tomo-3.1.8/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.028696 scipion-em-tomo-3.1.8/tomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/convert/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   101779 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.032696 scipion-em-tomo-3.1.8/tomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_assignTransformationTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2tomoMask.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_consensus_classes_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ctf_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_extract_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates_from_scipion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomomasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_misalignTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_particles_to_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_rotate_astigmatism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_split_evenodd_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_tomo_to_mics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_consensus_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_convert_coords3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_correct_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_estimate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.032696 scipion-em-tomo-3.1.8/tomo/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/HIV-Picking-with-Dynamo.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/HIV-Reconstruction.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/HIV-Subtomogram-averaging.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/Membrane picking-with-PySeg.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/tomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_base_centralized_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_fit_vesicles.py
--rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_tomo_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/tomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/viewer_split_evenodd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.568217 scipion-em-tomo-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-25 10:20:11.568217 scipion-em-tomo-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.556217 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-25 10:20:11.000000 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-25 10:20:11.000000 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:20:11.000000 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 10:20:11.000000 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 10:20:11.000000 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 10:20:11.000000 scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:20:11.568217 scipion-em-tomo-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.556217 scipion-em-tomo-3.1.9/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.556217 scipion-em-tomo-3.1.9/tomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/convert/mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   103618 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.564217 scipion-em-tomo-3.1.9/tomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_assignTransformationTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_assign_tomo2subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_assign_tomo2tomoMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_consensus_classes_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ctf_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_extract_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_coordinates_from_scipion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_tomomasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_misalignTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_particles_to_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_rotate_astigmatism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_split_evenodd_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_tomo_to_mics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_consensus_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_convert_coords3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_correct_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_estimate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.564217 scipion-em-tomo-3.1.9/tomo/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/templates/HIV-Picking-with-Dynamo.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/templates/HIV-Reconstruction.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/templates/HIV-Subtomogram-averaging.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/templates/Membrane picking-with-PySeg.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.568217 scipion-em-tomo-3.1.9/tomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_base_centralized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_fit_vesicles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_tomo_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:20:11.568217 scipion-em-tomo-3.1.9/tomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/viewers/viewer_ctf_tomo_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/viewers/viewer_split_evenodd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/viewers/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42289 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-25 10:15:15.000000 scipion-em-tomo-3.1.9/tomo/wizards.py
```

### Comparing `scipion-em-tomo-3.1.8/LICENSE` & `scipion-em-tomo-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/PKG-INFO` & `scipion-em-tomo-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.8
+Version: 3.1.9
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.8/README.rst` & `scipion-em-tomo-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/PKG-INFO` & `scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.8
+Version: 3.1.9
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/SOURCES.txt` & `scipion-em-tomo-3.1.9/scipion_em_tomo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 tomo/protocols/protocol_alignment_assign.py
 tomo/protocols/protocol_assignTransformationTS.py
 tomo/protocols/protocol_assign_tomo2subtomo.py
 tomo/protocols/protocol_assign_tomo2tomoMask.py
 tomo/protocols/protocol_base.py
 tomo/protocols/protocol_compose_TS.py
 tomo/protocols/protocol_consensus_classes_subtomo.py
+tomo/protocols/protocol_ctf_consensus.py
 tomo/protocols/protocol_ctf_validate.py
 tomo/protocols/protocol_extract_coordinates.py
 tomo/protocols/protocol_fit_ellipsoid.py
 tomo/protocols/protocol_import_coordinates.py
 tomo/protocols/protocol_import_coordinates_from_scipion.py
 tomo/protocols/protocol_import_subtomograms.py
 tomo/protocols/protocol_import_tomograms.py
@@ -54,11 +55,12 @@
 tomo/tests/test_compose_TS.py
 tomo/tests/test_fit_vesicles.py
 tomo/tests/test_import.py
 tomo/tests/test_objects.py
 tomo/tests/test_tomo_base.py
 tomo/tests/test_transformations.py
 tomo/viewers/__init__.py
+tomo/viewers/viewer_ctf_tomo_consensus.py
 tomo/viewers/viewer_split_evenodd.py
 tomo/viewers/viewers_data.py
 tomo/viewers/views.py
 tomo/viewers/views_tkinter_tree.py
```

### Comparing `scipion-em-tomo-3.1.8/setup.py` & `scipion-em-tomo-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/__init__.py` & `scipion-em-tomo-3.1.9/tomo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 
-__version__ = '3.1.8'
+__version__ = '3.1.9'
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwem.Plugin):
     @classmethod
     def _defineVariables(cls):
```

### Comparing `scipion-em-tomo-3.1.8/tomo/constants.py` & `scipion-em-tomo-3.1.9/tomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/convert/__init__.py` & `scipion-em-tomo-3.1.9/tomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/convert/convert.py` & `scipion-em-tomo-3.1.9/tomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/convert/mdoc.py` & `scipion-em-tomo-3.1.9/tomo/convert/mdoc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/icon.png` & `scipion-em-tomo-3.1.9/tomo/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/objects.py` & `scipion-em-tomo-3.1.9/tomo/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,36 @@
 class TiltImageBase:
     """ Base class for TiltImageM and TiltImage. """
 
     def __init__(self, tsId=None, tiltAngle=None, acquisitionOrder=None, **kwargs):
         self._tiltAngle = Float(tiltAngle)
         self._tsId = String(tsId)
         self._acqOrder = Integer(acquisitionOrder)
+        self._oddEvenFileNames = CsvList(pType=str) #IMPORTANT: The odd is the first one and the even the second one
+
+    def hasOddEven(self):
+        return not self._oddEvenFileNames.isEmpty()
+
+    def getOddEven(self):
+        return self._oddEvenFileNames
+
+    def getOdd(self):
+        return self._oddEvenFileNames[0]
+
+    def getEven(self):
+        return self._oddEvenFileNames[1]
+
+    def setOdd(self, fnOdd):
+        self._oddEvenFileNames[0] = fnOdd
+
+    def setEven(self, fnEven):
+        self._oddEvenFileNames[1] = fnEven
+
+    def setOddEven(self, listFileNames):
+        self._oddEvenFileNames.set(listFileNames)
 
     def getTsId(self):
         """ Get unique TiltSerie ID, usually retrieved from the
         file pattern provided by the user at the import time.
         """
         return self._tsId.get()
 
@@ -156,23 +178,25 @@
 
     def copyInfo(self, other, copyId=False, copyTM=True):
         self.copyAttributes(other, '_tiltAngle', '_tsId', '_acqOrder')
         if copyId:
             self.copyObjId(other)
         if copyTM and other.hasTransform():
             self.copyAttributes(other, '_transform')
-
+        if other.hasOddEven():
+            self.copyAttributes(other, '_oddEvenFileNames')
 
 class TiltImage(data.Image, TiltImageBase):
     """ Tilt image """
 
     def __init__(self, location=None, **kwargs):
         data.Image.__init__(self, location, **kwargs)
         TiltImageBase.__init__(self, **kwargs)
 
+
     def copyInfo(self, other, copyId=False, copyTM=True, copyStatus=True):
         data.Image.copyInfo(self, other)
         TiltImageBase.copyInfo(self, other, copyId=copyId, copyTM=copyTM)
         if copyStatus:
             self.setEnabled(other.isEnabled())
 
     def parseFileName(self, suffix="", extension=None):
@@ -188,35 +212,39 @@
 
         if extension is not None:
             fileExtension = extension
 
         return fileName + suffix + fileExtension
 
 
-TS_IGNORE_ATTRS = ['_mapperPath', '_size', '_hasAlignment']
+TS_IGNORE_ATTRS = ['_mapperPath', '_size', '_hasAlignment', '_hasOddEven']
 
 
 class TiltSeriesBase(data.SetOfImages):
     TS_ID_FIELD = '_tsId'
     def __init__(self, **kwargs):
         data.SetOfImages.__init__(self, **kwargs)
         self._tsId = String(kwargs.get('tsId', None))
         # TiltSeries will always be used inside a SetOfTiltSeries
         # so, let's do not store the mapper path by default
         self._mapperPath.setStore(False)
         self._acquisition = TomoAcquisition()
         self._origin = Transform()
         self._anglesCount = Integer()
         self._hasAlignment = Boolean(False)
+        self._hasOddEven = Boolean(False)
         self._interpolated = Boolean(False)
         self._ctfCorrected = Boolean(False)
 
     def getAnglesCount(self):
         return self._anglesCount
 
+    def hasOddEven(self):
+        return self._hasOddEven.get()
+
     def setAnglesCount(self, value):
 
         if isinstance(value, int):
             self._anglesCount.set(value)
         else:
             self._anglesCount = value
 
@@ -264,14 +292,17 @@
     def append(self, tiltImage: TiltImageBase):
         tiltImage.setTsId(self.getTsId())
         data.SetOfImages.append(self, tiltImage)
 
         if tiltImage.hasTransform():
             self._hasAlignment.set(True)
 
+        if tiltImage.hasOddEven():
+            self._hasOddEven.set(True)
+
     def clone(self, ignoreAttrs=TS_IGNORE_ATTRS):
         clone = self.getClass()()
         clone.copy(self, ignoreAttrs=ignoreAttrs)
         return clone
 
     def close(self):
         # Do nothing on close, since the db will be closed by SetOfTiltSeries
@@ -371,14 +402,18 @@
     if tiltSeries.interpolated():
         s.append('! interp')
 
     # CTF status
     if tiltSeries.ctfCorrected():
         s.append('+ctf')
 
+    # Odd even associated
+    if tiltSeries.hasOddEven():
+        s.append('+oe')
+
     return (", " + ", ".join(s)) if len(s) else ""
 
 
 class TiltSeries(TiltSeriesBase):
     ITEM_TYPE = TiltImage
 
     def __str__(self):
@@ -612,17 +647,21 @@
     """
 
     def __init__(self, **kwargs):
         data.SetOfImages.__init__(self, **kwargs)
         self._anglesCount = Integer()
         self._acquisition = TomoAcquisition()
         self._hasAlignment = Boolean(False)
+        self._hasOddEven = Boolean(False)
         self._ctfCorrected = Boolean(False)
         self._interpolated = Boolean(False)
 
+    def hasOddEven(self):
+        return self._hasOddEven.get()
+
     def getAnglesCount(self):
         return self._anglesCount.get()
 
     def setAnglesCount(self, value):
         self._anglesCount.set(value)
 
     def ctfCorrected(self):
@@ -718,14 +757,15 @@
     def update(self, item: TiltSeriesBase):
 
         self.setDim(item.getDim())
         self._anglesCount.set(item.getSize())
         self._hasAlignment.set(item.hasAlignment())
         self._interpolated.set(item.interpolated())
         self._ctfCorrected.set(item.ctfCorrected())
+        self._hasOddEven.set(item.hasOddEven())
 
         super().update(item)
 
     def updateDim(self):
         """ Update dimensions of this set base on the first element. """
 
         logger.warning("TO DEVELOPERS: update is called always before this. This call to updateDim could be removed.")
@@ -1067,19 +1107,41 @@
 class SetOfTomograms(data.SetOfVolumes):
     ITEM_TYPE = Tomogram
     EXPOSE_ITEMS = False
 
     def __init__(self, *args, **kwargs):
         data.SetOfVolumes.__init__(self, **kwargs)
         self._acquisition = TomoAcquisition()
+        self._hasOddEven = Boolean(False)
+
+    def hasOddEven(self):
+        return self._hasOddEven.get()
 
     def updateDim(self):
         """ Update dimensions of this set base on the first element. """
         self.setDim(self.getFirstItem().getDim())
 
+    def __str__(self):
+        sampling = self.getSamplingRate()
+        tomoStr = "+oe," if self.hasOddEven() else ''
+
+        if not sampling:
+            logger.error("FATAL ERROR: Object %s has no sampling rate!!!"
+                         % self.getName())
+            sampling = -999.0
+
+        s = "%s (%d items, %s, %s %0.2f Å/px%s)" % \
+            (self.getClassName(), self.getSize(),
+             self._dimStr(), tomoStr, sampling, self._appendStreamState())
+        return s
+
+    def update(self, item: Tomogram):
+        self._hasOddEven.set(item.hasHalfMaps())
+        super().update(item)
+
 
 class TomoMask(Tomogram):
     """ Object used to represent segmented tomograms
     """
 
     def __init__(self, **kwargs):
         Tomogram.__init__(self, **kwargs)
@@ -1629,25 +1691,25 @@
 
     def getVolName(self):
         """ Return the tomogram filename if the coordinate is not None.
         or have set the _volName property.
         """
         if self._volName.hasValue():
             return self._volName.get()
-        # getVolume does not exists!
-        # if self.getVolume():
-        #     return self.getVolume().getFileName()
+
+        if self.hasCoordinate3D():
+            return self.getCoordinate3D().getVolName()
 
         return "Missing"
 
     def setVolName(self, volName):
         self._volName.set(volName)
 
     def getVolumeOrigin(self, angstrom=False):
-        """Return the a vector that can be used to move the position of the Coordinate3D
+        """Return the vector that can be used to move the position of the Coordinate3D
         associated to the SubTomogram (referred to the center of the Tomogram or other
         origin specified by the user) to the bottom left corner of the Tomogram
         """
         if angstrom:
             return self.getShiftsFromOrigin()
         else:
             sr = self.getSamplingRate()
```

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/__init__.py` & `scipion-em-tomo-3.1.9/tomo/protocols/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 from .protocol_ctf_validate import ProtCTFTomoSeriesValidate
 from .protocol_particles_to_subtomograms import Prot2DParticlesToSubtomograms
 from .protocol_rotate_astigmatism import ProtRotateAstigmatism
 from .protocol_tomo_to_mics import ProtTomoToMics, Prot2DcoordsTo3DCoords
 from .protocol_ts_convert_coords3d import ProtTsConvertCoordinates3d
 from .protocol_compose_TS import ProtComposeTS
 from .protocol_misalignTS import ProtTomoMisalignTiltSeries
+from .protocol_ctf_consensus import ProtCTFTomoSeriesConsensus
 from .protocol_fit_ellipsoid import TomoProtFitEllipsoid, XmippProtFitEllipsoid
```

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_alignment_assign.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_assignTransformationTS.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_assignTransformationTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2subtomo.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_assign_tomo2subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2tomoMask.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_assign_tomo2tomoMask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_base.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_compose_TS.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_compose_TS.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,52 +26,59 @@
 import time
 import os
 from glob import glob
 from pwem.protocols.protocol_import.base import ProtImport
 import pyworkflow as pw
 from pyworkflow.protocol import params, STEPS_PARALLEL
 import pyworkflow.protocol.constants as cons
+from pyworkflow.object import Set
 from tomo.convert.mdoc import MDoc
 import pwem.objects as emobj
 import tomo.objects as tomoObj
+from tomo.objects import SetOfTiltSeries
 from pwem.objects.data import Transform
 from pyworkflow.object import Integer
 from tomo.protocols import ProtTomoBase
 from pwem.emlib.image import ImageHandler
 
+OUT_STS = "TiltSeries"
+
 
 class ProtComposeTS(ProtImport, ProtTomoBase):
-    """ Compose in streaming a set of tilt series based on a sets of micrographs and mdoc files.
-    Three time parameters are abailable for the streaming behaviour:
-    Time for next tilt, Time for next micrograph and Time for next Tilt Serie
+    """ Compose in streaming a set of tilt series based on a set of micrographs and mdoc files.
+    Two time parameters are abailable for the streaming behaviour:
+    Time to next tilt and time to next tilt serie
     """
     _devStatus = pw.BETA
     _label = 'Compose Tilt Serie'
+    _possibleOutputs = {OUT_STS: SetOfTiltSeries}
 
     def __init__(self, **args):
         ProtImport.__init__(self, **args)
         self.stepsExecutionMode = STEPS_PARALLEL  # Defining that the protocol contain parallel steps
         self.newSteps = []
         self.listMdocsRead = []
+        self.list_reading = []
         self.TiltSeries = None
         self.waitingMdoc = True
+        self.time4NextMic = 10
         self.time4NextTS_current = time.time()
 
     # -------------------------- DEFINES AND STEPS -----------------------
     def _defineParams(self, form):
         form.addSection(label='Import')
 
-        form.addParam('inputMicrographs', params.PointerParam,
+        form.addParam('inputMicrographs', params.PointerParam, allowsNull=False,
                       pointerClass='SetOfMicrographs',
                       important=True,
                       label="Input micrographs",
                       help='Select the SetOfMicrographs to import')
 
         form.addParam('filesPath', params.PathParam,
-                      label="Files directory ot the tiltSerie files",
+                      label="Path with the *.mdoc files for each TiltSerie",
                       help="Root directory of the tilt-series. "
                            "Will be search the *.mdoc file for each Tilt Serie")
 
         form.addParam('mdoc_bug_Correction', params.BooleanParam, default=False,
                       label="mdoc bug Correction",
                       help="Setting True, the mdoc generated by SerialEM "
                            "will be read considering the bug")
@@ -88,22 +95,17 @@
                            "be used right away by next steps.")
 
         form.addParam('time4NextTilt', params.IntParam, default=180,
                       condition='dataStreaming',
                       label="Time for next Tilt (secs)",
                       help="Delay (in seconds) until the next tilt is "
                            "registered in the mdoc file. After "
-                           "timeout,\n if there is no new tilt, the tilt serie"
-                           "is considered as completed.\n"
-                           "Minimum time 20 segs")
-        form.addParam('time4NextMic', params.IntParam, default=12,
-                      condition='dataStreaming',
-                      label="Time for next micograph processed (secs)",
-                      help="Delay (in seconds) until the next micograph is "
-                           "processed by the previous protocol")
+                           "timeout, if there is no new tilt, the tilt serie "
+                           "is considered as completed."
+                           "Minimum time recomended 20 segs")
         form.addParam('time4NextTS', params.IntParam, default=1800,
                       condition='dataStreaming',
                       label="Time for next TiltSerie (secs)",
                       help="Interval of time (in seconds) after which, "
                            "if no new tilt serie is detected, the protocol will "
                            "end. "
                            "The default value is  high (30 min) to "
@@ -122,40 +124,55 @@
         self.CloseStep_ID = self._insertFunctionStep('closeSet',
                                                      prerequisites=[],
                                                      wait=True)
         self.newSteps.append(self.CloseStep_ID)
 
     def _stepsCheck(self):
         """
-        Read all the mdoc files abailable, sort by date and run 'readMdoc'
+        Read all available mdoc files, sort them by date and runs 'readMdoc'
 
         """
         current_time = time.time()
         delay = int(current_time - self.time4NextTS_current)
         if self.waitingMdoc:
             self.debug('Timeout for next TiltSerie (.mdoc file) ' +
                        str(self.time4NextTS.get()) + ' segs ...')
         self.waitingMdoc = False
-        list_current = self.findMdoc()
-        list_remain = [x for x in list_current if x not in self.listMdocsRead]
+        self.list_current = self.findMdoc()
+        self.list_remain = [x for x in self.list_current if x not in self.listMdocsRead
+                       and x not in self.list_reading]
+
         # STREAMING CHECKPOINT
         if delay > int(self.time4NextTS.get()):
+            self.info('Time waiting next Tilt Serie has expired. ({}s)'.format(
+                str(self.time4NextTS.get())))
+            output_step = self._getFirstJoinStep()
+            self.TiltSeries.setStreamState(Set.STREAM_CLOSED)
+            if output_step and output_step.isWaiting():
+                output_step.setStatus(cons.STATUS_NEW)
+
+        elif self.list_remain == [] and self._loadInputList()[1] == False:
+            self.info('There is no more mdoc file to read and the set of micrographs is closed')
             output_step = self._getFirstJoinStep()
+            self.TiltSeries.setStreamState(Set.STREAM_CLOSED)
             if output_step and output_step.isWaiting():
                 output_step.setStatus(cons.STATUS_NEW)
 
-        elif list_remain:
+        elif self.list_remain:
             self.waitingMdoc = True
-            self.listMdocsRead.append(list_remain[0])
+            #self.listMdocsRead.append(list_remain[0])
             self.time4NextTS_current = time.time()
-            new_step_id = self._insertFunctionStep('readMdoc', list_remain[0],
+            self.list_reading.append(self.list_remain[0])
+            new_step_id = self._insertFunctionStep('readMdoc', self.list_remain[0],
                                                    prerequisites=[], wait=False)
             self.newSteps.append(new_step_id)
             self.updateSteps()
 
+
+
     def closeSet(self):
         pass
 
     def _getFirstJoinStep(self):
         for s in self._steps:
             if s.funcName == self._getFirstJoinStepName():
                 return s
@@ -181,126 +198,142 @@
 
     def readMdoc(self, file2read):
         """
         Main function to launch the match with the set of micrographs and
         launch the create of SetOfTiltSeries and each TiltSerie
         :param file2read: mdoc file in the path
         """
+        self.info('Reading mdoc file: {}'.format(file2read))
         statusMdoc, mdoc_order_angle_list = self.readingMdocTiltInfo(file2read)
         # STREAMING CHECKPOINT
         while time.time() - self.readDateFile(file2read) < \
                 self.time4NextTilt.get():
             self.debug('Waiting next tilt... ({} tilts found)'.format(
                 len(mdoc_order_angle_list)))
             time.sleep(self.time4NextTilt.get() / 2)
             statusMdoc, mdoc_order_angle_list = \
                 self.readingMdocTiltInfo(file2read)
+        self.info('mdoc file {} is considered closed'.format(os.path.basename(file2read)))
         if statusMdoc:
             if len(mdoc_order_angle_list) < 3:
-                self.error('Mdoc error. Less than 3 tilts in the serie')
-            elif self.matchTS(mdoc_order_angle_list):
+                self.info('Mdoc error. Less than 3 tilts on the serie')
+                self.listMdocsRead.append(file2read)
+
+            elif self.matchTS(mdoc_order_angle_list, file2read):
                 self.createTS(self.mdoc_obj)
+                self.listMdocsRead.append(file2read)
+                self.listMdocsRead.append(file2read)
+
+                self.info("Tilt Serie ({} tilts) composed from mdoc file: {}\n".
+                    format(len(mdoc_order_angle_list), file2read))
                 # SUMMARY INFO
                 summaryF = self._getPath("summary.txt")
                 summaryF = open(summaryF, "a")
                 summaryF.write(
                     "Tilt Serie ({} tilts) composed from mdoc file: {}\n".
                     format(len(mdoc_order_angle_list), file2read))
                 summaryF.close()
 
+
+        self.list_reading.remove(file2read)
+
     def readingMdocTiltInfo(self, file2read):
         """
         :param file2read: mdoc file to read
         :return: Bool: if the validation of the mdoc goes good or bad
                  mdoc_order_angle_list: list with info for each tilt
                     file, acquisition order and tilt Angle
         """
         mdoc_order_angle_list = []
         self.mdoc_obj = MDoc(file2read)
         validation_error = self.mdoc_obj.read(ignoreFilesValidation=True)
         if validation_error:
             self.debug(validation_error)
             return False, mdoc_order_angle_list
-        self.info('mdoc file to read: {}'.format(file2read))
         for tilt_metadata in self.mdoc_obj.getTiltsMetadata():
             filepath = tilt_metadata.getAngleMovieFile()
             tiltA = tilt_metadata.getTiltAngle()
             if self.mdoc_bug_Correction.get():
                 filepath, tiltA = self.fixingMdocBug(filepath, tiltA)
 
             mdoc_order_angle_list.append((filepath,
-                                          '{:03d}'.format(tilt_metadata.getAcqOrder()), tiltA))
+                '{:03d}'.format(tilt_metadata.getAcqOrder()), tiltA))
         return True, mdoc_order_angle_list
 
+
     def fixingMdocBug(self, filepath, tiltA):
         idx = filepath.find(']_')
         filepath = filepath[:idx + 2] + filepath[idx + 2].upper() + filepath[idx + 3:]
         if float(tiltA) - round(float(tiltA), 0) != 0:
             filepath = filepath.replace(str(tiltA), str(round(float(tiltA))) + '.00')
             tiltA = str(round(float(tiltA))) + '.00'
         return filepath, tiltA
 
     def readDateFile(self, file):
         return os.path.getmtime(file)
 
-    def matchTS(self, mdoc_order_angle_list):
+    def matchTS(self, mdoc_order_angle_list, file2read):
         """
         Edit the self.listOfMics with the ones in the mdoc file
         :param mdoc_order_angle_list: for each tilt:
                 filename, acquisitionOrder, Angle
         """
-        len_mics_input_1 = self._loadInputList()
+        len_mics_input_1, streamOpen = self._loadInputList()
         # STREAMING CHECKPOINT
-        while len(mdoc_order_angle_list) > len_mics_input_1:
-            self.info('Tilts in the mdoc file: {} Micrographs  abailables: {}'.format(
-                len(mdoc_order_angle_list), len(self.listOfMics)))
+        while len(mdoc_order_angle_list) > len_mics_input_1 and streamOpen == True:
+            self.info('Tilts on the mdoc {}: {} Micrographs abailables: {}'.format(
+                os.path.basename(file2read), len(mdoc_order_angle_list), len(self.listOfMics)))
             self.info('Waiting next micrograph...')
-            time.sleep(self.time4NextMic.get())
-            len_mics_input_2 = self._loadInputList()
-            if len_mics_input_2 == len_mics_input_1:
-                return False
-            len_mics_input_1 = self._loadInputList()
+            time.sleep(self.time4NextMic)
+            len_mics_input_1, streamOpen = self._loadInputList()
 
-        self.info('Tilts in the mdoc file: {}\n'
+        self.info('Tilts on the mdoc file: {}\n'
                   'Micrographs availables: {}'.format(
             len(mdoc_order_angle_list), len(self.listOfMics)))
 
-        # MATCH
-        list_mdoc_files = [os.path.basename(fp[0]) for fp in mdoc_order_angle_list]
+        #MATCH
+        list_mdoc_files = [os.path.splitext(os.path.basename(fp[0]))[0] for fp in mdoc_order_angle_list] #quitar la extension que no tiene por k ser mrc!!
         list_mics_matched = []
         for x, mic in enumerate(self.listOfMics):
-            if mic.getMicName() in list_mdoc_files:
+            if os.path.splitext(mic.getMicName())[0] in list_mdoc_files:
                 list_mics_matched.append(mic)
-        self.listOfMics = list_mics_matched
 
-        if len(self.listOfMics) != len(mdoc_order_angle_list):
-            self.error('Micrographs doesnt match with mdoc read.\n'
-                      'number of mics: {}, number of mics on mdoc: {}'.format(
+        if len(list_mics_matched) != len(mdoc_order_angle_list):
+            if streamOpen == False:
+                self.info('Micrographs doesnt match with mdoc {} read'
+                      'Number of mics: {}, number of mics on mdoc: {}\n'
+                       'The set of micrographs is closed but has not all'
+                       ' the micrographs the mdoc refer'.format(file2read,
                 len(self.listOfMics), len(mdoc_order_angle_list)))
-            return False
+                self.listMdocsRead.append(file2read)
+                return False
+            else:
+                self.info('The micrographs read does not belong the mdoc {}. '
+                          'The mdoc will be read in furute'.format(os.path.basename(file2read)))
         else:
             self.info('Micrographs matched for the mdoc file: {}'.format(
-                len(self.listOfMics)))
+                len(list_mics_matched)))
             return True
 
     def _loadInputList(self):
         """ Load the input set of mics and create a list. """
         mic_file = self.inputMicrographs.get().getFileName()
-        self.info("Loading input db: %s" % mic_file)
+        self.debug("Loading input db: %s" % mic_file)
         mic_set = emobj.SetOfMicrographs(filename=mic_file)
         mic_set.loadAllProperties()
         self.listOfMics = [m.clone() for m in mic_set]
         mic_set.close()
-        return len(self.listOfMics)
+        return len(self.listOfMics), self.inputMicrographs.get().isStreamOpen()
 
     def createTS(self, mdoc_obj):
         """
         Create the SetOfTiltSeries and each TiltSerie
         :param mdoc_obj: mdoc object to manage
         """
+        self.info('Tilt Serie {} beeing composed...'.format(mdoc_obj.getTsId()))
         if self.TiltSeries is None:
             SOTS = self._createSetOfTiltSeries(suffix='')
             SOTS.setStreamState(SOTS.STREAM_OPEN)
             SOTS.enableAppend()
             self._defineOutputs(TiltSeries=SOTS)
             self._defineSourceRelation(self.inputMicrographs, SOTS)
             self._store(SOTS)
@@ -341,31 +374,33 @@
         origin = Transform()
         ts_obj.setOrigin(origin)
         SOTS.append(ts_obj)
 
         self.setingTS(SOTS, ts_obj, file_ordered_angle_list,
                       incoming_dose_list, accumulated_dose_list)
 
-        SOTS.setStreamState(SOTS.STREAM_CLOSED)
+        #SOTS.setStreamState(SOTS.STREAM_CLOSED)
         ts_obj.write(properties=False)
         SOTS.update(ts_obj)
         SOTS.updateDim()
         SOTS.write()
         self._store(SOTS)
 
+
     def setingTS(self, SOTS, ts_obj, file_ordered_angle_list,
                  incoming_dose_list, accumulated_dose_list):
         """
         Set all the info in each tilt and set the ts_obj information with all
         the tilts
         :param SOTS: Set Ot Tilt Serie
         :param ts_obj: Tilt Serie Object to add tilts
         :param file_ordered_angle_list: list of files sorted by angle
         :param incoming_dose_list: list of dose
         :param accumulated_dose_list: list of accumulated dose
+        :param origin: transform matrix
         :return:
         """
         ts_fn = self._getOutputTiltSeriesPath(ts_obj)
         ts_fn_dw = self._getOutputTiltSeriesPath(ts_obj, '_DW')
         counter_ti = 0
 
         TSAngleFile = self._getPath("{}.rawtlt".format(ts_obj.getTsId()))
@@ -418,17 +453,16 @@
         base = self._getExtraPath(self._getTiltImageMRoot(tilt_image))
         return base + '.mrc', base + '_Out.mrc'
 
     def _getTiltImageMRoot(self, tim):
         return '%s_%02d' % (tim.getTsId(), tim.getObjId())
 
     def _validate(self):
-        errors = [] if len(self.inputMicrographs.get()) > 1 else \
-            ["More than one Input micrographs is needed to run."]
-        return errors
+        pass
+
 
     def _summary(self):
         summary = []
 
         summaryF = self._getPath("summary.txt")
         if not os.path.exists(summaryF):
             summary.append("No summary file yet.")
```

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_consensus_classes_subtomo.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_consensus_classes_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ctf_validate.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ctf_validate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_extract_coordinates.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_fit_ellipsoid.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_fit_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates_from_scipion.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_coordinates_from_scipion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_subtomograms.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomograms.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_tomograms.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from os.path import abspath, basename
 
-from pwem import Ccp4Header
+from pwem.convert.headers import Ccp4Header
 from pwem.emlib.image import ImageHandler
 from pwem.objects import Transform
 from pyworkflow import BETA
 from pyworkflow.utils.path import createAbsLink, removeExt
 import pyworkflow.protocol.params as params
 
 from .protocol_base import ProtTomoImportFiles, ProtTomoImportAcquisition
```

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomomasks.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_import_tomomasks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_misalignTS.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_misalignTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_particles_to_subtomograms.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_particles_to_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_rotate_astigmatism.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_rotate_astigmatism.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_split_evenodd_subtomos.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_split_evenodd_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_tomo_to_mics.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_tomo_to_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_base.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_consensus_alignment.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_consensus_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_convert_coords3d.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_convert_coords3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_correct_motion.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_correct_motion.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import os
-from os.path import abspath
+from os.path import abspath, relpath
 
 import numpy as np
 
 import pyworkflow as pw
 import pyworkflow.protocol.params as params
+from pyworkflow.object import String, CsvList
 from pyworkflow.utils import removeBaseExt
 from pyworkflow.utils.properties import Message
 from pwem.emlib.image import ImageHandler
 
 from ..objects import TiltSeries, TiltImage, SetOfTiltSeries
 from .protocol_ts_base import ProtTsProcess
 
@@ -54,26 +55,21 @@
     or the cropping options (region of interest)
     """
     _possibleOutputs = {'outputTiltSeries': SetOfTiltSeries,
                         OUTPUT_TILT_SERIES_DW: SetOfTiltSeries,
                         OUTPUT_TILT_SERIES_EVEN: SetOfTiltSeries,
                         OUTPUT_TILT_SERIES_ODD: SetOfTiltSeries}
 
-    # Attributes used for even/odd frames splitting if requested
-    evenAvgFrameList = []
-    oddAvgFrameList = []
-    tsMList = []
-
     # Even / odd functionality
     evenOddCapable = False
     outputSetEven = None
     outputSetOdd = None
 
     # -------------------------- DEFINE param functions -----------------------
-    def _defineParams(self, form, addEvenOddParam=True):
+    def _defineParams(self, form, addEvenOddParam = True):
         form.addSection(label=Message.LABEL_INPUT)
 
         form.addParam('inputTiltSeriesM', params.PointerParam,
                       pointerClass='SetOfTiltSeriesM',
                       important=True,
                       label='Input Tilt-Series (movies)',
                       help='Select input tilt-series movies that you want'
@@ -163,129 +159,121 @@
             args = '--img %s ' % abspath(alignedFrameStack)
             args += '--type frames '
             args += '-o %s ' % (evenName + '.xmd')
             args += '-e %s ' % (oddName + '.xmd')
             args += '--sum_frames '
             self.runJob('xmipp_image_odd_even', args)
 
-            # Store the corresponding tsImM to use its data later in the even/odd TS
-            self.tsMList.append(tiltImageM)
-
             # Update even and odd average lists
-            self.evenAvgFrameList.append(evenName + '_aligned.mrc')
-            self.oddAvgFrameList.append(oddName + '_aligned.mrc')
+            oddfn = oddName + '_aligned.mrc'
+            evenfn = evenName + '_aligned.mrc'
 
+            tiltImageM.setOddEven([oddfn, evenfn])
             pw.utils.cleanPath(alignedFrameStack)
 
         tiFn, tiFnDW = self._getOutputTiltImagePaths(tiltImageM)
         if not os.path.exists(tiFn):
             raise Exception("Expected output file '%s' not produced!" % tiFn)
 
         if not pw.utils.envVarOn('SCIPION_DEBUG_NOCLEAN'):
             pw.utils.cleanPath(workingFolder)
 
-    def processTiltSeriesStep(self, tsId):
-        """ Create a single stack with the tiltseries. """
-
-        def addTiltImage(tiFile, tsObject, suffix, tsMov, tsIde, samplingRate, objId, index):
+    def createOddEvenTs(self, ts, odd=True):
+        def addTiltImage(tiLocation, tsObject, mainti, tsIde, samplingRate):
             """
-            :param tiFile: aligned tilt image file
+            :param tiLocation: Location of the aligned tilt image in the stack
             :param tsObject: Tilt Series to which the new Ti Image will be added
-            :param suffix: used for the location. Admitted values are even or odd
-            :param tsMov: Tilt Series Movies object
+            :param mainti: Tilt Series Movies object
             :param tsIde: Tilt series identifier
             :param samplingRate: current Tilt Series sampling rate
-            :param objId: location of the Tilt Image which will be added
-            :param index: position of the slice in the generated slack
             """
-            ta = tsMov.getTiltAngle()
-            to = tsMov.getAcquisitionOrder()
-            acq = tsMov.getAcquisition()
+            ta = mainti.getTiltAngle()
+            to = mainti.getAcquisitionOrder()
+            acq = mainti.getAcquisition()
             ti = TiltImage(tiltAngle=ta, tsId=tsIde, acquisitionOrder=to)
             ti.setSamplingRate(samplingRate)
-            ti.setIndex(index)
             ti.setAcquisition(acq)
-            newLocation = (objId, self._getExtraPath(tsIde + '_' + suffix + '.mrcs'))
-            ih.convert(tiFile, newLocation)
-            ti.setLocation(newLocation)
+            index, fname = tiLocation.split("@")
+            ti.setLocation(int(index), fname)
             tsObject.append(ti)
-            pw.utils.cleanPath(tiFile)
+            pw.utils.cleanPath(tiLocation)
+
+        if odd:
+            suffix = ODD
+            outputAttr = 'outputSetOdd'
+            oddEvenIndex = 0
+        else:
+            suffix = EVEN
+            outputAttr = 'outputSetEven'
+            oddEvenIndex = 1
+
+        template = 'tiltseries%s.sqlite'
+        sRate = self._getOutputSampling()
+
+        output = getattr(self, outputAttr)
+        if output:
+            output.enableAppend()
+        else:
+            output = SetOfTiltSeries.create(self._getPath(), template=template, suffix=suffix)
+            setattr(self, outputAttr, output)
+            output.setSamplingRate(sRate)
+
+        tsObj = TiltSeries()
+        tsObj.copyInfo(ts, copyId=True)
+        output.append(tsObj)
+
+        tsId = ts.getTsId()
+        for ti in ts:
+            fnImg = ti.getOddEven()[oddEvenIndex]
+            addTiltImage(fnImg, tsObj, ti, tsId, sRate)
+
+        # update items and size info
+        output.update(tsObj)
+
+    def processTiltSeriesStep(self, tsId):
+        """ Create a single stack with the tiltseries. """
+        def createStack(tiList, tsFn, fngetter, locationSetter=None):
+            """ This function creates a stack from individual images """
+            for i, ti in enumerate(tiList):
+                tiFn = fngetter(ti)
+                #newLocation = (i + 1, tsFn)
+                #ih.convert(tiFn, newLocation)
+                #pw.utils.cleanPath(tiFn)
+                if os.path.exists(tiFn):
+                    newLocation = (i + 1, tsFn)
+                    ih.convert(tiFn, newLocation)
+                    pw.utils.cleanPath(tiFn)
+                if locationSetter:
+                    locationSetter(newLocation, ti)
 
         ts = self._tsDict.getTs(tsId)
         ts.setDim([])
 
         tiList = self._tsDict.getTiList(tsId)
         tiList.sort(key=lambda ti: ti.getTiltAngle())
 
         ih = ImageHandler()
 
         tsFn = self._getOutputTiltSeriesPath(ts)
         tsFnDW = self._getOutputTiltSeriesPath(ts, '_DW')
 
         # Merge all micrographs from the same tilt images in a single "mrcs" stack file
-        for i, ti in enumerate(tiList):
-            tiFn, tiFnDW = self._getOutputTiltImagePaths(ti)
-            if os.path.exists(tiFn):
-                newLocation = (i+1, tsFn)
-                ih.convert(tiFn, newLocation)
-                ti.setLocation(newLocation)
-                pw.utils.cleanPath(tiFn)
-            if os.path.exists(tiFnDW):
-                ih.convert(tiFnDW, (i+1, tsFnDW))
-                pw.utils.cleanPath(tiFnDW)
-
-        self._tsDict.setFinished(tsId)
+        createStack(tiList, tsFn, self._getOutputTiltImagePath, locationSetter=lambda newloc, ti: ti.setLocation(newloc))
+        if self._createOutputWeightedTS():
+            createStack(tiList, tsFnDW, self._getOutputTiltImageDWPath)
 
-        # Even and odd stuff
         if self._doSplitEvenOdd():
-            template = 'tiltseries%s.sqlite'
-            sRate = self._getOutputSampling()
-            # Even
-            if self.outputSetEven:
-                self.outputSetEven.enableAppend()
-            else:
-                self.outputSetEven = SetOfTiltSeries.create(self._getPath(), template=template, suffix=EVEN)
-                self.outputSetEven.setSamplingRate(sRate)
-            # Odd
-            if self.outputSetOdd:
-                self.outputSetOdd.enableAppend()
-            else:
-                self.outputSetOdd = SetOfTiltSeries.create(self._getPath(), template=template, suffix=ODD)
-                self.outputSetOdd.setSamplingRate(sRate)
-
-            tsObjEven = TiltSeries()
-            tsObjOdd = TiltSeries()
-            tsObjEven.copyInfo(ts, copyId=True)
-            tsObjOdd.copyInfo(ts, copyId=True)
-            self.outputSetEven.append(tsObjEven)
-            self.outputSetOdd.append(tsObjOdd)
-
-            # Merge all micrographs from the same tilt images in a sorted-by-tilt single "mrcs" stack file,
-            ind = np.argsort([ti.getTiltAngle() for ti in self.tsMList])
-            counter = 1
-            # for fileEven, fileOdd, tsImM in zip(self.evenAvgFrameList, self.oddAvgFrameList, self.tsMList):
-            for i in ind:
-                tiEvenFile = self.evenAvgFrameList[i]
-                tiOddFile = self.oddAvgFrameList[i]
-                tsM = self.tsMList[i]
-                # Even
-                addTiltImage(tiEvenFile, tsObjEven, EVEN, tsM, tsId, sRate, counter, counter)
-                # Odd
-                addTiltImage(tiOddFile, tsObjOdd, ODD, tsM, tsId, sRate, counter, counter)
+            tsFnOdd = self._getOutputTiltSeriesPath(ts, '_odd')
+            tsFnEven = self._getOutputTiltSeriesPath(ts, '_even')
+            createStack(tiList, tsFnOdd, self._getOutputTiltImageOddPath,
+                        locationSetter=lambda newloc, ti: ti.setOdd(ih.locationToXmipp(newloc)))
+            createStack(tiList, tsFnEven, self._getOutputTiltImageEvenPath,
+                        locationSetter=lambda newloc, ti: ti.setEven(ih.locationToXmipp(newloc)))
 
-                counter += 1
-
-            # update items and size info
-            self.outputSetEven.update(tsObjEven)
-            self.outputSetOdd.update(tsObjOdd)
-
-            # Empty lists for next iteration
-            self.evenAvgFrameList = []
-            self.oddAvgFrameList = []
-            self.tsMList = []
+        self._tsDict.setFinished(tsId)
 
         # Dose weighting
         if self._createOutputWeightedTS():
             if getattr(self, 'outputSetDW', None) is None:
                 self.outputSetDW = self._createOutputSet(suffix='_dose-weighted')
                 self.outputSetDW.setSamplingRate(self._getOutputSampling())
             else:
@@ -301,39 +289,24 @@
                 tiOut.setAcquisition(ti.getAcquisition())
                 tiOut.setSamplingRate(self._getOutputSampling())
                 tiOut.setObjId(ti.getIndex())
                 tsObjDW.append(tiOut)
 
             self.outputSetDW.update(tsObjDW)
 
-    def createOutputStep(self):
-        """" Overwrites the parent method to allow the creation of odd and even outputs"""
-        ProtTsProcess.createOutputStep(self)
-
-        if self._doSplitEvenOdd():
-            # Even
-            self.outputSetEven.setStreamState(self.outputSetEven.STREAM_CLOSED)
-            self.outputSetEven.write()
-            self._store(self.outputSetEven)
-            # Odd
-            self.outputSetOdd.setStreamState(self.outputSetOdd.STREAM_CLOSED)
-            self.outputSetOdd.write()
-            self._store(self.outputSetOdd)
-
-        if self._createOutputWeightedTS():
-            self.outputSetDW.setStreamState(self.outputSetDW.STREAM_CLOSED)
-            self.outputSetDW.write()
-            self._store(self.outputSetDW)
-
     def _updateOutput(self, tsIdList):
         """ Update the output set with the finished Tilt-series.
         Params:
             :param tsIdList: list of ids of finished tasks.
         """
 
+        def writeAndStore(obj):
+            obj.write()
+            self._store(obj)
+
         # Flag to check the first time we save output
         self._createOutput = getattr(self, '_createOutput', True)
 
         outputSet = self._getOutputSet()
 
         if outputSet is None:
             # Special case just to update the outputSet status
@@ -378,24 +351,20 @@
 
             if self._createOutputWeightedTS():
                 self._defineSourceRelation(self._getInputTsPointer(), self.outputSetDW)
 
             self._defineSourceRelation(self._getInputTsPointer(), outputSet)
             self._createOutput = False
         else:
-            outputSet.write()
-            self._store(outputSet)
+            writeAndStore(outputSet)
             if self._doSplitEvenOdd():
-                self.outputSetEven.write()
-                self._store(self.outputSetEven)
-                self.outputSetOdd.write()
-                self._store(self.outputSetOdd)
+                writeAndStore(self.outputSetEven)
+                writeAndStore(self.outputSetOdd)
             if self._createOutputWeightedTS():
-                self.outputSetDW.write()
-                self._store(self.outputSetDW)
+                writeAndStore(self.outputSetDW)
 
         outputSet.close()
         if self._doSplitEvenOdd():
             self.outputSetEven.close()
             self.outputSetOdd.close()
 
         if self._createOutputWeightedTS():
@@ -411,28 +380,34 @@
             ts = TiltSeries()
             ts.copyInfo(self._tsDict.getTs(tsId), copyId=True)
             ts.setSamplingRate(self._getOutputSampling())
             outputSet.append(ts)
             tList = self._tsDict.getTiList(tsId)
             ind = np.argsort([ti.getTiltAngle() for ti in tList])
             counter = 1
+
             for i in ind:  # Make each row of the sqlite file be sorted by
                 # index after having been sorted by angle previously, in order to avoid tilt image mismatching in
                 # another operations, such as the fiducial alignment, which expects the sqlite to be sorted that way
                 ti = tList[i]
                 tiOut = TiltImage(location=(counter, ti.getFileName()))
                 tiOut.copyInfo(ti, copyId=True)
                 tiOut.setAcquisition(ti.getAcquisition())
                 tiOut.setSamplingRate(self._getOutputSampling())
                 tiOut.setObjId(ti.getIndex())
                 ts.append(tiOut)
                 counter += 1
 
             outputSet.update(ts)
 
+            # Even and odd stuff
+            if self._doSplitEvenOdd():
+                self.createOddEvenTs(ts, True)
+                self.createOddEvenTs(ts, False)
+
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
         return errors
 
     def _summary(self):
         return [self.summaryVar.get('')]
@@ -500,16 +475,35 @@
 
     def __getTiltImageMWorkingFolder(self, tiltImageM):
         return self._getTmpPath(self._getTiltImageMRoot(tiltImageM))
 
     def _getOutputTiltImagePaths(self, tiltImageM):
         """ Return expected output path for correct movie and DW one.
         """
-        base = self._getExtraPath(self._getTiltImageMRoot(tiltImageM))
-        return base + '.mrc', base + '_DW.mrc'
+        return self._getOutputTiltImagePath(tiltImageM), self._getOutputTiltImageDWPath(tiltImageM)
+
+    def _getOutputTiltImagePath(self, tiltImageM):
+        """ Return the main path for the tilt image corrected movie.
+        """
+        return self._getExtraPath(self._getTiltImageMRoot(tiltImageM)) + '.mrc'
+
+    def _getOutputTiltImageDWPath(self, tiltImageM):
+        """ Return the main path for the tilt image dose weighted corrected movie.
+        """
+        return self._getExtraPath(self._getTiltImageMRoot(tiltImageM)) + '_DW.mrc'
+
+    def _getOutputTiltImageOddPath(self, tiltImageM):
+        """ Return the path for the odd tilt image corrected movie.
+        """
+        return tiltImageM.getOdd()
+
+    def _getOutputTiltImageEvenPath(self, tiltImageM):
+        """ Return the path for the even tilt image corrected movie.
+        """
+        return tiltImageM.getEven()
 
     def _getOutputTiltSeriesPath(self, ts, suffix=''):
         return self._getExtraPath('%s%s.mrcs' % (ts.getTsId(), suffix))
 
     def _useAlignToSum(self):
         return True
```

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_estimate_ctf.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_import.py` & `scipion-em-tomo-3.1.9/tomo/protocols/protocol_ts_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/protocols.conf` & `scipion-em-tomo-3.1.9/tomo/protocols.conf`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 	]},
 	{"tag": "section", "text": "Tilt-series movies", "children": [
 	    {"tag": "protocol", "value": "ProtTsAverage",      "text": "default"}
 	]},
 	{"tag": "section", "text": "Tilt-series", "children": [
 		{"tag": "protocol_group", "text": "Tilt-series preprocess", "openItem": "False", "children": []},
 	    {"tag": "protocol_group", "text": "CTF", "openItem": "False", "children": [
-	        {"tag": "protocol", "value": "ProtRotateAstigmatism", "text": "default"}
+	        {"tag": "protocol", "value": "ProtRotateAstigmatism", "text": "default"},
+	        {"tag": "protocol", "value": "ProtCTFTomoSeriesConsensus", "text": "default"}
 	    ]},
 		{"tag": "protocol_group", "text": "Alignment", "openItem": "False", "children": []},
 		{"tag": "protocol", "value": "ProtConsensusAlignmentTS", "text": "tomo - alignment consensus"},
 		{"tag": "protocol_group", "text": "Coordinates", "openItem": "False", "children": [
 		    {"tag": "protocol", "value": "ProtTsConvertCoordinates3d", "text": "tomo - Convert TS coordinates to 3D"}
 		]}
 	]},
```

### Comparing `scipion-em-tomo-3.1.8/tomo/templates/HIV-Picking-with-Dynamo.json.template` & `scipion-em-tomo-3.1.9/tomo/templates/HIV-Picking-with-Dynamo.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/templates/HIV-Reconstruction.json.template` & `scipion-em-tomo-3.1.9/tomo/templates/HIV-Reconstruction.json.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Reconstruction of HIV EMPIAR10164. INSTRUCTIONS: Download tilt series 01, 03 and 54 with their mdoc in the same folder.
 [
     {
         "object.className": "ProtImportTsMovies",
         "object.id": "8340",
         "object.label": "tomo - import tilt-series movies",
-        "object.comment": "HOW TH GET THE DATA: Download the movies for 01, 03 and 54 tilt series. Place its mdoc files in the same folder where the movies are."
+        "object.comment": "HOW TO GET THE DATA: Download the movies for 01, 03 and 54 tilt series. Place its mdoc files in the same folder where the movies are.",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "filesPath": "~EMPIAR-10164 mdocs folder|/home/scipion/data/Day1_HIV/frames/|2|pathtomdocs~",
         "filesPattern": "*.mdoc",
```

### Comparing `scipion-em-tomo-3.1.8/tomo/templates/HIV-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.9/tomo/templates/HIV-Subtomogram-averaging.json.template`

 * *Files 2% similar despite different names*

```diff
@@ -210,34 +210,34 @@
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "useGpu": true,
         "gpuList": "0",
         "numberOfIters": "2 2 2",
-        "dim": "0",
+        "dim": "48",
         "useDynamoGui": false,
-        "cr": "60 30 10",
-        "cs": "10 5 2",
+        "cr": "12 6 4",
+        "cs": "6 3 2",
         "cf": "0",
-        "inplane_range": "45 15 4",
-        "inplane_sampling": "5 3 2",
+        "inplane_range": "60 30 4",
+        "inplane_sampling": "6 6 2",
         "inplane_flip": "0",
-        "rf": "5",
+        "rf": "0",
         "rff": "2 ",
-        "lim": "24 8 4",
-        "limm": "1 2 2",
-        "separation": 0,
-        "threshold": "0.2",
-        "thresholdMode": "0",
+        "lim": "8",
+        "limm": "1",
+        "separation": 2,
+        "threshold": "0.5",
+        "thresholdMode": "5",
         "threshold2": "0.2",
         "thresholdMode2": "0",
         "high": "2",
-        "low": "32",
-        "sym": "c6 c6 c6",
+        "low": "12",
+        "sym": "c1",
         "ccmatrixBatch": 128,
         "hostName": "localhost",
         "numberOfThreads": 4,
         "inputVolumes": "2160.subtomograms",
         "templateRef": "2262.average"
     },
     {
@@ -427,63 +427,14 @@
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "maskPath": "~Path to Bin4 mask|%(SCIPION_TESTS)s/relion40_sta_tutorial_data/masks/mask_align_bin4.mrc|2|maskb4~",
         "samplingRate": 5.4
     },
     {
-        "object.className": "ProtRelion3DClassifySubtomograms",
-        "object.id": "924",
-        "object.label": "reliontomo - 3D Classification of subtomograms (copy)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "isMapAbsoluteGreyScale": true,
-        "initialLowPassFilterA": 40.0,
-        "symmetry": "C6",
-        "doCTF": true,
-        "ignoreCTFUntilFirstPeak": false,
-        "numberOfClasses": 1,
-        "regularisation": 4.0,
-        "nIterations": 3,
-        "useFastSubsets": false,
-        "maskDiameter": 230,
-        "zeroMask": true,
-        "limitResolutionEStepTo": -1.0,
-        "doImageAlignment": true,
-        "angularSamplingDeg": 2,
-        "offsetSearchRangePix": 5,
-        "offsetSearchStepPix": 1.0,
-        "doLocalAngleSearch": false,
-        "localAngularSearchRange": 5.0,
-        "relaxSym": null,
-        "allowCoarser": false,
-        "parallelDiscIO": true,
-        "pooledSubtomos": 16,
-        "skipGridding": true,
-        "allParticlesRam": false,
-        "combineItersDisc": false,
-        "scratchDir": null,
-        "skipPadding": false,
-        "doGpu": true,
-        "gpusToUse": "0",
-        "keepOnlyLastIterFiles": false,
-        "oversampling": 1,
-        "extraParams": "--sigma_tilt 3.667 --sigma_psi 3.667",
-        "hostName": "localhost",
-        "numberOfThreads": 1,
-        "numberOfMpi": 3,
-        "inReParticles": "717.relionParticles",
-        "referenceVolume": "802.average",
-        "solventMask": "841.outputMask"
-    },
-    {
         "object.className": "ProtImportMask",
         "object.id": "994",
         "object.label": "pwem - Bin2_import mask",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
@@ -506,15 +457,15 @@
         "numberOfThreads": 12,
         "numberOfMpi": 5,
         "boxSize": 256,
         "croppedBoxSize": 128,
         "binningFactor": 2.0,
         "symmetry": "C6",
         "snrWiener": 0.0,
-        "inReParticles": "924.relionParticles"
+        "inReParticles": "717.relionParticles"
     },
     {
         "object.className": "ProtRelionMakePseudoSubtomograms",
         "object.id": "1155",
         "object.label": "reliontomo - Make pseudo-subtomograms (2)",
         "object.comment": "",
         "_useQueue": false,
@@ -528,15 +479,15 @@
         "boxSize": 256,
         "croppedBoxSize": 128,
         "binningFactor": 2.0,
         "applyConeWeight": false,
         "coneAngle": 10.0,
         "applyOffsets": false,
         "outputInFloat16": false,
-        "inReParticles": "924.relionParticles"
+        "inReParticles": "717.relionParticles"
     },
     {
         "object.className": "ProtRelion3DClassifySubtomograms",
         "object.id": "1343",
         "object.label": "reliontomo - 3D Classification of subtomograms (copy 2)",
         "object.comment": "",
         "_useQueue": false,
@@ -581,28 +532,27 @@
         "numberOfMpi": 3,
         "solventMask": "994.outputMask",
         "referenceVolume": "1116.average",
         "inReParticles": "1155.relionParticles"
     },
     {
         "object.className": "XmippProtSubtomoMapBack",
-        "object.id": "1461",
+        "object.id": "9071",
         "object.label": "xmipptomo - map back subtomos",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "selection": 1,
+        "selection": 0,
         "invertContrast": false,
         "paintingType": 2,
         "removeBackground": true,
         "threshold": 0.5,
         "constant": 100000.0,
         "hostName": "localhost",
         "numberOfThreads": 1,
-        "numberOfMpi": 1,
-        "inputSubtomos": "227.coordinates",
-        "inputRef": "1116.average"
+        "numberOfMpi": 3,
+        "inputClasses": "1343.classes"
     }
 ]
```

### Comparing `scipion-em-tomo-3.1.8/tomo/templates/Membrane picking-with-PySeg.json.template` & `scipion-em-tomo-3.1.9/tomo/templates/Membrane picking-with-PySeg.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/templates/Ribosomes-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.9/tomo/templates/Ribosomes-Subtomogram-averaging.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/__init__.py` & `scipion-em-tomo-3.1.9/tomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_base_centralized_layer.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_base_centralized_layer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_compose_TS.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_compose_TS.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 
         # ComposeTS
         protCompose = self.newProtocol(ProtComposeTS,
                                        objLabel='ComposeTS',
                                        inputMicrographs=protAlign.outputMicrographs,
                                        filesPath=self.partFolderPath,
                                        time4NextTilt=20,
-                                       time4NextMic=12,
                                        time4NextTS=30)
         # self.proj.scheduleProtocol(protCompose)
         # checkOutputs(protCompose, 20)#timeout
         self.launchProtocol(protCompose)
         self.assertIsNotNone(protCompose.TiltSeries, 'TiltSeries not composed')
 
         # xcor prealignment
```

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_fit_vesicles.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_fit_vesicles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_import.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_objects.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_tomo_base.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_tomo_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/tests/test_transformations.py` & `scipion-em-tomo-3.1.9/tomo/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/utils.py` & `scipion-em-tomo-3.1.9/tomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/viewers/__init__.py` & `scipion-em-tomo-3.1.9/tomo/viewers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .viewers_data import (TomoDataViewer, TSMotionCorrectionViewer,
                            CtfEstimationTomoViewer)
 from .viewer_split_evenodd import SplitEvenOddViewer
+from .viewer_ctf_tomo_consensus import CtfConsensusTomoViewer
```

### Comparing `scipion-em-tomo-3.1.8/tomo/viewers/viewer_split_evenodd.py` & `scipion-em-tomo-3.1.9/tomo/viewers/viewer_split_evenodd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/viewers/viewers_data.py` & `scipion-em-tomo-3.1.9/tomo/viewers/viewers_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,14 +185,18 @@
         """ To be implemented in the viewers. """
         return None
 
     def plot2D(self, ctfSet, ctfId):
         """ To be implemented in the viewers. """
         return None
 
+    def plotExtra(self, ctfSet, ctfId):
+        """ To be implemented in the viewers. """
+        return None
+
     def visualize(self, obj, windows=None, protocol=None):
         if not isinstance(obj, EMProtocol):
             self.visualizeSet(obj)
         else:
             for name, output in self._protocol._iterOutputsNew():
                 if isinstance(output, tomo.objects.SetOfCTFTomoSeries):
                     self.visualizeSet(output)
@@ -205,28 +209,35 @@
         self._provider = CtfEstimationTreeProvider(self._tkParent,
                                                    self._protocol,
                                                    obj)
 
         CtfEstimationListDialog(self._tkParent, self._title, self._provider,
                                 self._protocol, self._inputSetOfTiltSeries,
                                 plot1Dfunc=self.getPlot1DCallback(),
-                                plot2Dfunc=self.getPlot2DCallback())
+                                plot2Dfunc=self.getPlot2DCallback(),
+                                plotExtrafunc=self.getPlotExtraCallback())
 
     def getPlot1DCallback(self):
         if not pwutils.isSameFunction(self.plot1D,
                                       CtfEstimationTomoViewer.plot1D):
             return self.plot1D
         return None
 
     def getPlot2DCallback(self):
         if not pwutils.isSameFunction(self.plot2D,
                                       CtfEstimationTomoViewer.plot2D):
             return self.plot2D
         return None
 
+    def getPlotExtraCallback(self):
+        if not pwutils.isSameFunction(self.plotExtra,
+                                      CtfEstimationTomoViewer.plotExtra):
+            return self.plotExtra
+        return None
+
 
 # Register specific sets in pwem dataviewer.
 DataViewer.registerConfig(tomo.objects.SetOfSubTomograms,
                           config={MODE: MODE_MD,
                                   VISIBLE: 'id _filename _volName _coordinate._x _coordinate._y _coordinate._z '
                                            '_transform._matrix '})
```

### Comparing `scipion-em-tomo-3.1.8/tomo/viewers/views.py` & `scipion-em-tomo-3.1.9/tomo/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.8/tomo/viewers/views_tkinter_tree.py` & `scipion-em-tomo-3.1.9/tomo/viewers/views_tkinter_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -817,14 +817,15 @@
         self._project = protocol.getProject()
         self._protocol = protocol
         self._inputSetOfTiltSeries = inputTS
         self._checkedItems = provider._checkedItems
         # the funcs below should be implemented in viewers
         self._show1DPLot = kwargs.pop('plot1Dfunc', None)
         self._show2DPLot = kwargs.pop('plot2Dfunc', None)
+        self._showExtraPlot = kwargs.pop('plotExtrafunc', None)
         ListDialog.__init__(self, parent, title, provider, allowSelect=False,
                             cancelButton=True, **kwargs)
 
     def body(self, bodyFrame):
         bodyFrame.config()
         self._col = 1
         self._fillCTFEstimationGUI(bodyFrame)
@@ -852,14 +853,16 @@
     def _createTopPanel(self, topPanel):
         self._createFilterBox(topPanel)
         topRigthPanel = tk.Frame(topPanel)
         topRigthPanel.grid(row=0, column=1, padx=0, pady=0, sticky='news')
         self._createSubsetButton(topRigthPanel)
         if self._show1DPLot is not None:
             self._createShowFit(topRigthPanel)
+        if self._showExtraPlot is not None:
+            self._createShowExtra(topRigthPanel)
         self._createViewerHelp(topRigthPanel)
 
     def _createSubsetButton(self, topRigthPanel):
         state = tk.NORMAL
         if self._checkedItems or self._checkedItems == len(self.provider.getCTFSeries()):
             state = tk.DISABLED
         self.generateSubsetButton = self._addButton(topRigthPanel,
@@ -888,14 +891,34 @@
                     if ctfSerie.getTsId() in itemSelected:
                         # TODO: sort ctfSerie by id
                         ctfId = int(itemSelected.split('.')[-1])
                         plot = self._show1DPLot(ctfSerie, ctfId)
                         plot.show()
                         break
 
+    def _createShowExtra(self, topRigthPanel):
+        self.createShowFitButton = self._addButton(topRigthPanel, 'Extra plots',
+                                                   pwutils.Icon.ACTION_RESULTS, self._showExtra,
+                                                   state=tk.DISABLED,
+                                                   sticky='ne')
+
+    def _showExtra(self, event=None):
+        itemSelected = self.tree.getSelectedItem()
+        obj = self.tree.getSelectedObj()
+        if self.tree.parent(itemSelected):  # child item
+            if obj is not None:
+                for ctfSerie in self.provider.getCTFSeries():
+                    if ctfSerie.getTsId() in itemSelected:
+                        # TODO: sort ctfSerie by id
+                        ctfId = int(itemSelected.split('.')[-1])
+                        plot = self._showExtraPlot(ctfSerie, ctfId)
+                        plot.show()
+                        break
+
+
     def _actionCreateSets(self, event=None):
         if self.generateSubsetButton['state'] == tk.NORMAL:
             protocol = self.provider.protocol
             ctfSeries = self.provider.getCTFSeries()
             suffix = self._getSuffix(protocol)
             goodCTFName = 'goodCtf%s' % suffix
             badCTFName = 'badCtf%s' % suffix
@@ -1083,13 +1106,18 @@
         else:
             self.generateSubsetButton['state'] = tk.DISABLED
 
         if obj is not None:
             if self.tree.parent(itemSelected):  # child item
                 if self._show1DPLot is not None:
                     self.createShowFitButton['state'] = tk.NORMAL
+                if self._showExtraPlot is not None:
+                    self.createShowFitButton['state'] = tk.NORMAL
                 self.plotterChildItem(itemSelected)
 
             else:  # parent item
                 if self._show1DPLot is not None:
                     self.createShowFitButton['state'] = tk.DISABLED
+                if self._showExtraPlot is not None:
+                    self.createShowFitButton['state'] = tk.DISABLED
+
                 self.plotterParentItem(itemSelected)
```

### Comparing `scipion-em-tomo-3.1.8/tomo/wizards.py` & `scipion-em-tomo-3.1.9/tomo/wizards.py`

 * *Files identical despite different names*

