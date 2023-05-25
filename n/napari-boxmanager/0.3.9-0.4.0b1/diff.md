# Comparing `tmp/napari_boxmanager-0.3.9.tar.gz` & `tmp/napari_boxmanager-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_boxmanager-0.3.9.tar", last modified: Fri Feb 17 15:40:24 2023, max compression
+gzip compressed data, was "napari_boxmanager-0.4.0b1.tar", last modified: Thu May 25 06:49:11 2023, max compression
```

## Comparing `napari_boxmanager-0.3.9.tar` & `napari_boxmanager-0.4.0b1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.501256 napari_boxmanager-0.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/bin/napari_boxmanager
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/_static/version-alert.js
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/general.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/manual.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/read.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/write.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/reader_backup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/reader_backup/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_tlpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/tepkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/tlpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/tmpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/to_napari_backup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.501256 napari_boxmanager-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/src/box_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/FilterImage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    82644 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/SelectMetric.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_black.png
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/_dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/box_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/tif.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/tloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.521256 napari_boxmanager-0.3.9/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_0_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_center_float.box
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_corrupt_has_string.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_corrupt_unqual_columns.box
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_empty.box
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_left.box
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_particles.cbox
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/3d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/3d.mrci
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/3d_particle.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/box_data/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/create_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_0.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_0_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2_new.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_3.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_4.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_4.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_4_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_5.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_5.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_6.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_6.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_6_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_7.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_7_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_7_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_8.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_8.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_8_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_9.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_9.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_9_new.box
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_02885.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03047.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03070.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03211.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_04203.cbox
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/empty.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/particle_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/valid_box/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_box/2d.box
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_box/2d_0.box
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_missing_dim_z.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/valid_mrc/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_mrc/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_mrc/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.498072 napari_boxmanager-0.4.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.450072 napari_boxmanager-0.4.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.454072 napari_boxmanager-0.4.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.454072 napari_boxmanager-0.4.0b1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-25 06:49:11.498072 napari_boxmanager-0.4.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.454072 napari_boxmanager-0.4.0b1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/bin/napari_boxmanager
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.458072 napari_boxmanager-0.4.0b1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.458072 napari_boxmanager-0.4.0b1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/_static/version-alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.458072 napari_boxmanager-0.4.0b1/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/manual/general.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/manual/manual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/manual/read.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/manual/write.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.458072 napari_boxmanager-0.4.0b1/reader_backup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.458072 napari_boxmanager-0.4.0b1/reader_backup/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/_tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/_tests/test_tlpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/tepkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/tlpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/tmpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/reader_backup/to_napari_backup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-25 06:49:11.498072 napari_boxmanager-0.4.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.450072 napari_boxmanager-0.4.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.462072 napari_boxmanager-0.4.0b1/src/box_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.462072 napari_boxmanager-0.4.0b1/src/box_manager/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/FilterImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/OrganizeBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/OrganizeLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83497 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/SelectMetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.462072 napari_boxmanager-0.4.0b1/src/box_manager/_qt/_icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/_icons/checkmark_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_qt/_icons/checkmark_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.466072 napari_boxmanager-0.4.0b1/src/box_manager/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/_dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.466072 napari_boxmanager-0.4.0b1/src/box_manager/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_utils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/box_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.466072 napari_boxmanager-0.4.0b1/src/box_manager/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/io/tloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/src/box_manager/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.470072 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 06:49:11.000000 napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.482072 napari_boxmanager-0.4.0b1/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_0_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_center_float.box
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_corrupt_has_string.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_corrupt_unqual_columns.box
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_empty.box
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_left.box
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/2d_particles.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/3d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/3d.mrci
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/3d_particle.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.490072 napari_boxmanager-0.4.0b1/test_data/box_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_0_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_1.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_1.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_1_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_1_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_2.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_2.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_2_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_2_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_3.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_4.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_4.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_4_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_5.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_5.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_6.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_6.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_6_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_7.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_7_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_7_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_8.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_8.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_8_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_9.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_9.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/box_data/test_9_new.box
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.494072 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_02885.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_03047.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_03070.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_03211.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_04203.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/empty.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.494072 napari_boxmanager-0.4.0b1/test_data/particle_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/valid.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.494072 napari_boxmanager-0.4.0b1/test_data/valid_box/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/valid_box/2d.box
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/valid_box/2d_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/valid_missing_dim_z.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:49:11.494072 napari_boxmanager-0.4.0b1/test_data/valid_mrc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/valid_mrc/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/test_data/valid_mrc/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-25 06:48:51.000000 napari_boxmanager-0.4.0b1/tox.ini
```

### Comparing `napari_boxmanager-0.3.9/.github/workflows/test_and_deploy.yml` & `napari_boxmanager-0.4.0b1/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This workflows will upload a Python Package using Twine when a release is created
 # For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
 
 name: tests
-
 on:
   push:
     branches:
       - main
       - npe2
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
@@ -23,15 +22,14 @@
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.10']
 
     steps:
       - uses: actions/checkout@v2
-
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       # these libraries enable testing on Qt on linux
       - uses: tlambert03/setup-qt-libs@v1
