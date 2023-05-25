# Comparing `tmp/napari_animation-0.0.6.tar.gz` & `tmp/napari_animation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_animation-0.0.6.tar", last modified: Mon May  1 14:39:31 2023, max compression
+gzip compressed data, was "napari_animation-0.0.7.tar", last modified: Thu May 25 14:47:35 2023, max compression
```

## Comparing `napari_animation-0.0.6.tar` & `napari_animation-0.0.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.703702 napari_animation-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.695701 napari_animation-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.695701 napari_animation-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-01 14:39:12.000000 napari_animation-0.0.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-01 14:39:12.000000 napari_animation-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-01 14:39:12.000000 napari_animation-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-01 14:39:12.000000 napari_animation-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 14:39:12.000000 napari_animation-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-01 14:39:31.703702 napari_animation-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-01 14:39:12.000000 napari_animation-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 14:39:12.000000 napari_animation-0.0.6/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.695701 napari_animation-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/animate2D.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/animate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/animateMixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/ease_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/interactive_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/programmatic_notebook_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/_qt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/_tests/test_animation_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/animation_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/frame_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/keyframelistcontrol_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/keyframeslist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/savedialog_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_easing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_frame_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/easing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/frame_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/base_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/interpolation_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/viewer_state_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/key_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/viewer_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 14:39:12.000000 napari_animation-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 14:39:12.000000 napari_animation-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   607232 2023-05-01 14:39:12.000000 napari_animation-0.0.6/resources/screenshot-animation-widget.png
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-01 14:39:31.703702 napari_animation-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 14:39:12.000000 napari_animation-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 14:39:12.000000 napari_animation-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.666994 napari_animation-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.658994 napari_animation-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.658994 napari_animation-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-25 14:47:24.000000 napari_animation-0.0.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 14:47:24.000000 napari_animation-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 14:47:24.000000 napari_animation-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-25 14:47:24.000000 napari_animation-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 14:47:24.000000 napari_animation-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-25 14:47:35.666994 napari_animation-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-25 14:47:24.000000 napari_animation-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 14:47:24.000000 napari_animation-0.0.7/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/animate2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/animate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/animateMixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/ease_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/interactive_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/programmatic_notebook_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/_qt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/_tests/test_animation_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/animation_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/frame_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/keyframelistcontrol_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/keyframeslist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/savedialog_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_easing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_frame_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/easing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/frame_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.666994 napari_animation-0.0.7/napari_animation/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/base_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/interpolation_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/viewer_state_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/key_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/viewer_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 14:47:24.000000 napari_animation-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 14:47:24.000000 napari_animation-0.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.666994 napari_animation-0.0.7/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   607232 2023-05-25 14:47:24.000000 napari_animation-0.0.7/resources/screenshot-animation-widget.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-25 14:47:35.666994 napari_animation-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 14:47:24.000000 napari_animation-0.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-25 14:47:24.000000 napari_animation-0.0.7/tox.ini
```

### Comparing `napari_animation-0.0.6/.github/workflows/test_and_deploy.yml` & `napari_animation-0.0.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/.gitignore` & `napari_animation-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/.pre-commit-config.yaml` & `napari_animation-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/LICENSE` & `napari_animation-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/PKG-INFO` & `napari_animation-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_animation
-Version: 0.0.6
+Version: 0.0.7
 Summary: A plugin for making animations in napari
 Home-page: https://github.com/napari/napari-animation
 Download-URL: https://github.com/napari/napari-animation
 Author: Nicholas Sofroniew, Alister Burt, Guillaume Witz, Faris Abouakil, Talley Lambert
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `napari_animation-0.0.6/README.md` & `napari_animation-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/examples/animate2D.py` & `napari_animation-0.0.7/examples/animate2D.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/examples/animate3D.py` & `napari_animation-0.0.7/examples/animate3D.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/examples/animateMixed.py` & `napari_animation-0.0.7/examples/animateMixed.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/examples/programmatic_notebook_example.ipynb` & `napari_animation-0.0.7/examples/programmatic_notebook_example.ipynb`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_qt/_tests/test_animation_widget.py` & `napari_animation-0.0.7/napari_animation/_qt/_tests/test_animation_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_qt/animation_widget.py` & `napari_animation-0.0.7/napari_animation/_qt/animation_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_qt/frame_widget.py` & `napari_animation-0.0.7/napari_animation/_qt/frame_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_qt/keyframelistcontrol_widget.py` & `napari_animation-0.0.7/napari_animation/_qt/keyframelistcontrol_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_qt/keyframeslist_widget.py` & `napari_animation-0.0.7/napari_animation/_qt/keyframeslist_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_qt/savedialog_widget.py` & `napari_animation-0.0.7/napari_animation/_qt/savedialog_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_tests/conftest.py` & `napari_animation-0.0.7/napari_animation/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_tests/test_animation.py` & `napari_animation-0.0.7/napari_animation/_tests/test_animation.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_tests/test_easing.py` & `napari_animation-0.0.7/napari_animation/_tests/test_easing.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_tests/test_frame_sequence.py` & `napari_animation-0.0.7/napari_animation/_tests/test_frame_sequence.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/_tests/test_interpolation.py` & `napari_animation-0.0.7/napari_animation/_tests/test_interpolation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import asdict
+from typing import NamedTuple
 
 import numpy as np
 import pytest
 
 from napari_animation.interpolation import interpolate_viewer_state
 from napari_animation.interpolation.base_interpolation import (
     interpolate_bool,
@@ -68,7 +69,25 @@
         nested_assert_close(asdict(result), asdict(initial_state))
     elif fraction == 1:
         # assert result == final_state
         nested_assert_close(asdict(result), asdict(final_state))
 
     # else:
     # should find something else to test
+
+
+class NTuple(NamedTuple):
+    a: float
+    b: int
+
+
+@pytest.mark.parametrize(
+    "fraction,expected",
+    [(0.0, (0.0, 0)), (0.5, (0.5, 0)), (1.0, (1.0, 1))],
+)
+def test_interpolate_namedtuple(fraction, expected):
+    initial_state = NTuple(a=0.0, b=0)
+    final_state = NTuple(a=1.0, b=1)
+    expected = NTuple(*expected)
+    result = interpolate_sequence(initial_state, final_state, fraction)
+    assert isinstance(result, NTuple)
+    assert result == expected
```

### Comparing `napari_animation-0.0.6/napari_animation/_tests/test_utils.py` & `napari_animation-0.0.7/napari_animation/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/animation.py` & `napari_animation-0.0.7/napari_animation/animation.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/easing.py` & `napari_animation-0.0.7/napari_animation/easing.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/frame_sequence.py` & `napari_animation-0.0.7/napari_animation/frame_sequence.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/interpolation/base_interpolation.py` & `napari_animation-0.0.7/napari_animation/interpolation/base_interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,21 @@
 
     Returns
     ----------
         : sequence of type a
     Interpolated sequence between a and b at fraction.
     """
     seq_cls = type(a)
-    return seq_cls(
-        default_interpolation(v0, v1, fraction) for v0, v1 in zip(a, b)
-    )
+    gen = (default_interpolation(v0, v1, fraction) for v0, v1 in zip(a, b))
+    try:
+        seq = seq_cls(gen)
+    except TypeError:
+        # some interables, like NamedTuple, want the arguments separately
+        seq = seq_cls(*gen)
+    return seq
 
 
 def interpolate_num(a: Number, b: Number, fraction: float) -> Number:
     """Linear interpolation for numeric types.
 
     Parameters
     ----------
```

### Comparing `napari_animation-0.0.6/napari_animation/interpolation/interpolation_constants.py` & `napari_animation-0.0.7/napari_animation/interpolation/interpolation_constants.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/interpolation/utils.py` & `napari_animation-0.0.7/napari_animation/interpolation/utils.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/interpolation/viewer_state_interpolation.py` & `napari_animation-0.0.7/napari_animation/interpolation/viewer_state_interpolation.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/key_frame.py` & `napari_animation-0.0.7/napari_animation/key_frame.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/utils.py` & `napari_animation-0.0.7/napari_animation/utils.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation/viewer_state.py` & `napari_animation-0.0.7/napari_animation/viewer_state.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/napari_animation.egg-info/PKG-INFO` & `napari_animation-0.0.7/napari_animation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-animation
-Version: 0.0.6
+Version: 0.0.7
 Summary: A plugin for making animations in napari
 Home-page: https://github.com/napari/napari-animation
 Download-URL: https://github.com/napari/napari-animation
 Author: Nicholas Sofroniew, Alister Burt, Guillaume Witz, Faris Abouakil, Talley Lambert
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `napari_animation-0.0.6/napari_animation.egg-info/SOURCES.txt` & `napari_animation-0.0.7/napari_animation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/resources/screenshot-animation-widget.png` & `napari_animation-0.0.7/resources/screenshot-animation-widget.png`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/setup.cfg` & `napari_animation-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.6/tox.ini` & `napari_animation-0.0.7/tox.ini`

 * *Files identical despite different names*

