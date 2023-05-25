# Comparing `tmp/kfactory-0.7.0.tar.gz` & `tmp/kfactory-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.7.0.tar", last modified: Tue May 23 05:30:28 2023, max compression
+gzip compressed data, was "kfactory-0.7.1.tar", last modified: Thu May 25 14:16:41 2023, max compression
```

## Comparing `kfactory-0.7.0.tar` & `kfactory-0.7.1.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 05:30:10.000000 kfactory-0.7.0/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 05:30:10.000000 kfactory-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-23 05:30:10.000000 kfactory-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 05:30:10.000000 kfactory-0.7.0/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 05:30:10.000000 kfactory-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 05:30:10.000000 kfactory-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 05:30:28.466122 kfactory-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-23 05:30:10.000000 kfactory-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.458122 kfactory-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.458122 kfactory-0.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/klive.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.458122 kfactory-0.7.0/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-23 05:30:10.000000 kfactory-0.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-23 05:30:10.000000 kfactory-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 05:30:28.466122 kfactory-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    90612 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/klayout_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/layer_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.364492 kfactory-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 14:16:20.000000 kfactory-0.7.1/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.340491 kfactory-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.340491 kfactory-0.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 14:16:20.000000 kfactory-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-25 14:16:20.000000 kfactory-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-25 14:16:20.000000 kfactory-0.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.340491 kfactory-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-25 14:16:20.000000 kfactory-0.7.1/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 14:16:20.000000 kfactory-0.7.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-25 14:16:20.000000 kfactory-0.7.1/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 14:16:20.000000 kfactory-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-25 14:16:20.000000 kfactory-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 14:16:20.000000 kfactory-0.7.1/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 14:16:20.000000 kfactory-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 14:16:20.000000 kfactory-0.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 14:16:41.364492 kfactory-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-25 14:16:20.000000 kfactory-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.340491 kfactory-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.340491 kfactory-0.7.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.344491 kfactory-0.7.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.348492 kfactory-0.7.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.348492 kfactory-0.7.1/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-25 14:16:20.000000 kfactory-0.7.1/docs/source/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-25 14:16:20.000000 kfactory-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:16:41.364492 kfactory-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.336491 kfactory-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.352492 kfactory-0.7.1/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.356492 kfactory-0.7.1/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.356492 kfactory-0.7.1/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/cells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90612 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.356492 kfactory-0.7.1/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.360492 kfactory-0.7.1/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/klayout_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/layer_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/technology/yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.360492 kfactory-0.7.1/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.360492 kfactory-0.7.1/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-25 14:16:20.000000 kfactory-0.7.1/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.352492 kfactory-0.7.1/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 14:16:41.000000 kfactory-0.7.1/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-25 14:16:41.000000 kfactory-0.7.1/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:16:41.000000 kfactory-0.7.1/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 14:16:41.000000 kfactory-0.7.1/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 14:16:41.000000 kfactory-0.7.1/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:16:41.364492 kfactory-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-25 14:16:20.000000 kfactory-0.7.1/tests/test_spiral.py
```

### Comparing `kfactory-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/.github/workflows/release.yml` & `kfactory-0.7.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/.github/workflows/test_code.yml` & `kfactory-0.7.1/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/.pre-commit-config.yaml` & `kfactory-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/LICENSE` & `kfactory-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/PKG-INFO` & `kfactory-0.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.0
+Version: 0.7.1
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.0
+# KFactory 0.7.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
+| :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
+|---------------------------------------------------------------------------------------------------------------------------------|
+
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.1` for example.
+
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
+- [x] Jupyter integration
+- [x] PDK/package configuration
+- [x] Plugin system (simulations etc.) - Check [kplugins](https://github.com/gdsfactory/kplugins)
+- [x] Generic PDK example - Check [kgeneric](https://github.com/gdsfactory/kgeneric)
 
 
 Notable missing Features:
-- [ ] PDK/package configuration
+
 - [ ] CrossSection
 - [ ] Netlist/Schematics and LVS
 - [ ] More advanced routing
-- [ ] Plugin system (simulations etc.)
-- [ ] Jupyter integration
 
 
 New/Improved Features:
 - Fully hierarchical bi-directional conversion to YAML
 - Automatic snapping to grid thanks to KLayout
 - More features for vector geometries due to concept of Point/Edge/Vector/Polygon from Klayout
 - Easy booleans thanks to KLayout Regions
@@ -45,23 +52,23 @@
   which are built into KLayout
 
 
 ## Installation
 
 kfactory is available on [pypi](https://pypi.org/project/kfactory/)
 
-```
+```bash
 pip install kfactory
 ```
 
 At the moment kfactory works only on python 3.10
 
 ### Development Installation
 
 
 A development environment can be installed with
 
