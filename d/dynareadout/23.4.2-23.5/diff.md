# Comparing `tmp/dynareadout-23.4.2.tar.gz` & `tmp/dynareadout-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynareadout-23.4.2.tar", last modified: Mon Apr 24 10:15:43 2023, max compression
+gzip compressed data, was "dynareadout-23.5.tar", last modified: Thu May 25 12:55:51 2023, max compression
```

## Comparing `dynareadout-23.4.2.tar` & `dynareadout-23.5.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.289532 dynareadout-23.4.2/
--rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.4.2/LICENSE
--rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5172 2023-04-24 10:15:43.289532 dynareadout-23.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4395 2023-04-24 08:55:05.000000 dynareadout-23.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.167860 dynareadout-23.4.2/lib/
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.166863 dynareadout-23.4.2/lib/dynareadout/
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.210744 dynareadout-23.4.2/lib/dynareadout/src/
--rw-rw-rw-   0        0        0    15215 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binary_search.c
--rw-rw-rw-   0        0        0     4052 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binary_search.h
--rw-rw-rw-   0        0        0    30340 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout.c
--rw-rw-rw-   0        0        0     5758 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout.h
--rw-rw-rw-   0        0        0     3252 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_defines.h
--rw-rw-rw-   0        0        0    11391 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_directory.c
--rw-rw-rw-   0        0        0     5670 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_directory.h
--rw-rw-rw-   0        0        0     3791 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_glob.c
--rw-rw-rw-   0        0        0     1784 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_glob.h
--rw-rw-rw-   0        0        0    12007 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_read.c
--rw-rw-rw-   0        0        0     4794 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_read.h
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.220717 dynareadout-23.4.2/lib/dynareadout/src/cpp/
--rw-rw-rw-   0        0        0    10941 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/array.hpp
--rw-rw-rw-   0        0        0     8819 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.cpp
--rw-rw-rw-   0        0        0     3521 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.hpp
--rw-rw-rw-   0        0        0    17892 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.cpp
--rw-rw-rw-   0        0        0     7664 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.hpp
--rw-rw-rw-   0        0        0     7685 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.cpp
--rw-rw-rw-   0        0        0     4841 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.hpp
--rw-rw-rw-   0        0        0     6898 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/key.cpp
--rw-rw-rw-   0        0        0    16564 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/key.hpp
--rw-rw-rw-   0        0        0     2005 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/vec.hpp
--rw-rw-rw-   0        0        0    14051 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.c
--rw-rw-rw-   0        0        0     3502 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.h
--rw-rw-rw-   0        0        0     6230 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3_defines.h
--rw-rw-rw-   0        0        0    84060 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot.c
--rw-rw-rw-   0        0        0    15111 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot.h
--rw-rw-rw-   0        0        0    12089 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_data.c
--rw-rw-rw-   0        0        0     4169 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_error_macros.h
--rw-rw-rw-   0        0        0     6690 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.c
--rw-rw-rw-   0        0        0     5034 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.h
--rw-rw-rw-   0        0        0    11849 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_state.c
--rw-rw-rw-   0        0        0     4550 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/extra_string.c
--rw-rw-rw-   0        0        0     2236 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/extra_string.h
--rw-rw-rw-   0        0        0    43016 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/key.c
--rw-rw-rw-   0        0        0     9032 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/key.h
--rw-rw-rw-   0        0        0     5323 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path.c
--rw-rw-rw-   0        0        0     2490 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path.h
--rw-rw-rw-   0        0        0     4143 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path_view.c
--rw-rw-rw-   0        0        0     3545 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path_view.h
--rw-rw-rw-   0        0        0    25367 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/pgni.h
--rw-rw-rw-   0        0        0     9855 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/profiling.c
--rw-rw-rw-   0        0        0     3589 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/profiling.h
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.225703 dynareadout-23.4.2/lib/dynareadout/src/python/
--rw-rw-rw-   0        0        0    17631 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/conversions.hpp
--rw-rw-rw-   0        0        0     3434 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_binout.cpp
--rw-rw-rw-   0        0        0    12216 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_d3plot.cpp
--rw-rw-rw-   0        0        0     4897 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_key.cpp
--rw-rw-rw-   0        0        0     1786 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_module.cpp
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.226701 dynareadout-23.4.2/lib/pybind11/
--rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.167860 dynareadout-23.4.2/lib/pybind11/include/
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.250637 dynareadout-23.4.2/lib/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.258614 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.259613 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl/
--rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl_bind.h
--rw-rw-rw-   0        0        0      860 2023-04-24 10:15:15.000000 dynareadout-23.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 10:15:43.289532 dynareadout-23.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2417 2023-04-24 10:15:11.000000 dynareadout-23.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.169854 dynareadout-23.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.260610 dynareadout-23.4.2/src/dynareadout/
--rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.4.2/src/dynareadout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.288538 dynareadout-23.4.2/src/dynareadout.egg-info/
--rw-rw-rw-   0        0        0     5172 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3095 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.4.2/src/dynareadout.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.794273 dynareadout-23.5/
+-rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.5/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5295 2023-05-25 12:55:51.794273 dynareadout-23.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4520 2023-05-08 11:43:26.000000 dynareadout-23.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.390680 dynareadout-23.5/lib/
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.389682 dynareadout-23.5/lib/dynareadout/
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.546511 dynareadout-23.5/lib/dynareadout/src/
+-rw-rw-rw-   0        0        0    15215 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binary_search.c
+-rw-rw-rw-   0        0        0     4052 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binary_search.h
+-rw-rw-rw-   0        0        0    30340 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout.c
+-rw-rw-rw-   0        0        0     5758 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout.h
+-rw-rw-rw-   0        0        0     3252 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_defines.h
+-rw-rw-rw-   0        0        0    11391 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_directory.c
+-rw-rw-rw-   0        0        0     5670 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_directory.h
+-rw-rw-rw-   0        0        0     3791 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_glob.c
+-rw-rw-rw-   0        0        0     1784 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_glob.h
+-rw-rw-rw-   0        0        0    12007 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_read.c
+-rw-rw-rw-   0        0        0     4794 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_read.h
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.586717 dynareadout-23.5/lib/dynareadout/src/cpp/
+-rw-rw-rw-   0        0        0    11031 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/array.hpp
+-rw-rw-rw-   0        0        0     8819 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/binout.cpp
+-rw-rw-rw-   0        0        0     3521 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/binout.hpp
+-rw-rw-rw-   0        0        0    18739 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.cpp
+-rw-rw-rw-   0        0        0     7831 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.hpp
+-rw-rw-rw-   0        0        0     7685 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.cpp
+-rw-rw-rw-   0        0        0     4841 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.hpp
+-rw-rw-rw-   0        0        0     4418 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_state.cpp
+-rw-rw-rw-   0        0        0     2636 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_state.hpp
+-rw-rw-rw-   0        0        0     6911 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/key.cpp
+-rw-rw-rw-   0        0        0    16564 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/key.hpp
+-rw-rw-rw-   0        0        0     2005 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/vec.hpp
+-rw-rw-rw-   0        0        0    18933 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3_buffer.c
+-rw-rw-rw-   0        0        0     3786 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3_buffer.h
+-rw-rw-rw-   0        0        0     6785 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3_defines.h
+-rw-rw-rw-   0        0        0    90823 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot.c
+-rw-rw-rw-   0        0        0    17901 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot.h
+-rw-rw-rw-   0        0        0    12090 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_data.c
+-rw-rw-rw-   0        0        0     4169 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_error_macros.h
+-rw-rw-rw-   0        0        0     6690 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.c
+-rw-rw-rw-   0        0        0     5034 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.h
+-rw-rw-rw-   0        0        0    11850 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_state.c
+-rw-rw-rw-   0        0        0     4550 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/extra_string.c
+-rw-rw-rw-   0        0        0     2236 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/extra_string.h
+-rw-rw-rw-   0        0        0    48374 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/key.c
+-rw-rw-rw-   0        0        0    10040 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/key.h
+-rw-rw-rw-   0        0        0     5980 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/path.c
+-rw-rw-rw-   0        0        0     2671 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/path.h
+-rw-rw-rw-   0        0        0     4143 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/path_view.c
+-rw-rw-rw-   0        0        0     3545 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/path_view.h
+-rw-rw-rw-   0        0        0    25367 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/pgni.h
+-rw-rw-rw-   0        0        0     9855 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/profiling.c
+-rw-rw-rw-   0        0        0     3589 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/profiling.h
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.605811 dynareadout-23.5/lib/dynareadout/src/python/
+-rw-rw-rw-   0        0        0    17631 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/python/conversions.hpp
+-rw-rw-rw-   0        0        0     5735 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_binout.cpp
+-rw-rw-rw-   0        0        0    19773 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_d3plot.cpp
+-rw-rw-rw-   0        0        0     4897 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_key.cpp
+-rw-rw-rw-   0        0        0     1786 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_module.cpp
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.611795 dynareadout-23.5/lib/pybind11/
+-rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.391678 dynareadout-23.5/lib/pybind11/include/
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.726198 dynareadout-23.5/lib/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.768676 dynareadout-23.5/lib/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.774324 dynareadout-23.5/lib/pybind11/include/pybind11/stl/
+-rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/stl_bind.h
+-rw-rw-rw-   0        0        0      858 2023-05-25 12:54:31.000000 dynareadout-23.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:55:51.794273 dynareadout-23.5/setup.cfg
+-rw-rw-rw-   0        0        0     2489 2023-05-25 12:55:08.000000 dynareadout-23.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.392675 dynareadout-23.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.775335 dynareadout-23.5/src/dynareadout/
+-rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.5/src/dynareadout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.793275 dynareadout-23.5/src/dynareadout.egg-info/
+-rw-rw-rw-   0        0        0     5295 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3177 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.5/src/dynareadout.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/top_level.txt
```

### Comparing `dynareadout-23.4.2/LICENSE` & `dynareadout-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/PKG-INFO` & `dynareadout-23.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.4.2
+Version: 23.5
 Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -16,14 +16,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dynareadout
 
 An Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 
