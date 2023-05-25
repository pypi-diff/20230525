# Comparing `tmp/napari-hdf5-netcdf-viewer-0.1.0.tar.gz` & `tmp/napari-hdf5-netcdf-viewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-hdf5-netcdf-viewer-0.1.0.tar", last modified: Thu May 25 14:03:49 2023, max compression
+gzip compressed data, was "napari-hdf5-netcdf-viewer-0.1.1.tar", last modified: Thu May 25 16:02:49 2023, max compression
```

## Comparing `napari-hdf5-netcdf-viewer-0.1.0.tar` & `napari-hdf5-netcdf-viewer-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,11 @@
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.458721 napari-hdf5-netcdf-viewer-0.1.0/
--rw-rw-r--   0 yunhalee   (501) staff       (20)     1517 2022-10-28 18:43:40.000000 napari-hdf5-netcdf-viewer-0.1.0/LICENSE
--rw-r--r--   0 yunhalee   (501) staff       (20)       96 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.1.0/MANIFEST.in
--rw-r--r--   0 yunhalee   (501) staff       (20)     1262 2023-05-25 14:03:49.458938 napari-hdf5-netcdf-viewer-0.1.0/PKG-INFO
--rw-rw-r--   0 yunhalee   (501) staff       (20)      529 2023-05-25 13:53:44.000000 napari-hdf5-netcdf-viewer-0.1.0/README.md
--rw-r--r--   0 yunhalee   (501) staff       (20)       91 2022-10-11 15:38:42.000000 napari-hdf5-netcdf-viewer-0.1.0/pyproject.toml
--rw-r--r--   0 yunhalee   (501) staff       (20)     1306 2023-05-25 14:03:49.460310 napari-hdf5-netcdf-viewer-0.1.0/setup.cfg
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.451593 napari-hdf5-netcdf-viewer-0.1.0/src/
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.454766 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/
--rw-r--r--   0 yunhalee   (501) staff       (20)      106 2022-10-28 18:32:59.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/__init__.py
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.458301 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/_tests/
--rw-r--r--   0 yunhalee   (501) staff       (20)        0 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/_tests/__init__.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      407 2023-04-11 23:50:14.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/_tests/test_quick_hdf5_netcdf_viewer.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      574 2023-04-11 23:39:29.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/napari.yaml
--rw-r--r--   0 yunhalee   (501) staff       (20)    14965 2023-05-24 16:27:25.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 14:03:49.457349 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/
--rw-r--r--   0 yunhalee   (501) staff       (20)     1262 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yunhalee   (501) staff       (20)      635 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       84 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)      107 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/requires.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       26 2023-05-25 14:03:49.000000 napari-hdf5-netcdf-viewer-0.1.0/src/napari_hdf5_netcdf_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 16:02:49.365298 napari-hdf5-netcdf-viewer-0.1.1/
+-rw-r--r--   0 yunhalee   (501) staff       (20)      433 2023-05-25 16:02:49.365031 napari-hdf5-netcdf-viewer-0.1.1/PKG-INFO
+-rw-r--r--   0 yunhalee   (501) staff       (20)      209 2023-05-25 16:02:34.000000 napari-hdf5-netcdf-viewer-0.1.1/README.md
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-05-25 16:02:49.364681 napari-hdf5-netcdf-viewer-0.1.1/napari_hdf5_netcdf_viewer.egg-info/
+-rw-r--r--   0 yunhalee   (501) staff       (20)      433 2023-05-25 16:02:49.000000 napari-hdf5-netcdf-viewer-0.1.1/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yunhalee   (501) staff       (20)      262 2023-05-25 16:02:49.000000 napari-hdf5-netcdf-viewer-0.1.1/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-05-25 16:02:49.000000 napari-hdf5-netcdf-viewer-0.1.1/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       25 2023-05-25 16:02:49.000000 napari-hdf5-netcdf-viewer-0.1.1/napari_hdf5_netcdf_viewer.egg-info/requires.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-05-25 16:02:49.000000 napari-hdf5-netcdf-viewer-0.1.1/napari_hdf5_netcdf_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       38 2023-05-25 16:02:49.365396 napari-hdf5-netcdf-viewer-0.1.1/setup.cfg
+-rw-r--r--   0 yunhalee   (501) staff       (20)      595 2023-05-25 16:02:34.000000 napari-hdf5-netcdf-viewer-0.1.1/setup.py
```