-```
-python -m pip install .[dev]
+```bash
+python -m pip install -e .[dev]
 ```
 
 It is defined in `pyproject.toml`. For committing `pre-commit` should be installed with `pre-commit install`.
```

### Comparing `kfactory-0.7.0/README.md` & `kfactory-0.7.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-# KFactory 0.7.0
+# KFactory 0.7.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
+| :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
+|---------------------------------------------------------------------------------------------------------------------------------|
+
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.1` for example.
+
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
+- [x] Jupyter integration
+- [x] PDK/package configuration
+- [x] Plugin system (simulations etc.) - Check [kplugins](https://github.com/gdsfactory/kplugins)
+- [x] Generic PDK example - Check [kgeneric](https://github.com/gdsfactory/kgeneric)
 
 
 Notable missing Features:
-- [ ] PDK/package configuration
+
 - [ ] CrossSection
 - [ ] Netlist/Schematics and LVS
 - [ ] More advanced routing
-- [ ] Plugin system (simulations etc.)
-- [ ] Jupyter integration
 
 
 New/Improved Features:
 - Fully hierarchical bi-directional conversion to YAML
 - Automatic snapping to grid thanks to KLayout
 - More features for vector geometries due to concept of Point/Edge/Vector/Polygon from Klayout
 - Easy booleans thanks to KLayout Regions
@@ -29,23 +36,23 @@
   which are built into KLayout
 
 
 ## Installation
 
 kfactory is available on [pypi](https://pypi.org/project/kfactory/)
 
-```
+```bash
 pip install kfactory
 ```
 
 At the moment kfactory works only on python 3.10
 
 ### Development Installation
 
 
 A development environment can be installed with
 
-```
-python -m pip install .[dev]
+```bash
+python -m pip install -e .[dev]
 ```
 
 It is defined in `pyproject.toml`. For committing `pre-commit` should be installed with `pre-commit install`.
```

### Comparing `kfactory-0.7.0/docs/_static/complex.png` & `kfactory-0.7.1/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/_static/klive.webm` & `kfactory-0.7.1/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/_static/waveguide.png` & `kfactory-0.7.1/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/complex_cell.py` & `kfactory-0.7.1/docs/source/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/config.md` & `kfactory-0.7.1/docs/source/config.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/gen_ref_pages.py` & `kfactory-0.7.1/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/index.md` & `kfactory-0.7.1/src/kfactory.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,49 @@
-# KFactory 0.6.3
+Metadata-Version: 2.1
+Name: kfactory
+Version: 0.7.1
+Summary: KLayout API implementation of gdsfactory
+Author-email: gdsfactory community <contact@gdsfactory.com>
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: git
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: ci
+Provides-Extra: ipy
+License-File: LICENSE
+
+# KFactory 0.7.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
+| :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
+|---------------------------------------------------------------------------------------------------------------------------------|
+
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.1` for example.
+
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
+- [x] Jupyter integration
+- [x] PDK/package configuration
+- [x] Plugin system (simulations etc.) - Check [kplugins](https://github.com/gdsfactory/kplugins)
+- [x] Generic PDK example - Check [kgeneric](https://github.com/gdsfactory/kgeneric)
 
 
 Notable missing Features:
-- [ ] PDK/package configuration
+
 - [ ] CrossSection
 - [ ] Netlist/Schematics and LVS
 - [ ] More advanced routing
-- [ ] Plugin system (simulations etc.)
-- [ ] Jupyter integration
 
 
 New/Improved Features:
 - Fully hierarchical bi-directional conversion to YAML
 - Automatic snapping to grid thanks to KLayout
 - More features for vector geometries due to concept of Point/Edge/Vector/Polygon from Klayout
 - Easy booleans thanks to KLayout Regions
@@ -29,23 +52,23 @@
   which are built into KLayout
 
 
 ## Installation
 
 kfactory is available on [pypi](https://pypi.org/project/kfactory/)
 
-```
+```bash
 pip install kfactory
 ```
 
 At the moment kfactory works only on python 3.10
 
 ### Development Installation
 
 
 A development environment can be installed with
 
-```
-python -m pip install .[dev]
+```bash
+python -m pip install -e .[dev]
 ```
 
 It is defined in `pyproject.toml`. For committing `pre-commit` should be installed with `pre-commit install`.
```