+## Documentation
+
+You can find a [Wiki](https://github.com/PucklaJ/dynareadout/wiki) with API Documentation for python.
+
 ## Examples
 
 ### Binout
 
 ```python
 from dynareadout import Binout, BinoutType
```

### Comparing `dynareadout-23.4.2/README.md` & `dynareadout-23.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # dynareadout
 
 An Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 
+## Documentation
+
+You can find a [Wiki](https://github.com/PucklaJ/dynareadout/wiki) with API Documentation for python.
+
 ## Examples
 
 ### Binout
 
 ```python
 from dynareadout import Binout, BinoutType
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binary_search.c` & `dynareadout-23.5/lib/dynareadout/src/binary_search.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binary_search.h` & `dynareadout-23.5/lib/dynareadout/src/binary_search.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout.c` & `dynareadout-23.5/lib/dynareadout/src/binout.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout.h` & `dynareadout-23.5/lib/dynareadout/src/binout.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_defines.h` & `dynareadout-23.5/lib/dynareadout/src/binout_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_directory.c` & `dynareadout-23.5/lib/dynareadout/src/binout_directory.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_directory.h` & `dynareadout-23.5/lib/dynareadout/src/binout_directory.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_glob.c` & `dynareadout-23.5/lib/dynareadout/src/binout_glob.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_glob.h` & `dynareadout-23.5/lib/dynareadout/src/binout_glob.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_read.c` & `dynareadout-23.5/lib/dynareadout/src/binout_read.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/binout_read.h` & `dynareadout-23.5/lib/dynareadout/src/binout_read.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/array.hpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/array.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -285,19 +285,22 @@
     : m_data(data), m_size(size), m_delete_data(delete_data) {}
 
 template <typename T>
 Array<T>::Array(Array<T> &&rhs) noexcept
     : m_data(rhs.m_data), m_size(rhs.m_size), m_delete_data(rhs.m_delete_data) {
   rhs.m_data = nullptr;
   rhs.m_size = 0;
+  rhs.m_delete_data = false;
 }
 
 template <typename T> Array<T>::~Array() noexcept {
-  if (m_delete_data && m_data)
+  if (m_delete_data && m_data) {
     free(m_data);
+    m_data = nullptr;
+  }
 }
 
 template <typename T> T &Array<T>::operator[](size_t index) {
   if (empty() || index > m_size - 1) {
     throw std::runtime_error("Index out of Range");
   }
 
@@ -314,14 +317,15 @@
 
 template <typename T> Array<T> &Array<T>::operator=(Array<T> &&rhs) noexcept {
   m_data = rhs.m_data;
   m_size = rhs.m_size;
   m_delete_data = rhs.m_delete_data;
   rhs.m_data = nullptr;
   rhs.m_size = 0;
+  rhs.m_delete_data = false;
   return *this;
 }
 
 template <typename T> std::string Array<T>::str() const noexcept {
   static_assert(std::is_same_v<T, char> || std::is_same_v<T, int8_t> ||
                 std::is_same_v<T, uint8_t>);
   return SizedString(reinterpret_cast<char *>(m_data), m_size, false).str();
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.cpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.hpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/binout.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.cpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -344,45 +344,47 @@
   if (m_handle.error_string) {
     throw Exception(String(m_handle.error_string, false));
   }
 
   return Array<d3plot_solid>(elements, num_elements);
 }
 
-Array<d3plot_thick_shell> D3plot::read_thick_shells_state(size_t state) {
+D3plotThickShellsState D3plot::read_thick_shells_state(size_t state) {
   size_t num_elements;
-  d3plot_thick_shell *elements =
-      d3plot_read_thick_shells_state(&m_handle, state, &num_elements);
+  size_t num_history_variables;
+  d3plot_thick_shell *elements = d3plot_read_thick_shells_state(
+      &m_handle, state, &num_elements, &num_history_variables);
   if (m_handle.error_string) {
     throw Exception(String(m_handle.error_string, false));
   }
 
-  return Array<d3plot_thick_shell>(elements, num_elements);
+  return D3plotThickShellsState(elements, num_elements, num_history_variables);
 }
 
 Array<d3plot_beam> D3plot::read_beams_state(size_t state) {
   size_t num_elements;
   d3plot_beam *elements =
       d3plot_read_beams_state(&m_handle, state, &num_elements);
   if (m_handle.error_string) {
     throw Exception(String(m_handle.error_string, false));
   }
 
   return Array<d3plot_beam>(elements, num_elements);
 }
 
-Array<d3plot_shell> D3plot::read_shells_state(size_t state) {
+D3plotShellsState D3plot::read_shells_state(size_t state) {
   size_t num_elements;
-  d3plot_shell *elements =
-      d3plot_read_shells_state(&m_handle, state, &num_elements);
+  size_t num_history_variables;
+  d3plot_shell *elements = d3plot_read_shells_state(
+      &m_handle, state, &num_elements, &num_history_variables);
   if (m_handle.error_string) {
     throw Exception(String(m_handle.error_string, false));
   }
 
-  return Array<d3plot_shell>(elements, num_elements);
+  return D3plotShellsState(elements, num_elements, num_history_variables);
 }
 
 Array<d3plot_solid_con> D3plot::read_solid_elements() {
   size_t num_elements;
   d3plot_solid_con *elements =
       d3plot_read_solid_elements(&m_handle, &num_elements);
   if (m_handle.error_string) {
@@ -470,14 +472,22 @@
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_tensor &t) {
   return stream << "(X: " << t.x << "; Y: " << t.y << "; Z: " << t.z
                 << "; XY: " << t.xy << "; YZ: " << t.yz << ": XZ: " << t.xz
                 << ")";
 }
 
+std::ostream &operator<<(std::ostream &stream, const d3plot_x_y &x) {
+  return stream << "(" << x.x << "; " << x.y << ")";
+}
+
+std::ostream &operator<<(std::ostream &stream, const d3plot_x_y_xy &x) {
+  return stream << "(" << x.x << "; " << x.y << "; " << x.xy << ")";
+}
+
 std::ostream &operator<<(std::ostream &stream, const d3plot_surface &s) {
   return stream << "Stress: " << s.stress
                 << "; Effective Plastic Strain: " << s.effective_plastic_strain;
 }
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_solid &s) {
   return stream << "Stress: " << s.stress
@@ -503,14 +513,21 @@
 }
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_shell &s) {
   return stream << "Mid: " << s.mid << "; Inner: " << s.inner
                 << "; Outer: " << s.outer
                 << "; Inner Strain: " << s.inner_strain
                 << "; Outer Strain: " << s.outer_strain
+                << "; Bending Moment: " << s.bending_moment
+                << "; Shear Resultant: " << s.shear_resultant
+                << "; Normal Resultant: " << s.normal_resultant
+                << "; Thickness: " << s.thickness
+                << "; Element Dependent Variables: ("
+                << s.element_dependent_variables[0] << ", "
+                << s.element_dependent_variables[1] << ")"
                 << "; Internal Energy: " << s.internal_energy;
 }
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_solid_con &s) {
   return stream << "(" << s.node_indices[0] << ", " << s.node_indices[1] << ", "
                 << s.node_indices[2] << ", " << s.node_indices[3] << ", "
                 << s.node_indices[4] << ", " << s.node_indices[5] << ", "
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.hpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #pragma once
 #include "array.hpp"
 #include "d3plot_part.hpp"
+#include "d3plot_state.hpp"
 #include "vec.hpp"
 #include <chrono>
 #include <d3plot.h>
 #include <exception>
 #include <filesystem>
 #include <vector>
 
@@ -101,22 +102,22 @@
   // Read the time of a given state (time step) in milliseconds
   float read_time_32(size_t state);
   // Reads all time of every state (time step) in milliseconds
   Array<float> read_all_time_32();
   // Returns stress, strain (if NEIPH >= 6) for a given state
   Array<d3plot_solid> read_solids_state(size_t state);
   // Returns stress, strain (if ISTRN == 1) for a given state
-  Array<d3plot_thick_shell> read_thick_shells_state(size_t state);
+  D3plotThickShellsState read_thick_shells_state(size_t state);
   // Returns Axial Force, S shear resultant, T shear resultant, S bending
   // moment, T bending moment and Torsional resultant of all beams for a given
   // state
   Array<d3plot_beam> read_beams_state(size_t state);
   // Returns stress, strain (if ISTRN == 1) and some other variables (see docs
   // pg. 36) of all shells for a given state
-  Array<d3plot_shell> read_shells_state(size_t state);
+  D3plotShellsState read_shells_state(size_t state);
 
   // Returns the node connectivity + material number of all 8 node solid
   // elements
   Array<d3plot_solid_con> read_solid_elements();
   // Returns the node connectivity + material number of all 8 node thick shell
   // elements
   Array<d3plot_thick_shell_con> read_thick_shell_elements();
@@ -152,14 +153,16 @@
   d3plot_file m_handle;
 };
 
 } // namespace dro
 
 // Stream output operators for structs
 std::ostream &operator<<(std::ostream &stream, const d3plot_tensor &t);
+std::ostream &operator<<(std::ostream &stream, const d3plot_x_y &x);
+std::ostream &operator<<(std::ostream &stream, const d3plot_x_y_xy &x);
 std::ostream &operator<<(std::ostream &stream, const d3plot_surface &s);
 std::ostream &operator<<(std::ostream &stream, const d3plot_solid &s);
 std::ostream &operator<<(std::ostream &stream, const d3plot_thick_shell &ts);
 std::ostream &operator<<(std::ostream &stream, const d3plot_beam &b);
 std::ostream &operator<<(std::ostream &stream, const d3plot_shell &s);
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_solid_con &s);
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.cpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.hpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/key.cpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/key.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,16 @@
          void *user_data) {
         KeyFile::Callback *callback =
             reinterpret_cast<KeyFile::Callback *>(user_data);
 
         (*callback)(String(const_cast<char *>(keyword_name), false),
                     Card(const_cast<card_t *>(card)), card_index);
       },
-      static_cast<int>(parse_includes), &error_string, &callback, NULL, NULL);
+      static_cast<int>(parse_includes), &error_string, &callback, NULL, NULL,
+      NULL);
 
   if (error_string) {
     throw Exception(String(error_string));
   }
 }
 
 } // namespace dro
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/key.hpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/key.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/cpp/vec.hpp` & `dynareadout-23.5/lib/dynareadout/src/cpp/vec.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.c` & `dynareadout-23.5/lib/dynareadout/src/d3_buffer.c`

 * *Files 22% similar despite different names*

```diff
@@ -54,256 +54,248 @@
   return;
 #define ERROR_AND_RETURN_BUFFER_F_PTR(format_str, ...)                         \
   {                                                                            \
     char format_buffer[1024];                                                  \
     sprintf(format_buffer, format_str, __VA_ARGS__);                           \
     ERROR_AND_RETURN_BUFFER_PTR(format_buffer);                                \
   }
+#define ERROR_AND_NO_RETURN_BUFFER_F_PTR(format_str, ...)                      \
+  {                                                                            \
+    char format_buffer[1024];                                                  \
+    sprintf(format_buffer, format_str, __VA_ARGS__);                           \
+    ERROR_AND_NO_RETURN_BUFFER_PTR(format_buffer);                             \
+  }
 
 d3_buffer d3_buffer_open(const char *root_file_name) {
   BEGIN_PROFILE_FUNC();
 
   d3_buffer buffer;
-  buffer.num_file_handles = 0;
-  buffer.cur_file_handle = 0;
+  buffer.num_files = 0;
+  buffer.cur_file = 0;
   buffer.cur_word = 0;
-  buffer.file_handles = NULL;
-  buffer.file_sizes = NULL;
+  buffer.first_open_file = 0;
+  buffer.last_open_file = ~0;
+  buffer.files = NULL;
   buffer.error_string = NULL;
 
-  /* Store number 01 through 999*/
-  char numbers[3];
-  numbers[0] = '\0';
+  /* Allocate 1000 d3_files*/
+  buffer.files = malloc(1000 * sizeof(d3_file));
+  buffer.files[0].index_string[0] = '\0';
+
+  buffer.root_file_name_length = strlen(root_file_name);
+  /* Store the root file name which is used to open unopened d3plot files in the
+   * future*/
+  buffer.root_file_name = malloc(buffer.root_file_name_length + 3 + 1);
+  memcpy(buffer.root_file_name, root_file_name, buffer.root_file_name_length);
 
-  const size_t root_len = strlen(root_file_name);
   /* Store the root name + numbers + '\0'*/
-  char *file_name_buffer = malloc(root_len + 3 + 1);
-  memcpy(file_name_buffer, root_file_name, root_len);
-  memcpy(&file_name_buffer[root_len], numbers, 3);
-  file_name_buffer[root_len + 3] = '\0';
+  char *file_name_buffer = malloc(buffer.root_file_name_length + 3 + 1);
+  memcpy(file_name_buffer, root_file_name, buffer.root_file_name_length);
+  memcpy(&file_name_buffer[buffer.root_file_name_length],
+         buffer.files[0].index_string, 3);
+  file_name_buffer[buffer.root_file_name_length + 3] = '\0';
 
-  const char *patterns[2] = {"%d", "%02d"};
+  const char *patterns[2] = {"%zu", "%02zu"};
 
   size_t i = 0;
   while (i < 1000) {
     if (!path_is_file(file_name_buffer)) {
       break;
     }
 
-    FILE *file = fopen(file_name_buffer, "rb");
-    if (!file) {
-      const char *error_string = strerror(errno);
-      buffer.error_string = malloc(root_len + 3 + 2 + strlen(error_string) + 1);
-      sprintf(buffer.error_string, "%s: %s", file_name_buffer, error_string);
-      free(file_name_buffer);
-
-      END_PROFILE_FUNC();
-      return buffer;
-    }
+    /* Store number 01 through 999*/
+    buffer.files[i].file_size = path_get_file_size(file_name_buffer);
+    buffer.files[i].file_handle = fopen(file_name_buffer, "rb");
+    if (!buffer.files[i].file_handle) {
+      /* If the error is not 'Too many open files'*/
+      if (errno != EMFILE) {
+        const char *error_string = strerror(errno);
+        buffer.error_string = malloc(buffer.root_file_name_length + 3 + 2 +
+                                     strlen(error_string) + 1);
+        sprintf(buffer.error_string, "%s: %s", file_name_buffer, error_string);
+        free(file_name_buffer);
 
-    /* Calculate the file size*/
-    if (fseek(file, 0, SEEK_END) != 0) {
-      ERROR_AND_RETURN_BUFFER("Failed to calculate file size. SEEK_END");
-    }
-    const size_t file_size = ftell(file);
-    if (fseek(file, 0, SEEK_SET) != 0) {
-      ERROR_AND_RETURN_BUFFER("Failed to calculate file size. SEEK_SET");
+        END_PROFILE_FUNC();
+        return buffer;
+      }
+    } else {
+      buffer.last_open_file = i;
     }
 
-    buffer.num_file_handles++;
-    buffer.file_handles =
-        realloc(buffer.file_handles, buffer.num_file_handles * sizeof(FILE *));
-    buffer.file_handles[buffer.num_file_handles - 1] = file;
-
-    buffer.file_sizes =
-        realloc(buffer.file_sizes, buffer.num_file_handles * sizeof(size_t));
-    buffer.file_sizes[buffer.num_file_handles - 1] = file_size;
+    buffer.num_files++;
 
     /* Generate the new file name*/
     i++;
-    sprintf(numbers, patterns[i < 10], i);
-    memcpy(&file_name_buffer[root_len], numbers, 3);
+    sprintf(buffer.files[i].index_string, patterns[i < 10], i);
+    memcpy(&file_name_buffer[buffer.root_file_name_length],
+           buffer.files[i].index_string, 3);
   }
 
   free(file_name_buffer);
 
-  if (buffer.num_file_handles == 0) {
+  if (buffer.num_files == 0) {
     ERROR_AND_RETURN_BUFFER_F("No files with the name %s do exist",
                               root_file_name);
   }
 
+  if (buffer.last_open_file == ~0) {
+    ERROR_AND_RETURN_BUFFER(
+        "No files could be opened because too many files are open");
+  }
+
+  /* Shrink to fit*/
+  buffer.files = realloc(buffer.files, buffer.num_files * sizeof(d3_file));
+
   /* Determine word_size by reading NDIM*/
   buffer.word_size = 4;
   uint32_t ndim32;
   d3_buffer_read_words_at(&buffer, &ndim32, 1, 15);
+  if (buffer.error_string) {
+    ndim32 = 0;
+    free(buffer.error_string);
+    buffer.error_string = NULL;
+  }
 
   buffer.word_size = 8;
   uint64_t ndim64;
   d3_buffer_read_words_at(&buffer, &ndim64, 1, 15);
+  if (buffer.error_string) {
+    ndim64 = 0;
+    free(buffer.error_string);
+    buffer.error_string = NULL;
+  }
 
   const int makes_sense32 = ndim32 >= 2 && ndim32 <= 7;
   const int makes_sense64 = ndim64 >= 2 && ndim64 <= 7;
 
   if ((!makes_sense32 && !makes_sense64) || (makes_sense32 && makes_sense64)) {
     ERROR_AND_RETURN_BUFFER("The d3plot files are broken");
   }
 
   /* The word size could be determined*/
   buffer.word_size = 4 + 4 * makes_sense64;
 
   /* Seek back to the beginning. We know that NDIM is inside the first file*/
-  if (fseek(buffer.file_handles[0], 0, SEEK_SET) != 0) {
+  if (fseek(buffer.files[0].file_handle, 0, SEEK_SET) != 0) {
     ERROR_AND_RETURN_BUFFER("Failed to seek back after determining word size");
   }
   buffer.cur_word = 0;
 
   END_PROFILE_FUNC();
   return buffer;
 }
 
 void d3_buffer_close(d3_buffer *buffer) {
   BEGIN_PROFILE_FUNC();
 
   /* Close all files*/
-  buffer->cur_file_handle = 0;
-  while (buffer->cur_file_handle < buffer->num_file_handles) {
-    fclose(buffer->file_handles[buffer->cur_file_handle++]);
+  size_t i = 0;
+  while (i < buffer->num_files) {
+    if (buffer->files[i].file_handle)
+      fclose(buffer->files[i].file_handle);
+    i++;
   }
 
-  free(buffer->file_handles);
-  free(buffer->file_sizes);
+  free(buffer->files);
   free(buffer->error_string);
+  free(buffer->root_file_name);
 
   /* Set everything to NULL so that access after close does not crash*/
-  buffer->file_handles = NULL;
-  buffer->file_sizes = NULL;
+  buffer->files = NULL;
   buffer->error_string = NULL;
-  buffer->num_file_handles = 0;
+  buffer->root_file_name = NULL;
+  buffer->root_file_name_length = 0;
+  buffer->num_files = 0;
   buffer->cur_word = 0;
+  buffer->cur_file = 0;
 
   END_PROFILE_FUNC();
 }
 
 void d3_buffer_read_words(d3_buffer *buffer, void *words, size_t num_words) {
   BEGIN_PROFILE_FUNC();
 
-  size_t cur_file_pos = ftell(buffer->file_handles[buffer->cur_file_handle]);
+  long cur_file_pos = ftell(buffer->files[buffer->cur_file].file_handle);
   uint8_t *words_ptr = (uint8_t *)words;
 
-  if (buffer->file_sizes[buffer->cur_file_handle] - cur_file_pos >=
+  if (buffer->files[buffer->cur_file].file_size - cur_file_pos >=
       num_words * buffer->word_size) {
     /* We can read everything from the current file*/
     if (fread(words, buffer->word_size, num_words,
-              buffer->file_handles[buffer->cur_file_handle]) < num_words) {
+              buffer->files[buffer->cur_file].file_handle) < num_words) {
       ERROR_AND_RETURN_BUFFER_PTR("Read Error");
     }
     buffer->cur_word += num_words;
 
     END_PROFILE_FUNC();
     return;
   } else {
     /* Read from as much files as necessary to read all number of words*/
     size_t words_read = 0;
     while (words_read < num_words) {
 
       /* How much words can be read from the current file*/
       const size_t words_from_cur_file =
-          (buffer->file_sizes[buffer->cur_file_handle] - cur_file_pos) /
+          (buffer->files[buffer->cur_file].file_size - cur_file_pos) /
           buffer->word_size;
 
       const size_t words_left = num_words - words_read;
       if (words_from_cur_file >= words_left) {
         /* We can read all of the rest of the words from the current file*/
         if (fread(&words_ptr[words_read * buffer->word_size], buffer->word_size,
                   words_left,
-                  buffer->file_handles[buffer->cur_file_handle]) < words_left) {
+                  buffer->files[buffer->cur_file].file_handle) < words_left) {
           ERROR_AND_RETURN_BUFFER_PTR("Read Error");
         }
 
         buffer->cur_word += words_left;
         words_read = num_words;
         break;
       } else {
-        /* Read the rest of the current file*/
-        if (fread(&words_ptr[words_read * buffer->word_size], buffer->word_size,
-                  words_from_cur_file,
-                  buffer->file_handles[buffer->cur_file_handle]) <
-            words_from_cur_file) {
-          ERROR_AND_RETURN_BUFFER_PTR("Read Error");
+
+        if (words_from_cur_file != 0) {
+          /* Read the rest of the current file*/
+          if (fread(&words_ptr[words_read * buffer->word_size],
+                    buffer->word_size, words_from_cur_file,
+                    buffer->files[buffer->cur_file].file_handle) <
+              words_from_cur_file) {
+            ERROR_AND_RETURN_BUFFER_PTR("Read Error");
+          }
+
+          buffer->cur_word += words_from_cur_file;
+          words_read += words_from_cur_file;
         }
 
-        buffer->cur_word += words_from_cur_file;
-        words_read += words_from_cur_file;
-        buffer->cur_file_handle++;
+        if (!d3_buffer_next_file(buffer)) {
+          if (buffer->error_string) {
+            ERROR_AND_RETURN_BUFFER_F_PTR(
+                "Error when switching to next file: %s", buffer->error_string);
+          }
 
-        /* Check if out of bounds*/
-        if (buffer->cur_file_handle >= buffer->num_file_handles) {
           ERROR_AND_RETURN_BUFFER_PTR("Requested too much words");
         }
 
         cur_file_pos = 0;
-        if (fseek(buffer->file_handles[buffer->cur_file_handle], 0, SEEK_SET) !=
-            0) {
-          ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
-        }
       }
     }
   }
 
   END_PROFILE_FUNC();
 }
 
 void d3_buffer_read_words_at(d3_buffer *buffer, void *words, size_t num_words,
                              size_t word_pos) {
   BEGIN_PROFILE_FUNC();
 
-  if (word_pos == 0) {
-    buffer->cur_word = 0;
-    buffer->cur_file_handle = 0;
-    if (fseek(buffer->file_handles[0], 0, SEEK_SET) != 0) {
-      ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
-    }
-
-    d3_buffer_read_words(buffer, words, num_words);
-
-    END_PROFILE_FUNC();
-    return;
-  }
-
-  size_t pos_in_bytes = word_pos * buffer->word_size;
-  buffer->cur_file_handle = 0;
-
-  while (pos_in_bytes > 0) {
-    const size_t file_size = buffer->file_sizes[buffer->cur_file_handle];
-
-    if (file_size > pos_in_bytes) {
-      if (fseek(buffer->file_handles[buffer->cur_file_handle], pos_in_bytes,
-                SEEK_SET) != 0) {
-        ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
-      }
-      pos_in_bytes = 0;
-    } else {
-      pos_in_bytes -= file_size;
-      buffer->cur_file_handle++;
-
-      /* Check if out of bounds*/
-      if (buffer->cur_file_handle >= buffer->num_file_handles) {
-        ERROR_AND_RETURN_BUFFER_PTR("Read position is out of bounds");
-      }
-
-      if (pos_in_bytes == 0) {
-        if (fseek(buffer->file_handles[buffer->cur_file_handle], 0, SEEK_SET) !=
-            0) {
-          ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
-        }
-      }
-    }
+  d3_buffer_seek(buffer, word_pos);
+  if (buffer->error_string) {
+    ERROR_AND_RETURN_BUFFER_F_PTR("Failed to seek the buffer: %s",
+                                  buffer->error_string);
   }
 
-  buffer->cur_word = word_pos;
   d3_buffer_read_words(buffer, words, num_words);
 
   END_PROFILE_FUNC();
 }
 
 void d3_buffer_read_double_word(d3_buffer *buffer, double *word) {
   BEGIN_PROFILE_FUNC();
@@ -333,73 +325,212 @@
   }
 
   END_PROFILE_FUNC();
 }
 
 void d3_buffer_skip_words(d3_buffer *buffer, size_t num_words) {
   BEGIN_PROFILE_FUNC();
-  d3_buffer_skip_bytes(buffer, num_words * buffer->word_size);
+  d3_buffer_seek(buffer, buffer->cur_word + num_words);
   END_PROFILE_FUNC();
 }
 
 void d3_buffer_skip_bytes(d3_buffer *buffer, size_t num_bytes) {
   BEGIN_PROFILE_FUNC();
-
-  size_t cur_file_pos = ftell(buffer->file_handles[buffer->cur_file_handle]);
-  if (cur_file_pos + num_bytes < buffer->file_sizes[buffer->cur_file_handle]) {
-    if (fseek(buffer->file_handles[buffer->cur_file_handle], num_bytes,
-              SEEK_CUR) != 0) {
-      ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
-    }
-    const size_t advanced = num_bytes / buffer->word_size;
-    if (advanced * buffer->word_size != num_bytes) {
-      ERROR_AND_RETURN_BUFFER_F_PTR(
-          "The number of bytes %lu is not divisible by the word size %d",
-          num_bytes, buffer->word_size);
-    }
-    buffer->cur_word += advanced;
-  } else {
-    const size_t bytes_skipped =
-        (buffer->file_sizes[buffer->cur_file_handle] - cur_file_pos);
-    buffer->cur_file_handle++;
-    if (fseek(buffer->file_handles[buffer->cur_file_handle], 0, SEEK_SET) !=
-        0) {
-      ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
-    }
-    const size_t advanced = bytes_skipped / buffer->word_size;
-    if (advanced * buffer->word_size != bytes_skipped) {
-      ERROR_AND_RETURN_BUFFER_F_PTR(
-          "The number of bytes %lu is not divisible by the word size %d",
-          bytes_skipped, buffer->word_size);
-    }
-    buffer->cur_word += bytes_skipped;
-
-    d3_buffer_skip_bytes(buffer, num_bytes - bytes_skipped);
-  }
-
+  d3_buffer_skip_words(buffer, num_bytes / buffer->word_size);
   END_PROFILE_FUNC();
 }
 
 int d3_buffer_next_file(d3_buffer *buffer) {
   BEGIN_PROFILE_FUNC();
 
-  const size_t cur_file_pos =
-      ftell(buffer->file_handles[buffer->cur_file_handle]);
+  const long cur_file_pos = ftell(buffer->files[buffer->cur_file].file_handle);
   buffer->cur_word +=
-      (buffer->file_sizes[buffer->cur_file_handle] - cur_file_pos) /
+      (buffer->files[buffer->cur_file].file_size - cur_file_pos) /
       buffer->word_size;
-  buffer->cur_file_handle++;
+  buffer->cur_file++;
 
-  if (buffer->cur_file_handle == buffer->num_file_handles) {
+  if (buffer->cur_file == buffer->num_files) {
     END_PROFILE_FUNC();
     return 0;
   }
 
-  if (fseek(buffer->file_handles[buffer->cur_file_handle], 0, SEEK_SET) != 0) {
+  /* Open the next file if it isn't open and close the first opened file*/
+  if (!buffer->files[buffer->cur_file].file_handle) {
+    fclose(buffer->files[buffer->first_open_file].file_handle);
+    buffer->files[buffer->first_open_file].file_handle = NULL;
+    buffer->first_open_file++;
+    buffer->last_open_file++;
+
+    memcpy(&buffer->root_file_name[buffer->root_file_name_length],
+           buffer->files[buffer->cur_file].index_string, 4);
+
+    buffer->files[buffer->cur_file].file_handle =
+        fopen(buffer->root_file_name, "rb");
+    if (!buffer->files[buffer->cur_file].file_handle) {
+      ERROR_AND_NO_RETURN_BUFFER_F_PTR("Failed to open next file(%zu): %s: %s",
+                                       buffer->cur_file, buffer->root_file_name,
+                                       strerror(errno));
+      END_PROFILE_FUNC();
+      return 0;
+    }
+  }
+
+  if (fseek(buffer->files[buffer->cur_file].file_handle, 0, SEEK_SET) != 0) {
     ERROR_AND_NO_RETURN_BUFFER_PTR("Seek Error");
     END_PROFILE_FUNC();
     return 0;
   }
 
   END_PROFILE_FUNC();
   return 1;
 }
+
+void d3_buffer_seek(d3_buffer *buffer, size_t word_pos) {
+  BEGIN_PROFILE_FUNC();
+
+  buffer->cur_word = word_pos;
+
+  /* Determine to which file the word position points*/
+  size_t i = 0;
+  while (i < buffer->num_files) {
+    const size_t file_size_words =
+        ((size_t)buffer->files[i].file_size) / buffer->word_size;
+    if (file_size_words > word_pos) {
+      break;
+    }
+    word_pos -= file_size_words;
+
+    i++;
+  }
+
+  if (i == buffer->num_files) {
+    /* Out of bounds*/
+    ERROR_AND_RETURN_BUFFER_PTR("Out of bounds");
+  }
+
+  buffer->cur_file = i;
+  /* If the file is not yet open close enough files so that it can be opened*/
+  if (!buffer->files[buffer->cur_file].file_handle) {
+    /* Wether all files need to be closed and opened at the current file,
+     * because moving towards the file would open too many files*/
+    int out_of_range = 0;
+    if (buffer->first_open_file < buffer->last_open_file) {
+      if (buffer->cur_file > buffer->last_open_file) {
+        if (buffer->cur_file - buffer->last_open_file >
+            buffer->last_open_file - buffer->first_open_file + 1) {
+          out_of_range = 1;
+        }
+      } else {
+        if (buffer->first_open_file - buffer->cur_file >
+            buffer->last_open_file - buffer->first_open_file + 1) {
+          out_of_range = 1;
+        }
+      }
+    }
+
+    if (out_of_range) {
+      /* Close all files*/
+      size_t file_range = 0;
+      i = buffer->first_open_file;
+      while (i <= buffer->last_open_file) {
+        fclose(buffer->files[i].file_handle);
+        buffer->files[i].file_handle = NULL;
+
+        file_range++;
+        i++;
+      }
+
+      /* Make sure that first_open_file < last_open_file*/
+      size_t start_offset = 0;
+      if (buffer->num_files - buffer->cur_file < file_range) {
+        start_offset = buffer->cur_file - (buffer->num_files - file_range);
+      }
+
+      /* Open all files from the new position*/
+      i = buffer->cur_file - start_offset;
+      buffer->first_open_file = i;
+      while (file_range > 0) {
+        memcpy(&buffer->root_file_name[buffer->root_file_name_length],
+               buffer->files[i].index_string, 4);
+        buffer->files[i].file_handle = fopen(buffer->root_file_name, "rb");
+        if (!buffer->files[i].file_handle) {
+          ERROR_AND_RETURN_BUFFER_F_PTR("Error when opening file(%zu): %s: %s",
+                                        i, buffer->root_file_name,
+                                        strerror(errno));
+        }
+
+        i++;
+        file_range--;
+      }
+      buffer->last_open_file = i - 1;
+    } else {
+      if (buffer->first_open_file < buffer->last_open_file) {
+        if (buffer->cur_file < buffer->first_open_file) {
+          const size_t files_to_close =
+              buffer->first_open_file - buffer->cur_file;
+          /* Close backwards*/
+          i = buffer->last_open_file;
+          while (i > buffer->last_open_file - files_to_close) {
+            fclose(buffer->files[i].file_handle);
+            buffer->files[i].file_handle = NULL;
+            i--;
+          }
+          buffer->last_open_file -= files_to_close;
+
+          /* Open backwards*/
+          i = buffer->first_open_file;
+          while (i >= buffer->cur_file) {
+            memcpy(&buffer->root_file_name[buffer->root_file_name_length],
+                   buffer->files[i].index_string, 4);
+
+            buffer->files[i].file_handle = fopen(buffer->root_file_name, "rb");
+            if (!buffer->files[i].file_handle) {
+              ERROR_AND_RETURN_BUFFER_F_PTR(
+                  "Error when opening file(%zu): %s: %s", i,
+                  buffer->root_file_name, strerror(errno));
+            }
+            i--;
+          }
+          buffer->first_open_file = buffer->cur_file;
+        } else {
+          const size_t files_to_close =
+              buffer->cur_file - buffer->last_open_file;
+
+          /* Close forwards*/
+          i = buffer->first_open_file;
+          while (i < buffer->first_open_file + files_to_close) {
+            fclose(buffer->files[i].file_handle);
+            buffer->files[i].file_handle = NULL;
+            i++;
+          }
+          buffer->first_open_file += files_to_close;
+
+          /* Open forwards*/
+          i = buffer->last_open_file;
+          while (i <= buffer->cur_file) {
+            memcpy(&buffer->root_file_name[buffer->root_file_name_length],
+                   buffer->files[i].index_string, 4);
+
+            buffer->files[i].file_handle = fopen(buffer->root_file_name, "rb");
+            if (!buffer->files[i].file_handle) {
+              ERROR_AND_RETURN_BUFFER_F_PTR(
+                  "Error when opening file(%zu): %s: %s", i,
+                  buffer->root_file_name, strerror(errno));
+            }
+            i++;
+          }
+          buffer->last_open_file = buffer->cur_file;
+        }
+      }
+    }
+  }
+
+  /* Seek to the correct location in the file*/
+  const long seek_pos = (long)(word_pos * (size_t)buffer->word_size);
+
+  if (fseek(buffer->files[buffer->cur_file].file_handle, seek_pos, SEEK_SET) !=
+      0) {
+    ERROR_AND_RETURN_BUFFER_PTR("Seek Error");
+  }
+
+  END_PROFILE_FUNC();
+}
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.h` & `dynareadout-23.5/lib/dynareadout/src/d3_buffer.h`

 * *Files 7% similar despite different names*

```diff
@@ -24,21 +24,30 @@
  ************************************************************************************/
 
 #ifndef D3_BUFFER_H
 #define D3_BUFFER_H
 #include <stdint.h>
 #include <stdio.h>
 
+typedef struct {
+  char index_string[4];
+  uint64_t file_size;
+  FILE *file_handle;
+} d3_file;
+
 /* Represents a whole family of d3 files*/
 typedef struct {
-  FILE **file_handles;
-  size_t *file_sizes;
-  size_t num_file_handles;
-  size_t cur_file_handle;
+  char *root_file_name;
+  size_t root_file_name_length;
+  d3_file *files;
+  size_t num_files;
+  size_t cur_file;
   size_t cur_word;
+  size_t first_open_file;
+  size_t last_open_file;
 
   uint8_t word_size; /* 4 byte for single precision and 8 byte for double
                         precision*/
   char *error_string;
 } d3_buffer;
 
 #ifdef __cplusplus
@@ -69,13 +78,15 @@
 /* Similar to d3_buffer_skip_words, but it skips bytes instead of words. Try to
  * use the words one. This function ist just for some cases where the number of
  * bytes is always the same no matter what the words size is*/
 void d3_buffer_skip_bytes(d3_buffer *buffer, size_t num_bytes);
 /* Skip to the next file. Especially needed a the end of the first file when
  * done with all the headers. Sets error_string on error*/
 int d3_buffer_next_file(d3_buffer *buffer);
+/* Jumps to the word position indicated by word pos*/
+void d3_buffer_seek(d3_buffer *buffer, size_t word_pos);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3_defines.h` & `dynareadout-23.5/lib/dynareadout/src/d3_defines.h`

 * *Files 10% similar despite different names*

```diff
@@ -98,14 +98,25 @@
   union {
     double zx;
     double xz;
   };
 } d3plot_tensor;
 
 typedef struct {
+  double x;
+  double y;
+} d3plot_x_y;
+
+typedef struct {
+  double x;
+  double y;
+  double xy;
+} d3plot_x_y_xy;
+
+typedef struct {
   union {
     d3plot_tensor sigma;
     d3plot_tensor stress;
   };
   union {
     double effective_plastic_strain;
     double material_dependent_value;
@@ -124,14 +135,18 @@
     d3plot_tensor sigma;
     d3plot_tensor stress;
   };
   union {
     double effective_plastic_strain;
     double material_dependent_value;
   };
+
+  /* All history variables of all elements are allocated in one big array and
+   * this is a pointer somewhere into said array*/
+  double *history_variables;
 } d3plot_surface;
 
 typedef struct {
   d3plot_surface mid;
   d3plot_surface inner;
   d3plot_surface outer;
   union {
@@ -161,14 +176,24 @@
     d3plot_tensor inner_epsilon;
     d3plot_tensor inner_strain;
   };
   union {
     d3plot_tensor outer_epsilon;
     d3plot_tensor outer_strain;
   };
+
+  d3plot_x_y_xy bending_moment;
+  d3plot_x_y shear_resultant;
+  d3plot_x_y_xy normal_resultant;
+  double thickness;
+#ifdef __cplusplus
+  std::array<double, 2> element_dependent_variables;
+#else
+  double element_dependent_variables[2];
+#endif
   double internal_energy;
 } d3plot_shell;
 
 #define D3_FILE_TYPE_D3PLOT 1
 #define D3_FILE_TYPE_D3DRLF 2
 #define D3_FILE_TYPE_D3THDT 3
 #define D3_FILE_TYPE_INTFOR 4
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot.c` & `dynareadout-23.5/lib/dynareadout/src/d3plot.c`

 * *Files 12% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         CDA.ndim = 3;
       }
     }
   }
 
   /* Quit immediately if NDIM is not supported*/
   if (CDA.ndim != 3) {
-    ERROR_AND_RETURN_F("A ndim value of %lu is not supported", CDA.ndim);
+    ERROR_AND_RETURN_F("A ndim value of %llu is not supported", CDA.ndim);
   }
 
   i = 0;
   while (i < 4) {
     CDA.ioshl[i] -= 999 * (CDA.ioshl[i] == 1000);
 
     i++;
@@ -237,15 +237,15 @@
   } else if (CDA.maxint < -10000) {
     CDA.mdlopt = 2;
     CDA.maxint = CDA.maxint * -1 - 10000;
   } else if (CDA.maxint < 0) {
     CDA.mdlopt = 1;
     CDA.maxint *= -1;
   } else {
-    ERROR_AND_RETURN_F("Invalid value for MAXINT: %ld", CDA.maxint);
+    ERROR_AND_RETURN_F("Invalid value for MAXINT: %lld", CDA.maxint);
   }
 
   if (idtdt < 100) {
     /* We need to compute ISTRN*/
     /*ISTRN can only be computed as follows and if NV2D > 0.
       If NV2D-MAXINT*(6*IOSHL(1)+IOSHL(2)+NEIPS)+8*IOSHL(3)+4*IOSHL(4) > 1
       Then ISTRN = 1, else ISTRN = 0
@@ -335,15 +335,15 @@
 
   /* Read EOF marker*/
   double eof_marker;
   d3_buffer_read_double_word(&plot_file.buffer, &eof_marker);
 
   if (eof_marker != D3_EOF) {
     ERROR_AND_RETURN_F(
-        "Here (before header) 'd3plot':(%lu) should be the EOF marker",
+        "Here (before header) 'd3plot':(%zu) should be the EOF marker",
         plot_file.buffer.cur_word - 1);
   }
 
   if (!_d3plot_read_header(&plot_file)) {
     END_PROFILE_FUNC();
     return plot_file;
   }
@@ -1024,15 +1024,15 @@
 }
 
 double d3plot_read_time(d3plot_file *plot_file, size_t state) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
 
     END_PROFILE_FUNC();
     return -1.0;
   }
 
   double time;
   if (plot_file->buffer.word_size == 4) {
@@ -1113,15 +1113,15 @@
 }
 
 float d3plot_read_time_32(d3plot_file *plot_file, size_t state) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
 
     END_PROFILE_FUNC();
     return -1.0f;
   }
 
   float time;
   if (plot_file->buffer.word_size == 8) {
@@ -1209,15 +1209,15 @@
   *num_solids = plot_file->control_data.nel8;
   if (*num_solids == 0) {
     END_PROFILE_FUNC();
     return NULL;
   }
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     *num_solids = 0;
 
     END_PROFILE_FUNC();
     return NULL;
   }
 
   d3plot_solid *solids = malloc(*num_solids * sizeof(d3plot_solid));
