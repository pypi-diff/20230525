# Comparing `tmp/physrisk-lib-0.7.0.tar.gz` & `tmp/physrisk-lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physrisk-lib-0.7.0.tar", last modified: Fri Feb  3 16:30:43 2023, max compression
+gzip compressed data, was "physrisk-lib-0.9.0.tar", last modified: Sat Mar 11 21:56:14 2023, max compression
```

## Comparing `physrisk-lib-0.7.0.tar` & `physrisk-lib-0.9.0.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.586968 physrisk-lib-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-02-03 16:30:33.000000 physrisk-lib-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-03 16:30:33.000000 physrisk-lib-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-03 16:30:43.586968 physrisk-lib-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-03 16:30:33.000000 physrisk-lib-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-03 16:30:33.000000 physrisk-lib-0.7.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-03 16:30:43.586968 physrisk-lib-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.566968 physrisk-lib-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.570968 physrisk-lib-0.7.0/src/physrisk/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.570968 physrisk-lib-0.7.0/src/physrisk/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.570968 physrisk-lib-0.7.0/src/physrisk/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/v1/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/v1/example_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/v1/hazard_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/v1/impact_req_resp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.574968 physrisk-lib-0.7.0/src/physrisk/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/api/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.574968 physrisk-lib-0.7.0/src/physrisk/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/colormap_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/geotiff_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.574968 physrisk-lib-0.7.0/src/physrisk/data/hazard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/hazard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/hazard_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/image_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/pregenerated_hazard_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.578968 physrisk-lib-0.7.0/src/physrisk/data/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.578968 physrisk-lib-0.7.0/src/physrisk/data/static/example_portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/static/example_portfolios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.578968 physrisk-lib-0.7.0/src/physrisk/data/static/vulnerability/
--rw-r--r--   0 runner    (1001) docker     (123)    14405 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/static/vulnerability/EU JRC global flood depth-damage functions.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/static/vulnerability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/static/world.json
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/static/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/data/zarr_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.582968 physrisk-lib-0.7.0/src/physrisk/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/asset_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/financial_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/hazard_event_distrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/hazard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/hazards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/impact_distrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/loss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/vulnerability_distrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/vulnerability_matrix_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/kernel/vulnerability_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.582968 physrisk-lib-0.7.0/src/physrisk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/models/chronic_heat_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/models/example_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/models/labour_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/models/power_generating_asset_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/models/real_estate_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.586968 physrisk-lib-0.7.0/src/physrisk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-03 16:30:34.000000 physrisk-lib-0.7.0/src/physrisk/utils/lazy_importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:30:43.586968 physrisk-lib-0.7.0/src/physrisk_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-03 16:30:43.000000 physrisk-lib-0.7.0/src/physrisk_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-02-03 16:30:43.000000 physrisk-lib-0.7.0/src/physrisk_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:30:43.000000 physrisk-lib-0.7.0/src/physrisk_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-03 16:30:43.000000 physrisk-lib-0.7.0/src/physrisk_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-03 16:30:43.000000 physrisk-lib-0.7.0/src/physrisk_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.146765 physrisk-lib-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.146765 physrisk-lib-0.9.0/src/physrisk/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.146765 physrisk-lib-0.9.0/src/physrisk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.146765 physrisk-lib-0.9.0/src/physrisk/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v1/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v1/example_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v1/hazard_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v1/hazard_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v1/impact_req_resp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.146765 physrisk-lib-0.9.0/src/physrisk/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/api/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/colormap_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/geotiff_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/data/hazard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/hazard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/hazard_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/image_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22906 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/inventory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/pregenerated_hazard_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/data/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/data/static/example_portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/static/example_portfolios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/data/static/vulnerability/
+-rw-r--r--   0 runner    (1001) docker     (123)    14405 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/static/vulnerability/EU JRC global flood depth-damage functions.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/static/vulnerability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/static/world.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/static/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/data/zarr_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/asset_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/financial_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/hazard_event_distrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/hazard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/hazards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/impact_distrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/loss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/vulnerability_distrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/vulnerability_matrix_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/kernel/vulnerability_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/models/chronic_heat_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/models/example_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/models/labour_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/models/power_generating_asset_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/models/real_estate_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-11 21:56:06.000000 physrisk-lib-0.9.0/src/physrisk/utils/lazy_importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 21:56:14.150765 physrisk-lib-0.9.0/src/physrisk_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-11 21:56:14.000000 physrisk-lib-0.9.0/src/physrisk_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-03-11 21:56:14.000000 physrisk-lib-0.9.0/src/physrisk_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 21:56:14.000000 physrisk-lib-0.9.0/src/physrisk_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-11 21:56:14.000000 physrisk-lib-0.9.0/src/physrisk_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-11 21:56:14.000000 physrisk-lib-0.9.0/src/physrisk_lib.egg-info/top_level.txt
```

### Comparing `physrisk-lib-0.7.0/LICENSE` & `physrisk-lib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/PKG-INFO` & `physrisk-lib-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physrisk-lib
-Version: 0.7.0
+Version: 0.9.0
 Summary: Physical risk calculation engine
 Home-page: https://github.com/os-climate/physrisk
 Author: OS-Climate
 Author-email: joe.moorhouse@gmail.com
 Project-URL: Bug Tracker, https://github.com/os-climate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `physrisk-lib-0.7.0/README.md` & `physrisk-lib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/pyproject.toml` & `physrisk-lib-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/setup.cfg` & `physrisk-lib-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/api/v1/common.py` & `physrisk-lib-0.9.0/src/physrisk/api/v1/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,23 @@
 
 class Assets(BaseModel):
     """Defines a collection of assets."""
 
     items: List[Asset]
 
 