```

### Comparing `napari_boxmanager-0.3.9/.gitignore` & `napari_boxmanager-0.4.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/.napari/DESCRIPTION.md` & `napari_boxmanager-0.4.0b1/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/.pre-commit-config.yaml` & `napari_boxmanager-0.4.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/LICENSE` & `napari_boxmanager-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/PKG-INFO` & `napari_boxmanager-0.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_boxmanager
-Version: 0.3.9
+Version: 0.4.0b1
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.3.9/README.md` & `napari_boxmanager-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/docs/_static/version-alert.js` & `napari_boxmanager-0.4.0b1/docs/_static/version-alert.js`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/docs/conf.py` & `napari_boxmanager-0.4.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/docs/manual/general.rst` & `napari_boxmanager-0.4.0b1/docs/manual/general.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/reader_backup/_tests/test_box.py` & `napari_boxmanager-0.4.0b1/reader_backup/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/reader_backup/_tests/test_interface.py` & `napari_boxmanager-0.4.0b1/reader_backup/_tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/reader_backup/_tests/test_tlpkl.py` & `napari_boxmanager-0.4.0b1/reader_backup/_tests/test_tlpkl.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/reader_backup/tlpkl.py` & `napari_boxmanager-0.4.0b1/reader_backup/tlpkl.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/reader_backup/to_napari_backup.txt` & `napari_boxmanager-0.4.0b1/reader_backup/to_napari_backup.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/setup.cfg` & `napari_boxmanager-0.4.0b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 	Topic :: Software Development :: Testing
 
 [options]
 packages = find:
 install_requires = 
 	matplotlib
 	mrcfile
-	numpy ==1.23.5
+	numpy <=1.23.5
 	pandas
-	pystardb
+	pystardb>=0.4.2
 python_requires = >=3.10
 include_package_data = True
 package_dir = 
 	=src
 scripts = 
 	bin/napari_boxmanager
 setup_requires =
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_qt/FilterImage.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_qt/FilterImage.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeBox.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_qt/OrganizeBox.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from copy import deepcopy
 from .._utils import general
 import napari.layers
 import numpy as np
 from napari.layers.base.base import Layer
 from napari.utils.events.event import Event
 from napari.utils.notifications import show_error, show_info
+from napari.layers.shapes._shapes_constants import Mode
 from qtpy.QtCore import Qt, Signal, Slot
 from qtpy.QtWidgets import (
     QComboBox,
     QFormLayout,
     QLineEdit,
     QPushButton,
     QTableWidget,
@@ -245,15 +246,14 @@
             for idx, value in layer_coord.metadata.items()
             if isinstance(idx, int) and "path" in value
         }
 
         old_data, old_state, old_type_str = layer_coord.as_layer_data_tuple()
         new_data = deepcopy(old_data)
         ident_data = general.get_identifier(layer_coord, 0)
-
         new_meta = {
             key: value
             for key, value in layer_coord.metadata.items()
             if not isinstance(key, int)
         }
         new_meta["prefix"] = prefix_coord
         new_meta["suffix"] = suffix_coord
@@ -293,15 +293,22 @@
                     new_coord_name = new_meta[image_idx]["name"]
                 else:
                     new_coord_name = "-"
             table_list.append((mic_name, box_name, new_coord_name))
 
             slice_mask = np.round(ident_data, 0) == coord_idx
             total_mask = total_mask | slice_mask
-            new_data[slice_mask, 0] = image_idx
+            try:
+                # new data is an numpy array
+                new_data[slice_mask, 0] = image_idx
+            except TypeError:
+                # In this case it is shape layer and new_data is list of arrays
+                for slice_index, do_change in enumerate(slice_mask):
+                    if do_change:
+                        new_data[slice_index][:,0] = image_idx
 
         try:
             new_data = new_data[total_mask, :]
         except TypeError:
             new_data = [
                 entry for entry, keep in zip(new_data, total_mask) if keep
             ]
@@ -346,22 +353,30 @@
                         new_state[key] = value[total_mask]
                     except TypeError:
                         new_state[key] = value
                 else:
                     new_state[key] = value
 
             layer_coord.visible = False
+            if 'edge_width' in new_state and len(np.unique(new_state['edge_width']))==1:
+                # Otherwise, the edge_width will be 1 in case of a list of edge_widths
+                new_state['edge_width'] = new_state['edge_width'][0]
+
             new = Layer.create(new_data, new_state, old_type_str)
+
             self.napari_viewer.layers.events.inserted.disconnect(
                 self._update_combo
             )
             self.napari_viewer.layers.append(
                 # self.napari_viewer.layers.index(layer_coord) + 1, new
                 new
             )
+            if old_type_str == "shapes":
+                self.napari_viewer.layers[-1].mode = Mode.ADD_PATH
+
             self.napari_viewer.layers.events.inserted.connect(
                 self._update_combo
             )
             self.coord_layer.setCurrentText(new.name)
             self.coord_layer.currentTextChanged.emit(new.name)
             self._update_combo(do_match=False)
         elif create_layer:
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeLayer.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_qt/OrganizeLayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self._add_seperator()
         self._save_ui()
         self._add_seperator()
         self._link_ui()
 
         self._apply_icons()
         self.layout().addStretch(True)
+        self.saved_dir_path = os.getcwd()
 
     def _link_ui(self):
         self.napari_viewer.layers.events.inserted.connect(
             self._update_link_combo
         )
         self.napari_viewer.layers.events.removed.connect(
             self._update_link_combo
@@ -116,32 +117,32 @@
 
         inner_layout.addWidget(QLabel("Write layer", self))
         self.save_layers = {
             "layer": QComboBox(self),
             "dimension": QComboBox(self),
             "type": QComboBox(self),
             "format": QComboBox(self),
-            "filament spacing": QLineEdit(self),
+            "inter-box distance": QLineEdit(self),
             "dummyf": QLabel(self),
             "suffix": QLineEdit(self),
         }
         self.save_layers["layer"].addItems([""])
         self.save_layers["dimension"].addItems(["", "2D", "3D"])
         self.save_layers["type"].addItems(["", "Particles", "Filaments"])
         self.save_layers["suffix"].setPlaceholderText("e.g., _suffix")
-        self.save_layers["filament spacing"].setPlaceholderText(
+        self.save_layers["inter-box distance"].setPlaceholderText(
             "spacing in pixel"
         )
 
         int_validator = QIntValidator()
         int_validator.setBottom(0)
-        self.save_layers["filament spacing"].setValidator(int_validator)
-        self.save_layers["filament spacing"].setText("0")
-        self.save_layers["filament spacing"].setToolTip(
-            "If 0, an overlap of 80% is used."
+        self.save_layers["inter-box distance"].setValidator(int_validator)
+        self.save_layers["inter-box distance"].setText("0")
+        self.save_layers["inter-box distance"].setToolTip(
+            "Inter-box distance in pixel. If 0, an overlap of 80% of box-size is used."
         )
 
         self.formats = {
             "2D": {
                 "Particles": [
                     ".cbox",
                     ".box",
@@ -228,31 +229,32 @@
     @Slot()
     def _run_save(self):
         cur_format = self.save_layers["format"].currentText().split(" ", 1)[0]
         cur_layer = self.napari_viewer.layers[
             self.save_layers["layer"].currentText()
         ]
 
-        cur_spacing = self.save_layers["filament spacing"].text()
+        cur_spacing = self.save_layers["inter-box distance"].text()
         cur_type = self.save_layers["type"].currentText()
         if cur_type == "Filaments" and not cur_spacing:
-            show_error("Filament format requires Filament spacing")
+            show_error("Filament format requires inter-box distance")
             return
 
-        dir_path = QFileDialog.getExistingDirectory(
+        self.saved_dir_path = QFileDialog.getExistingDirectory(
             self,
             "Open directory",
-            os.getcwd(),
+            self.saved_dir_path,
             QFileDialog.ShowDirsOnly | QFileDialog.DontResolveSymlinks,
         )
-        if not dir_path:
+        if not self.saved_dir_path:
+            self.saved_dir_path = os.getcwd()
             return
 
         napari_get_writer(
-            dir_path,
+            self.saved_dir_path,
             [cur_layer.as_layer_data_tuple()],
             cur_format,
             self.save_layers["suffix"].text() + cur_format,
             cur_spacing=int(cur_spacing),
         )
 
     @Slot(object)
@@ -347,15 +349,15 @@
             cur_type = "Particles"
         prev_signal = self.save_layers["type"].blockSignals(True)
         self.save_layers["type"].setCurrentText(cur_type)
         self.save_layers["type"].blockSignals(prev_signal)
 
         type_field_d = self.save_layers["dummyf"]
         type_label_d = self._save_form_layout.labelForField(type_field_d)
-        type_field = self.save_layers["filament spacing"]
+        type_field = self.save_layers["inter-box distance"]
         type_label = self._save_form_layout.labelForField(type_field)
         if self.save_layers["type"].currentText() == "Filaments":
             type_field.show()
             type_label.show()
             type_field_d.hide()
             type_label_d.hide()
         else:
@@ -422,15 +424,15 @@
         # self._add_label.setIcon(point_icon)
 
     def _get_metadata(self):
         layer_name = self._layer.currentText()
 
         metadata = {
             "do_activate_on_insert": True,
-            "linked_image_layers": [general.get_layer_id(self.napari_viewer, self._layer)],
+            "linked_image_layers": [general.get_layer_id(self.napari_viewer, self.napari_viewer.layers[layer_name])],
             "skip_match": None,
         }
         if not layer_name:
             return metadata
         layer_meta = self.napari_viewer.layers[layer_name].metadata
         for key, value in layer_meta.items():
             if isinstance(key, int):
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_qt/SelectMetric.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_qt/SelectMetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import enum
 import itertools
 import os
 import pathlib
-import sys
 import typing
-from .._utils import general
+
 import napari.layers
 import numpy as np
 import pandas as pd
 import tqdm
 from matplotlib.backends.backend_qt5agg import FigureCanvas
 from napari.utils.notifications import show_info
 from qtpy.QtCore import (
@@ -1132,15 +1131,17 @@
             entry for entry in layer.metadata if isinstance(entry, int)
         ]
         full_range = np.arange(
             *self.napari_viewer.dims.range[0], dtype=int
         ).tolist()
 
         if range_list:
-            range_dict = {k:layer.metadata[k] for k in range_list if k in layer.metadata}
+            range_dict = {
+                k: layer.metadata[k] for k in range_list if k in layer.metadata
+            }
             if "ignore_idx" in layer.metadata:
                 ignore_idx = layer.metadata.pop("ignore_idx")
                 label_data = pd.DataFrame(range_dict).loc[:, :].T
                 layer.metadata["ignore_idx"] = ignore_idx
             else:
                 label_data = pd.DataFrame(range_dict).loc[:, :].T
         else:
@@ -1288,17 +1289,17 @@
 
                 if (
                     slice_idx in label_data.index
                     and label_max in label_data.columns
                 ):
                     val = label_data.loc[slice_idx, label_max]
                 else:
-                    val = general.get_max_floor(label_data[label_max])
+                    val = general.get_max_ceil(label_data[label_max])
                     if not np.all(val == label_data[label_max].dropna()):
-                        val = general.get_max_floor(features[col_name])
+                        val = general.get_max_ceil(features[col_name])
                 if not np.isnan(val):
                     output_dict[label_max] = str(val)
                 else:
                     output_dict[label_max] = "-"
 
         else:
             output_dict["write"] = "-"
@@ -1537,38 +1538,61 @@
                 viewer.set_col_max(col_idx)
             else:
                 assert False, label
         self.table_model.remove_labels(invalid_labels)
         if do_update_hist:
             self.update_hist()
 
+    def _get_linked_image_layer_ids(
+        self,
+        layers: typing.List[napari.layers.Layer],
+        *,
+        done: typing.Set[int] = None,
+    ) -> typing.Set[int]:
+        """
+        Get linked layer ids of the provided layers.
+        Do a recursive search to cover nested linking, e.g., for filtered images.
+        Only on the very first run select the provided layers.
+        Do avoid infinite recursion problems, keep track of already covered
+        layers via the `done` variable.
+        Stop the recursion if no new linked images are identified.
+
+        layers - List of napari layers
+        done - Set of already covered layers
+
+        Returns:
+        Set of linked layers
+        """
+        if done is None:
+            done = set()
 
-
-    def _get_linked_image_layer_ids(self, layers: typing.List[napari.layers.Layer]) -> typing.List[int]:
         linked_images = set()
         for layer in layers:
-            self.napari_viewer.layers.selection.add(layer)
             try:
                 image_ids = layer.metadata["linked_image_layers"]
             except KeyError:
                 show_info(
                     f"Layer {layer.name} does not have an 'linked_image_layers' entry."
                     "Use the link layers tool to allow image highlighting in the boxmanager"
                 )
                 layer.metadata["linked_image_layers"] = []
             else:
                 if image_ids is not None:
                     linked_images.update(image_ids)
+        image_layer_ids = general.get_layers_from_ids(
+            self.napari_viewer, linked_images - done
+        )
+        done.update(linked_images)
 
-        for layer in self.napari_viewer.layers:
-            if "linked_image_layers" in layer.metadata:
-                if layer.metadata["linked_image_layers"]:
-                    linked_images.update(layer.metadata["linked_image_layers"])
+        if image_layer_ids:
+            linked_images.update(
+                self._get_linked_image_layer_ids(image_layer_ids, done=done)
+            )
 
-        return list(linked_images)
+        return linked_images
 
     def update_hist(self, *_, change_selection=True):
         rows_candidates_navigate = self.table_widget.get_row_candidates(False)
         rows_candidates = self.table_widget.get_row_candidates(
             self.global_checkbox.isChecked()
         )
         if not rows_candidates:
@@ -1675,20 +1699,26 @@
                 layer.visible = layer.metadata["prev_visible"]
             else:
                 assert False, self.hide_dim.currentText()
             layer.events.opacity.connect(self._update_opacity)
             layer.events.visible.connect(self._update_visible)
 
         self.napari_viewer.layers.selection.clear()
-        valid_images = self._get_linked_image_layer_ids(valid_layers)
+        for layer in valid_layers:
+            self.napari_viewer.layers.selection.add(layer)
+        valid_images = list(self._get_linked_image_layer_ids(valid_layers))
         if valid_images:
+
             for layer in self.napari_viewer.layers:
                 if not isinstance(layer, napari.layers.Image):
                     continue
-                elif general.get_layer_id(self.napari_viewer, layer) not in valid_images:
+                elif (
+                    general.get_layer_id(self.napari_viewer, layer)
+                    not in valid_images
+                ):
                     layer.visible = False
                 else:
                     layer.visible = True
 
         metric_done = []
         if "boxsize" in self.metric_dict:
             labels_data = self._get_all_data("boxsize", layer_mask)
@@ -1916,15 +1946,15 @@
 
     def set_data(self, label_data=None, cur_val_min=None, cur_val_max=None):
         if label_data is None:
             label_data = self._label_data
         else:
             self._label_data = label_data
         val_min = general.get_min_floor(label_data.min())
-        val_max = general.get_max_floor(label_data.max())
+        val_max = general.get_max_ceil(label_data.max())
         val_min = val_min if not np.isnan(val_min) else 0
         val_max = val_max if not np.isnan(val_max) else 0
         self.slider_min.set_range(val_min, val_max)
         self.slider_max.set_range(val_min, val_max)
 
         if cur_val_min is None:
             cur_val_min = val_min
@@ -2002,17 +2032,18 @@
                 ticks = np.round(
                     np.linspace(
                         np.min(data_list[idx]), np.max(data_list[idx]), n_ticks
                     ),
                     3,
                 )
                 if np.all(ticks == ticks[0]):
-                    ticks[0] -= 1
-                    ticks[-1] += 1
-                    margin = 1.2
+                    ticks = [ticks[0]]
+                    # ticks[0] -= 0.01
+                    # ticks[-1] += 0.01
+                    margin = 0
                 else:
                     margin = (
                         np.max(data_list[idx]) - np.min(data_list[idx])
                     ) * 0.05
 
                 entry["axis"].set_xticks(ticks)
                 if n_data != 1:
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_black.png` & `napari_boxmanager-0.4.0b1/src/box_manager/_qt/_icons/checkmark_black.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_white.png` & `napari_boxmanager-0.4.0b1/src/box_manager/_qt/_icons/checkmark_white.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_reader.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import glob
 import os
+import sys
 import typing
 from collections.abc import Callable
+import numpy as np
 
 import pandas as pd
 
 from . import io as bm_readers
 
 if typing.TYPE_CHECKING:
     import numpy.typing as npt
 
+def is_tomo(path: str, reader: Callable):
+    img = reader(path)
+    num_dim = np.squeeze(img[0][0]).ndim
+    return num_dim== 3
 
 def get_dir(path):
     layers = []
     for file_ext in bm_readers._VALID_IOS.keys():
         files = glob.glob(os.path.join(path, f"*.{file_ext}"))
+        reader = bm_readers.get_reader(file_ext)
         if not files:
             continue
-        print("ext", file_ext)
-        layers.extend(bm_readers.get_reader(file_ext)(sorted(files)))
+
+        is_first_file_tomo=is_tomo(files[0],reader)
+        if is_first_file_tomo:
+            for file in files:
+                layers.extend(reader(file))
+        else:
+            layers.extend(reader(sorted(files)))
     return layers
 
 
 def napari_get_reader(
     path: os.PathLike | list[os.PathLike],
 ) -> "Callable[[os.PathLike | list[os.PathLike] | pd.DataFrame], list[tuple[npt.ArrayLike, dict[str, typing.Any], str]]] | None":
     """A basic implementation of a Reader contribution.
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_tests/test_box.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_tests/test_reader.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_tests/test_widget.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_utils/filters.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_utils/general.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_utils/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import napari
 import numpy as np
 import pandas
 
 
 def get_min_floor(vals, step=1000):
     try:
@@ -12,33 +14,46 @@
                 return np.round(np.floor(np.nanmin(vals) * step) / step, 3)
         else:
             return np.round(np.floor(np.nanmin(vals) * step) / step, 3)
     except ValueError:
         return np.nan
 
 
-def get_max_floor(vals, step=1000):
+def get_max_ceil(vals, step=1000):
     try:
         if isinstance(vals, pandas.Series):
             if pandas.isnull(vals).all():
                 return np.nan
             else:
-                return np.round(np.floor(np.nanmax(vals) * step) / step, 3)
+                return np.round(np.ceil(np.nanmax(vals) * step) / step, 3)
         else:
-            return np.round(np.floor(np.nanmax(vals) * step) / step, 3)
+            return np.round(np.ceil(np.nanmax(vals) * step) / step, 3)
     except ValueError:
         return np.nan
 
 
 def get_identifier(layer, cur_slice):
     if isinstance(layer, napari.layers.Points):
         return layer.data[:, cur_slice]
     elif isinstance(layer, napari.layers.Shapes):
         return np.array([entry[0, cur_slice] for entry in layer.data])
     else:
         assert False, (layer, type(layer))
 
-def get_layer_id(napari_viewer: napari.Viewer, layer: napari.layers.Layer) -> int:
+
+def get_layer_id(
+    napari_viewer: napari.Viewer, layer: napari.layers.Layer
+) -> int:
     added_layers = [_ for _ in napari_viewer.layers if layer.name == _.name]
     if added_layers:
         return id([_ for _ in napari_viewer.layers if layer.name == _.name][0])
     return id(layer)
+
+
+def get_layers_from_ids(
+    napari_viewer: napari.Viewer, layer_ids: typing.List[int]
+) -> typing.List[napari.layers.Layer]:
+    """
+    Get a list of layers from a list or set of layer ids created by the python `id` function
+    """
+    added_layers = [_ for _ in napari_viewer.layers if id(_) in layer_ids]
+    return added_layers
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_widget.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/_writer.py` & `napari_boxmanager-0.4.0b1/src/box_manager/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/__init__.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/box.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/cbox.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/cbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import copy
 import os
+import sys
 import typing
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import warnings
-warnings.simplefilter(action='ignore', category=FutureWarning)
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
 from pyStarDB import sp_pystardb as star
 
 from . import io_utils as coordsio
 from .interface import NapariLayerData
 
 valid_extensions = ["cbox"]
 coords_3d_idx = ["x", "y", "z"]
 coords_2d_idx = ["y", "z"]
-#meta_columns = []
-#feature_columns = []
+# meta_columns = []
+# feature_columns = []
 
 #########################
 # GENERAL STUFF
 #########################
 
 ### READING ####
 ################
@@ -33,52 +35,59 @@
 def to_napari(
     path: os.PathLike | list[os.PathLike],
 ) -> "list[NapariLayerData]":
     r = coordsio.to_napari_coordinates(
         path=path,
         read_func=read,
         prepare_napari_func=_prepare_napari,
-        meta_columns=["confidence","size","num_boxes"],
-        feature_columns=['angle','fid'],
+        meta_columns=["confidence", "size", "num_boxes"],
+        feature_columns=["angle", "fid"],
         valid_extensions=get_valid_extensions(),
     )
-
     return r
 
-
-
 def read_cbox_boxfile_old(path):
     """
     Read a box file in EMAN1 box format.
     :param path: Path to box file
     :return: List of bounding boxes
     """
     boxreader = np.atleast_2d(np.genfromtxt(path))
     box_dat = {
         "_CoordinateX": [box[0] for box in boxreader],
         "_CoordinateY": [box[1] for box in boxreader],
         "_Width": [box[2] for box in boxreader],
         "_Height": [box[3] for box in boxreader],
-        "_Confidence": [box[4] for box in boxreader]
+        "_Confidence": [box[4] for box in boxreader],
     }
 
     return pd.DataFrame(box_dat)
 
 
 def read(path: os.PathLike) -> pd.DataFrame:
+    verticis = None
     try:
         starfile = star.StarFile(path)
-        data_dict = starfile["cryolo"]
+        segmented_coords = starfile["cryolo"]
+        if "filament_vertices" in starfile:
+            verticis = starfile["filament_vertices"]
     except Exception:
         try:
-            a =  read_cbox_boxfile_old(path)
-        except Exception:
+            a = read_cbox_boxfile_old(path)
+        except Exception as e:
+            print(e)
             return None
         return a
-    return pd.DataFrame(data_dict)
+    if verticis is not None:
+        temp = copy.deepcopy(verticis['_CoordinateX'])
+        verticis['_CoordinateX'] = verticis['_CoordinateY']
+        verticis['_CoordinateY'] = temp
+        segmented_coords.attrs["filament_vertices"] = verticis
+
+    return segmented_coords
 
 
 ### Writing ####
 ################
 
 
 def from_napari(
@@ -116,15 +125,14 @@
 def _make_df_data_filament(
     coordinates: pd.DataFrame,
     box_size: npt.ArrayLike,
     features: pd.DataFrame,
     filament_spacing: int,
     **kwargs,
 ) -> pd.DataFrame:
-
     is_3d = coordinates.shape[1] == 4
     data = {}
     data["_CoordinateX"] = []
     data["_CoordinateY"] = []
     if is_3d:
         data["_CoordinateZ"] = []
 
@@ -133,14 +141,15 @@
     if is_3d:
         data["_Depth"] = []
 
     data["_filamentid"] = []
 
     feature_map = {}
     other_interpolation_cols = []
+
     coord_columns = ["_CoordinateX", "_CoordinateY"]
     constant_columns = ["_filamentid", "_Width", "_Height"]
     if is_3d:
         coord_columns.append("_CoordinateZ")
         constant_columns.append("_Depth")
 
     if "confidence" in features:
@@ -190,16 +199,21 @@
         filaments[index_fil] = coordsio.resample_filament(
             fil,
             distance,
             coordinate_columns=coord_columns,
             constant_columns=constant_columns,
             other_interpolation_col=other_interpolation_cols,
         )
-
-    return pd.concat(filaments)
+    verts = pd.DataFrame(
+        coordinates, columns=["_CoordinateX", "_CoordinateY", "_filamentid"]
+    )
+    verts["_Width"] = box_size
+    verts["_Height"] = box_size
+    result = {"cryolo": pd.concat(filaments), "filament_vertices": verts}
+    return result
 
 
 #########################
 # PARTICLE STUFF
 #########################
 
 ### READING ####
@@ -217,38 +231,38 @@
     -------
     Dataframe with centered coordinates and additional metadate if necessary.
 
     """
 
     cryolo_data = input_df
 
-
     feature_columns, meta_columns = _fill_meta_features_idx(cryolo_data)
 
+    # Filament verticis are already centered coords
+    centered_coords = "is_centered_coords" in cryolo_data.attrs and cryolo_data.attrs["is_centered_coords"]==True
+
     is_3d = True
     if (
         "_CoordinateZ" not in cryolo_data
         or cryolo_data["_CoordinateZ"].isnull().values.any()
     ):
         is_3d = False
 
     columns = ["z", "y"]
     if is_3d:
         columns.append("x")
 
-    output_data: pd.DataFrame = pd.DataFrame(
-        columns=columns + meta_columns
-    )
+    output_data: pd.DataFrame = pd.DataFrame(columns=columns + meta_columns)
 
-    output_data["z"] = np.array(cryolo_data["_CoordinateX"]) + np.array(
-        cryolo_data["_Width"] / 2
-    )
-    output_data["y"] = np.array(cryolo_data["_CoordinateY"]) + np.array(
-        cryolo_data["_Height"] / 2
-    )
+    output_data["z"] = np.array(cryolo_data["_CoordinateX"])
+    output_data["y"] = np.array(cryolo_data["_CoordinateY"])
+
+    if not centered_coords:
+        output_data["z"] = output_data["z"] + np.array(cryolo_data["_Width"] / 2)
+        output_data["y"] = output_data["y"] + np.array(cryolo_data["_Height"] / 2)
     if is_3d:
         output_data["x"] = cryolo_data["_CoordinateZ"]
 
     output_data["boxsize"] = (
         np.array(cryolo_data["_Width"]) + np.array(cryolo_data["_Height"])
     ) / 2
 
@@ -269,15 +283,17 @@
 
     if "fid" in feature_columns:
         output_data["fid"] = cryolo_data["_filamentid"]
 
     return output_data
 
 
-def _fill_meta_features_idx(input_df: pd.DataFrame) -> typing.Tuple[typing.List[str], typing.List[str]]:
+def _fill_meta_features_idx(
+    input_df: pd.DataFrame,
+) -> typing.Tuple[typing.List[str], typing.List[str]]:
     """
     Fills the meta idx array.
 
     Parameters
     ----------
     input_dict Raw input data
 
@@ -319,43 +335,46 @@
     ) and "fid" not in feature_columns:
         feature_columns.append("fid")
     return feature_columns, meta_columns
 
 
 ### Writing ####
 ################
+from typing import Dict
 
 
-def write_cbox(path: os.PathLike, df: pd.DataFrame, **kwargs):
-
+def write_cbox(path: os.PathLike, data: Dict[str, pd.DataFrame], **kwargs):
     sfile = star.StarFile(path)
-
+    tags = []
     version_df = pd.DataFrame([["1.0"]], columns=["_cbox_format_version"])
     sfile.update("global", version_df, False)
+    tags.append("global")
+    if "filament_vertices" in data:
+        sfile.update("filament_vertices", data["filament_vertices"], True)
+        tags.append("filament_vertices")
+
+    df = data["cryolo"]
     include_slices = []
     if "_CoordinateZ" in df.columns:
         if not df["_CoordinateZ"].isnull().values.any():
             include_slices = [
                 a
                 for a in np.unique(df["_CoordinateZ"]).tolist()
                 if not np.isnan(a)
             ]
 
     if "empty_slices" in kwargs:
         include_slices.extend(kwargs["empty_slices"])
     include_slices.sort()
-
     sfile.update("cryolo", df, True)
-
+    tags.append("cryolo")
     include_df = pd.DataFrame(include_slices, columns=["_slice_index"])
     sfile.update("cryolo_include", include_df, True)
-
-    sfile.write_star_file(
-        overwrite=True, tags=["global", "cryolo", "cryolo_include"]
-    )
+    tags.append("cryolo_include")
+    sfile.write_star_file(overwrite=True, tags=tags)
 
 
 def _make_df_data(
     coordinates: pd.DataFrame,
     box_size: npt.ArrayLike,
     features: pd.DataFrame,
     **kwargs,
@@ -414,8 +433,12 @@
             data["_NumBoxes"].append(np.nan)
 
         if "angle" in features:
             data["_Angle"].append(features["angle"].iloc[i])
         else:
             data["_Angle"].append(np.nan)
 
-    return pd.DataFrame(data)
+    result = {
+        "cryolo": pd.DataFrame(data),
+    }
+
+    return result
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/coords.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/coords.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/interface.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/io_utils.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/io_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 import io
 import itertools
 import os
 import pathlib
 import typing
 import warnings
 from collections.abc import Callable
-from typing import Protocol
+from typing import Protocol, Union, Dict
 
 import matplotlib.pyplot as plt
+import napari
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from .._qt import OrganizeBox as orgbox
+from PyQt5.QtWidgets import QMessageBox
+
 from .interface import NapariLayerData, NapariMetaData
 
 
 class IllegalFormatException(Exception):
     pass
 
 
@@ -40,40 +43,64 @@
     def __call__(
         self,
         coordinates: pd.DataFrame,
         boxsize: npt.ArrayLike,
         features: pd.DataFrame,
         metadata: dict,
         filament_spacing: int,
-    ) -> pd.DataFrame:
+    ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
         ...
 
 
 def _split_filaments(data: pd.DataFrame) -> typing.List[pd.DataFrame]:
+    vert = None
+    if 'filament_vertices' in data.attrs:
+        vert = data.attrs['filament_vertices']
     filament_ids = np.unique(data["fid"])
     filaments = []
     for id in filament_ids:
         mask = data["fid"] == id
-        filaments.append(data[mask])
+        filament = data[mask]
+
+        if vert:
+            mask = vert["_filamentid"] == id
+            vert_fil = vert[mask]
+            filament.attrs['filament_vertices'] = vert_fil
+
+        filaments.append(filament)
     return filaments
 
 
 def _prepare_coords_df(
     path: list[os.PathLike],
     read_func: Callable[[os.PathLike], pd.DataFrame],
     prepare_napari_func: Callable,
     meta_columns: typing.List[str] = [],
 ) -> tuple[typing.List[pd.DataFrame], dict, bool]:
 
     data_df: list[pd.DataFrame] = []
     metadata: dict = {}
     is_3d = True
     is_filament = False
+    make_filament_shape_layer = False
     for idx, entry in enumerate(path):
         input_data = read_func(entry)
+        if idx == 0:
+            if 'filament_vertices' in input_data.attrs:
+                qm = QMessageBox()
+                reply = qm.question(None, 'Quit',
+                            'File contains segmented boxes and filament verticis from training. Continue creating training data?',
+                            QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
+                if reply == qm.Yes:
+                    make_filament_shape_layer = True
+
+        if make_filament_shape_layer:
+            input_data = input_data.attrs['filament_vertices']
+            input_data.attrs["is_centered_coords"] = True
+
 
         box_napari_data = pd.DataFrame(columns=meta_columns)
 
         if input_data is not None:
             box_napari_data = prepare_napari_func(input_data)
 
             if "x" not in box_napari_data:
@@ -114,14 +141,15 @@
                     for col in meta_columns
                     if col in min_max_data
                 }
             )
         except ValueError:
             pass
     metadata["is_filament_layer"] = is_filament
+    metadata["make_filament_shape_layer"] = make_filament_shape_layer
 
     return data_df, metadata, is_3d
 
 
 def is_filament_layer(
     layer_data: typing.Union[NapariLayerData, list[NapariLayerData]]
 ) -> bool:
@@ -142,19 +170,24 @@
             )
         is_filament = check(layer_data[0])
     else:
         is_filament = check(layer_data)
     return is_filament
 
 
-def get_layers_name(path: os.PathLike):
-    if len(path) >= MAX_LAYER_NAME + 3:
-        name = f"...{path[-MAX_LAYER_NAME:]}"  # type: ignore
+def get_layers_name(path: os.PathLike | list[os.PathLike]):
+
+    if not isinstance(path, list):
+        if len(path) >= MAX_LAYER_NAME + 3:
+            name = f"...{path[-MAX_LAYER_NAME:]}"  # type: ignore
+        else:
+            name = path  # type: ignore
     else:
-        name = path  # type: ignore
+        name = (os.path.splitext(path[0])[1]).upper()[1:]
+
     return name
 
 
 def _to_napari_filament(input_df: list[pd.DataFrame], coord_columns, is_3d):
     # boxsize_ = [np.mean(fil['boxsize']) for fil in input_df]
 
     color = []
@@ -181,14 +214,30 @@
         "opacity": 0.8,
     }
     dat = input_df
     layer_type = "points"
 
     return dat, kwargs, layer_type
 
+def _to_napari_filament_shapes(input_df: list[pd.DataFrame], coord_columns, is_3d):
+    boxsize = np.median([np.mean(fil["boxsize"]) for fil in input_df])
+    input_df = np.array([fil[coord_columns].to_numpy() for fil in input_df])
+
+    kwargs = {
+        "edge_color": ["red"],
+        "face_color": "transparent",
+        "edge_width": boxsize,
+        "opacity": 0.4,
+        "shape_type": "path",
+    }
+    dat = input_df
+    layer_type = "shapes"
+
+    return dat, kwargs, layer_type
+
 
 def _to_napari_particle(input_df, coord_columns, is_3d):
     input_df = pd.concat(input_df, ignore_index=True)
 
     kwargs: NapariMetaData = {
         "edge_color": "red",
         "face_color": "transparent",
@@ -209,24 +258,23 @@
     path: os.PathLike | list[os.PathLike],
     load_image: typing.Callable[[str], np.array],
     get_pixel_size: typing.Callable[[str], float],
     do_normalize: bool = True,
 ) -> "list[tuple[npt.ArrayLike, dict[str, typing.Any], str]]":
 
     is_2d_stack = isinstance(path, list) or "*" in path
+    name = get_layers_name(path)
 
     if not isinstance(path, list):
         original_path = path
-        name = get_layers_name(path)
         path = sorted(glob.glob(path))  # type: ignore
     else:
         original_path = (
             f"{os.path.dirname(path[0])}/*{os.path.splitext(path[0])[1]}"
         )
-        name = "images"
 
     # arrays = []
     voxel_size = 1
     metadata: dict = {
         "pixel_spacing": voxel_size,
         "original_path": original_path,
     }
@@ -260,14 +308,15 @@
 
     add_kwargs = {"metadata": metadata, "name": name}
 
     layer_type = "image"  # optional, default is "image"
     return [(data, add_kwargs, layer_type)]
 
 
+
 def to_napari_coordinates(
     path: os.PathLike | list[os.PathLike],
     read_func: Callable[[os.PathLike], pd.DataFrame],
     prepare_napari_func: Callable,
     meta_columns: typing.List[str] = [],
     feature_columns: typing.List[str] = [],
     valid_extensions: typing.List[str] = [],
@@ -275,58 +324,71 @@
 
     input_df_list: list[pd.DataFrame]
     features: dict[str, typing.Any]
 
     is_2d_stack = isinstance(path, list) or "*" in path
     orgbox_meta = orgbox.get_metadata(path)
 
-    if not isinstance(path, list):
-        layer_name = get_layers_name(path)
-    else:
-        layer_name = (os.path.splitext(path[0])[1]).upper()[1:]
+
+    layer_name = get_layers_name(path)
+
 
     if not isinstance(path, list):
         path = sorted(glob.glob(path))  # type: ignore
 
     input_df_list, metadata, is_3d = _prepare_coords_df(
         path,
         read_func=read_func,
         prepare_napari_func=prepare_napari_func,
         meta_columns=meta_columns,
     )
     metadata.update(orgbox_meta)
     metadata["is_2d_stack"] = is_2d_stack
     metadata["ignore_idx"] = feature_columns
+
+    make_filament_shape_layer = False
+    if "make_filament_shape_layer" in metadata: # this metadata entry has to be set by _prepare_coords_df
+        make_filament_shape_layer = metadata["make_filament_shape_layer"]
+
     features = {}
     for entry in feature_columns + meta_columns:
         if metadata["is_filament_layer"]:
             for fil in input_df_list:
                 if entry not in fil:
                     continue
+                entry_data = fil[entry].to_numpy()
+                if make_filament_shape_layer:
+                    # instead per filament box, in case of shapes layer it is per shape
+                    entry_data = np.unique(entry_data)
                 if entry in features:
                     features[entry] = np.concatenate(
-                        [features[entry], fil[entry].to_numpy()]
+                        [features[entry], entry_data]
                     )
                 else:
-                    features[entry] = fil[entry].to_numpy()
+                    features[entry] = entry_data
         else:
             all = pd.concat(input_df_list)
             if entry in all:
                 features[entry] = all[entry].to_numpy()
 
     if is_2d_stack or is_3d:
         # Happens for --stack option and '*.ext'
         coord_columns = ["x", "y", "z"]
     else:
         coord_columns = ["y", "z"]
 
     if metadata["is_filament_layer"]:
-        dat, kwargs, layer_type = _to_napari_filament(
-            input_df_list, coord_columns, is_3d
-        )
+        if make_filament_shape_layer:
+            dat, kwargs, layer_type = _to_napari_filament_shapes(
+                input_df_list, coord_columns, is_3d
+            )
+        else:
+            dat, kwargs, layer_type = _to_napari_filament(
+                input_df_list, coord_columns, is_3d
+            )
     else:
         dat, kwargs, layer_type = _to_napari_particle(
             input_df_list, coord_columns, is_3d
         )
     kwargs["name"] = layer_name
     kwargs["metadata"] = metadata
     kwargs["features"] = features
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/mrc.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/mrc.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 if typing.TYPE_CHECKING:
     import numpy.typing as npt
 
 
 def load_image(path: str) -> np.array:
 
     extension = os.path.splitext(path)[1]
-
     with mrcfile.mmap(path, "r", permissive=True) as mrc:
         data = mrc.data
+        data = data.astype(np.float32)
     if extension == ".mrci":
         return data.astype(np.int32)
     else:
         return data
 
 
 def get_pixel_size(path: str) -> float:
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/star.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/star.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/tif.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/tif.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     import numpy.typing as npt
 
 
 def load_image(path: str) -> np.ndarray:
 
     with tifffile.TiffFile(path) as tif:
         img = tif.pages[0].asarray()
+        img = img.astype(np.float32)
         if len(img.shape) == 3:
             img = np.flip(img, 1)
         else:
             img = np.flip(img, 0)
         return img
     return None
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/io/tloc.py` & `napari_boxmanager-0.4.0b1/src/box_manager/io/tloc.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 "write": None,
             }
             metadata[idx].update(
                 {
                     f"{entry}_{'min' if 'min' in func.__name__ else 'max'}": func(
                         idx_view_df[entry]
                     )
-                    for func in [general.get_min_floor, general.get_max_floor]
+                    for func in [general.get_min_floor, general.get_max_ceil]
                     for entry in _get_meta_idx()
                 }
             )
 
         cur_color = colors(cidx / (n_layers - 1))
         kwargs["edge_color"] = [cur_color]
```