@@ -1344,34 +1344,41 @@
     free(data);
   }
 
   END_PROFILE_FUNC();
   return solids;
 }
 
-d3plot_thick_shell *d3plot_read_thick_shells_state(d3plot_file *plot_file,
-                                                   size_t state,
-                                                   size_t *num_thick_shells) {
+d3plot_thick_shell *
+d3plot_read_thick_shells_state(d3plot_file *plot_file, size_t state,
+                               size_t *num_thick_shells,
+                               size_t *num_history_variables) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   *num_thick_shells = plot_file->control_data.nelt;
   if (*num_thick_shells == 0) {
+    *num_history_variables = 0;
     END_PROFILE_FUNC();
     return NULL;
   }
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     *num_thick_shells = 0;
 
     END_PROFILE_FUNC();
     return NULL;
   }
 
+  /* Allocate memory for all history variables of all thick shells*/
+  *num_history_variables = plot_file->control_data.neips;
+  double *history_variables =
+      malloc(*num_thick_shells * 3 * *num_history_variables * sizeof(double));
+
   d3plot_thick_shell *thick_shells =
       malloc(*num_thick_shells * sizeof(d3plot_thick_shell));
   if (plot_file->buffer.word_size == 4) {
     float *data = malloc(plot_file->control_data.nelt *
                          plot_file->control_data.nv3dt * sizeof(float));
 
     d3_buffer_read_words_at(
@@ -1396,34 +1403,70 @@
       thick_shells[i].mid.sigma.x = data[o++];
       thick_shells[i].mid.sigma.y = data[o++];
       thick_shells[i].mid.sigma.z = data[o++];
       thick_shells[i].mid.sigma.xy = data[o++];
       thick_shells[i].mid.sigma.yz = data[o++];
       thick_shells[i].mid.sigma.zx = data[o++];
       thick_shells[i].mid.effective_plastic_strain = data[o++];
-      /* TODO: Define NEIPS additional history values here for mid surface*/
-      o += plot_file->control_data.neips;
+
+      /* Define NEIPS additional history values here for mid surface*/
+      if (plot_file->control_data.neips != 0) {
+        thick_shells[i].mid.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               0 * *num_history_variables];
+        size_t j = 0;
+        while (j < *num_history_variables) {
+          thick_shells[i].mid.history_variables[j++] = data[o++];
+        }
+      } else {
+        thick_shells[i].mid.history_variables = NULL;
+      }
+
       thick_shells[i].inner.sigma.x = data[o++];
       thick_shells[i].inner.sigma.y = data[o++];
       thick_shells[i].inner.sigma.z = data[o++];
       thick_shells[i].inner.sigma.xy = data[o++];
       thick_shells[i].inner.sigma.yz = data[o++];
       thick_shells[i].inner.sigma.zx = data[o++];
       thick_shells[i].inner.effective_plastic_strain = data[o++];
-      /* TODO: Define NEIPS additional history values here for inner surface*/
-      o += plot_file->control_data.neips;
+
+      /* Define NEIPS additional history values here for inner surface*/
+      if (plot_file->control_data.neips != 0) {
+        thick_shells[i].inner.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               1 * *num_history_variables];
+        size_t j = 0;
+        while (j < *num_history_variables) {
+          thick_shells[i].inner.history_variables[j++] = data[o++];
+        }
+      } else {
+        thick_shells[i].inner.history_variables = NULL;
+      }
+
       thick_shells[i].outer.sigma.x = data[o++];
       thick_shells[i].outer.sigma.y = data[o++];
       thick_shells[i].outer.sigma.z = data[o++];
       thick_shells[i].outer.sigma.xy = data[o++];
       thick_shells[i].outer.sigma.yz = data[o++];
       thick_shells[i].outer.sigma.zx = data[o++];
       thick_shells[i].outer.effective_plastic_strain = data[o++];