+class BaseHazardRequest(BaseModel):
+    group_ids: List[str] = Field(
+        ["public"],
+        description="""List of data groups which can be used to service the request,
+            e.g. 'osc': available to OS-Climate members (e.g. pending license decision),
+                 'public'.""",
+    )
+
+
 class Country(BaseModel):
     """Country information."""
 
     country: str
     continent: str
     country_iso_a3: str
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/api/v1/hazard_data.py` & `physrisk-lib-0.9.0/src/physrisk/api/v1/hazard_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from enum import Flag, auto
+from pathlib import PosixPath
 from typing import Dict, List, Optional, Tuple
 
 from pydantic import BaseModel, Field
 
-from physrisk.api.v1.common import IntensityCurve
+from physrisk.api.v1.common import BaseHazardRequest, IntensityCurve
+
+# region HazardModel
 
 
 class Colormap(BaseModel):
     """Provides details of colormap."""
 
     min_index: Optional[int] = Field(
         1, description="Value of colormap minimum. Constant min for a group of maps can facilitate comparison."
@@ -23,30 +26,30 @@
     )
     name: str = Field(description="Name of colormap, e.g. 'flare', 'heating'.")
     nodata_index: Optional[int] = Field(0, description="Index used for no data.")
     units: str = Field(description="Units, e.g. 'degree days', 'metres'.")
 
 
 class MapInfo(BaseModel):
-    """Provides information about map layer"""
+    """Provides information about map layer."""
 
     colormap: Optional[Colormap] = Field(description="Details of colormap.")
     array_name: Optional[str] = Field(
         description="Name of array reprojected to Web Mercator for on-the-fly display or to hash to obtain tile ID. If not supplied, convention is to add '_map' to array_name."  # noqa
     )
     bounds: Optional[List[Tuple[float, float]]] = Field(
         [[-180.0, 85.0], [180.0, 85.0], [180.0, -85.0], [-180.0, -85.0]],
         description="Bounds (top/left, top/right, bottom/right, bottom/left) as degrees. Note applied to map reprojected into Web Mercator CRS.",  # noqa
     )
     # note that the bounds should be consistent with the array attributes
     source: Optional[str] = Field(description="Source of map image: 'map_array' or 'tiles'.")
 
 
 class Period(BaseModel):
-    """A period belonging to a scenario"""
+    """Provides information about a period, which currently corresponds to a year, belonging to a scenario."""
 
     year: int
     map_id: str = Field(description="If present, identifier to be used for looking up map tiles from server.")
 
 
 class Scenario(BaseModel):
     """Scenario ID and the list of available years for that scenario e.g. RCP8.5 = 'rcp8.5'"""
@@ -56,24 +59,25 @@
     periods: Optional[List[Period]]
 
 
 def expanded(item: str, key: str, param: str):
     return item and item.replace("{" + key + "}", param)
 
 
-class HazardModel(BaseModel):
-    """Provides the scenarios associated with a hazard model."""
+class HazardResource(BaseModel):
+    """Describes a set of data arrays that provide models of a hazard."""
 
-    type: Optional[str] = Field(description="Type of hazard.")
+    type: str = Field(description="Type of hazard.")
+    group_id: Optional[str] = Field("public")
     path: str
     id: str
     params: Optional[Dict[str, List[str]]]
     display_name: str
     description: str
-    array_name: Optional[str]  # alias of filename
+    array_name: str
     map: Optional[MapInfo]
     scenarios: List[Scenario]
     units: str
 
     def expand(self):
         # should be only one key
         if not self.params:
@@ -88,54 +92,77 @@
                     "id": expanded(self.id, key, param),
                     "display_name": expanded(self.display_name, key, param),
                     "array_name": expanded(self.array_name, key, param),
                     "map": self.map.copy(deep=True, update={"array_name": expanded(self.map.array_name, key, param)}),
                 },
             )
 
+    def key(self):
+        return str(PosixPath(self.path, self.id))
+
+
+# endregion
+
 
 # region HazardAvailability
 
 
 class InventorySource(Flag):
     """Source of inventory. Where multiple are selected, order is as shown:
     results from HAZARD_TEST override those of HAZARD and EMBEDDED (to facilitate testing).
     """
 
     EMBEDDED = auto()  # inventory embedded in physrisk
     HAZARD = auto()  # inventory stored in the S3 hazard location
     HAZARD_TEST = auto()  # inventory stored in the S3 hazard_test location
 
 
-class HazardEventAvailabilityRequest(BaseModel):
-    event_types: Optional[List[str]]  # e.g. RiverineInundation
-    source: Optional[InventorySource]
+class HazardAvailabilityRequest(BaseModel):
+    types: Optional[List[str]]  # e.g. ["RiverineInundation"]
+    sources: Optional[List[str]] = Field(
+        description="Sources of inventory, can be 'embedded', 'hazard' or 'hazard_test'."
+    )
 
 
-class HazardEventAvailabilityResponse(BaseModel):
-    models: List[HazardModel]
+class HazardAvailabilityResponse(BaseModel):
+    models: List[HazardResource]
     colormaps: dict
 
 
 # endregion
 
+
+# region HazardDescription
+
+
+class HazardDescriptionRequest(BaseModel):
+    paths: List[str] = Field(description="List of paths to markdown objects.")
+
+
+class HazardDescriptionResponse(BaseModel):
+    descriptions: Dict[str, str] = Field(description="For each path (key), the description markdown (value).")
+
+
+# endregion
+
+
 # region HazardEventData
 
 
 class HazardEventDataRequestItem(BaseModel):
     longitudes: List[float]
     latitudes: List[float]
     request_item_id: str
     event_type: str  # e.g. RiverineInundation
     model: str
     scenario: str  # e.g. rcp8p5
     year: int
 
 
-class HazardEventDataRequest(BaseModel):
+class HazardEventDataRequest(BaseHazardRequest):
     interpolation: str = "floor"
     items: List[HazardEventDataRequestItem]
 
 
 class HazardEventDataResponseItem(BaseModel):
     intensity_curve_set: List[IntensityCurve]
     request_item_id: str
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/api/v1/impact_req_resp.py` & `physrisk-lib-0.9.0/src/physrisk/api/v1/impact_req_resp.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/colormap_provider.py` & `physrisk-lib-0.9.0/src/physrisk/data/colormap_provider.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/geotiff_reader.py` & `physrisk-lib-0.9.0/src/physrisk/data/geotiff_reader.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/hazard_data_provider.py` & `physrisk-lib-0.9.0/src/physrisk/data/hazard_data_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
 from abc import ABC