### Comparing `napari_boxmanager-0.3.9/src/box_manager/napari.yaml` & `napari_boxmanager-0.4.0b1/src/box_manager/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/PKG-INFO` & `napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-boxmanager
-Version: 0.3.9
+Version: 0.4.0b1
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/SOURCES.txt` & `napari_boxmanager-0.4.0b1/src/napari_boxmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/2d.mrc` & `napari_boxmanager-0.4.0b1/test_data/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/2d_0.mrc` & `napari_boxmanager-0.4.0b1/test_data/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/2d_particles.cbox` & `napari_boxmanager-0.4.0b1/test_data/2d_particles.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/3d.mrc` & `napari_boxmanager-0.4.0b1/test_data/3d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/3d.mrci` & `napari_boxmanager-0.4.0b1/test_data/3d.mrci`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/3d_particle.cbox` & `napari_boxmanager-0.4.0b1/test_data/3d_particle.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/create_data.py` & `napari_boxmanager-0.4.0b1/test_data/box_data/create_data.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_0.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_1.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_1.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_2.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_2.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_3.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_3.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_4.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_4.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_5.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_5.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_6.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_6.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_7.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_7.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_8.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_8.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/box_data/test_9.mrc` & `napari_boxmanager-0.4.0b1/test_data/box_data/test_9.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_02885.cbox` & `napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_02885.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03047.cbox` & `napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_03047.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03070.cbox` & `napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_03070.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03211.cbox` & `napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_03211.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_04203.cbox` & `napari_boxmanager-0.4.0b1/test_data/filament_cbox_2d/ActLifeact_04203.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox` & `napari_boxmanager-0.4.0b1/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox` & `napari_boxmanager-0.4.0b1/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/valid.tloc` & `napari_boxmanager-0.4.0b1/test_data/valid.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/valid_missing_dim_z.tloc` & `napari_boxmanager-0.4.0b1/test_data/valid_missing_dim_z.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/valid_mrc/2d.mrc` & `napari_boxmanager-0.4.0b1/test_data/valid_mrc/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/test_data/valid_mrc/2d_0.mrc` & `napari_boxmanager-0.4.0b1/test_data/valid_mrc/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.9/tox.ini` & `napari_boxmanager-0.4.0b1/tox.ini`

 * *Files identical despite different names*