-      /* TODO: Define NEIPS additional history values here for outer surface*/
-      o += plot_file->control_data.neips;
+
+      /* Define NEIPS additional history values here for outer surface*/
+      if (plot_file->control_data.neips != 0) {
+        thick_shells[i].outer.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               2 * *num_history_variables];
+        size_t j = 0;
+        while (j < *num_history_variables) {
+          thick_shells[i].outer.history_variables[j++] = data[o++];
+        }
+      } else {
+        thick_shells[i].outer.history_variables = NULL;
+      }
+
       if (plot_file->control_data.istrn == 1) {
         thick_shells[i].inner_epsilon.x = data[o++];
         thick_shells[i].inner_epsilon.y = data[o++];
         thick_shells[i].inner_epsilon.z = data[o++];
         thick_shells[i].inner_epsilon.xy = data[o++];
         thick_shells[i].inner_epsilon.yz = data[o++];
         thick_shells[i].inner_epsilon.zx = data[o++];
@@ -1470,26 +1513,62 @@
       END_PROFILE_FUNC();
       return NULL;
     }
 
     size_t i = 0;
     size_t o = 0;
     while (i < *num_thick_shells) {
-      memcpy(&thick_shells[i].mid, &data[o], 7 * sizeof(double));
-      o += 7;
-      /* TODO: Define NEIPS additional history values here for mid surface*/
+      memcpy(&thick_shells[i].mid, &data[o],
+             sizeof(d3plot_tensor) + sizeof(double));
+      o += (sizeof(d3plot_tensor) + sizeof(double)) / sizeof(double);
+
+      /* Define NEIPS additional history values here for mid surface*/
+      if (plot_file->control_data.neips != 0) {
+        thick_shells[i].mid.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               0 * *num_history_variables];
+        memcpy(thick_shells[i].mid.history_variables, &data[o],
+               *num_history_variables * sizeof(double));
+      } else {
+        thick_shells[i].mid.history_variables = NULL;
+      }
       o += plot_file->control_data.neips;