-from typing import List, MutableMapping, Optional
+from pathlib import PosixPath
+from typing import Dict, List, MutableMapping, Optional
 
 from typing_extensions import Protocol
 
+from physrisk.data.inventory import Inventory
+from physrisk.kernel import hazards
+
 from .zarr_reader import ZarrReader
 
 
 class SourcePath(Protocol):
     """Provides path to hazard event data source. Each source should have its own implementation.
     Args:
         model: model identifier.
@@ -182,7 +186,25 @@
         return _osc_chronic_heat_prefix() + "/" + f"{type}_{levels[0]}_{scenario}_{year}"
 
     else:
         raise ValueError("valid types are {valid_types}")
 
 
 # endregion
+
+
+def get_source_path_generic(inventory: Inventory, hazard_type: str, embedded: Optional[Dict[type, SourcePath]]):
+    resources_dict = dict(
+        (id, resources[0])
+        for ((htype, id), resources) in inventory.resources_by_type_id.items()
+        if htype == hazard_type
+    )
+
+    def get_source_path(*, model: str, scenario: str, year: int):
+        if model not in resources_dict:
+            if embedded is None:
+                return None
+            return embedded[hazards.hazard_class(hazard_type)](model=model, scenario=scenario, year=year)
+        resource = resources_dict[model]
+        return str(PosixPath(resource.path, resource.array_name.format(id=model, scenario=scenario, year=year)))
+
+    return get_source_path
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/image_creator.py` & `physrisk-lib-0.9.0/src/physrisk/data/image_creator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,92 @@
 import io
 from typing import Callable, List, MutableMapping, Optional
 
 import numpy as np
+import PIL.Image as Image
 import zarr.storage
-from PIL import Image
 
 from physrisk.data import colormap_provider
 from physrisk.data.zarr_reader import ZarrReader
 
 
 class ImageCreator:
     """Convert small arrays into images for map display.