### Comparing `kfactory-0.7.0/docs/intro.md` & `kfactory-0.7.1/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/notebooks/00_geometry.py` & `kfactory-0.7.1/docs/source/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/notebooks/01_references.py` & `kfactory-0.7.1/docs/source/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/notebooks/02_DRC.py` & `kfactory-0.7.1/docs/source/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/notebooks/03_Enclosures.py` & `kfactory-0.7.1/docs/source/notebooks/03_Enclosures.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/star.py` & `kfactory-0.7.1/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/docs/waveguide.py` & `kfactory-0.7.1/docs/source/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/mkdocs.yml` & `kfactory-0.7.1/docs/mkdocs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,52 @@
-site_name: KFactory 0.6.3
+site_name: KFactory
+repo_url: https://github.com/gdsfactory/kfactory
+site_url: https://gdsfactory.github.io/kfactory
+docs_dir: source
 
 nav:
   - Home: index.md
+  - First Steps:
+    - Prerequisites: pre.md
+    - 5min Intro to KFactory: intro.md
   - Tutorials:
     - Basice Geometry in KLayout: notebooks/00_geometry.py
     - KCell & Instance: notebooks/01_references.py
     - DRC utils: notebooks/02_DRC.py
     - Enclosures: notebooks/03_Enclosures.py
+  - Config Class: config.md
   - API: reference/
 theme:
   name: "material"
   features:
     - navigation.tabs
     - navigation.tabs.sticky
+  custom_dir: overrides
 
-  markdown_extensions:
-    - pymdownx.superfences
-    - pymdownx.tasklist
-    - pymdownx.tabbed
   palette:
     # Palette toggle for dark mode
     - scheme: slate
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
    # Palette toggle for light mode
     - scheme: default
       toggle:
         icon: material/brightness-7
         name: Switch to dark mode
 watch:
-  - src/kfactory
+  - ../src/kfactory
+
+markdown_extensions:
+  - pymdownx.superfences
+  - pymdownx.tasklist
+  - pymdownx.tabbed
+  - pymdownx.emoji
+  - pymdownx.snippets:
+      check_paths: true
 
 plugins:
   - mkdocstrings:
       enabled: true
       custom_templates: templates
       default_handler: python
       handlers:
@@ -48,23 +60,26 @@
             show_signature_annotations: true
             preload_modules:
               - klayout.db
               - klayout.lay
             members_order: alphabetical
   - gen-files:
       scripts:
-        - docs/gen_ref_pages.py
-  - mkdocs-video
+        - source/gen_ref_pages.py
+  - mkdocs-video:
+      is_video: true
+      video_type: webm
+      video_muted: true
   - search
   - mkdocs-jupyter:
       include_source: true
       # ignore_h1_titles: true
       include_requirejs: true
       execute: true
       allow_errors: false
       kernel_name: python3
       execute_ignore:
-        - "docs/*.py"
-      ignore: ["docs/*.py"]
+        - "source/*.py"
+      ignore: ["source/*.py"]
   - literate-nav:
       nav_file: SUMMARY.md
   - section-index
```

### Comparing `kfactory-0.7.0/pyproject.toml` & `kfactory-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.7.0"
+version = "0.7.1"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
@@ -49,14 +49,15 @@
 	"mkdocs-jupyter>=0.24",
   "mkdocstrings[python]",
   "mkdocs-material",
   "mkdocs_gen_files",
 	"mkdocs-literate-nav",
 	"mkdocs-section-index",
 	"mkdocs-video",