-      memcpy(&thick_shells[i].inner, &data[o], 7 * sizeof(double));
-      o += 7;
-      /* TODO: Define NEIPS additional history values here for inner surface*/
+
+      memcpy(&thick_shells[i].inner, &data[o],
+             sizeof(d3plot_tensor) + sizeof(double));
+      o += (sizeof(d3plot_tensor) + sizeof(double)) / sizeof(double);
+
+      /* Define NEIPS additional history values here for inner surface*/
+      if (plot_file->control_data.neips != 0) {
+        thick_shells[i].inner.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               1 * *num_history_variables];
+        memcpy(thick_shells[i].inner.history_variables, &data[o],
+               *num_history_variables * sizeof(double));
+      } else {
+        thick_shells[i].inner.history_variables = NULL;
+      }
       o += plot_file->control_data.neips;
-      memcpy(&thick_shells[i].outer, &data[o], 7 * sizeof(double));
-      o += 7;
-      /* TODO: Define NEIPS additional history values here for outer surface*/
+
+      memcpy(&thick_shells[i].outer, &data[o],
+             sizeof(d3plot_tensor) + sizeof(double));
+      o += (sizeof(d3plot_tensor) + sizeof(double)) / sizeof(double);
+
+      /* Define NEIPS additional history values here for outer surface*/
+      if (plot_file->control_data.neips != 0) {
+        thick_shells[i].outer.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               2 * *num_history_variables];
+        memcpy(thick_shells[i].outer.history_variables, &data[o],
+               *num_history_variables * sizeof(double));
+      } else {
+        thick_shells[i].outer.history_variables = NULL;
+      }
       o += plot_file->control_data.neips;
+
       if (plot_file->control_data.istrn == 1) {
         memcpy(&thick_shells[i].inner_epsilon, &data[o], 6 * sizeof(double));
         o += 6;
         memcpy(&thick_shells[i].outer_epsilon, &data[o], 6 * sizeof(double));
         o += 6;
       } else {
         memset(&thick_shells[i].inner_epsilon, 0, 12 * sizeof(double));
@@ -1522,15 +1601,15 @@
   *num_beams = plot_file->control_data.nel2;
   if (*num_beams == 0) {
     END_PROFILE_FUNC();
     return NULL;
   }
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     *num_beams = 0;
 
     END_PROFILE_FUNC();
     return NULL;
   }
 
   d3plot_beam *beams = malloc(*num_beams * sizeof(d3plot_beam));
@@ -1611,32 +1690,39 @@
   }
 
   END_PROFILE_FUNC();
   return beams;
 }
 
 d3plot_shell *d3plot_read_shells_state(d3plot_file *plot_file, size_t state,
-                                       size_t *num_shells) {
+                                       size_t *num_shells,
+                                       size_t *num_history_variables) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   *num_shells = plot_file->control_data.nel4;
   if (*num_shells == 0) {
+    *num_history_variables = 0;
     END_PROFILE_FUNC();
     return NULL;
   }
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     *num_shells = 0;
 
     END_PROFILE_FUNC();
     return NULL;
   }
 
+  /* Allocate memory for all history variables of all shells*/
+  *num_history_variables = plot_file->control_data.neips;
+  double *history_variables =
+      malloc(*num_history_variables * *num_shells * sizeof(double));
+
   d3plot_shell *shells = malloc(*num_shells * sizeof(d3plot_shell));
   if (plot_file->buffer.word_size == 4) {
     float *data = malloc(plot_file->control_data.nel4 *
                          plot_file->control_data.nv2d * sizeof(float));
 
     d3_buffer_read_words_at(
         &plot_file->buffer, data,
@@ -1660,57 +1746,93 @@
       shells[i].mid.sigma.x = data[o++];
       shells[i].mid.sigma.y = data[o++];
       shells[i].mid.sigma.z = data[o++];
       shells[i].mid.sigma.xy = data[o++];
       shells[i].mid.sigma.yz = data[o++];
       shells[i].mid.sigma.zx = data[o++];
       shells[i].mid.effective_plastic_strain = data[o++];
-      /* TODO: Define NEIPS additional history values here for mid surface*/
-      o += plot_file->control_data.neips;
+
+      /* Define NEIPS additional history values here for mid surface*/
+      if (plot_file->control_data.neips != 0) {
+        shells[i].mid.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               0 * *num_history_variables];
+        size_t j = 0;
+        while (j < *num_history_variables) {
+          shells[i].mid.history_variables[j++] = data[o++];
+        }
+      } else {
+        shells[i].mid.history_variables = NULL;
+      }
+
       shells[i].inner.sigma.x = data[o++];
       shells[i].inner.sigma.y = data[o++];
       shells[i].inner.sigma.z = data[o++];
       shells[i].inner.sigma.xy = data[o++];
       shells[i].inner.sigma.yz = data[o++];
       shells[i].inner.sigma.zx = data[o++];
       shells[i].inner.effective_plastic_strain = data[o++];
-      /* TODO: Define NEIPS additional history values here for inner surface*/
-      o += plot_file->control_data.neips;
+
+      /* Define NEIPS additional history values here for inner surface*/
+      if (plot_file->control_data.neips != 0) {
+        shells[i].inner.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               1 * *num_history_variables];
+        size_t j = 0;
+        while (j < *num_history_variables) {
+          shells[i].inner.history_variables[j++] = data[o++];
+        }
+      } else {
+        shells[i].inner.history_variables = NULL;
+      }
+
       shells[i].outer.sigma.x = data[o++];
       shells[i].outer.sigma.y = data[o++];
       shells[i].outer.sigma.z = data[o++];
       shells[i].outer.sigma.xy = data[o++];
       shells[i].outer.sigma.yz = data[o++];
       shells[i].outer.sigma.zx = data[o++];
       shells[i].outer.effective_plastic_strain = data[o++];
-      /* TODO: Define NEIPS additional history values here for outer surface*/
-      o += plot_file->control_data.neips;
+
+      /* Define NEIPS additional history values here for outer surface*/
+      if (plot_file->control_data.neips != 0) {
+        shells[i].outer.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               2 * *num_history_variables];
+        size_t j = 0;
+        while (j < *num_history_variables) {
+          shells[i].outer.history_variables[j++] = data[o++];
+        }
+      } else {
+        shells[i].outer.history_variables = NULL;
+      }
+
       if (plot_file->control_data.maxint > 3) {
         /* TODO: If MAXINT >3 then define an additional (MAXINT-3 )* (6*IOSHL(1)
          * + 1*IOSHL(2) + 8*IOSHL(3) + 4*IOSHL(4) + NEIPS) quantities here*/
         o += (plot_file->control_data.maxint - 3) *
              (6 * plot_file->control_data.ioshl[0] +
               1 * plot_file->control_data.ioshl[1] +
               8 * plot_file->control_data.ioshl[2] +
               4 * plot_file->control_data.ioshl[3] +
               plot_file->control_data.neips);
       }
-      /* TODO:
-       * Bending moment-Mx (local shell coordinate system)
-       * Bending moment-My
-       * Bending moment-Mxy
-       * Shear resultant-Qx
-       * Shear resultant-Qy
-       * Normal resultant-Nx
-       * Normal resultant-Ny
-       * Normal resultant-Nxy
-       * Thickness
-       * Element dependent variable
-       * Element dependent variable*/
-      o += 11;
+
+      shells[i].bending_moment.x = data[o++];
+      shells[i].bending_moment.y = data[o++];
+      shells[i].bending_moment.xy = data[o++];
+      shells[i].shear_resultant.x = data[o++];
+      shells[i].shear_resultant.y = data[o++];
+      shells[i].normal_resultant.x = data[o++];
+      shells[i].normal_resultant.y = data[o++];
+      shells[i].normal_resultant.xy = data[o++];
+      shells[i].thickness = data[o++];
+      shells[i].element_dependent_variables[0] = data[o++];
+      shells[i].element_dependent_variables[1] = data[o++];
+
       if (plot_file->control_data.istrn == 0) {
         shells[i].internal_energy = data[o++];
         memset(&shells[i].inner_epsilon, 0, 2 * sizeof(d3plot_tensor));
       } else if (plot_file->control_data.istrn == 1) {
         shells[i].inner_epsilon.x = data[o++];
         shells[i].inner_epsilon.y = data[o++];
         shells[i].inner_epsilon.z = data[o++];
@@ -1755,49 +1877,84 @@
       END_PROFILE_FUNC();
       return NULL;
     }
 
     size_t i = 0;
     size_t o = 0;
     while (i < *num_shells) {
-      memcpy(&shells[i].mid, &data[o], sizeof(d3plot_surface));
-      o += sizeof(d3plot_surface) / sizeof(double);
-      /* TODO: Define NEIPS additional history values here for mid surface*/
+      /* Read data of mid surface*/
+      memcpy(&shells[i].mid, &data[o], sizeof(d3plot_tensor) + sizeof(double));
+      o += (sizeof(d3plot_tensor) + sizeof(double)) / sizeof(double);
+
+      /* Define NEIPS additional history values here for mid surface*/
+      if (plot_file->control_data.neips != 0) {
+        shells[i].mid.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               0 * *num_history_variables];
+        memcpy(shells[i].mid.history_variables, &data[o],
+               *num_history_variables * sizeof(double));
+      } else {
+        shells[i].mid.history_variables = NULL;
+      }
       o += plot_file->control_data.neips;
-      memcpy(&shells[i].inner, &data[o], sizeof(d3plot_surface));
-      o += sizeof(d3plot_surface) / sizeof(double);
-      /* TODO: Define NEIPS additional history values here for inner surface*/
+
+      /* Read data of inner surface*/
+      memcpy(&shells[i].inner, &data[o],
+             sizeof(d3plot_tensor) + sizeof(double));
+      o += (sizeof(d3plot_tensor) + sizeof(double)) / sizeof(double);
+
+      /* Define NEIPS additional history values here for inner surface*/
+      if (plot_file->control_data.neips != 0) {
+        shells[i].inner.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               1 * *num_history_variables];
+        memcpy(shells[i].inner.history_variables, &data[o],
+               *num_history_variables * sizeof(double));
+      } else {
+        shells[i].inner.history_variables = NULL;
+      }
       o += plot_file->control_data.neips;
-      memcpy(&shells[i].outer, &data[o], sizeof(d3plot_surface));
-      o += sizeof(d3plot_surface) / sizeof(double);
-      /* TODO: Define NEIPS additional history values here for outer surface*/
+
+      /* Read data of outer surface*/
+      memcpy(&shells[i].outer, &data[o],
+             sizeof(d3plot_tensor) + sizeof(double));
+      o += (sizeof(d3plot_tensor) + sizeof(double)) / sizeof(double);
+
+      /* Define NEIPS additional history values here for outer surface*/
+      if (plot_file->control_data.neips != 0) {
+        shells[i].outer.history_variables =
+            &history_variables[i * 3 * *num_history_variables +
+                               2 * *num_history_variables];
+        memcpy(shells[i].outer.history_variables, &data[o],
+               *num_history_variables * sizeof(double));
+      } else {
+        shells[i].outer.history_variables = NULL;
+      }
       o += plot_file->control_data.neips;
+
       if (plot_file->control_data.maxint > 3) {
         /* TODO: If MAXINT >3 then define an additional (MAXINT-3 )* (6*IOSHL(1)
          * + 1*IOSHL(2) + 8*IOSHL(3) + 4*IOSHL(4) + NEIPS) quantities here*/
         o += (plot_file->control_data.maxint - 3) *
              (6 * plot_file->control_data.ioshl[0] +
               1 * plot_file->control_data.ioshl[1] +
               8 * plot_file->control_data.ioshl[2] +
               4 * plot_file->control_data.ioshl[3] +
               plot_file->control_data.neips);
       }
-      /* TODO:
-       * Bending moment-Mx (local shell coordinate system)
-       * Bending moment-My
-       * Bending moment-Mxy
-       * Shear resultant-Qx
-       * Shear resultant-Qy
-       * Normal resultant-Nx
-       * Normal resultant-Ny
-       * Normal resultant-Nxy
-       * Thickness
-       * Element dependent variable
-       * Element dependent variable*/
-      o += 11;
+      memcpy(&shells[i].bending_moment, &data[o],
+             sizeof(d3plot_x_y_xy) +     /* Bending moment (Mx, My, Mxy)*/
+                 sizeof(d3plot_x_y) +    /* Shear resultant (Qx, Qy)*/
+                 sizeof(d3plot_x_y_xy) + /* Normal resultant (Nx, Ny, Nxy)*/
+                 sizeof(double) +        /* Thickness*/
+                 sizeof(double) * 2      /* 2 Element dependent variables*/
+      );
+      o += (sizeof(d3plot_x_y_xy) + sizeof(d3plot_x_y) + sizeof(d3plot_x_y_xy) +
+            sizeof(double) + sizeof(double) * 2) /
+           sizeof(double);
       if (plot_file->control_data.istrn == 0) {
         shells[i].internal_energy = data[o++];
         memset(&shells[i].inner_epsilon, 0, 2 * sizeof(d3plot_tensor));
       } else if (plot_file->control_data.istrn == 1) {
         memcpy(&shells[i].inner_epsilon, &data[o], 2 * sizeof(d3plot_tensor));
         o += 2 * sizeof(d3plot_tensor) / sizeof(double);
 
@@ -2254,30 +2411,30 @@
                        d3plot_read_shell_elements, d3plot_shell_con, num_shells,
                        shell_ids, shell_indices);
 
   /* If no elements have been found, this means that the part with the given
    * index does not exist*/
   if (part.num_solids == 0 && part.num_thick_shells == 0 &&
       part.num_beams == 0 && part.num_shells == 0) {
-    ERROR_AND_NO_RETURN_F_PTR("The part with index %lu does not exist",
+    ERROR_AND_NO_RETURN_F_PTR("The part with index %zu does not exist",
                               part_index);
     END_PROFILE_FUNC();
     return part;
   }
 
   END_PROFILE_FUNC();
   return part;
 }
 
 d3plot_part d3plot_read_part_by_id(d3plot_file *plot_file, d3_word part_id,
                                    const d3_word *part_ids, size_t num_parts) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