-    Intended for arrays <~1500x1500 (otherwise, recommended to use Mapbox tiles).
+    Intended for arrays <~1500x1500 (otherwise, recommended to use Mapbox tiles - or similar).
     """
 
     def __init__(self, store: Optional[MutableMapping] = None):
         self.reader = ZarrReader(store=store)
 
     def convert(
         self,
-        path,
+        path: str,
         format="PNG",
         colormap: str = "heating",
         min_value: Optional[float] = None,
         max_value: Optional[float] = None,
     ) -> bytes:
+        """Create image for path specified as array of bytes.
+
+        Args:
+            resource (str): Full path to array.
+            format (str, optional): Image format. Defaults to "PNG".
+            colormap (str, optional): Colormap name. Defaults to "heating".
+            min_value (Optional[float], optional): Min value. Defaults to None.
+            max_value (Optional[float], optional): Max value. Defaults to None.
+
+        Returns:
+            bytes: Image data.
+        """
+        image = self._to_image(path, colormap, min_value=min_value, max_value=max_value)
+        image_bytes = io.BytesIO()
+        image.save(image_bytes, format=format)
+        return image_bytes.getvalue()
+
+    def to_file(
+        self,
+        filename: str,
+        path: str,
+        format="PNG",
+        colormap: str = "heating",
+        min_value: Optional[float] = None,
+        max_value: Optional[float] = None,
+    ):
+        """Create image for path specified and save as file.
+
+        Args:
+            filename (str): Filename.
+            path (str): Path to array.
+            format (str, optional): Image format. Defaults to "PNG".
+            colormap (str, optional): Colormap name. Defaults to "heating".
+            min_value (Optional[float], optional): Min value. Defaults to None.
+            max_value (Optional[float], optional): Max value. Defaults to None.
+        """
+        image = self._to_image(path, colormap, min_value=min_value, max_value=max_value)
+        image.save(filename, format=format)
+
+    def _to_image(
+        self, path, colormap: str = "heating", min_value: Optional[float] = None, max_value: Optional[float] = None
+    ) -> Image.Image:
         """Get image for path specified as array of bytes."""
         data = self.reader.all_data(path)
         if len(data.shape) == 3:
             data = data[:, :, :].squeeze(axis=0)
         if any(dim > 1500 for dim in data.shape):
             raise Exception("dimension too large (over 1500).")
         map_defn = colormap_provider.colormap(colormap)
 
         def get_colors(index: int):
             return map_defn[str(index)]
 
-        rgba = self.to_rgba(data, get_colors, min_value=min_value, max_value=max_value)
+        rgba = self._to_rgba(data, get_colors, min_value=min_value, max_value=max_value)
         image = Image.fromarray(rgba, mode="RGBA")
-        image_bytes = io.BytesIO()
-        image.save(image_bytes, format=format)
-        return image_bytes.getvalue()
-        # final = image_bytes.read()
-        # image.save("test_image.tiff", format='TIFF')
+        return image
 
-    def to_rgba(  # noqa: C901
+    def _to_rgba(  # noqa: C901
         self,
         data: np.ndarray,
         get_colors: Callable[[int], List[int]],
         min_value: Optional[float] = None,
         max_value: Optional[float] = None,
         nodata_lower: Optional[float] = None,
         nodata_upper: Optional[float] = None,
@@ -84,24 +122,24 @@
         a = np.zeros(256, dtype=np.uint32)
         for i in range(256):
             (red[i], green[i], blue[i], a[i]) = get_colors(i)
         if nodata_bin_transparent:
             a[0] = 0
         if min_bin_transparent:
             a[1] = 0
-        mask_nodata = None
+        mask_nodata = np.isnan(data)
         if nodata_lower:
             mask_nodata = data <= nodata_lower
         if nodata_upper:
             mask_nodata = (mask_nodata | (data >= nodata_upper)) if mask_nodata is not None else (data >= nodata_upper)
 
         if min_value is None:
-            min_value = data.min()
+            min_value = np.nanmin(data)
         if max_value is None:
-            max_value = data.max()
+            max_value = np.nanmax(data)
 
         mask_ge_max = data >= max_value
         mask_le_min = data <= min_value
 
         np.add(data, -min_value, out=data)
         np.multiply(data, 253.0 / (max_value - min_value), out=data)
         np.add(data, 2.0, out=data)  # np.clip seems a bit slow so we do not use
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/inventory.py` & `physrisk-lib-0.9.0/src/physrisk/data/inventory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # flake8: noqa: E501
 import hashlib
-from typing import List
+from collections import defaultdict
+from pathlib import PosixPath
+from typing import DefaultDict, Dict, Iterable, List, Tuple
 
 from pydantic import parse_obj_as
 
 import physrisk.data.colormap_provider as colormap_provider
 
-from ..api.v1.hazard_data import HazardModel, Period
+from ..api.v1.hazard_data import HazardResource, Period
 
 methodology_doc = """
 For more details and relevant citations see the
 [OS-Climate Physical Climate Risk Methodology document](https://github.com/os-climate/physrisk/blob/main/methodology/PhysicalRiskMethodology.pdf).
 """
 
 aqueduct_description = (
@@ -36,16 +38,32 @@
     "max_index": 255,
     "max_value": 2.0,
     "units": "m",
 }
 
 
 class Inventory:
+    def __init__(self, hazard_resources: Iterable[HazardResource]):
+        """Store the hazard resources with look up via:
+        - key: combination of path and model identifier which is unique, or
+        - type and model identifier: (requires choice of provider/version)
+
+        Args:
+            hazard_resources (Iterable[HazardResource]): list of resources
+        """
+        self.resources: Dict[str, HazardResource] = {}
+        self.resources_by_type_id: DefaultDict[Tuple[str, str], List[HazardResource]] = defaultdict(list)
+        for resource in hazard_resources:
+            self.resources[resource.key()] = resource
+            self.resources_by_type_id[(resource.type, resource.id)].append(resource)
+
+
+class EmbeddedInventory:
     """Contains an  of available hazard data.
-    model id is given by {type}/{model group identifier}/{version}/{model identifier}
+    path is given by {type}/{model group identifier}/{version}/{model identifier}
     """
 
     def __init__(self):
         osc_chronic_heat_models = [
             {
                 "type": "ChronicHeat",
                 "path": "chronic_heat/osc/v1",
@@ -100,15 +118,15 @@
 The mean work loss indicator is calculated from the 'Wet Bulb Globe Temperature' (WBGT) indicator:
 $$
 I^\\text{WBGT}_i = 0.567 \\times T^\\text{avg}_i + 0.393 \\times P^\\text{vapour}_i
 $$
 $I^\\text{WBGT}_i$ is the WBGT indicator, $T^\\text{avg}_i$ is the daily average surface temperature (in degress Celsius) on day index, $i$, and $P^\\text{vapour}$
 is the water vapour partial pressure (in kPa). $P^\\text{vapour}$ is calculated from relative humidity $H_R$ via:
 $$
-P^\\text{vapour}_i = \\frac{H_R}{100} \\times 6.105 \\times \\exp \\left( \\frac{17.27 \\times T^\\text{avg}_i}{237.7 \\times T^\\text{avg}_i} \\right)
+P^\\text{vapour}_i = \\frac{H_R}{100} \\times 6.105 \\times \\exp \\left( \\frac{17.27 + T^\\text{avg}_i}{237.7 + T^\\text{avg}_i} \\right)
 $$
 The work ability indicator, $I^{\\text{WA}}$ is finally calculated via:
 $$
 I^{\\text{WA}}_i = 0.1 + 0.9 / \\left( 1 + (I^\\text{WBGT}_i / \\alpha_1)^{\\alpha_2} \\right)
 $$
 An annual average work ability indicator, $I^{\\text{WA}}$ is calculated via:
 $$
@@ -141,15 +159,15 @@
                 ],
             },
         ]
 
         wri_riverine_inundation_models = [
             {
                 "type": "RiverineInundation",
-                "path": "riverine_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "000000000WATCH",
                 "display_name": "WRI/Baseline",
                 "description": """
 World Resources Institute Aqueduct Floods baseline riverine model using historical data.
 
                 """
                 + aqueduct_description,
@@ -160,15 +178,15 @@
                     "source": "mapbox",
                 },
                 "units": "metres",
                 "scenarios": [{"id": "historical", "years": [1980], "periods": [{"year": 1980, "map_id": "gw4vgq"}]}],
             },
             {
                 "type": "RiverineInundation",
-                "path": "riverine_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "00000NorESM1-M",
                 "display_name": "WRI/NorESM1-M",
                 "description": """
 World Resources Institute Aqueduct Floods riverine model using GCM model from
 Bjerknes Centre for Climate Research, Norwegian Meteorological Institute.
 
                 """
@@ -183,15 +201,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "RiverineInundation",
-                "path": "riverine_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "0000GFDL-ESM2M",
                 "display_name": "WRI/GFDL-ESM2M",
                 "description": """
 World Resource Institute Aqueduct Floods riverine model using GCM model from
 Geophysical Fluid Dynamics Laboratory (NOAA).
 
                 """
@@ -205,15 +223,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "RiverineInundation",
-                "path": "riverine_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "0000HadGEM2-ES",
                 "display_name": "WRI/HadGEM2-ES",
                 "description": """
 World Resource Institute Aqueduct Floods riverine model using GCM model:
 Met Office Hadley Centre.
 
                 """
@@ -228,15 +246,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "RiverineInundation",
-                "path": "riverine_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "00IPSL-CM5A-LR",
                 "display_name": "WRI/IPSL-CM5A-LR",
                 "description": """
 World Resource Institute Aqueduct Floods riverine model using GCM model from
 Institut Pierre Simon Laplace
 
                 """
@@ -251,15 +269,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "RiverineInundation",
-                "path": "riverine_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "MIROC-ESM-CHEM",
                 "display_name": "WRI/MIROC-ESM-CHEM",
                 "description": """World Resource Institute Aqueduct Floods riverine model using
  GCM model from Atmosphere and Ocean Research Institute
  (The University of Tokyo), National Institute for Environmental Studies, and Japan Agency
  for Marine-Earth Science and Technology.
 
@@ -286,15 +304,15 @@
                 ],
             },
         ]
 
         wri_coastal_inundation_models = [
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "nosub",
                 "display_name": "WRI/Baseline no subsidence",
                 "description": """
 World Resources Institute Aqueduct Floods baseline coastal model using historical data. Model excludes subsidence.
 
                 """
                 + aqueduct_description,
@@ -305,15 +323,15 @@
                     "source": "mapbox",
                 },
                 "units": "metres",
                 "scenarios": [{"id": "historical", "years": [1980]}],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "nosub/95",
                 "display_name": "WRI/95% no subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods coastal model, exclusing subsidence; 95th percentile sea level rise.
 
                 """
                 + aqueduct_description,
@@ -327,15 +345,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "nosub/5",
                 "display_name": "WRI/5% no subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods coastal model, excluding subsidence; 5th percentile sea level rise.
 
                 """
                 + aqueduct_description,