+	"pymdown-extensions",
 ]
 ci = [
 	"flake8",
 	"flake8-pyproject",
 	"pytest",
 	"pytest_regressions",
 	"mypy",
```

### Comparing `kfactory-0.7.0/src/kfactory/__init__.py` & `kfactory-0.7.1/src/kfactory/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     LayerEnum,
     show,
 )
 from . import cells, placer, routing, utils, port, pdk
 from .conf import config
 from .pdk import Pdk
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
```

### Comparing `kfactory-0.7.0/src/kfactory/cells/bezier.py` & `kfactory-0.7.1/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/cells/circular.py` & `kfactory-0.7.1/src/kfactory/cells/circular.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/cells/dbu/taper.py` & `kfactory-0.7.1/src/kfactory/cells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/cells/dbu/waveguide.py` & `kfactory-0.7.1/src/kfactory/cells/dbu/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/cells/euler.py` & `kfactory-0.7.1/src/kfactory/cells/euler.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/cells/taper.py` & `kfactory-0.7.1/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/cells/waveguide.py` & `kfactory-0.7.1/src/kfactory/cells/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/conf.py` & `kfactory-0.7.1/src/kfactory/conf.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/kcell.py` & `kfactory-0.7.1/src/kfactory/kcell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/pdk.py` & `kfactory-0.7.1/src/kfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/placer.py` & `kfactory-0.7.1/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/port.py` & `kfactory-0.7.1/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/routing/electrical.py` & `kfactory-0.7.1/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/routing/manhattan.py` & `kfactory-0.7.1/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/routing/optical.py` & `kfactory-0.7.1/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/technology/klayout_tech.py` & `kfactory-0.7.1/src/kfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/technology/layer_map.py` & `kfactory-0.7.1/src/kfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/technology/layer_stack.py` & `kfactory-0.7.1/src/kfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/technology/layer_views.py` & `kfactory-0.7.1/src/kfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/technology/xml_utils.py` & `kfactory-0.7.1/src/kfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/technology/yaml_utils.py` & `kfactory-0.7.1/src/kfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/typings.py` & `kfactory-0.7.1/src/kfactory/typings.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/utils/__init__.py` & `kfactory-0.7.1/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/utils/enclosure.py` & `kfactory-0.7.1/src/kfactory/utils/enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/utils/fill.py` & `kfactory-0.7.1/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/utils/simplify.py` & `kfactory-0.7.1/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/utils/violations.py` & `kfactory-0.7.1/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory/widgets/interactive.py` & `kfactory-0.7.1/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.7.1/src/kfactory.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 .bumpversion.cfg
 .gitignore
 .pre-commit-config.yaml
 .sourcery.yaml
 LICENSE
 Makefile
 README.md
-mkdocs.yml
 pyproject.toml
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/pages.yml
 .github/workflows/release.yml
 .github/workflows/test_code.yml
-docs/CHANGELOG.md
-docs/_config.yml
-docs/_toc.yml
-docs/complex_cell.py
-docs/config.md
-docs/gen_ref_pages.py
-docs/index.md
-docs/intro.md
-docs/klive.md
-docs/layers.py
-docs/star.py
-docs/waveguide.py
-docs/_static/complex.png
-docs/_static/klive.webm
-docs/_static/waveguide.png
-docs/notebooks/00_geometry.py
-docs/notebooks/01_references.py
-docs/notebooks/02_DRC.py
-docs/notebooks/03_Enclosures.py
+docs/mkdocs.yml
+docs/overrides/main.html
+docs/source/CHANGELOG.md
+docs/source/complex_cell.py
+docs/source/config.md
+docs/source/gen_ref_pages.py
+docs/source/index.md
+docs/source/intro.md
+docs/source/layers.py
+docs/source/pre.md
+docs/source/star.py
+docs/source/waveguide.py
+docs/source/_static/complex.png
+docs/source/_static/klive.webm
+docs/source/_static/waveguide.png
+docs/source/notebooks/00_geometry.py
+docs/source/notebooks/01_references.py
+docs/source/notebooks/02_DRC.py
+docs/source/notebooks/03_Enclosures.py
 src/kfactory/__init__.py
 src/kfactory/conf.py
 src/kfactory/kcell.py
 src/kfactory/pdk.py
 src/kfactory/placer.py
 src/kfactory/port.py
 src/kfactory/py.typed
```

### Comparing `kfactory-0.7.0/src/kfactory.egg-info/requires.txt` & `kfactory-0.7.1/src/kfactory.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 mkdocs-jupyter>=0.24
 mkdocstrings[python]
 mkdocs-material
 mkdocs_gen_files
 mkdocs-literate-nav
 mkdocs-section-index
 mkdocs-video
+pymdown-extensions
 
 [git]
 gitpython
 
 [ipy]
 ipython
 ipywidgets
```

### Comparing `kfactory-0.7.0/tests/conftest.py` & `kfactory-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_cells.py` & `kfactory-0.7.1/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_cplxcells.py` & `kfactory-0.7.1/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_enclosure.py` & `kfactory-0.7.1/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_extrude.py` & `kfactory-0.7.1/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_pdk.py` & `kfactory-0.7.1/tests/test_pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_ports.py` & `kfactory-0.7.1/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_rename.py` & `kfactory-0.7.1/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_routing.py` & `kfactory-0.7.1/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.0/tests/test_spiral.py` & `kfactory-0.7.1/tests/test_spiral.py`

 * *Files identical despite different names*

