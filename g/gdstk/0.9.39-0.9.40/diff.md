# Comparing `tmp/gdstk-0.9.39.tar.gz` & `tmp/gdstk-0.9.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdstk-0.9.39.tar", last modified: Mon Apr 24 17:19:52 2023, max compression
+gzip compressed data, was "gdstk-0.9.40.tar", last modified: Tue Apr 25 15:16:14 2023, max compression
```

## Comparing `gdstk-0.9.39.tar` & `gdstk-0.9.40.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:19:52.293912 gdstk-0.9.39/
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-24 17:19:39.000000 gdstk-0.9.39/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-24 17:19:39.000000 gdstk-0.9.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 17:19:39.000000 gdstk-0.9.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-24 17:19:52.293912 gdstk-0.9.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-24 17:19:39.000000 gdstk-0.9.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:19:52.265911 gdstk-0.9.39/gdstk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-24 17:19:52.000000 gdstk-0.9.39/gdstk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-24 17:19:52.000000 gdstk-0.9.39/gdstk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:19:52.000000 gdstk-0.9.39/gdstk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:19:52.000000 gdstk-0.9.39/gdstk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 17:19:52.000000 gdstk-0.9.39/gdstk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 17:19:52.000000 gdstk-0.9.39/gdstk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-24 17:19:39.000000 gdstk-0.9.39/gdstk.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 17:19:39.000000 gdstk-0.9.39/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:19:52.269911 gdstk-0.9.39/python/
--rw-r--r--   0 runner    (1001) docker     (123)    44164 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/cell_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/curve_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   128218 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/docstrings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    95122 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/flexpath_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    87046 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/gdstk_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/gdswriter_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/label_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/library_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24531 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/parsing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/polygon_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/rawcell_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/reference_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/repetition_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    90116 2023-04-24 17:19:39.000000 gdstk-0.9.39/python/robustpath_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:19:52.293912 gdstk-0.9.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-24 17:19:39.000000 gdstk-0.9.39/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:19:52.281912 gdstk-0.9.39/src/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/allocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/array.h
--rw-r--r--   0 runner    (1001) docker     (123)    39454 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/cell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/cell.h
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/clipper_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/clipper_tools.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:19:52.285912 gdstk-0.9.39/src/clipperlib/
--rw-r--r--   0 runner    (1001) docker     (123)   153647 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/clipperlib/clipper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/clipperlib/clipper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/curve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/curve.h
--rw-r--r--   0 runner    (1001) docker     (123)    49359 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/flexpath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/flexpath.h
--rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/font.h
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/gdsii.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/gdsii.h
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/gdstk.h
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/gdswriter.h
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/label.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/label.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:19:52.293912 gdstk-0.9.39/src/libqhull_r/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83123 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/geom2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    51296 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/geom_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/geom_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   108561 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/global_r.c
--rw-r--r--   0 runner    (1001) docker     (123)   156212 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/io_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/io_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    80295 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/libqhull_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    62510 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/libqhull_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    23930 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/mem_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/mem_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   242779 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/merge_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/merge_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   180894 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/poly2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    58558 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/poly_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/poly_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/qhull_ra.h
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/qset_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/qset_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/random_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/random_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/rboxlib_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    34822 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/stat_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/stat_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    25503 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/user_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    36663 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/user_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/usermem_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/userprintf_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/libqhull_r/userprintf_rbox_r.c
--rw-r--r--   0 runner    (1001) docker     (123)   126051 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/library.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/map.h
--rw-r--r--   0 runner    (1001) docker     (123)    37490 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/oasis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/oasis.h
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/pathcommon.h
--rw-r--r--   0 runner    (1001) docker     (123)    64723 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/polygon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/polygon.h
--rw-r--r--   0 runner    (1001) docker     (123)    15710 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/property.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/property.h
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/rawcell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/rawcell.h
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/reference.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/reference.h
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/repetition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/repetition.h
--rw-r--r--   0 runner    (1001) docker     (123)    67329 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/robustpath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/robustpath.h
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/set.h
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/sort.h
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/style.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/style.h
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-24 17:19:39.000000 gdstk-0.9.39/src/vec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:16:14.546761 gdstk-0.9.40/
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-25 15:16:03.000000 gdstk-0.9.40/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-25 15:16:03.000000 gdstk-0.9.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-25 15:16:03.000000 gdstk-0.9.40/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-25 15:16:14.546761 gdstk-0.9.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-25 15:16:03.000000 gdstk-0.9.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:16:14.510760 gdstk-0.9.40/gdstk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-25 15:16:14.000000 gdstk-0.9.40/gdstk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-25 15:16:14.000000 gdstk-0.9.40/gdstk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:16:14.000000 gdstk-0.9.40/gdstk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:16:14.000000 gdstk-0.9.40/gdstk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 15:16:14.000000 gdstk-0.9.40/gdstk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 15:16:14.000000 gdstk-0.9.40/gdstk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 15:16:03.000000 gdstk-0.9.40/gdstk.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 15:16:03.000000 gdstk-0.9.40/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:16:14.518761 gdstk-0.9.40/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    44164 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/cell_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/curve_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   128218 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/docstrings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    95122 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/flexpath_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    87046 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/gdstk_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/gdswriter_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/label_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/library_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24531 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/parsing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/polygon_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/rawcell_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/reference_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/repetition_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    90116 2023-04-25 15:16:03.000000 gdstk-0.9.40/python/robustpath_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:16:14.546761 gdstk-0.9.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-25 15:16:03.000000 gdstk-0.9.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:16:14.534761 gdstk-0.9.40/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/allocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39454 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/cell.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/clipper_tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/clipper_tools.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:16:14.534761 gdstk-0.9.40/src/clipperlib/
+-rw-r--r--   0 runner    (1001) docker     (123)   153647 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/clipperlib/clipper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/clipperlib/clipper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/curve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/curve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49359 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/flexpath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/flexpath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/font.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/gdsii.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/gdsii.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/gdstk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/gdswriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/label.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/label.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:16:14.546761 gdstk-0.9.40/src/libqhull_r/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83123 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/geom2_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51296 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/geom_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/geom_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   108561 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/global_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)   156212 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/io_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/io_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80295 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/libqhull_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    62510 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/libqhull_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23930 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/mem_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/mem_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   242779 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/merge_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/merge_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   180894 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/poly2_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58558 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/poly_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/poly_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/qhull_ra.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/qset_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/qset_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/random_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/random_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/rboxlib_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34822 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/stat_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/stat_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25503 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/user_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36663 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/user_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/usermem_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/userprintf_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/libqhull_r/userprintf_rbox_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)   126051 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/library.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37490 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/oasis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/oasis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/pathcommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64723 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/polygon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/polygon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15710 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/property.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/property.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/rawcell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/rawcell.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/reference.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/reference.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/repetition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/repetition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67329 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/robustpath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/robustpath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/style.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/style.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-25 15:16:03.000000 gdstk-0.9.40/src/vec.h
```

### Comparing `gdstk-0.9.39/CMakeLists.txt` & `gdstk-0.9.40/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/LICENSE` & `gdstk-0.9.40/LICENSE`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/PKG-INFO` & `gdstk-0.9.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdstk
-Version: 0.9.39
+Version: 0.9.40
 Summary: Python module for creation and manipulation of GDSII files.
 Home-page: https://github.com/heitzmann/gdstk
 Author: Lucas H. Gabrielli
 Author-email: heitzmann@gmail.com
 License: Boost Software License v1.0
 Keywords: GDSII CAD layout
 Platform: OS Independent
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Provides: gdstk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GDSTK 0.9.39
+# GDSTK 0.9.40
 
 [![Boost Software License - Version 1.0](https://img.shields.io/github/license/heitzmann/gdstk.svg)](https://www.boost.org/LICENSE_1_0.txt)
 [![Tests Runner](https://github.com/heitzmann/gdstk/workflows/Tests%20Runner/badge.svg)](https://github.com/heitzmann/gdstk/actions)
 [![Publish Docs](https://github.com/heitzmann/gdstk/workflows/Publish%20Docs/badge.svg)](http://heitzmann.github.io/gdstk)
 [![Downloads](https://img.shields.io/github/downloads/heitzmann/gdstk/total.svg)](https://github.com/heitzmann/gdstk/releases)
 
 Gdstk (GDSII Tool Kit) is a C++ library for creation and manipulation of GDSII and OASIS files.
```