-  d3plot_part part;
+  d3plot_part part = {0};
 
   d3_word *p_part_ids = part_ids ? (d3_word *)part_ids
                                  : d3plot_read_part_ids(plot_file, &num_parts);
   if (plot_file->error_string) {
     END_PROFILE_FUNC();
     return part;
   }
@@ -2291,15 +2448,15 @@
   const size_t index =
       d3_word_binary_search(p_part_ids, 0, num_parts - 1, part_id);
   if (!part_ids) {
     free(p_part_ids);
   }
 
   if (index == ~0) {
-    ERROR_AND_NO_RETURN_F_PTR("The part id %lu has not been found", part_id);
+    ERROR_AND_NO_RETURN_F_PTR("The part id %llu has not been found", part_id);
     END_PROFILE_FUNC();
     return part;
   }
 
   part = d3plot_read_part(plot_file, index);
 
   END_PROFILE_FUNC();
@@ -2397,15 +2554,15 @@
 
     free(coords32);
 
     return coords;
   }
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     return NULL;
   }
 
   *num_nodes = plot_file->control_data.numnp;
   double *coords = malloc(*num_nodes * 3 * sizeof(double));
 
   d3_buffer_read_words_at(&plot_file->buffer, coords, *num_nodes * 3,
@@ -2445,15 +2602,15 @@
 
     free(coords64);
 
     return coords;
   }
 
   if (state >= plot_file->num_states) {
-    ERROR_AND_NO_RETURN_F_PTR("%lu is out of bounds for the states", state);
+    ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     return NULL;
   }
 
   *num_nodes = plot_file->control_data.numnp;
   float *coords = malloc(*num_nodes * 3 * sizeof(float));
 
   d3_buffer_read_words_at(&plot_file->buffer, coords, *num_nodes * 3,
@@ -2588,7 +2745,25 @@
   part->num_solids = 0;
   part->num_thick_shells = 0;
   part->num_beams = 0;
   part->num_shells = 0;
 
   END_PROFILE_FUNC();
 }
+
+void d3plot_free_shells_state(d3plot_shell *shells) {
+  BEGIN_PROFILE_FUNC();
+
+  free(shells->mid.history_variables);
+  free(shells);
+
+  END_PROFILE_FUNC();
+}
+
+void d3plot_free_thick_shells_state(d3plot_thick_shell *thick_shells) {
+  BEGIN_PROFILE_FUNC();
+
+  free(thick_shells->mid.history_variables);
+  free(thick_shells);
+
+  END_PROFILE_FUNC();
+}
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot.h` & `dynareadout-23.5/lib/dynareadout/src/d3plot.h`

 * *Files 25% similar despite different names*

```diff
@@ -29,22 +29,61 @@
 #include "d3_defines.h"
 #include <time.h>
 
 /* This holds all data needed to read d3plot files*/
 typedef struct {
   struct {
     /* These are all the values inside the CONTROL DATA section of the first
-     * d3plot file (root file)*/
-    d3_word ndim, numnp, nglbv, it, iu, iv, ia, nummat8, nv3d, nel2, nummat2,
-        nv1d, nel4, nummat4, nv2d, neiph, neips, nmsph, narbs, nelt, nummatt,
-        nv3dt, ioshl[4], ialemat, ncfdv1, nadapt, nmmat, nel48, nel20, nt3d;
+     * d3plot file (root file) pg. 7*/
+
+    d3_word ndim, /* Number of dimensions */
+        numnp,    /* Number of nodal points*/
+        nglbv,    /* Number of global variable to be read with each state*/
+        it,       /* Flag for temperatures*/
+        iu,       /* Flag for current geometry*/
+        iv,       /* Flag for velocities*/
+        ia,       /* Flag for accelerations*/
+        nummat8,  /* Number of materials used by the 8 node solids*/
+        nv3d,     /* Number of values in database for each solid element*/
+        nel2,     /* Number of 2 node one-dimensional elements (beams)*/
+        nummat2,  /* Number of materials used by the 2 node 1D elements*/
+        nv1d,     /* Number of values in database for each 1D element*/
+        nel4,     /* Number of four node shells (2D or 3D) elements*/
+        nummat4,  /* Number of materials used by the 4 node 2D elements*/
+        nv2d,     /* Number of values in database for each 2D element*/
+        neiph,    /* Number of additional values per solid element to written in
+                     the type 6 database (history variables)*/
+        neips,    /* Number of additional values per integration point to be
+                     written into the type 6 database for shell elements (history
+                     variables)*/
+        nmsph,    /* Number of SPH Nodes*/
+        narbs,    /* Additional storage required for arbitrary node and element
+                     numbering in type 6 database*/
+        nelt,     /* Number of 8 node thick shell elements*/
+        nummatt,  /* Number of materials used for the 8 node thick shell
+                     elements*/
+        nv3dt,    /* Number of values in database for each thick shell*/
+        ioshl[4],
+        /* 0. 6 stress components flag, 1. Plastic strain flag, 2. Shell force
+           resultants flag, 3. Shell thickness, energy+2 others*/
+        ialemat, /* Size of array containing solid element parts numbers used as
+                    ALE material*/
+        ncfdv1,  /* Bit flags for CFD nodal values*/
+        nadapt,  /* Number of adapted element to parent pairs*/
+        nmmat,   /* Total number of materials*/
+        nel48,   /* Number of 8 node Shells*/
+        nel20,   /* Number of 20 Node Solid Elements*/
+        nt3d /* Number of Thermal Element Variables*/;
     /* This will be calculated*/
     d3_word numrbs;
     /* These variables can by negative*/
-    int64_t nel8, maxint;
+    int64_t nel8, /* Number of 8 node solid elements*/
+        maxint    /* Number of integration points dumped for each shell and the
+                     MDLOPT flag*/
+        ;
     /* These values will also be calculated*/
     uint8_t mdlopt, istrn;
 
     /* These are some values also being calculated, but are not part of the
      * documentation*/
     uint8_t plastic_strain_tensor_written, thermal_strain_tensor_written,
         element_connectivity_packed;
@@ -161,29 +200,33 @@
  * deallocated by free*/
 float *d3plot_read_all_time_32(d3plot_file *plot_file, size_t *num_states);
 
 /* Returns stress, strain (if NEIPH >= 6) for a given state. The return value
  * needs to be deallocated by free.*/
 d3plot_solid *d3plot_read_solids_state(d3plot_file *plot_file, size_t state,
                                        size_t *num_solids);
-/* Returns stress, strain (if ISTRN == 1) for a given state. The return value
- * needs to be deallocated by free.*/
-d3plot_thick_shell *d3plot_read_thick_shells_state(d3plot_file *plot_file,
-                                                   size_t state,
-                                                   size_t *num_thick_shells);
+/* Returns stress, strain (if ISTRN == 1) for a given state. The number of
+ * history variables is the same for every surface of every thick shell. The
+ * return value needs to be deallocated by d3plot_free_thick_shells_state.*/
+d3plot_thick_shell *
+d3plot_read_thick_shells_state(d3plot_file *plot_file, size_t state,
+                               size_t *num_thick_shells,
+                               size_t *num_history_variables);
 /* Returns Axial Force, S shear resultant, T shear resultant, S bending moment,
  * T bending moment and Torsional resultant of all beams for a given state. The
  * return value needs to be deallocated by free.*/
 d3plot_beam *d3plot_read_beams_state(d3plot_file *plot_file, size_t state,
                                      size_t *num_beams);
 /* Returns stress, strain (if ISTRN == 1) and some other variables (see docs pg.
- * 36) of all shells for a given state. The return value needs to be deallocated
- * by free.*/
+ * 36) of all shells for a given state. The number of history variables is the
+ * same for every surface of every shell. The return value needs to be
+ * deallocated by d3plot_free_shells_state.*/
 d3plot_shell *d3plot_read_shells_state(d3plot_file *plot_file, size_t state,
-                                       size_t *num_shells);
+                                       size_t *num_shells,
+                                       size_t *num_history_variables);
 /* Returns the node connectivity + material number of all 8 node solid
  * elements. The return value needs to be deallocated by free*/
 d3plot_solid_con *d3plot_read_solid_elements(d3plot_file *plot_file,
                                              size_t *num_solids);
 /* Returns the node connectivity + material number of all 8 node thick shell
  * elements. The return value needs to be deallocated by free*/
 d3plot_thick_shell_con *
@@ -252,14 +295,18 @@
 d3_word *_d3plot_read_ids(d3plot_file *plot_file, size_t *num_ids,
                           size_t data_type, size_t num_ids_value);
 /* Insert a sorted (ascending) array (src) into a sorted array (dst)*/
 d3_word *_insert_sorted(d3_word *dst, size_t dst_size, const d3_word *src,
                         size_t src_size);
 /* Deallocates all memory of a d3plot_part*/
 void d3plot_free_part(d3plot_part *part);