@@ -349,15 +367,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "nosub/50",
                 "display_name": "WRI/50% no subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods model, excluding subsidence; 50th percentile sea level rise.
 
                 """
                 + aqueduct_description,
@@ -371,15 +389,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "wtsub",
                 "display_name": "WRI/Baseline with subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods model, excluding subsidence; baseline (based on historical data).
 
                 """
                 + aqueduct_description,
@@ -390,15 +408,15 @@
                     "source": "mapbox",
                 },
                 "units": "metres",
                 "scenarios": [{"id": "historical", "years": [1980]}],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "wtsub/95",
                 "display_name": "WRI/95% with subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods model, including subsidence; 95th percentile sea level rise.
 
                 """
                 + aqueduct_description,
@@ -412,15 +430,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "wtsub/5",
                 "display_name": "WRI/5% with subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods model, including subsidence; 5th percentile sea level rise.
 
                 """
                 + aqueduct_description,
@@ -434,15 +452,15 @@
                 "scenarios": [
                     {"id": "rcp4p5", "years": [2030, 2050, 2080]},
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
             {
                 "type": "CoastalInundation",
-                "path": "coastal_inundation/wri/v2",
+                "path": "inundation/wri/v2",
                 "id": "wtsub/50",
                 "display_name": "WRI/50% with subsidence",
                 "description": """
 World Resource Institute Aqueduct Floods model, including subsidence; 50th percentile sea level rise.
 
                 """
                 + aqueduct_description,
@@ -458,16 +476,16 @@
                     {"id": "rcp8p5", "years": [2030, 2050, 2080]},
                 ],
             },
         ]
 
         self.models = osc_chronic_heat_models + wri_riverine_inundation_models + wri_coastal_inundation_models
 
-    def to_hazard_models(self) -> List[HazardModel]:
-        models = parse_obj_as(List[HazardModel], self.models)
+    def to_resources(self) -> List[HazardResource]:
+        models = parse_obj_as(List[HazardResource], self.models)
         expanded_models = [e for model in models for e in model.expand()]
         # we populate map_id hashes programmatically
         for model in expanded_models:
             for scenario in model.scenarios:
                 test_periods = scenario.periods
                 scenario.periods = []
                 for year in scenario.years:
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/pregenerated_hazard_model.py` & `physrisk-lib-0.9.0/src/physrisk/data/pregenerated_hazard_model.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/static/vulnerability/EU JRC global flood depth-damage functions.json` & `physrisk-lib-0.9.0/src/physrisk/data/static/vulnerability/EU JRC global flood depth-damage functions.json`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/static/world.json` & `physrisk-lib-0.9.0/src/physrisk/data/static/world.json`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/static/world.py` & `physrisk-lib-0.9.0/src/physrisk/data/static/world.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/data/zarr_reader.py` & `physrisk-lib-0.9.0/src/physrisk/data/zarr_reader.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/asset_impact.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/asset_impact.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/calculation.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/calculation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import logging
 from collections import defaultdict
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
+from physrisk.data.inventory import Inventory
+from physrisk.kernel import hazards
+
 from ..data.hazard_data_provider import (
+    SourcePath,
+    get_source_path_generic,
     get_source_path_osc_chronic_heat,
     get_source_path_wri_coastal_inundation,
     get_source_path_wri_riverine_inundation,
 )
 from ..data.pregenerated_hazard_model import ZarrHazardModel
 from ..models import power_generating_asset_models as pgam
-from ..models.chronic_heat_models import ChronicHeatGZN
+from ..models.chronic_heat_models import ChronicHeatGznModel
 from ..models.real_estate_models import RealEstateCoastalInundationModel, RealEstateRiverineInundationModel
 from ..utils.helpers import get_iterable
 from .assets import Asset, IndustrialActivity, PowerGeneratingAsset, RealEstateAsset, TestAsset
 from .hazard_event_distrib import HazardEventDistrib
 from .hazard_model import HazardDataRequest, HazardDataResponse, HazardModel
 from .hazards import ChronicHeat, CoastalInundation, RiverineInundation
 from .impact_distrib import ImpactDistrib
@@ -26,39 +31,46 @@
         self,
         impact: ImpactDistrib,
         vulnerability: Optional[VulnerabilityDistrib] = None,
         event: Optional[HazardEventDistrib] = None,
         hazard_data: Optional[Iterable[HazardDataResponse]] = None,
     ):
         self.impact = impact
-        # optional detailed results for drill-dowwn
+        # optional detailed results for drill-down
         self.hazard_data = hazard_data
         self.vulnerability = vulnerability
         self.event = event
 
 
 def get_default_zarr_source_paths():
     return {
         RiverineInundation: get_source_path_wri_riverine_inundation,
         CoastalInundation: get_source_path_wri_coastal_inundation,
         ChronicHeat: get_source_path_osc_chronic_heat,
     }
 
 