### Comparing `gdstk-0.9.39/README.md` & `gdstk-0.9.40/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GDSTK 0.9.39
+# GDSTK 0.9.40
 
 [![Boost Software License - Version 1.0](https://img.shields.io/github/license/heitzmann/gdstk.svg)](https://www.boost.org/LICENSE_1_0.txt)
 [![Tests Runner](https://github.com/heitzmann/gdstk/workflows/Tests%20Runner/badge.svg)](https://github.com/heitzmann/gdstk/actions)
 [![Publish Docs](https://github.com/heitzmann/gdstk/workflows/Publish%20Docs/badge.svg)](http://heitzmann.github.io/gdstk)
 [![Downloads](https://img.shields.io/github/downloads/heitzmann/gdstk/total.svg)](https://github.com/heitzmann/gdstk/releases)
 
 Gdstk (GDSII Tool Kit) is a C++ library for creation and manipulation of GDSII and OASIS files.
```

### Comparing `gdstk-0.9.39/gdstk.egg-info/PKG-INFO` & `gdstk-0.9.40/gdstk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdstk
-Version: 0.9.39
+Version: 0.9.40
 Summary: Python module for creation and manipulation of GDSII files.
 Home-page: https://github.com/heitzmann/gdstk
 Author: Lucas H. Gabrielli
 Author-email: heitzmann@gmail.com
 License: Boost Software License v1.0
 Keywords: GDSII CAD layout
 Platform: OS Independent
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Provides: gdstk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GDSTK 0.9.39
+# GDSTK 0.9.40
 
 [![Boost Software License - Version 1.0](https://img.shields.io/github/license/heitzmann/gdstk.svg)](https://www.boost.org/LICENSE_1_0.txt)
 [![Tests Runner](https://github.com/heitzmann/gdstk/workflows/Tests%20Runner/badge.svg)](https://github.com/heitzmann/gdstk/actions)
 [![Publish Docs](https://github.com/heitzmann/gdstk/workflows/Publish%20Docs/badge.svg)](http://heitzmann.github.io/gdstk)
 [![Downloads](https://img.shields.io/github/downloads/heitzmann/gdstk/total.svg)](https://github.com/heitzmann/gdstk/releases)
 
 Gdstk (GDSII Tool Kit) is a C++ library for creation and manipulation of GDSII and OASIS files.
```

### Comparing `gdstk-0.9.39/gdstk.egg-info/SOURCES.txt` & `gdstk-0.9.40/gdstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/cell_object.cpp` & `gdstk-0.9.40/python/cell_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/curve_object.cpp` & `gdstk-0.9.40/python/curve_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/docstrings.cpp` & `gdstk-0.9.40/python/docstrings.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/flexpath_object.cpp` & `gdstk-0.9.40/python/flexpath_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/gdstk_module.cpp` & `gdstk-0.9.40/python/gdstk_module.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/gdswriter_object.cpp` & `gdstk-0.9.40/python/gdswriter_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/label_object.cpp` & `gdstk-0.9.40/python/label_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/library_object.cpp` & `gdstk-0.9.40/python/library_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/parsing.cpp` & `gdstk-0.9.40/python/parsing.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/polygon_object.cpp` & `gdstk-0.9.40/python/polygon_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/rawcell_object.cpp` & `gdstk-0.9.40/python/rawcell_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/reference_object.cpp` & `gdstk-0.9.40/python/reference_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/repetition_object.cpp` & `gdstk-0.9.40/python/repetition_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/python/robustpath_object.cpp` & `gdstk-0.9.40/python/robustpath_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/setup.py` & `gdstk-0.9.40/setup.py`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/allocator.h` & `gdstk-0.9.40/src/allocator.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/array.h` & `gdstk-0.9.40/src/array.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/cell.cpp` & `gdstk-0.9.40/src/cell.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/cell.h` & `gdstk-0.9.40/src/cell.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/clipper_tools.cpp` & `gdstk-0.9.40/src/clipper_tools.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/clipper_tools.h` & `gdstk-0.9.40/src/clipper_tools.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/clipperlib/clipper.cpp` & `gdstk-0.9.40/src/clipperlib/clipper.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/clipperlib/clipper.hpp` & `gdstk-0.9.40/src/clipperlib/clipper.hpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/curve.cpp` & `gdstk-0.9.40/src/curve.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/curve.h` & `gdstk-0.9.40/src/curve.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/flexpath.cpp` & `gdstk-0.9.40/src/flexpath.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/flexpath.h` & `gdstk-0.9.40/src/flexpath.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/font.h` & `gdstk-0.9.40/src/font.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/gdsii.cpp` & `gdstk-0.9.40/src/gdsii.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/gdsii.h` & `gdstk-0.9.40/src/gdsii.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/gdstk.h` & `gdstk-0.9.40/src/gdstk.h`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #ifndef GDSTK_HEADER_GDSTK
 #define GDSTK_HEADER_GDSTK
 
 #define __STDC_FORMAT_MACROS
 #define _USE_MATH_DEFINES
 
-#define GDSTK_VERSION "0.9.39"
+#define GDSTK_VERSION "0.9.40"
 
 // If GDSTK_CUSTOM_ALLOCATOR is defined, the user must supply implementations
 // for the following dynamic memory management functions:
 // void* allocate(uint64_t size);
 // void* reallocate(void* ptr, uint64_t size);
 // void* allocate_clear(uint64_t size);
 // void free_allocation(void* ptr);
```

### Comparing `gdstk-0.9.39/src/gdswriter.h` & `gdstk-0.9.40/src/gdswriter.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/label.cpp` & `gdstk-0.9.40/src/label.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/label.h` & `gdstk-0.9.40/src/label.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/COPYING.txt` & `gdstk-0.9.40/src/libqhull_r/COPYING.txt`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/geom2_r.c` & `gdstk-0.9.40/src/libqhull_r/geom2_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/geom_r.c` & `gdstk-0.9.40/src/libqhull_r/geom_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/geom_r.h` & `gdstk-0.9.40/src/libqhull_r/geom_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/global_r.c` & `gdstk-0.9.40/src/libqhull_r/global_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/io_r.c` & `gdstk-0.9.40/src/libqhull_r/io_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/io_r.h` & `gdstk-0.9.40/src/libqhull_r/io_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/libqhull_r.c` & `gdstk-0.9.40/src/libqhull_r/libqhull_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/libqhull_r.h` & `gdstk-0.9.40/src/libqhull_r/libqhull_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/mem_r.c` & `gdstk-0.9.40/src/libqhull_r/mem_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/mem_r.h` & `gdstk-0.9.40/src/libqhull_r/mem_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/merge_r.c` & `gdstk-0.9.40/src/libqhull_r/merge_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/merge_r.h` & `gdstk-0.9.40/src/libqhull_r/merge_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/poly2_r.c` & `gdstk-0.9.40/src/libqhull_r/poly2_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/poly_r.c` & `gdstk-0.9.40/src/libqhull_r/poly_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/poly_r.h` & `gdstk-0.9.40/src/libqhull_r/poly_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/qhull_ra.h` & `gdstk-0.9.40/src/libqhull_r/qhull_ra.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/qset_r.c` & `gdstk-0.9.40/src/libqhull_r/qset_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/qset_r.h` & `gdstk-0.9.40/src/libqhull_r/qset_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/random_r.c` & `gdstk-0.9.40/src/libqhull_r/random_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/random_r.h` & `gdstk-0.9.40/src/libqhull_r/random_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/rboxlib_r.c` & `gdstk-0.9.40/src/libqhull_r/rboxlib_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/stat_r.c` & `gdstk-0.9.40/src/libqhull_r/stat_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/stat_r.h` & `gdstk-0.9.40/src/libqhull_r/stat_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/user_r.c` & `gdstk-0.9.40/src/libqhull_r/user_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/user_r.h` & `gdstk-0.9.40/src/libqhull_r/user_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/usermem_r.c` & `gdstk-0.9.40/src/libqhull_r/usermem_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/userprintf_r.c` & `gdstk-0.9.40/src/libqhull_r/userprintf_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/libqhull_r/userprintf_rbox_r.c` & `gdstk-0.9.40/src/libqhull_r/userprintf_rbox_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/library.cpp` & `gdstk-0.9.40/src/library.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/library.h` & `gdstk-0.9.40/src/library.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/map.h` & `gdstk-0.9.40/src/map.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/oasis.cpp` & `gdstk-0.9.40/src/oasis.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/oasis.h` & `gdstk-0.9.40/src/oasis.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/pathcommon.h` & `gdstk-0.9.40/src/pathcommon.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/polygon.cpp` & `gdstk-0.9.40/src/polygon.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/polygon.h` & `gdstk-0.9.40/src/polygon.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/property.cpp` & `gdstk-0.9.40/src/property.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/property.h` & `gdstk-0.9.40/src/property.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/rawcell.cpp` & `gdstk-0.9.40/src/rawcell.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/rawcell.h` & `gdstk-0.9.40/src/rawcell.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/reference.cpp` & `gdstk-0.9.40/src/reference.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/reference.h` & `gdstk-0.9.40/src/reference.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/repetition.cpp` & `gdstk-0.9.40/src/repetition.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/repetition.h` & `gdstk-0.9.40/src/repetition.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/robustpath.cpp` & `gdstk-0.9.40/src/robustpath.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/robustpath.h` & `gdstk-0.9.40/src/robustpath.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/set.h` & `gdstk-0.9.40/src/set.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/sort.h` & `gdstk-0.9.40/src/sort.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/style.cpp` & `gdstk-0.9.40/src/style.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/style.h` & `gdstk-0.9.40/src/style.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/utils.cpp` & `gdstk-0.9.40/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/utils.h` & `gdstk-0.9.40/src/utils.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.39/src/vec.h` & `gdstk-0.9.40/src/vec.h`

 * *Files identical despite different names*