+/* Deallocates all memory returned by d3plot_read_shells_state*/
+void d3plot_free_shells_state(d3plot_shell *shells);
+/* Deallocate all memory returned by d3plot_read_thick_shells_state*/
+void d3plot_free_thick_shells_state(d3plot_thick_shell *thick_shells);
 /********************************/
 
 /*********** Utility Functions ***************/
 /* These functions do some more computations *
  * to reach their outputs, so be aware of    *
  * that if you use them                      */
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot_data.c` & `dynareadout-23.5/lib/dynareadout/src/d3plot_data.c`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     return 0;
   }
 
   const size_t user_ids_end = plot_file->buffer.cur_word;
   const size_t user_ids_size = user_ids_end - user_ids_start;
   if (user_ids_size != CDP.narbs) {
     ERROR_AND_NO_RETURN_F_PTR(
-        "The USER IDENTIFICATION NUMBERS section is false (%lu != %lu)",
+        "The USER IDENTIFICATION NUMBERS section is false (%zu != %llu)",
         user_ids_size, CDP.narbs);
 
     END_PROFILE_FUNC();
     return 0;
   }
 
   END_PROFILE_FUNC();
@@ -356,15 +356,15 @@
         eof_marker = eof_marker32;
       } else {
         memcpy(&eof_marker, &ntype, plot_file->buffer.word_size);
       }
 
       if (eof_marker != D3_EOF) {
         ERROR_AND_NO_RETURN_F_PTR(
-            "Here (after header) 'd3plot':(%lu) should be "
+            "Here (after header) 'd3plot':(%zu) should be "
             "the EOF marker (%f != %f)",
             plot_file->buffer.cur_word - 1, eof_marker, D3_EOF);
         END_PROFILE_FUNC();
         return 0;
       }
 
       break;
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot_error_macros.h` & `dynareadout-23.5/lib/dynareadout/src/d3plot_error_macros.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.c` & `dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.h` & `dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/d3plot_state.c` & `dynareadout-23.5/lib/dynareadout/src/d3plot_state.c`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     return 0;
   }
 
   const size_t global_end = plot_file->buffer.cur_word;
   const size_t global_size = global_end - global_start;
 
   if (global_size != CDP.nglbv) {
-    ERROR_AND_NO_RETURN_F_PTR("Size of GLOBAL is %lu instead of %lu",
+    ERROR_AND_NO_RETURN_F_PTR("Size of GLOBAL is %zu instead of %llu",
                               global_size, CDP.nglbv);
     END_PROFILE_FUNC();
     return 0;
   }
 
   /* NODEDATA*/
   /**** Order of Node Data ******
@@ -244,15 +244,15 @@
     END_PROFILE_FUNC();
     return 0;
   }
 
   const size_t node_data_end = plot_file->buffer.cur_word;
   const size_t node_data_size = node_data_end - node_data_start;
   if (node_data_size != NND) {
-    ERROR_AND_NO_RETURN_F_PTR("NODEDATA should be %lu instead of %lu", NND,
+    ERROR_AND_NO_RETURN_F_PTR("NODEDATA should be %zu instead of %zu", NND,
                               node_data_size);
     END_PROFILE_FUNC();
     return 0;
   }
 
   /* THERMDATA*/
   d3_buffer_skip_words(&plot_file->buffer, CDP.nt3d * CDP.nel8);
@@ -294,15 +294,15 @@
     END_PROFILE_FUNC();
     return 0;
   }
 
   const size_t elem_data_end = plot_file->buffer.cur_word;
   const size_t elem_data_size = elem_data_end - elem_data_start;
   if (elem_data_size < ENN) {
-    ERROR_AND_NO_RETURN_F_PTR("ELEMDATA should be %lu instead of %lu", ENN,
+    ERROR_AND_NO_RETURN_F_PTR("ELEMDATA should be %zu instead of %zu", ENN,
                               elem_data_size);
     END_PROFILE_FUNC();
     return 0;
   }
 
   /* Element Deletion Option*/
   size_t skip_words;
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/extra_string.c` & `dynareadout-23.5/lib/dynareadout/src/extra_string.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/extra_string.h` & `dynareadout-23.5/lib/dynareadout/src/extra_string.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/key.c` & `dynareadout-23.5/lib/dynareadout/src/key.c`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,14 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #include "key.h"
 #include "binary_search.h"
-#include "extra_string.h"
 #include "profiling.h"
 #include <errno.h>
 #include <math.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
@@ -132,15 +131,15 @@
   data.num_keywords = num_keywords;
   *num_keywords = 0;
 
   char *internal_error_string;
 
   key_file_parse_with_callback(file_name, key_file_parse_callback,
                                parse_includes, &internal_error_string, &data,
-                               NULL, NULL);
+                               NULL, NULL, NULL);
 
   /* Deallocate the memory if an error occurred*/
   if (internal_error_string) {
     key_file_free(data.keywords, *data.num_keywords);
     data.keywords = NULL;
     *data.num_keywords = 0;
     if (error_string) {
@@ -156,15 +155,16 @@
   return data.keywords;
 }
 
 void key_file_parse_with_callback(const char *file_name,
                                   key_file_callback callback,
                                   int parse_includes, char **error_string,
                                   void *user_data, char ***include_paths,
-                                  size_t *num_include_paths) {
+                                  size_t *num_include_paths,
+                                  const char *root_folder) {
   BEGIN_PROFILE_FUNC();
 
   /* Variables to stack multiple errors*/
   char *error_stack = NULL;
   size_t error_stack_size = 0;
   size_t error_ptr = 0;
 
@@ -178,14 +178,17 @@
     END_PROFILE_FUNC();
     return;
   }
 
   /* This points to the include paths*/
   char ***include_paths_ptr;
   size_t *num_include_paths_ptr;
+  /* Stores the parent directory of the first file passed to
+   * key_file_parse_with_callback*/
+  char *root_folder_ptr;
 
   if (!include_paths) {
     include_paths_ptr = malloc(sizeof(char **));
     *include_paths_ptr = NULL;
   } else {
     include_paths_ptr = include_paths;
   }
@@ -193,36 +196,57 @@
   if (!num_include_paths) {
     num_include_paths_ptr = malloc(sizeof(size_t));
     *num_include_paths_ptr = 0;
   } else {
     num_include_paths_ptr = num_include_paths;
   }
 
-  /* Add the current directory to the include paths*/
-  char *current_wd = path_working_directory();
-
-  (*num_include_paths_ptr)++;
-  *include_paths_ptr =
-      realloc(*include_paths_ptr, *num_include_paths_ptr * sizeof(char *));
-  (*include_paths_ptr)[*num_include_paths_ptr - 1] = current_wd;
+  if (!root_folder) {
+    const size_t index = path_move_up_real(file_name);
+    if (index == (size_t)~0) {
+      root_folder_ptr = path_working_directory();
+    } else {
+      if (path_is_abs(file_name)) {
+        root_folder_ptr = malloc(index + 1 + 1);
+        memcpy(root_folder_ptr, file_name, index + 1);
+        root_folder_ptr[index + 1] = '\0';
+      } else {
+        char *current_wd = path_working_directory();
+        root_folder_ptr = path_join(current_wd, file_name);
+        root_folder_ptr[path_move_up_real(root_folder_ptr) + 1] = '\0';
+        free(current_wd);
+      }
+    }
+  } else {
+    root_folder_ptr = (char *)root_folder;
+  }
 
-  /* Store the parent path of the file if need by INCLUDE_PATH_RELATIVE*/
-  char *file_parent_path = NULL;
+  if (*num_include_paths_ptr == 0) {
+    /* Add the current working directory (local directory) to the
+     * include paths*/
+    (*num_include_paths_ptr)++;
+    *include_paths_ptr =
+        realloc(*include_paths_ptr, *num_include_paths_ptr * sizeof(char *));
+    (*include_paths_ptr)[*num_include_paths_ptr - 1] = path_working_directory();
+  }
 
   extra_string line;
   extra_string current_keyword_name;
   current_keyword_name.buffer[0] = '\0';
   current_keyword_name.extra = NULL;
   line.extra = NULL;
 
   size_t current_keyword_length = 0;
   size_t current_keyword_line = (size_t)~0;
   size_t card_index = 0;
   size_t line_count = 0;
 
+  char *current_multi_line_string = NULL;
+  size_t current_multi_line_index = 0;
+
   /* Loop until all lines have been read or an error occurred*/
   while (1) {
     /* Clear extra without freeing the memory*/
     if (line.extra) {
       line.extra[0] = '\0';
     }
 
@@ -393,108 +417,70 @@
       }
 
       /* -------- ⛅ Include Parsing ⛅ -------*/
       if (parse_includes &&
           extra_string_starts_with(&current_keyword_name, "INCLUDE")) {
         /* Parse all the different INCLUDE keywords*/
         if (extra_string_compare(&current_keyword_name, "INCLUDE") == 0) {
-          /* TODO: Support multi line file names (Remark 3)*/
-          char *include_file_name = card_parse_whole(&card);
-          char *final_include_file_name = NULL;
-
-          /* Loop over all include paths and look for file*/
-          i = 0;
-          while (i < *num_include_paths_ptr) {
-            char *full_include_file_name =
-                path_join((*include_paths_ptr)[i], include_file_name);
-
-            if (path_is_file(full_include_file_name)) {
-              final_include_file_name = full_include_file_name;
-              break;
-            }
-
-            free(full_include_file_name);
-
-            i++;
-          }
-
-          if (final_include_file_name) {
-            char *include_error;
-            /* Call the function recursively*/
-            key_file_parse_with_callback(
-                final_include_file_name, callback, 1, &include_error, user_data,
-                include_paths_ptr, num_include_paths_ptr);
-            free(final_include_file_name);
-
-            /* Add the error to the error stack if an error occurred in the
-             * recursive call*/
-            if (include_error != NULL) {
-              ERROR_MSG(include_error);
-              free(include_error);
-            }
-          } else {
-            ERROR_F("%s:%lu: \"%s\" could not be found", file_name, line_count,
-                    include_file_name);
-          }
-          free(include_file_name);
-
-          /* continue without calling the callback for the card*/
-          if (card.string != line.buffer) {
-            free(card.string);
-          }
-
-          card_index++;
+          _parse_include_file_name_card(
+              &card, &card_index, &line, line_length,
+              &current_multi_line_string, &current_multi_line_index,
+              num_include_paths_ptr, include_paths_ptr, callback, user_data,
+              &error_stack, &error_stack_size, &error_ptr, file_name,
+              line_count, root_folder_ptr);
           continue;
         } else if (extra_string_compare(&current_keyword_name,
                                         "INCLUDE_PATH") == 0) {
-          /* TODO: Support multi line path names (Remark 3)*/
-          char *include_path_name = card_parse_whole(&card);
+          /* Support multi line file names (LS Dyna Manual Volume I
+           * *INCLUDE Remark 2, p. 2690)*/
+          if (!_parse_multi_line_string(&current_multi_line_string,
+                                        &current_multi_line_index, &card,
+                                        line_length)) {
+            /* continue without calling the callback for the card*/
+            if (card.string != line.buffer) {
+              free(card.string);
+            }
+            continue;
+          }
 
           (*num_include_paths_ptr)++;
           *include_paths_ptr = realloc(*include_paths_ptr,
                                        *num_include_paths_ptr * sizeof(char *));
-          (*include_paths_ptr)[*num_include_paths_ptr - 1] = include_path_name;
+          (*include_paths_ptr)[*num_include_paths_ptr - 1] =
+              current_multi_line_string;
+
+          current_multi_line_string = NULL;
+          current_multi_line_index = 0;
 
           /* continue without calling the callback for the card*/
           if (card.string != line.buffer) {
             free(card.string);
           }
 
           card_index++;
           continue;
         } else if (extra_string_compare(&current_keyword_name,
                                         "INCLUDE_PATH_RELATIVE") == 0) {
-          /* TODO: Support multi line path names (Remark 3)*/
-          char *include_path_name = card_parse_whole(&card);
-
-          if (!file_parent_path) {
-            /* TODO: The relative path probably needs to be relative to the
-             * FIRST input given to LS Dyna by the command line
-             * 'i=parent_folder/file_name.k'*/
-            const size_t index = path_move_up_real(file_name);
-            if (index == (size_t)~0) {
-              const size_t current_wd_len = strlen(current_wd);
-              file_parent_path = malloc(current_wd_len + 1);
-              memcpy(file_parent_path, current_wd, current_wd_len + 1);
-            } else {
-              if (path_is_abs(file_name)) {
-                file_parent_path = malloc(index + 1 + 1);
-                memcpy(file_parent_path, file_name, index + 1);
-                file_parent_path[index + 1] = '\0';
-              } else {
-                file_parent_path = path_join(current_wd, file_name);
-                file_parent_path[path_move_up_real(file_parent_path) + 1] =
-                    '\0';
-              }
+          /* Support multi line file names (LS Dyna Manual Volume I
+           * *INCLUDE Remark 2, p. 2690)*/
+          if (!_parse_multi_line_string(&current_multi_line_string,
+                                        &current_multi_line_index, &card,
+                                        line_length)) {
+            /* continue without calling the callback for the card*/
+            if (card.string != line.buffer) {
+              free(card.string);
             }
+            continue;
           }
 
           char *full_include_path_name =
-              path_join(file_parent_path, include_path_name);
-          free(include_path_name);
+              path_join(root_folder_ptr, current_multi_line_string);
+          free(current_multi_line_string);
+          current_multi_line_string = NULL;
+          current_multi_line_index = 0;
 
           (*num_include_paths_ptr)++;
           *include_paths_ptr = realloc(*include_paths_ptr,
                                        *num_include_paths_ptr * sizeof(char *));
           (*include_paths_ptr)[*num_include_paths_ptr - 1] =
               full_include_path_name;
 
@@ -503,44 +489,74 @@
             free(card.string);
           }
 
           card_index++;
           continue;
         } else if (extra_string_compare(&current_keyword_name,
                                         "INCLUDE_BINARY") == 0) {
-          /* TODO*/
-          ERROR_KEYWORD_NOT_IMPLEMENTED("INCLUDE_BINARY");
+          /* Parse the first card like a normal INCLUDE*/
+          if (card_index == 0) {
+            _parse_include_file_name_card(
+                &card, &card_index, &line, line_length,
+                &current_multi_line_string, &current_multi_line_index,
+                num_include_paths_ptr, include_paths_ptr, callback, user_data,
+                &error_stack, &error_stack_size, &error_ptr, file_name,
+                line_count, root_folder_ptr);
+            continue;
+          } else {
+            ERROR_F(
+                "%s:%zu: Invalid number of cards for INCLUDE_BINARY keyword",
+                file_name, line_count);
+          }
+
+          /* continue without calling the callback for the card*/
+          if (card.string != line.buffer) {
+            free(card.string);
+          }
+
+          card_index++;
+          continue;
         } else if (extra_string_compare(&current_keyword_name,
                                         "INCLUDE_NASTRAN") == 0) {
-          /* TODO*/
-          ERROR_KEYWORD_NOT_IMPLEMENTED("INCLUDE_NASTRAN");
-        } else if (extra_string_compare(&current_keyword_name,
-                                        "INCLUDE_STAMPED_SET") == 0) {
-          /* TODO*/
-          ERROR_KEYWORD_NOT_IMPLEMENTED("INCLUDE_STAMPED_SET");
-        } else if (extra_string_starts_with(&current_keyword_name,
-                                            "INCLUDE_TRANSFORM") != 0) {
-          /* TODO*/
-          ERROR_KEYWORD_NOT_IMPLEMENTED(current_keyword_name.buffer);
-        } else if (extra_string_starts_with(&current_keyword_name,
-                                            "INCLUDE_STAMPED_PART") != 0) {
-          /* TODO*/
-          ERROR_KEYWORD_NOT_IMPLEMENTED(current_keyword_name.buffer);
+          /* Parse the first card like a normal INCLUDE*/
+          if (card_index == 0) {
+            _parse_include_file_name_card(
+                &card, &card_index, &line, line_length,
+                &current_multi_line_string, &current_multi_line_index,
+                num_include_paths_ptr, include_paths_ptr, callback, user_data,
+                &error_stack, &error_stack_size, &error_ptr, file_name,
+                line_count, root_folder_ptr);
+            continue;
+          } else if (card_index == 1) {
+            /* Ignore the card it is irrelevant for the parsing*/
+          } else {
+            ERROR_F(
+                "%s:%zu: Invalid number of cards for INCLUDE_NASTRAN keyword",
+                file_name, line_count);
+          }
+
+          /* continue without calling the callback for the card*/
+          if (card.string != line.buffer) {
+            free(card.string);
+          }
+
+          card_index++;
+          continue;
         } else {
           char *keyword_name;
           if (current_keyword_length < EXTRA_STRING_BUFFER_SIZE) {
             keyword_name = current_keyword_name.buffer;
           } else {
             keyword_name = malloc(current_keyword_length + 1);
             extra_string_copy_to_string(keyword_name, &current_keyword_name,
                                         current_keyword_length);
             keyword_name[current_keyword_length] = '\0';
           }
 
-          ERROR_F("%s:%lu: Invalid INCLUDE keyword: \"%s\"", file_name,
+          ERROR_F("%s:%zu: Unsupported INCLUDE keyword: \"%s\"", file_name,
                   current_keyword_line, keyword_name);
 
           if (keyword_name != current_keyword_name.buffer) {
             free(keyword_name);
           }
         }
       }
@@ -607,16 +623,18 @@
     }
     free(*include_paths_ptr);
     free(include_paths_ptr);
   }
   if (!num_include_paths) {
     free(num_include_paths_ptr);
   }
+  if (!root_folder) {
+    free(root_folder_ptr);
+  }
 
-  free(file_parent_path);
   free(line.extra);
   free(current_keyword_name.extra);
 
   fclose(file);
 
   if (error_stack) {
     if (!error_string) {
@@ -1333,15 +1351,15 @@
   END_PROFILE_FUNC();
   return value;
 }
 
 char *card_parse_whole_no_trim(const card_t *card) {
   BEGIN_PROFILE_FUNC();
 
-  const int len = strlen(card->string);
+  const size_t len = strlen(card->string);
   char *value = malloc(len + 1);
   memcpy(value, card->string, len + 1);
 
   END_PROFILE_FUNC();
   return value;
 }
 
@@ -1466,7 +1484,152 @@
       return CARD_PARSE_FLOAT;
     }
   }
 
   END_PROFILE_FUNC();
   return CARD_PARSE_STRING;
 }
+
+void _card_cpy(const card_t *card, char *dst, size_t len) {
+  BEGIN_PROFILE_FUNC();
+
+  memcpy(dst, card->string, len);
+
+  END_PROFILE_FUNC();
+}
+
+int _parse_multi_line_string(char **multi_line_string, size_t *multi_line_index,
+                             const card_t *card, size_t line_length) {
+  BEGIN_PROFILE_FUNC();
+
+  size_t card_string_index = 0;
+
+  if (!*multi_line_string) {
+    /* The maximum size of an include file name is 236 (+ null
+     * terminator)*/
+    *multi_line_string = malloc(237 * sizeof(char));
+    /* Trim leading white space*/
+    while (card_string_index != line_length &&
+           card->string[card_string_index] == ' ') {
+      card_string_index++;
+    }
+    if (card_string_index == line_length) {
+      (*multi_line_string)[0] = '\0';
+
+      END_PROFILE_FUNC();
+      return 1;
+    }
+  }
+
+  line_length -= card_string_index;
+
+  /* Support multi line strings which are longer than 236 (out of spec)*/
+  if (*multi_line_index + line_length > 236) {
+    *multi_line_string =
+        realloc(*multi_line_string,
+                (*multi_line_index + line_length + 1) * sizeof(char));
+  }
+
+  memcpy(&(*multi_line_string)[*multi_line_index],
+         &card->string[card_string_index], line_length);
+  *multi_line_index += line_length;
+  if ((*multi_line_string)[*multi_line_index - 2] == ' ' &&
+      (*multi_line_string)[*multi_line_index - 1] == '+') {
+    /* We have a multi line file name*/
+    *multi_line_index -= 2;
+
+    END_PROFILE_FUNC();
+    return 0;
+  }
+
+  /* Trim trailing white space*/
+  while ((*multi_line_string)[*multi_line_index - 1] == ' ' &&
+         *multi_line_index != 0) {
+    (*multi_line_index)--;
+  }
+
+  (*multi_line_string)[*multi_line_index] = '\0';
+
+  END_PROFILE_FUNC();
+  return 1;
+}
+
+void _parse_include_file_name_card(
+    const card_t *card, size_t *card_index, const extra_string *line,
+    size_t line_length, char **current_multi_line_string,
+    size_t *current_multi_line_index, size_t *num_include_paths,
+    char ***include_paths, key_file_callback callback, void *user_data,
+    char **error_stack, size_t *error_stack_size, size_t *error_ptr,
+    const char *file_name, size_t line_count, const char *root_folder) {
+  /* Support multi line file names (LS Dyna Manual Volume I
+   * *INCLUDE Remark 2, p. 2690)*/
+  if (!_parse_multi_line_string(current_multi_line_string,
+                                current_multi_line_index, card, line_length)) {
+    /* continue without calling the callback for the card*/
+    if (card->string != line->buffer) {
+      free(card->string);
+    }
+    return;
+  }
+
+  char *final_include_file_name = NULL;
+
+  /* Loop over all include paths and look for file*/
+  size_t i = 0;
+  while (i < *num_include_paths) {
+    char *full_include_file_name =
+        path_join((*include_paths)[i], *current_multi_line_string);
+
+    if (path_is_file(full_include_file_name)) {
+      final_include_file_name = full_include_file_name;
+      break;
+    }
+
+    free(full_include_file_name);
+
+    i++;
+  }
+
+  if (final_include_file_name) {
+    char *include_error;
+    /* Call the function recursively*/
+    key_file_parse_with_callback(final_include_file_name, callback, 1,
+                                 &include_error, user_data, include_paths,
+                                 num_include_paths, root_folder);
+    free(final_include_file_name);
+
+    /* Add the error to the error stack if an error occurred in the
+     * recursive call*/
+    if (include_error != NULL) {
+      const size_t error_msg_len = strlen(include_error);
+      *error_stack_size += error_msg_len + 1;
+      *error_stack = realloc(*error_stack, *error_stack_size);
+      memcpy(&(*error_stack)[*error_ptr], include_error, error_msg_len);
+      *error_ptr += error_msg_len;
+      (*error_stack)[*error_ptr] = '\n';
+      (*error_ptr)++;
+      free(include_error);
+    }
+  } else {
+    const int error_buffer_size =
+        snprintf(((void *)0), 0, "%s:%zu: \"%s\" could not be found", file_name,
+                 line_count, *current_multi_line_string);
+    *error_stack_size += error_buffer_size + 1;
+    *error_stack = realloc(*error_stack, *error_stack_size);
+    sprintf(&(*error_stack)[*error_ptr], "%s:%zu: \"%s\" could not be found",
+            file_name, line_count, *current_multi_line_string);
+    *error_ptr += error_buffer_size;
+    (*error_stack)[*error_ptr] = '\n';
+    (*error_ptr)++;
+  }
+
+  free(*current_multi_line_string);
+  *current_multi_line_string = NULL;
+  *current_multi_line_index = 0;
+
+  /* continue without calling the callback for the card*/
+  if (card->string != line->buffer) {
+    free(card->string);
+  }
+
+  (*card_index)++;
+}
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/key.h` & `dynareadout-23.5/lib/dynareadout/src/key.h`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #ifndef KEY_H
 #define KEY_H
 
-#include <stddef.h>
+#include "extra_string.h"
 #include <stdint.h>
 
 #define DEFAULT_VALUE_WIDTH 10
 #define NODE_VALUE_WIDTH 8
 #define INCLUDE_FILE_PATH_MAX 236
 
 /* The different types a value inside of a card can have*/
@@ -80,15 +80,16 @@
  * user_data: will be given to the callback untouched.
  * include_paths and num_include_paths: this is only used for recursion and both
  * should be set to NULL*/
 void key_file_parse_with_callback(const char *file_name,
                                   key_file_callback callback,
                                   int parse_includes, char **error_string,
                                   void *user_data, char ***include_paths,
-                                  size_t *num_include_paths);
+                                  size_t *num_include_paths,
+                                  const char *root_folder);
 /* Deallocates the data returned by key_file_parse*/
 void key_file_free(keyword_t *keywords, size_t num_keywords);
 /* Returns a certain keyword with name. If the key file contains more keywords
  * of the same name, index should be used to get the desired one. Where 0 refers
  * to the first one encountered in the file.*/
 keyword_t *key_file_get(keyword_t *keywords, size_t num_keywords,
                         const char *name, size_t index);
