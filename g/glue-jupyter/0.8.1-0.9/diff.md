# Comparing `tmp/glue-jupyter-0.8.1.tar.gz` & `tmp/glue-jupyter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-jupyter-0.8.1.tar", last modified: Tue Sep  7 22:03:41 2021, max compression
+gzip compressed data, was "glue-jupyter-0.9.tar", last modified: Tue Sep 14 15:31:50 2021, max compression
```

## Comparing `glue-jupyter-0.8.1.tar` & `glue-jupyter-0.9.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.349919 glue-jupyter-0.8.1/
--rw-r--r--   0 vsts      (1001) docker     (121)      456 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)      183 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      512 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/.validate-notebooks.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3503 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/CHANGES.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1546 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      140 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     2556 2021-09-07 22:03:41.349919 glue-jupyter-0.8.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2203 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      922 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/RELEASE.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      998 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/azure-pipelines.yml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/binder/
--rw-r--r--   0 vsts      (1001) docker     (121)     1192 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/binder/Dockerfile
--rwxr-xr-x   0 vsts      (1001) docker     (121)      580 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/binder/setup.sh
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/docs/
--rw-r--r--   0 vsts      (1001) docker     (121)     4597 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)      715 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/api.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     7387 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4199 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/developer_notes.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     7814 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/getting_started.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1679 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1717 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/installing.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     4513 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/docs/make.bat
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/glue_jupyter/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3435 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22047 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/glue_jupyter/bqplot/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/glue_jupyter/bqplot/common/
--rw-r--r--   0 vsts      (1001) docker     (121)       59 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14417 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/common/tools.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9534 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/common/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5075 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/layer_artist.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      789 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/tests/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1475 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2627 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/frb_mark.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8785 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/layer_artist.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3480 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2961 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/tests/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3611 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/image/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6114 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/layer_artist.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      821 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/tests/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1191 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    10264 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/layer_artist.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1736 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/tests/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)      860 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.329919 glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (121)     3259 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/data/bqplot.ipynb
--rw-r--r--   0 vsts      (1001) docker     (121)    11379 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/test_bqplot.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.333919 glue-jupyter-0.8.1/glue_jupyter/common/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      451 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/basic_jupyter_toolbar.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     3267 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/slice_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5897 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state3d.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.333919 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/
--rw-r--r--   0 vsts      (1001) docker     (121)      533 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      303 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_histogram.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3875 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_image.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4893 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_image.vue
--rw-r--r--   0 vsts      (1001) docker     (121)      637 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_profile.py
--rw-r--r--   0 vsts      (1001) docker     (121)      311 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_profile.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     2143 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_scatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.333919 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)      491 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/tests/test_viewer_image.py
--rw-r--r--   0 vsts      (1001) docker     (121)      636 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_histogram.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1530 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_histogram.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     3281 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_image.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2027 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_image.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     1014 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_profile.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1540 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_profile.vue
--rw-r--r--   0 vsts      (1001) docker     (121)      679 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_scatter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2862 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/common/toolbar_vuetify.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1564 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (121)      690 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/data.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/icons/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/icons/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6077 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/icons/glue_ellipse.svg
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/
--rw-r--r--   0 vsts      (1001) docker     (121)      112 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/
--rw-r--r--   0 vsts      (1001) docker     (121)      104 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3023 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/tools.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3631 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1369 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/viewer_options_widget.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6359 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/layer_artist.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1958 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/layer_style_widget.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1908 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/tests/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1036 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.337919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (121)     2697 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/data/ipyvolume.ipynb
--rw-r--r--   0 vsts      (1001) docker     (121)     6663 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/test_ipyvolume.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5321 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/layer_artist.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3837 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/layer_style_widget.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/tests/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1282 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1027 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/ipywidgets_layout.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/layout_widget.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     3993 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/link.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/matplotlib/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1860 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/base.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1191 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1658 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/image.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1118 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/profile.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1247 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/scatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/matplotlib/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/matplotlib/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (121)     3419 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/tests/data/matplotlib.ipynb
--rw-r--r--   0 vsts      (1001) docker     (121)      414 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/matplotlib/tests/test_matplotlib.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6120 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/state_traitlets_helpers.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/table/
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2688 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/table/table.vue
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/table/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/table/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1704 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/table/tests/test_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7273 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/table/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.341919 glue-jupyter-0.8.1/glue_jupyter/tests/
--rwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.345919 glue-jupyter-0.8.1/glue_jupyter/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (121)     8568 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/tests/data/state_widgets.ipynb
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6855 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/tests/main_test.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3015 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/tests/test_state_traitlets_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5975 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4749 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1944 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/vuetify_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1345 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/vuetify_layout.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.345919 glue-jupyter-0.8.1/glue_jupyter/widgets/
--rw-r--r--   0 vsts      (1001) docker     (121)      139 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2523 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/color.py
--rw-r--r--   0 vsts      (1001) docker     (121)      483 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/glue_float_field.vue
--rw-r--r--   0 vsts      (1001) docker     (121)      466 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/glue_throttled_slider.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     2862 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/layer_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2741 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/layeroptions.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     3318 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/linked_dropdown.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2254 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/size.py
--rw-r--r--   0 vsts      (1001) docker     (121)      709 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/subset_mode_test.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3322 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/subset_mode_vuetify.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2595 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/subset_select.vue
--rw-r--r--   0 vsts      (1001) docker     (121)     2899 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/subset_select_test.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3577 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/subset_select_vuetify.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2583 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/temp.vue
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.345919 glue-jupyter-0.8.1/glue_jupyter/widgets/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1970 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/glue_jupyter/widgets/tests/test_linked_dropdown.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.325919 glue-jupyter-0.8.1/glue_jupyter.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2556 2021-09-07 22:03:41.000000 glue-jupyter-0.8.1/glue_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     5577 2021-09-07 22:03:41.000000 glue-jupyter-0.8.1/glue_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-09-07 22:03:41.000000 glue-jupyter-0.8.1/glue_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-09-07 22:03:41.000000 glue-jupyter-0.8.1/glue_jupyter.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      317 2021-09-07 22:03:41.000000 glue-jupyter-0.8.1/glue_jupyter.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2021-09-07 22:03:41.000000 glue-jupyter-0.8.1/glue_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.321919 glue-jupyter-0.8.1/notebooks/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.321919 glue-jupyter-0.8.1/notebooks/Astronomy/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.345919 glue-jupyter-0.8.1/notebooks/Astronomy/GAIA/
--rw-r--r--   0 vsts      (1001) docker     (121)     9456 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/notebooks/Astronomy/GAIA/Distance to The Pleiades with Glupyter and Gaia DR2.ipynb
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.345919 glue-jupyter-0.8.1/notebooks/Astronomy/L1448/
--rw-r--r--   0 vsts      (1001) docker     (121)     2432 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/notebooks/Astronomy/L1448/L1448 in 3D.ipynb
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.349919 glue-jupyter-0.8.1/notebooks/Astronomy/W5/
--rw-r--r--   0 vsts      (1001) docker     (121)     8099 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/notebooks/Astronomy/W5/W5 Tutorial.ipynb
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.349919 glue-jupyter-0.8.1/notebooks/Generic/
--rw-r--r--   0 vsts      (1001) docker     (121)     1566 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/notebooks/Generic/demo_gaussian.ipynb
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-07 22:03:41.349919 glue-jupyter-0.8.1/notebooks/Planes/
--rw-r--r--   0 vsts      (1001) docker     (121)     3461 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/notebooks/Planes/Boston Planes.ipynb
--rw-r--r--   0 vsts      (1001) docker     (121)      132 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     1216 2021-09-07 22:03:41.349919 glue-jupyter-0.8.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)      455 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/setup.py
--rw-r--r--   0 vsts      (1001) docker     (121)      777 2021-09-07 22:03:25.000000 glue-jupyter-0.8.1/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2021-09-14 15:31:28.000000 glue-jupyter-0.9/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (121)      183 2021-09-14 15:31:28.000000 glue-jupyter-0.9/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      512 2021-09-14 15:31:28.000000 glue-jupyter-0.9/.validate-notebooks.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3639 2021-09-14 15:31:28.000000 glue-jupyter-0.9/CHANGES.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1546 2021-09-14 15:31:28.000000 glue-jupyter-0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      140 2021-09-14 15:31:28.000000 glue-jupyter-0.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     2554 2021-09-14 15:31:50.614531 glue-jupyter-0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2203 2021-09-14 15:31:28.000000 glue-jupyter-0.9/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      922 2021-09-14 15:31:28.000000 glue-jupyter-0.9/RELEASE.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      998 2021-09-14 15:31:28.000000 glue-jupyter-0.9/azure-pipelines.yml
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.590531 glue-jupyter-0.9/binder/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1192 2021-09-14 15:31:28.000000 glue-jupyter-0.9/binder/Dockerfile
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      580 2021-09-14 15:31:28.000000 glue-jupyter-0.9/binder/setup.sh
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.594531 glue-jupyter-0.9/docs/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4597 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (121)      715 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/api.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     7387 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4199 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/developer_notes.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     7814 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/getting_started.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1679 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1717 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/installing.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     4513 2021-09-14 15:31:28.000000 glue-jupyter-0.9/docs/make.bat
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.594531 glue-jupyter-0.9/glue_jupyter/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     3435 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22047 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.594531 glue-jupyter-0.9/glue_jupyter/bqplot/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/common/
+-rw-r--r--   0 vsts      (1001) docker     (121)       59 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15041 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/common/tools.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9534 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/common/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5075 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/layer_artist.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      789 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/tests/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1475 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/histogram/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/image/
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3489 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/frb_mark.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8785 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/layer_artist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3986 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/image/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2961 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/tests/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3630 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/image/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/profile/
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/profile/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6114 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/profile/layer_artist.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/profile/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/profile/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      821 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/profile/tests/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1191 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/profile/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)    10264 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/layer_artist.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1736 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/tests/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      860 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/scatter/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.598531 glue-jupyter-0.9/glue_jupyter/bqplot/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/bqplot/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3259 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/tests/data/bqplot.ipynb
+-rw-r--r--   0 vsts      (1001) docker     (121)    11379 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/bqplot/tests/test_bqplot.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/common/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      451 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/basic_jupyter_toolbar.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     3267 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/slice_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5897 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state3d.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/common/state_widgets/
+-rw-r--r--   0 vsts      (1001) docker     (121)      533 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      303 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3875 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_image.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4893 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_image.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)      637 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_profile.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      311 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_profile.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     2143 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_scatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/common/state_widgets/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)      491 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/tests/test_viewer_image.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      636 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1530 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_histogram.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     3281 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_image.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2027 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_image.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     1014 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_profile.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1540 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_profile.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)      679 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_scatter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2862 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/common/toolbar_vuetify.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1564 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      690 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/data.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/icons/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/icons/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6077 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/icons/glue_ellipse.svg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/ipyvolume/
+-rw-r--r--   0 vsts      (1001) docker     (121)      112 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.602531 glue-jupyter-0.9/glue_jupyter/ipyvolume/common/
+-rw-r--r--   0 vsts      (1001) docker     (121)      104 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3023 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/common/tools.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3631 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/common/viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1369 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/common/viewer_options_widget.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/
+-rw-r--r--   0 vsts      (1001) docker     (121)      108 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     6359 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/layer_artist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1958 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/layer_style_widget.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1908 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/tests/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1036 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2697 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/data/ipyvolume.ipynb
+-rw-r--r--   0 vsts      (1001) docker     (121)     6663 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/test_ipyvolume.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/
+-rw-r--r--   0 vsts      (1001) docker     (121)      108 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5321 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/layer_artist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3837 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/layer_style_widget.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/tests/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1282 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1027 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/ipywidgets_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/layout_widget.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     3993 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/link.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/matplotlib/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1860 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1191 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1658 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/image.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1118 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/profile.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1247 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/scatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/matplotlib/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/matplotlib/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3419 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/tests/data/matplotlib.ipynb
+-rw-r--r--   0 vsts      (1001) docker     (121)      414 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/matplotlib/tests/test_matplotlib.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6120 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/state_traitlets_helpers.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/table/
+-rw-r--r--   0 vsts      (1001) docker     (121)       40 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2688 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/table/table.vue
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.606531 glue-jupyter-0.9/glue_jupyter/table/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/table/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1704 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/table/tests/test_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7273 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/table/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/glue_jupyter/tests/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/glue_jupyter/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8568 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/tests/data/state_widgets.ipynb
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     6855 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/tests/main_test.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3015 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/tests/test_state_traitlets_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5975 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4749 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1944 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/vuetify_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1345 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/vuetify_layout.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/glue_jupyter/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (121)      139 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2523 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/color.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      483 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/glue_float_field.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)      466 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/glue_throttled_slider.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     2862 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/layer_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2741 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/layeroptions.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     3318 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/linked_dropdown.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2254 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/size.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      709 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/subset_mode_test.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3322 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/subset_mode_vuetify.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2595 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/subset_select.vue
+-rw-r--r--   0 vsts      (1001) docker     (121)     2899 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/subset_select_test.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3577 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/subset_select_vuetify.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2583 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/temp.vue
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/glue_jupyter/widgets/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1970 2021-09-14 15:31:28.000000 glue-jupyter-0.9/glue_jupyter/widgets/tests/test_linked_dropdown.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.594531 glue-jupyter-0.9/glue_jupyter.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2554 2021-09-14 15:31:50.000000 glue-jupyter-0.9/glue_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     5577 2021-09-14 15:31:50.000000 glue-jupyter-0.9/glue_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-09-14 15:31:50.000000 glue-jupyter-0.9/glue_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-09-14 15:31:50.000000 glue-jupyter-0.9/glue_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)      317 2021-09-14 15:31:50.000000 glue-jupyter-0.9/glue_jupyter.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       13 2021-09-14 15:31:50.000000 glue-jupyter-0.9/glue_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.590531 glue-jupyter-0.9/notebooks/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.590531 glue-jupyter-0.9/notebooks/Astronomy/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/notebooks/Astronomy/GAIA/
+-rw-r--r--   0 vsts      (1001) docker     (121)     9456 2021-09-14 15:31:28.000000 glue-jupyter-0.9/notebooks/Astronomy/GAIA/Distance to The Pleiades with Glupyter and Gaia DR2.ipynb
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/notebooks/Astronomy/L1448/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2432 2021-09-14 15:31:28.000000 glue-jupyter-0.9/notebooks/Astronomy/L1448/L1448 in 3D.ipynb
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/notebooks/Astronomy/W5/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8099 2021-09-14 15:31:28.000000 glue-jupyter-0.9/notebooks/Astronomy/W5/W5 Tutorial.ipynb
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/notebooks/Generic/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1566 2021-09-14 15:31:28.000000 glue-jupyter-0.9/notebooks/Generic/demo_gaussian.ipynb
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-14 15:31:50.610531 glue-jupyter-0.9/notebooks/Planes/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3461 2021-09-14 15:31:28.000000 glue-jupyter-0.9/notebooks/Planes/Boston Planes.ipynb
+-rw-r--r--   0 vsts      (1001) docker     (121)      132 2021-09-14 15:31:28.000000 glue-jupyter-0.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1216 2021-09-14 15:31:50.614531 glue-jupyter-0.9/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      455 2021-09-14 15:31:28.000000 glue-jupyter-0.9/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      777 2021-09-14 15:31:28.000000 glue-jupyter-0.9/tox.ini
```

### Comparing `glue-jupyter-0.8.1/.validate-notebooks.py` & `glue-jupyter-0.9/.validate-notebooks.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/CHANGES.rst` & `glue-jupyter-0.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.9 (2021-09-14)
+================
+
+* Add an option to allow fixed resolution buffer to be larger than
+  axes by a given factor. [#246]
+
 0.8.1 (2021-09-07)
 ==================
 
 * Better handle incompatible subsets in table viewer. [#256]
 
 * Better handle case where image artist has already been removed. [#256]
```

### Comparing `glue-jupyter-0.8.1/LICENSE` & `glue-jupyter-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/PKG-INFO` & `glue-jupyter-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-jupyter
-Version: 0.8.1
+Version: 0.9
 Summary: Jupyter notebook/lab viewers for glue
 Home-page: https://glueviz.org
 Author: Maarten A. Breddels and Thomas Robitaille
 Author-email: maartenbreddels@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `glue-jupyter-0.8.1/README.rst` & `glue-jupyter-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/RELEASE.rst` & `glue-jupyter-0.9/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/azure-pipelines.yml` & `glue-jupyter-0.9/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/binder/Dockerfile` & `glue-jupyter-0.9/binder/Dockerfile`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/binder/setup.sh` & `glue-jupyter-0.9/binder/setup.sh`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/Makefile` & `glue-jupyter-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/api.rst` & `glue-jupyter-0.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/conf.py` & `glue-jupyter-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/developer_notes.rst` & `glue-jupyter-0.9/docs/developer_notes.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/getting_started.rst` & `glue-jupyter-0.9/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/index.rst` & `glue-jupyter-0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/installing.rst` & `glue-jupyter-0.9/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/docs/make.bat` & `glue-jupyter-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/__init__.py` & `glue-jupyter-0.9/glue_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/app.py` & `glue-jupyter-0.9/glue_jupyter/app.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/common/tools.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/common/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,29 @@
     def __init__(self, viewer, **kwargs):
 
         super().__init__(viewer, **kwargs)
 
         self.interact = PanZoom(scales={'x': [self.viewer.scale_x],
                                         'y': [self.viewer.scale_y]})
 
+    def activate(self):
+        if hasattr(self.viewer, '_composite_image'):
+            self.viewer.state.add_callback('image_external_padding', self._sync_padding)
+            self._sync_padding()
+        super().activate()
+
+    def _sync_padding(self, *args):
+        self.viewer._composite_image.external_padding = self.viewer.state.image_external_padding
+
+    def deactivate(self):
+        if hasattr(self.viewer, '_composite_image'):
+            self.viewer.state.remove_callback('image_external_padding', self._sync_padding)
+            self.viewer._composite_image.external_padding = 0
+        super().deactivate()
+
 
 @viewer_tool
 class BqplotPanZoomXMode(InteractCheckableTool):
 
     icon = 'glue_move_x'
     tool_id = 'bqplot:panzoom_x'
     action_text = 'Pan and Zoom X Axis'
```

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/common/viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/common/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/layer_artist.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/histogram/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/tests/test_viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/histogram/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/histogram/viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/histogram/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/image/layer_artist.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/image/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/image/state.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/image/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import numpy as np
 
 from echo import CallbackProperty
 from glue.viewers.matplotlib.state import (DeferredDrawCallbackProperty as DDCProperty,
                                            DeferredDrawSelectionCallbackProperty as DDSCProperty)
 
-from glue.viewers.image.state import ImageLayerState
+from glue.viewers.image.state import ImageViewerState, ImageLayerState
 from glue.core.state_objects import StateAttributeLimitsHelper
 
 
+class BqplotImageViewerState(ImageViewerState):
+    image_external_padding = DDCProperty(0, docstring='How much padding to add to the '
+                                                      'fixed resolution buffer beyond the '
+                                                      'bounds of the image, as a value relative '
+                                                      'to the axes width/height (0 means no '
+                                                      'padding)')
+
+
 class BqplotImageLayerState(ImageLayerState):
     c_min = DDCProperty(docstring='The lower level used for the contours')
     c_max = DDCProperty(docstring='The upper level used for the contours')
     level_mode = DDSCProperty(0, docstring='How to distribute the contour levels')
     n_levels = DDCProperty(5, docstring='The number of levels, in Linear mode')
     levels = CallbackProperty(docstring='List of values where to create the contour lines')
     labels = CallbackProperty(docstring='List of labels for each contour')
```

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/image/tests/test_viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/image/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/image/viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/image/viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from glue.viewers.image.state import ImageViewerState
 from glue.viewers.image.composite_array import CompositeArray
 from bqplot_image_gl.viewlistener import ViewListener
 
 from ...link import on_change
 
 from ..common.viewer import BqplotBaseView
 from ..scatter.layer_artist import BqplotScatterLayerArtist
 
 from .layer_artist import BqplotImageLayerArtist, BqplotImageSubsetLayerArtist
 from .frb_mark import FRBImage
 
+from glue_jupyter.bqplot.image.state import BqplotImageViewerState
 from glue_jupyter.common.state_widgets.layer_scatter import ScatterLayerStateWidget
 from glue_jupyter.common.state_widgets.layer_image import (ImageLayerStateWidget,
                                                            ImageSubsetLayerStateWidget)
 from glue_jupyter.common.state_widgets.viewer_image import ImageViewerStateWidget
 
 __all__ = ['BqplotImageView']
 
@@ -23,15 +23,15 @@
     allow_duplicate_data = False
     allow_duplicate_subset = False
     large_data_size = 2e7
 
     _layer_style_widget_cls = {BqplotImageLayerArtist: ImageLayerStateWidget,
                                BqplotImageSubsetLayerArtist: ImageSubsetLayerStateWidget,
                                BqplotScatterLayerArtist: ScatterLayerStateWidget}
-    _state_cls = ImageViewerState
+    _state_cls = BqplotImageViewerState
     _options_cls = ImageViewerStateWidget
 
     tools = ['bqplot:home', 'bqplot:panzoom', 'bqplot:rectangle', 'bqplot:circle']
 
     def __init__(self, session):
 
         super(BqplotImageView, self).__init__(session)
```

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/layer_artist.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/profile/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/tests/test_viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/profile/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/profile/viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/profile/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/layer_artist.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/scatter/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/tests/test_viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/scatter/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/scatter/viewer.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/scatter/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/data/bqplot.ipynb` & `glue-jupyter-0.9/glue_jupyter/bqplot/tests/data/bqplot.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/bqplot/tests/test_bqplot.py` & `glue-jupyter-0.9/glue_jupyter/bqplot/tests/test_bqplot.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/slice_helpers.py` & `glue-jupyter-0.9/glue_jupyter/common/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state3d.py` & `glue-jupyter-0.9/glue_jupyter/common/state3d.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/__init__.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_image.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_image.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_image.vue` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_image.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_profile.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_profile.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/layer_scatter.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/layer_scatter.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_histogram.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_histogram.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_histogram.vue` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_histogram.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_image.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_image.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_image.vue` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_image.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_profile.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_profile.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_profile.vue` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_profile.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/state_widgets/viewer_scatter.py` & `glue-jupyter-0.9/glue_jupyter/common/state_widgets/viewer_scatter.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/common/toolbar_vuetify.py` & `glue-jupyter-0.9/glue_jupyter/common/toolbar_vuetify.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/conftest.py` & `glue-jupyter-0.9/glue_jupyter/conftest.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/data.py` & `glue-jupyter-0.9/glue_jupyter/data.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/icons/glue_ellipse.svg` & `glue-jupyter-0.9/glue_jupyter/icons/glue_ellipse.svg`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/tools.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/common/tools.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/viewer.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/common/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/common/viewer_options_widget.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/common/viewer_options_widget.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/layer_artist.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/layer_style_widget.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/layer_style_widget.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/tests/test_viewer.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/scatter/viewer.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/scatter/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/data/ipyvolume.ipynb` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/data/ipyvolume.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/tests/test_ipyvolume.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/tests/test_ipyvolume.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/layer_artist.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/layer_style_widget.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/layer_style_widget.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipyvolume/volume/viewer.py` & `glue-jupyter-0.9/glue_jupyter/ipyvolume/volume/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/ipywidgets_layout.py` & `glue-jupyter-0.9/glue_jupyter/ipywidgets_layout.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/layout_widget.vue` & `glue-jupyter-0.9/glue_jupyter/layout_widget.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/link.py` & `glue-jupyter-0.9/glue_jupyter/link.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/matplotlib/base.py` & `glue-jupyter-0.9/glue_jupyter/matplotlib/base.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/matplotlib/histogram.py` & `glue-jupyter-0.9/glue_jupyter/matplotlib/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/matplotlib/image.py` & `glue-jupyter-0.9/glue_jupyter/matplotlib/image.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/matplotlib/profile.py` & `glue-jupyter-0.9/glue_jupyter/matplotlib/profile.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/matplotlib/scatter.py` & `glue-jupyter-0.9/glue_jupyter/matplotlib/scatter.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/matplotlib/tests/data/matplotlib.ipynb` & `glue-jupyter-0.9/glue_jupyter/matplotlib/tests/data/matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/state_traitlets_helpers.py` & `glue-jupyter-0.9/glue_jupyter/state_traitlets_helpers.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/table/table.vue` & `glue-jupyter-0.9/glue_jupyter/table/table.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/table/tests/test_table.py` & `glue-jupyter-0.9/glue_jupyter/table/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/table/viewer.py` & `glue-jupyter-0.9/glue_jupyter/table/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/tests/data/state_widgets.ipynb` & `glue-jupyter-0.9/glue_jupyter/tests/data/state_widgets.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/tests/main_test.py` & `glue-jupyter-0.9/glue_jupyter/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/tests/test_state_traitlets_helpers.py` & `glue-jupyter-0.9/glue_jupyter/tests/test_state_traitlets_helpers.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/utils.py` & `glue-jupyter-0.9/glue_jupyter/utils.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/view.py` & `glue-jupyter-0.9/glue_jupyter/view.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/vuetify_helpers.py` & `glue-jupyter-0.9/glue_jupyter/vuetify_helpers.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/vuetify_layout.py` & `glue-jupyter-0.9/glue_jupyter/vuetify_layout.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/color.py` & `glue-jupyter-0.9/glue_jupyter/widgets/color.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/layer_options.py` & `glue-jupyter-0.9/glue_jupyter/widgets/layer_options.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/layeroptions.vue` & `glue-jupyter-0.9/glue_jupyter/widgets/layeroptions.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/linked_dropdown.py` & `glue-jupyter-0.9/glue_jupyter/widgets/linked_dropdown.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/size.py` & `glue-jupyter-0.9/glue_jupyter/widgets/size.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/subset_mode_test.py` & `glue-jupyter-0.9/glue_jupyter/widgets/subset_mode_test.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/subset_mode_vuetify.py` & `glue-jupyter-0.9/glue_jupyter/widgets/subset_mode_vuetify.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/subset_select.vue` & `glue-jupyter-0.9/glue_jupyter/widgets/subset_select.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/subset_select_test.py` & `glue-jupyter-0.9/glue_jupyter/widgets/subset_select_test.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/subset_select_vuetify.py` & `glue-jupyter-0.9/glue_jupyter/widgets/subset_select_vuetify.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/temp.vue` & `glue-jupyter-0.9/glue_jupyter/widgets/temp.vue`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter/widgets/tests/test_linked_dropdown.py` & `glue-jupyter-0.9/glue_jupyter/widgets/tests/test_linked_dropdown.py`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/glue_jupyter.egg-info/PKG-INFO` & `glue-jupyter-0.9/glue_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-jupyter
-Version: 0.8.1
+Version: 0.9
 Summary: Jupyter notebook/lab viewers for glue
 Home-page: https://glueviz.org
 Author: Maarten A. Breddels and Thomas Robitaille
 Author-email: maartenbreddels@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `glue-jupyter-0.8.1/glue_jupyter.egg-info/SOURCES.txt` & `glue-jupyter-0.9/glue_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/notebooks/Astronomy/GAIA/Distance to The Pleiades with Glupyter and Gaia DR2.ipynb` & `glue-jupyter-0.9/notebooks/Astronomy/GAIA/Distance to The Pleiades with Glupyter and Gaia DR2.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/notebooks/Astronomy/L1448/L1448 in 3D.ipynb` & `glue-jupyter-0.9/notebooks/Astronomy/L1448/L1448 in 3D.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/notebooks/Astronomy/W5/W5 Tutorial.ipynb` & `glue-jupyter-0.9/notebooks/Astronomy/W5/W5 Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/notebooks/Generic/demo_gaussian.ipynb` & `glue-jupyter-0.9/notebooks/Generic/demo_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/notebooks/Planes/Boston Planes.ipynb` & `glue-jupyter-0.9/notebooks/Planes/Boston Planes.ipynb`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/setup.cfg` & `glue-jupyter-0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `glue-jupyter-0.8.1/tox.ini` & `glue-jupyter-0.9/tox.ini`

 * *Files identical despite different names*