+def get_source_paths_from_inventory(inventory: Inventory, embedded: Optional[Dict[type, SourcePath]] = None):
+    source_paths: Dict[type, SourcePath] = {}
+    for key, resource in inventory.resources.items():
+        source_paths[hazards.hazard_class(resource.type)] = get_source_path_generic(inventory, resource.type, embedded)
+    return source_paths
+
+
 def get_default_hazard_model():
     # Model that gets hazard event data from Zarr storage
     return ZarrHazardModel(get_default_zarr_source_paths())
 
 
 def get_default_vulnerability_models():
     """Get default exposure/vulnerability models for different asset types."""
     return {
         PowerGeneratingAsset: [pgam.InundationModel()],
         RealEstateAsset: [RealEstateCoastalInundationModel(), RealEstateRiverineInundationModel()],
-        IndustrialActivity: [ChronicHeatGZN()],
+        IndustrialActivity: [ChronicHeatGznModel()],
         TestAsset: [pgam.TemperatureModel()],
     }
 
 
 def calculate_impacts(  # noqa: C901
     assets: Iterable[Asset],
     hazard_model: Optional[HazardModel] = None,
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/curve.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/curve.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/financial_model.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/financial_model.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/hazard_event_distrib.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/hazard_event_distrib.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/hazard_model.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/hazard_model.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/hazards.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/hazards.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from enum import Enum
 from typing import cast
 
 
 class HazardKind(Enum):
     acute = (1,)
     chronic = 2
@@ -14,29 +15,59 @@
 
 class Hazard:
     @staticmethod
     def kind(hazard_type):
         return cast(HazardKind, hazard_type.kind)
 
 
-class Drought(Hazard):
+class Inundation(Hazard):
+    kind = HazardKind.acute
+    pass
+
+
+class CoastalInundation(Inundation):
+    kind = HazardKind.acute
     pass
 
 
 class ChronicHeat(Hazard):
     kind = HazardKind.chronic
     pass
 
 
-class Inundation(Hazard):
-    kind = HazardKind.acute
+class CombinedInundation(Hazard):
+    kind = HazardKind.chronic
+    pass
+
+
+class Drought(Hazard):
+    kind = HazardKind.chronic
+    pass
+
+
+class Fire(Hazard):
+    kind = HazardKind.chronic
+    pass
+
+
+class Hail(Hazard):
+    kind = HazardKind.chronic
+    pass
+
+
+class Precipitation(Hazard):
+    kind = HazardKind.chronic
     pass
 
 
 class RiverineInundation(Inundation):
     kind = HazardKind.acute
     pass
 
 
-class CoastalInundation(Inundation):
-    kind = HazardKind.acute
+class Wind(Hazard):
+    kind = HazardKind.chronic
     pass
+
+
+def hazard_class(name: str):
+    return getattr(sys.modules[__name__], name)
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/impact_distrib.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/impact_distrib.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/loss_model.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/loss_model.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/vulnerability_distrib.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/vulnerability_distrib.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/vulnerability_matrix_provider.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/vulnerability_matrix_provider.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/kernel/vulnerability_model.py` & `physrisk-lib-0.9.0/src/physrisk/kernel/vulnerability_model.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/models/chronic_heat_models.py` & `physrisk-lib-0.9.0/src/physrisk/models/chronic_heat_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from physrisk.kernel.assets import Asset
 from physrisk.kernel.hazard_model import HazardDataRequest, HazardDataResponse
 from physrisk.kernel.hazards import ChronicHeat
 from physrisk.kernel.impact_distrib import ImpactDistrib, ImpactType
 from physrisk.kernel.vulnerability_model import VulnerabilityModelBase
 
 
-class ChronicHeatGZN(VulnerabilityModelBase):
+class ChronicHeatGznModel(VulnerabilityModelBase):
     """Model which estiamtes the labour productivity impact based on chronic heat based on the paper "Neidell M,
     Graff Zivin J, Sheahan M,  Willwerth J, Fant C, Sarofim M, et al. (2021) Temperature and work:
     Time allocated to work under varying climate and labor market conditions."
     Average annual work hours are based on USA values reported by the OECD for 2021."""
 
     def __init__(self, model: str = "mean_degree_days_above_32c", delta=True):
         super().__init__(model, ChronicHeat)  # opportunity to give a model hint, but blank here
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/models/example_models.py` & `physrisk-lib-0.9.0/src/physrisk/models/example_models.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/models/power_generating_asset_models.py` & `physrisk-lib-0.9.0/src/physrisk/models/power_generating_asset_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,13 +76,18 @@
 
         vul = VulnerabilityDistrib(RiverineInundation, depth_bins, impact_bins, np.diag(probs_protected))
         event = HazardEventDistrib(RiverineInundation, depth_bins, probs)
 
         return vul, event
 
 
+class WindTurbineModel:
+    def prob_collapse(self, turbine: Asset, wind_speed_hub: np.ndarray):
+        pass
+
+
 @applies_to_events([ChronicHeat])
 @applies_to_assets([PowerGeneratingAsset])
 class TemperatureModel(DeterministicVulnerabilityModel):
     def __init__(self):
         # does nothing
         pass
```

### Comparing `physrisk-lib-0.7.0/src/physrisk/models/real_estate_models.py` & `physrisk-lib-0.9.0/src/physrisk/models/real_estate_models.py`

 * *Files identical despite different names*

### Comparing `physrisk-lib-0.7.0/src/physrisk/requests.py` & `physrisk-lib-0.9.0/src/physrisk/requests.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,177 @@
 import importlib
 import json
+import os
 from importlib import import_module
+from pathlib import PosixPath
 from typing import Any, Dict, List, Optional, cast
 
+import fsspec.implementations.local as local
 import numpy as np
+import zarr
 
 import physrisk.data.static.example_portfolios
 from physrisk.api.v1.common import Distribution, ExceedanceCurve, VulnerabilityDistrib
+from physrisk.api.v1.hazard_image import HazardImageRequest
+from physrisk.data.inventory_reader import InventoryReader
 
 from .api.v1.hazard_data import (
-    HazardEventAvailabilityRequest,
-    HazardEventAvailabilityResponse,
+    HazardAvailabilityRequest,
+    HazardAvailabilityResponse,
+    HazardDescriptionRequest,
+    HazardDescriptionResponse,
     HazardEventDataRequest,
     HazardEventDataResponse,
     HazardEventDataResponseItem,
-    HazardModel,
+    HazardResource,
     IntensityCurve,
-    InventorySource,
 )
 from .api.v1.impact_req_resp import (
     AcuteHazardCalculationDetails,
     AssetImpactRequest,
     AssetImpactResponse,
     AssetLevelImpact,
     Assets,
     AssetSingleHazardImpact,
 )
 from .data.image_creator import ImageCreator
-from .data.inventory import Inventory
+from .data.inventory import EmbeddedInventory, Inventory
 from .data.pregenerated_hazard_model import ZarrHazardModel
 from .kernel import Asset, Hazard
 from .kernel import calculation as calc
 from .kernel.hazard_model import HazardDataRequest
 from .kernel.hazard_model import HazardEventDataResponse as hmHazardEventDataResponse
 from .kernel.hazard_model import HazardParameterDataResponse
 
+# module level singletons, populated/updated on hazard data availability request
+_inventory: Optional[Inventory] = None
+_colormaps: Optional[Dict[str, Any]] = None
+
+# hooks to facilitate testing
+_hazard_test_local_path = ""
+
+
+def _create_inventory_reader():
+    global _hazard_test_local_path
+    if _hazard_test_local_path == "":
+        return InventoryReader()
+    # otherwise, use local test version
+    return InventoryReader(fs=local.LocalFileSystem(), base_path=_hazard_test_local_path)
+
+
+def _create_zarr_store():
+    global _hazard_test_local_path
+    if _hazard_test_local_path == "":
+        return None
+    # otherwise, use local test version
+    return zarr.DirectoryStore(os.path.join(_hazard_test_local_path, "hazard_test", "hazard.zarr"))
+
 
 class NumpyArrayEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return json.JSONEncoder.default(self, obj)
 
 
 def dumps(dict):
     return json.dumps(dict, cls=NumpyArrayEncoder)
 
 
+def hazard_resources() -> Inventory:
+    global _inventory, _colormaps
+    if _inventory is None:
+        _inventory, _colormaps = _get_updated_hazard_resources()
+    return _inventory
+
+
+def colormaps() -> Dict[str, Any]:
+    global _inventory, _colormaps
+    if _colormaps is None:
+        _inventory, _colormaps = _get_updated_hazard_resources(["embedded", "hazard_test"])
+    return _colormaps
+
+
 def get(*, request_id, request_dict, store=None):
+    if store is None:
+        store = _create_zarr_store()
     if request_id == "get_hazard_data":
         request = HazardEventDataRequest(**request_dict)
         return json.dumps(_get_hazard_data(request, store=store).dict())
     elif request_id == "get_hazard_data_availability":
-        request = HazardEventAvailabilityRequest(**request_dict)
+        request = HazardAvailabilityRequest(**request_dict)
         return json.dumps(_get_hazard_data_availability(request).dict())
+    elif request_id == "get_hazard_data_description":
+        request = HazardDescriptionRequest(**request_dict)
+        return json.dumps(_get_hazard_data_description(request).dict())
     elif request_id == "get_asset_impact":
         request = AssetImpactRequest(**request_dict)
         return dumps(_get_asset_impacts(request, store=store).dict())
     elif request_id == "get_example_portfolios":
         return dumps(_get_example_portfolios())
     else:
         raise ValueError(f"request type '{request_id}' not found")
 
 
-def get_image(
-    path: str, colormap: str = "heating", min_value: Optional[float] = None, max_value: Optional[float] = None
-):
-    # creator = ImageCreator(path)
-    creator = ImageCreator()  # store=ImageCreator.test_store(path))
-    return creator.convert(path, colormap=colormap, min_value=min_value, max_value=max_value)
+def get_image(*, request_dict):
+    global _create_zarr_store
+    request = HazardImageRequest(**request_dict)
+    if not _read_permitted(request.group_ids, hazard_resources().resources[request.resource]):
+        raise PermissionError()
+    model = hazard_resources().resources[request.resource]
+    path = str(PosixPath(model.path, model.map.array_name)).format(scenario=request.scenarioId, year=request.year)
+    creator = ImageCreator(_create_zarr_store())  # store=ImageCreator.test_store(path))
+    return creator.convert(path, colormap=request.colormap, min_value=request.min_value, max_value=request.max_value)
+
+
+def _read_permitted(group_ids: List[str], resource: HazardResource):
+    """_summary_
+
+    Args:
+        group_ids (List[str]): Groups to which requester belongs.
+        resourceId (str): Resource identifier.
+
+    Returns:
+        bool: True is requester is permitted access to models comprising resource.
+    """
+    return ("osc" in group_ids) or resource.group_id == "public"
+
+
+def _get_hazard_data_availability(request: HazardAvailabilityRequest):
+    global _inventory, _colormaps
+    _inventory, _colormaps = _get_updated_hazard_resources(request.sources)
+    assert _inventory is not None
+    response = HazardAvailabilityResponse(
+        models=list(_inventory.resources.values()), colormaps=_colormaps
+    )  # type: ignore
+    return response
 
 
-def _get_hazard_data_availability(request: HazardEventAvailabilityRequest):
-    models: Dict[str, HazardModel] = {}
-    colormaps: Dict[str, Dict[str, Any]] = {}
-    request_source = request.source or InventorySource.EMBEDDED
-    for source in InventorySource:
-        if source in request_source:
-            if source == InventorySource.EMBEDDED:
-                inventory = Inventory()
-                for model in inventory.to_hazard_models():
-                    models[model.id] = model
-                colormaps.update(inventory.colormaps())
-            # can add support for S3 reads here
-    response = HazardEventAvailabilityResponse(models=list(models.values()), colormaps=colormaps)  # type: ignore
-    return response
+def _get_hazard_data_description(request: HazardDescriptionRequest):
+    reader = InventoryReader()
+    descriptions = reader.read_description_markdown(request.paths)
+    return HazardDescriptionResponse(descriptions=descriptions)
 
 
 def _get_hazard_data(request: HazardEventDataRequest, source_paths=None, store=None):
-    hazard_model = _create_hazard_model(interpolation=request.interpolation, source_paths=source_paths, store=store)
+    if any(
+        not _read_permitted(request.group_ids, hazard_resources().resources_by_type_id[(i.event_type, i.model)][0])
+        for i in request.items
+    ):
+        raise PermissionError()
+    hazard_model = _create_hazard_model(
+        interpolation=request.interpolation, inventory=hazard_resources(), source_paths=source_paths, store=store
+    )
 
     # get hazard event types:
     event_types = Hazard.__subclasses__()
     event_dict = dict((et.__name__, et) for et in event_types)
     event_dict.update((est.__name__, est) for et in event_types for est in et.__subclasses__())
 
-    # flatten list to let event processer decide how to group
+    # flatten list to let event processor decide how to group
     item_requests = []
     all_requests = []
     for item in request.items:
         event_type = event_dict[item.event_type]
 
         data_requests = [
             HazardDataRequest(event_type, lon, lat, model=item.model, scenario=item.scenario, year=item.year)
@@ -113,15 +185,14 @@
     # responses comes back as a dictionary because requests may be executed in different order to list
     # to optimise performance.
 
     response = HazardEventDataResponse(items=[])
 
     for i, item in enumerate(request.items):
         requests = item_requests[i]
-        # resps = (cast(hmHazardEventDataResponse, response_dict[req]) for req in requests)
         resps = (response_dict[req] for req in requests)
         intensity_curves = [
             IntensityCurve(intensities=list(resp.intensities), return_periods=list(resp.return_periods))
             if isinstance(resp, hmHazardEventDataResponse)
             else IntensityCurve(intensities=[resp.parameter], return_periods=[])
             if isinstance(resp, HazardParameterDataResponse)
             else None
@@ -137,14 +208,34 @@
                 year=item.year,
             )
         )
 
     return response
 
 
+def _get_updated_hazard_resources(sources: Optional[List[str]] = None):
+    global _create_inventory_reader
+    models: List[HazardResource] = []
+    colormaps: Dict[str, Dict[str, Any]] = {}
+    request_sources = ["embedded"] if sources is None else [s.lower() for s in sources]
+    reader = None
+    for source in request_sources:
+        if source == "embedded":
+            inventory = EmbeddedInventory()
+            for model in inventory.to_resources():
+                models.append(model)
+            colormaps.update(inventory.colormaps())
+        elif source == "hazard" or source == "hazard_test":
+            if reader is None:
+                reader = _create_inventory_reader()
+            for model in reader.read(source):
+                models.append(model)
+    return Inventory(models), colormaps
+
+
 def create_assets(assets: Assets):
     """Create list of Asset objects from the Assets API object:"""
     module = import_module("physrisk.kernel.assets")
     asset_objs = []
     for asset in assets.items:
         asset_obj = cast(
             Asset,
@@ -152,18 +243,21 @@
                 asset.latitude, asset.longitude, type=asset.type, location=asset.location
             ),
         )
         asset_objs.append(asset_obj)
     return asset_objs
 
 