@@ -175,12 +176,28 @@
  * card_parse_begin. If CARD_PARSE_INT is returned the card_parse_int functions
  * can parse it. If CARD_PARSE_FLOAT is returned the card_parse_float functions
  * can parse it. Else only the card_parse_string functions can parse it. Uses
  * the value width provided here.*/
 card_parse_type card_parse_get_type_width(const card_t *card,
                                           uint8_t value_width);
 
+/* ----- Private Functions -----*/
+/* Copy the contents of the card as a string directly into dst.*/
+void _card_cpy(const card_t *card, char *dst, size_t len);
+/* Handles the parsing of multi line string for include file names. Returns
+ * wether to multi line string has been completely parsed.*/
+int _parse_multi_line_string(char **multi_line_string, size_t *multi_line_index,
+                             const card_t *card, size_t line_length);
+void _parse_include_file_name_card(
+    const card_t *card, size_t *card_index, const extra_string *line,
+    size_t line_length, char **current_multi_line_string,
+    size_t *current_multi_line_index, size_t *num_include_paths,
+    char ***include_paths, key_file_callback callback, void *user_data,
+    char **error_stack, size_t *error_stack_size, size_t *error_ptr,
+    const char *file_name, size_t line_count, const char *root_folder);
+/* -----------------------------*/
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/path.c` & `dynareadout-23.5/lib/dynareadout/src/path.c`

 * *Files 11% similar despite different names*

```diff
@@ -210,8 +210,37 @@
                   (path_name[1] == ':') && (path_name[2] == REAL_PATH_SEP));
 #else
   const int rv = path_name[0] == PATH_SEP;
 #endif
 
   END_PROFILE_FUNC();
   return rv;
-}
+}
+
+#ifdef _WIN32
+uint64_t path_get_file_size(const char *path_name) {
+  BEGIN_PROFILE_FUNC();
+
+  ULONGLONG file_size = 0;
+  WIN32_FILE_ATTRIBUTE_DATA file_info;
+  if (GetFileAttributesEx(path_name, GetFileExInfoStandard, &file_info)) {
+    file_size =
+        ((ULONGLONG)file_info.nFileSizeHigh << 32) | file_info.nFileSizeLow;
+  }
+
+  END_PROFILE_FUNC();
+  return (uint64_t)file_size;
+}
+#else
+uint64_t path_get_file_size(const char *path_name) {
+  BEGIN_PROFILE_FUNC();
+
+  uint64_t size = 0;
+  struct stat st;
+  if (stat(path_name, &st) == 0) {
+    size = (uint64_t)st.st_size;
+  }
+
+  END_PROFILE_FUNC();
+  return size;
+}
+#endif
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/path.h` & `dynareadout-23.5/lib/dynareadout/src/path.h`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #ifndef PATH_H
 #define PATH_H
+#include <stdint.h>
 #include <stdlib.h>
 
 /* TODO: Make sure to use the correct PATH_SEP on windows when working with the
  * real file system*/
 #define PATH_SEP '/'
 #ifdef _WIN32
 #define REAL_PATH_SEP '\\'
@@ -58,12 +59,16 @@
 
 /* Returns the current working directory. Needs to be deallocated by free.*/
 char *path_working_directory();
 
 /* Returns wether a path is absolute*/
 int path_is_abs(const char *path_name);
 
+/* Returns the size of the file given by path_name in bytes. If the retrieval
+ * fails it returns 0.*/
+uint64_t path_get_file_size(const char *path_name);
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/path_view.c` & `dynareadout-23.5/lib/dynareadout/src/path_view.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/path_view.h` & `dynareadout-23.5/lib/dynareadout/src/path_view.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/pgni.h` & `dynareadout-23.5/lib/dynareadout/src/pgni.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/profiling.c` & `dynareadout-23.5/lib/dynareadout/src/profiling.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/profiling.h` & `dynareadout-23.5/lib/dynareadout/src/profiling.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/python/conversions.hpp` & `dynareadout-23.5/lib/dynareadout/src/python/conversions.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_key.cpp` & `dynareadout-23.5/lib/dynareadout/src/python/pybind11_key.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_module.cpp` & `dynareadout-23.5/lib/dynareadout/src/python/pybind11_module.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/LICENSE` & `dynareadout-23.5/lib/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/attr.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/buffer_info.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/cast.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/chrono.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/complex.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/class.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/common.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/descr.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/init.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/internals.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/typeid.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/eigen.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/embed.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/eval.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/functional.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/gil.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/iostream.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/numpy.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/operators.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/options.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/pybind11.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/pytypes.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/stl/filesystem.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/stl.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/lib/pybind11/include/pybind11/stl_bind.h` & `dynareadout-23.5/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/pyproject.toml` & `dynareadout-23.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynareadout"
-version = "23.04.2"
+version = "23.05"
 authors = [
   { name = "PucklaJ", email = "jonaas.pucher000000@gmail.com"},
 ]
 description = "Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dynareadout-23.4.2/setup.py` & `dynareadout-23.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,21 @@
         os.path.join(dynareadout_dir, 'src', 'key.c'),
         os.path.join(dynareadout_dir, 'src', 'path.c'),
         os.path.join(dynareadout_dir, 'src', 'path_view.c'),
         # C++ Source Files
         os.path.join(dynareadout_dir, 'src', 'cpp', 'binout.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot_part.cpp'),
+        os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot_state.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'key.cpp'),
         # C++ Source Files for pybind11 module
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_binout.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_d3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_key.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_module.cpp'),
     ])
 
 setup(name='dynareadout',
-      version='23.04.2',
+      version='23.05',
       ext_modules=[dynareadout_c],
       zip_safe=False,
       include_package_data=True)
```

### Comparing `dynareadout-23.4.2/src/dynareadout/__init__.py` & `dynareadout-23.5/src/dynareadout/__init__.py`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.2/src/dynareadout.egg-info/PKG-INFO` & `dynareadout-23.5/src/dynareadout.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.4.2
+Version: 23.5
 Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -16,14 +16,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dynareadout
 
 An Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 
+## Documentation
+
+You can find a [Wiki](https://github.com/PucklaJ/dynareadout/wiki) with API Documentation for python.
+
 ## Examples
 
 ### Binout
 
 ```python
 from dynareadout import Binout, BinoutType
```

### Comparing `dynareadout-23.4.2/src/dynareadout.egg-info/SOURCES.txt` & `dynareadout-23.5/src/dynareadout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 lib/dynareadout/src/cpp/array.hpp
 lib/dynareadout/src/cpp/binout.cpp
 lib/dynareadout/src/cpp/binout.hpp
 lib/dynareadout/src/cpp/d3plot.cpp
 lib/dynareadout/src/cpp/d3plot.hpp
 lib/dynareadout/src/cpp/d3plot_part.cpp
 lib/dynareadout/src/cpp/d3plot_part.hpp
+lib/dynareadout/src/cpp/d3plot_state.cpp
+lib/dynareadout/src/cpp/d3plot_state.hpp
 lib/dynareadout/src/cpp/key.cpp
 lib/dynareadout/src/cpp/key.hpp
 lib/dynareadout/src/cpp/vec.hpp
 lib/dynareadout/src/python/conversions.hpp
 lib/dynareadout/src/python/pybind11_binout.cpp
 lib/dynareadout/src/python/pybind11_d3plot.cpp
 lib/dynareadout/src/python/pybind11_key.cpp
```