-def _create_hazard_model(interpolation="floor", source_paths=None, store=None):
+def _create_hazard_model(interpolation="floor", inventory: Optional[Inventory] = None, source_paths=None, store=None):
     if source_paths is None:
         source_paths = calc.get_default_zarr_source_paths()
 
+    if inventory is not None:
+        source_paths = calc.get_source_paths_from_inventory(inventory, source_paths)
+
     hazard_model = ZarrHazardModel(source_paths, store=store, interpolation=interpolation)
 
     return hazard_model
 
 
 def _get_asset_impacts(request: AssetImpactRequest, source_paths=None, store=None):
     hazard_model = _create_hazard_model(source_paths=source_paths, store=store)
```

### Comparing `physrisk-lib-0.7.0/src/physrisk_lib.egg-info/PKG-INFO` & `physrisk-lib-0.9.0/src/physrisk_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physrisk-lib
-Version: 0.7.0
+Version: 0.9.0
 Summary: Physical risk calculation engine
 Home-page: https://github.com/os-climate/physrisk
 Author: OS-Climate
 Author-email: joe.moorhouse@gmail.com
 Project-URL: Bug Tracker, https://github.com/os-climate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `physrisk-lib-0.7.0/src/physrisk_lib.egg-info/SOURCES.txt` & `physrisk-lib-0.9.0/src/physrisk_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 src/physrisk/__init__.py
 src/physrisk/requests.py
 src/physrisk/api/__init__.py
 src/physrisk/api/v1/__init__.py
 src/physrisk/api/v1/common.py
 src/physrisk/api/v1/example_portfolios.py
 src/physrisk/api/v1/hazard_data.py
+src/physrisk/api/v1/hazard_image.py
 src/physrisk/api/v1/impact_req_resp.py
 src/physrisk/api/v2/__init__.py
 src/physrisk/data/__init__.py
 src/physrisk/data/colormap_provider.py
 src/physrisk/data/geotiff_reader.py
 src/physrisk/data/hazard_data_provider.py
 src/physrisk/data/image_creator.py
 src/physrisk/data/inventory.py
+src/physrisk/data/inventory_reader.py
 src/physrisk/data/pregenerated_hazard_model.py
 src/physrisk/data/zarr_reader.py
 src/physrisk/data/hazard/__init__.py
 src/physrisk/data/static/__init__.py
 src/physrisk/data/static/world.json
 src/physrisk/data/static/world.py
 src/physrisk/data/static/example_portfolios/__init__.py
```

