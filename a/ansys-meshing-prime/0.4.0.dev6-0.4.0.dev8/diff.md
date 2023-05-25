# Comparing `tmp/ansys-meshing-prime-0.4.0.dev6.tar.gz` & `tmp/ansys_meshing_prime-0.4.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-meshing-prime-0.4.0.dev6.tar", last modified: Wed Apr 19 19:50:42 2023, max compression
+gzip compressed data, was "ansys_meshing_prime-0.4.0.dev8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-meshing-prime-0.4.0.dev6.tar` & `ansys_meshing_prime-0.4.0.dev8.tar`

### file list

```diff
@@ -1,117 +1,119 @@
--rw-r--r--   0        0        0     1090 2023-04-19 19:50:28.381177 ansys-meshing-prime-0.4.0.dev6/LICENSE
--rw-r--r--   0        0        0     2983 2023-04-19 19:50:28.381177 ansys-meshing-prime-0.4.0.dev6/README.md
--rw-r--r--   0        0        0     2054 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     6098 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/__init__.py
--rw-r--r--   0        0        0     2650 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/automesh.py
--rw-r--r--   0        0        0    59522 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/automeshstructs.py
--rw-r--r--   0        0        0     6111 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
--rw-r--r--   0        0        0     3847 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetool.py
--rw-r--r--   0        0        0    14701 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
--rw-r--r--   0        0        0    15524 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commonstructs.py
--rw-r--r--   0        0        0     3875 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commontypes.py
--rw-r--r--   0        0        0    12295 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connect.py
--rw-r--r--   0        0        0    54150 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connectstructs.py
--rw-r--r--   0        0        0    10456 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controldata.py
--rw-r--r--   0        0        0    55335 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controlstructs.py
--rw-r--r--   0        0        0      714 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/coreobject.py
--rw-r--r--   0        0        0     3427 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetool.py
--rw-r--r--   0        0        0    13990 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetoolstructs.py
--rw-r--r--   0        0        0     5573 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextraction.py
--rw-r--r--   0        0        0    33896 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextractionstructs.py
--rw-r--r--   0        0        0    29402 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileio.py
--rw-r--r--   0        0        0   126575 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileiostructs.py
--rw-r--r--   0        0        0    60431 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/igastructs.py
--rw-r--r--   0        0        0     4093 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanager.py
--rw-r--r--   0        0        0    16296 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
--rw-r--r--   0        0        0     4858 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfo.py
--rw-r--r--   0        0        0    60035 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfostructs.py
--rw-r--r--   0        0        0    16491 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/model.py
--rw-r--r--   0        0        0    27227 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/modelstructs.py
--rw-r--r--   0        0        0     3793 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpher.py
--rw-r--r--   0        0        0     7831 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
--rw-r--r--   0        0        0    25161 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpherstructs.py
--rw-r--r--   0        0        0    58131 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/part.py
--rw-r--r--   0        0        0   167481 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/partstructs.py
--rw-r--r--   0        0        0     7502 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrol.py
--rw-r--r--   0        0        0    13315 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
--rw-r--r--   0        0        0    27640 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/primeconfig.py
--rw-r--r--   0        0        0     5727 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrol.py
--rw-r--r--   0        0        0    14563 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
--rw-r--r--   0        0        0     3773 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/quadtospline.py
--rw-r--r--   0        0        0     7237 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolder.py
--rw-r--r--   0        0        0    29265 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolderstructs.py
--rw-r--r--   0        0        0    18382 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrol.py
--rw-r--r--   0        0        0    52720 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
--rw-r--r--   0        0        0     2790 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefield.py
--rw-r--r--   0        0        0    18893 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefieldstructs.py
--rw-r--r--   0        0        0     4241 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/splittoolstructs.py
--rw-r--r--   0        0        0    19710 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearch.py
--rw-r--r--   0        0        0   117867 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
--rw-r--r--   0        0        0    22036 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilities.py
--rw-r--r--   0        0        0   144419 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
--rw-r--r--   0        0        0     7182 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfer.py
--rw-r--r--   0        0        0    42738 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surferstructs.py
--rw-r--r--   0        0        0     4432 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
--rw-r--r--   0        0        0     6689 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
--rw-r--r--   0        0        0     8477 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topodata.py
--rw-r--r--   0        0        0     2646 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilities.py
--rw-r--r--   0        0        0    13167 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilitystructs.py
--rw-r--r--   0        0        0     2960 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transform.py
--rw-r--r--   0        0        0     8727 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transformstructs.py
--rw-r--r--   0        0        0     5980 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrol.py
--rw-r--r--   0        0        0     6259 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
--rw-r--r--   0        0        0     4893 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtool.py
--rw-r--r--   0        0        0    29508 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
--rw-r--r--   0        0        0     2761 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearch.py
--rw-r--r--   0        0        0    25492 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearchstructs.py
--rw-r--r--   0        0        0     4886 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesweeper.py
--rw-r--r--   0        0        0    25535 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
--rw-r--r--   0        0        0     5426 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapper.py
--rw-r--r--   0        0        0    10816 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrappercontrol.py
--rw-r--r--   0        0        0    61895 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapperstructs.py
--rw-r--r--   0        0        0    13848 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/controldata.py
--rw-r--r--   0        0        0    17032 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/fileio.py
--rw-r--r--   0        0        0    10734 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/model.py
--rw-r--r--   0        0        0     4207 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/part.py
--rw-r--r--   0        0        0     2314 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/periodiccontrol.py
--rw-r--r--   0        0        0     2193 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/sizecontrol.py
--rw-r--r--   0        0        0     4091 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfaceutilities.py
--rw-r--r--   0        0        0     4400 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfer.py
--rw-r--r--   0        0        0     2308 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/volumecontrol.py
--rw-r--r--   0        0        0     2823 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/volumesweeper.py
--rw-r--r--   0        0        0     5692 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrapper.py
--rw-r--r--   0        0        0     2141 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrappercontrol.py
--rw-r--r--   0        0        0      347 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/download_utilities.py
--rw-r--r--   0        0        0    15180 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/examples.py
--rw-r--r--   0        0        0       59 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/__init__.py
--rw-r--r--   0        0        0    34726 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/graphics.py
--rw-r--r--   0        0        0     2234 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/bin.png
--rw-r--r--   0        0        0     1708 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/invert_visibility.png
--rw-r--r--   0        0        0     2510 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/parts.png
--rw-r--r--   0        0        0     1297 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/selectioninfo.png
--rw-r--r--   0        0        0     2440 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/show_edges.png
--rw-r--r--   0        0        0      203 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/show_ruler.png
--rw-r--r--   0        0        0     1547 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/surface_body.png
--rw-r--r--   0        0        0     4484 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/client.py
--rw-r--r--   0        0        0      238 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/comm_manager.py
--rw-r--r--   0        0        0      506 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/communicator.py
--rw-r--r--   0        0        0     2960 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/config.py
--rw-r--r--   0        0        0     3077 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/defaults.py
--rw-r--r--   0        0        0    33288 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/error_handling.py
--rw-r--r--   0        0        0     6130 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/grpc_communicator.py
--rw-r--r--   0        0        0      492 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/grpc_utils.py
--rw-r--r--   0        0        0     1444 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/json_utils.py
--rw-r--r--   0        0        0     8029 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/launcher.py
--rw-r--r--   0        0        0     1720 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/prime_communicator.py
--rw-r--r--   0        0        0     7634 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/utils.py
--rw-r--r--   0        0        0      143 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/__init__.py
--rw-r--r--   0        0        0    68592 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/mesh_util.py
--rw-r--r--   0        0        0     7399 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/scope.py
--rw-r--r--   0        0        0     1649 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/utils.py
--rw-r--r--   0        0        0     2059 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/params/primestructs.py
--rw-r--r--   0        0        0     4345 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/__init__.py
--rw-r--r--   0        0        0    10039 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/decoder.py
--rw-r--r--   0        0        0    12256 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/encoder.py
--rw-r--r--   0        0        0     2623 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/scanner.py
--rw-r--r--   0        0        0     4882 1970-01-01 00:00:00.000000 ansys-meshing-prime-0.4.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-19 16:26:35.466403 ansys_meshing_prime-0.4.0.dev8/LICENSE
+-rw-r--r--   0        0        0     3036 2023-05-19 16:26:35.466403 ansys_meshing_prime-0.4.0.dev8/README.md
+-rw-r--r--   0        0        0     2029 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     6098 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/__init__.py
+-rw-r--r--   0        0        0     2650 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automesh.py
+-rw-r--r--   0        0        0    59522 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automeshstructs.py
+-rw-r--r--   0        0        0     6111 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
+-rw-r--r--   0        0        0     3847 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetool.py
+-rw-r--r--   0        0        0    14701 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
+-rw-r--r--   0        0        0    15524 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commonstructs.py
+-rw-r--r--   0        0        0     3875 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commontypes.py
+-rw-r--r--   0        0        0     9883 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connect.py
+-rw-r--r--   0        0        0    39669 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connectstructs.py
+-rw-r--r--   0        0        0    10456 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controldata.py
+-rw-r--r--   0        0        0    55335 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controlstructs.py
+-rw-r--r--   0        0        0      714 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/coreobject.py
+-rw-r--r--   0        0        0     3427 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetool.py
+-rw-r--r--   0        0        0    13990 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetoolstructs.py
+-rw-r--r--   0        0        0     5573 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextraction.py
+-rw-r--r--   0        0        0    33896 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextractionstructs.py
+-rw-r--r--   0        0        0    24627 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileio.py
+-rw-r--r--   0        0        0   112910 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileiostructs.py
+-rw-r--r--   0        0        0    60431 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/igastructs.py
+-rw-r--r--   0        0        0     4093 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanager.py
+-rw-r--r--   0        0        0    16296 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
+-rw-r--r--   0        0        0     4858 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfo.py
+-rw-r--r--   0        0        0    60035 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfostructs.py
+-rw-r--r--   0        0        0    16491 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/model.py
+-rw-r--r--   0        0        0    27227 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/modelstructs.py
+-rw-r--r--   0        0        0     3793 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpher.py
+-rw-r--r--   0        0        0     7831 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
+-rw-r--r--   0        0        0    24059 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherstructs.py
+-rw-r--r--   0        0        0    58131 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/part.py
+-rw-r--r--   0        0        0   167481 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/partstructs.py
+-rw-r--r--   0        0        0     7502 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrol.py
+-rw-r--r--   0        0        0    13315 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
+-rw-r--r--   0        0        0    28641 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/primeconfig.py
+-rw-r--r--   0        0        0     5727 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrol.py
+-rw-r--r--   0        0        0    14563 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
+-rw-r--r--   0        0        0     3773 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/quadtospline.py
+-rw-r--r--   0        0        0     7237 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolder.py
+-rw-r--r--   0        0        0    29265 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolderstructs.py
+-rw-r--r--   0        0        0    18382 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrol.py
+-rw-r--r--   0        0        0    52720 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
+-rw-r--r--   0        0        0     2790 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefield.py
+-rw-r--r--   0        0        0    18893 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefieldstructs.py
+-rw-r--r--   0        0        0     4241 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/splittoolstructs.py
+-rw-r--r--   0        0        0    19710 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearch.py
+-rw-r--r--   0        0        0   117867 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
+-rw-r--r--   0        0        0    22036 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilities.py
+-rw-r--r--   0        0        0   144419 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
+-rw-r--r--   0        0        0     7182 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfer.py
+-rw-r--r--   0        0        0    44962 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surferstructs.py
+-rw-r--r--   0        0        0     4448 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
+-rw-r--r--   0        0        0     6689 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
+-rw-r--r--   0        0        0     8477 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topodata.py
+-rw-r--r--   0        0        0     2646 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilities.py
+-rw-r--r--   0        0        0    13167 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilitystructs.py
+-rw-r--r--   0        0        0     2960 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transform.py
+-rw-r--r--   0        0        0     8727 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transformstructs.py
+-rw-r--r--   0        0        0     5980 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrol.py
+-rw-r--r--   0        0        0     6259 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
+-rw-r--r--   0        0        0     4893 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtool.py
+-rw-r--r--   0        0        0    29508 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
+-rw-r--r--   0        0        0     2761 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearch.py
+-rw-r--r--   0        0        0    25492 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearchstructs.py
+-rw-r--r--   0        0        0     4886 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeper.py
+-rw-r--r--   0        0        0    25535 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
+-rw-r--r--   0        0        0     5426 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapper.py
+-rw-r--r--   0        0        0    10816 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrappercontrol.py
+-rw-r--r--   0        0        0    61895 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapperstructs.py
+-rw-r--r--   0        0        0    13848 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/controldata.py
+-rw-r--r--   0        0        0    17135 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/fileio.py
+-rw-r--r--   0        0        0    10887 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/model.py
+-rw-r--r--   0        0        0     4207 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/part.py
+-rw-r--r--   0        0        0     2314 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/periodiccontrol.py
+-rw-r--r--   0        0        0     2193 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/sizecontrol.py
+-rw-r--r--   0        0        0     4091 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfaceutilities.py
+-rw-r--r--   0        0        0     4400 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfer.py
+-rw-r--r--   0        0        0     2308 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumecontrol.py
+-rw-r--r--   0        0        0     2823 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumesweeper.py
+-rw-r--r--   0        0        0     5692 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrapper.py
+-rw-r--r--   0        0        0     2141 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrappercontrol.py
+-rw-r--r--   0        0        0      691 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/__init__.py
+-rw-r--r--   0        0        0     4227 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/download_utilities.py
+-rw-r--r--   0        0        0    24869 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/examples.py
+-rw-r--r--   0        0        0     1392 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/unit_test_examples.py
+-rw-r--r--   0        0        0       59 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/__init__.py
+-rw-r--r--   0        0        0    35690 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/graphics.py
+-rw-r--r--   0        0        0     2234 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/bin.png
+-rw-r--r--   0        0        0     1708 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/invert_visibility.png
+-rw-r--r--   0        0        0     2510 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/parts.png
+-rw-r--r--   0        0        0     1297 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/selectioninfo.png
+-rw-r--r--   0        0        0     2440 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/show_edges.png
+-rw-r--r--   0        0        0      203 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/show_ruler.png
+-rw-r--r--   0        0        0     1547 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/surface_body.png
+-rw-r--r--   0        0        0     1600 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/trame_gui.py
+-rw-r--r--   0        0        0     4550 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/client.py
+-rw-r--r--   0        0        0      238 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/comm_manager.py
+-rw-r--r--   0        0        0      506 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/communicator.py
+-rw-r--r--   0        0        0     2960 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/config.py
+-rw-r--r--   0        0        0     3077 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/defaults.py
+-rw-r--r--   0        0        0    34238 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/error_handling.py
+-rw-r--r--   0        0        0     6130 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/grpc_communicator.py
+-rw-r--r--   0        0        0      492 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/grpc_utils.py
+-rw-r--r--   0        0        0     1444 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/json_utils.py
+-rw-r--r--   0        0        0     8029 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/launcher.py
+-rw-r--r--   0        0        0     1720 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/prime_communicator.py
+-rw-r--r--   0        0        0     7632 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/utils.py
+-rw-r--r--   0        0        0      143 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/__init__.py
+-rw-r--r--   0        0        0    68591 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/mesh_util.py
+-rw-r--r--   0        0        0     7399 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/scope.py
+-rw-r--r--   0        0        0     1493 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/utils.py
+-rw-r--r--   0        0        0     2059 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/params/primestructs.py
+-rw-r--r--   0        0        0     4345 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/__init__.py
+-rw-r--r--   0        0        0    10039 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/decoder.py
+-rw-r--r--   0        0        0    12256 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/encoder.py
+-rw-r--r--   0        0        0     2623 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/scanner.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.4.0.dev8/PKG-INFO
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/LICENSE` & `ansys_meshing_prime-0.4.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/README.md` & `ansys_meshing_prime-0.4.0.dev8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 # PyPrimeMesh
 
 [![pyansys](https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC)](https://docs.pyansys.com/)
-[![GH-CI](https://github.com/pyansys/pyprimemesh/actions/workflows/ci_cd.yml/badge.svg)](https://github.com/pyansys/pyprimemesh/actions/workflows/ci_cd.yml)
+[![GH-CI](https://github.com/ansys/pyprimemesh/actions/workflows/ci_cd.yml/badge.svg)](https://github.com/ansys/pyprimemesh/actions/workflows/ci_cd.yml)
 [![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
 
 ## Overview
 
-PyPrimeMesh provides a python client to Ansys Prime Server. Ansys Prime Server delivers core Ansys meshing technology.
+PyPrimeMesh is a Python client to Ansys Prime Server, which
+delivers core Ansys meshing technology.
 
 ## Documentation and Issues
 
 For information on PyPrimeMesh, refer to the latest [documentation](
 https://prime.docs.pyansys.com).
 
-For queries related to PyPrimeMesh, post on the [discussion](
-https://github.com/pyansys/pyprimemesh/discussions) page. 
+For queries related to PyPrimeMesh, post on the [PyPrimeMesh Discussions](
+https://github.com/ansys/pyprimemesh/discussions) page. 
 
-For bugs or enhancement requests, file an issue on our [issues](
-https://github.com/pyansys/pyprimemesh/issues) page. 
+For bugs or enhancement requests, post an issue on the [PyPrimeMesh Issues](
+https://github.com/ansys/pyprimemesh/issues) page. 
 
-For assistance, reach out to the PyAnsys
-Support team at [pyansys.support@ansys.com](mailto:pyansys.support@ansys.com).
+For assistance, reach out to the support team at
+[pyansys.core@ansys.com](mailto:pyansys.core@ansys.com).
 
 ## Installation
 
-The `ansys-meshing-prime` package supports Python 3.7 to Python 3.11 on Windows and Linux
-operating system.
+The `ansys-meshing-prime` package supports Python 3.8 to Python 3.11 on the Windows and Linux
+operating systems.
 
-PyPrimeMesh can be installed with all dependencies directly from PyPi as follows:
+
+PyPrimeMesh can be installed with all dependencies directly from PyPi by running
+this command:
 
 ```bash
 pip install ansys-meshing-prime[all]
 ```
 
 Alternatively, you can clone this repository and install the client using
+these commands:
 
 ```bash
-git clone https://github.com/pyansys/pyprimemesh
+git clone https://github.com/ansys/pyprimemesh
 cd pyprimemesh
 pip install -e .[all]
 ```
 
-The above command will install all functionality that is important to development.
-To install a basic version of the client, use the following command instead.
+The preceding commands install all functionality that is important to development.
+To install a basic version of the client, use this command instead:
 
 ```bash
 pip install -e .
 ```
 
 ## Dependencies
 
-You must have Ansys 2023 R1 or newer versions installed for Ansys Prime Server (optionally, CAD readers can be configured).  Ansys Prime Server requires a Preppost or CFD Preppost license to run.
+You must have Ansys 2023 R1 or later installed for access to Ansys Prime Server.
+Optionally, CAD readers can be configured. Ansys Prime Server requires
+an Ansys Mechanical PrepPost or Fluids PrepPost (CFD) license to run.
 
 ## Get Started
 
 ### Launching PyPrimeMesh
 
-To launch PyPrimeMesh:
+To launch PyPrimeMesh, use this code:
 
 ```python
 import ansys.meshing.prime as prime
 
 with prime.launch_prime() as prime_client:
     model = prime_client.model
 ```
@@ -69,8 +75,8 @@
 ## License and Acknowledgments
 
 PyPrimeMesh is licensed under the MIT license.
 
 PyPrimeMesh makes no commercial claim over Ansys whatsoever. This library extends the functionality of
 Ansys Prime Server by adding a Python interface without changing the core behavior or license
 of the original software. The use of Ansys Prime Server requires a legally licensed copy of Ansys
-Workbench.
+2023 or later.
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/pyproject.toml` & `ansys_meshing_prime-0.4.0.dev8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-meshing-prime"
-version = "0.4.0.dev6"
-description = "PyPrimeMesh provides a python client to Ansys Prime Server. Ansys Prime Server delivers core Ansys meshing technology."
+version = "0.4.0.dev8"
+description = "PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology."
 readme = "README.md"
-requires-python = ">=3.7,<4"
+requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
-authors = [{name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"}]
-maintainers = [{name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"}]
+authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
+maintainers =  [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
@@ -32,42 +31,44 @@
 [project.optional-dependencies]
 graphics = [
   "pyvista>=0.32.0",
 ]
 tests = [
   "pytest==7.3.1",
   "pytest-cov==4.0.0",
+  "pytest-pyvista==0.1.8",
+  "pyvista[trame]==0.38.6"
 ]
 doc = [
-  "ansys-sphinx-theme==0.9.7",
+  "ansys-sphinx-theme==0.9.8",
   "jupyter-sphinx==0.4.0",
   "numpydoc==1.5.0",
-  "pyvista==0.38.5",
-  "Sphinx==5.3.0",
-  "sphinx-autodoc-typehints==1.22",
-  "sphinx-copybutton==0.5.1",
-  "sphinx-gallery==0.12.2",
+  "Sphinx==6.2.0",
+  "pyvista==0.38.6",
+  "sphinx-autodoc-typehints==1.23.0",
+  "sphinx-copybutton==0.5.2",
+  "sphinx-gallery==0.13.0",
   "sphinx-notfound-page==0.8.3",
   "sphinxemoji==0.2.0",
 ]
 all = [
   "pyvista>=0.32.0",
 ]
 
 [project.urls]
-Source = "https://github.com/pyansys/pyprimemesh"
+Source = "https://github.com/ansys/pyprimemesh"
 Documentation = "https://prime.docs.pyansys.com"
 
 
 [tool.flit.module]
 name = "ansys.meshing.prime"
 
 [tool.black]
 line-length = 100
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 skip-string-normalization = true
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/__init__.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/automesh.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automesh.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/automeshstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automeshstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetool.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetool.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetoolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commonstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commonstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commontypes.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commontypes.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connect.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connect.py`

 * *Files 13% similar despite different names*

```diff
@@ -209,52 +209,7 @@
         "with_face_zonelet_ids" : with_face_zonelet_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Connect/StitchFaceZonelets"
         self._model._print_logs_before_command("stitch_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("stitch_face_zonelets", ConnectResults(model = self._model, json_data = result))
         return ConnectResults(model = self._model, json_data = result)
-
-    def mesh_match_within_part_face_zonelets(self, part_id : int, source_face_zonelet_ids : Iterable[int], target_face_zonelet_ids : Iterable[int], params : MeshMatchParams) -> MeshMatchResults:
-        """ Perform mesh matching between overlapping face zonelets within a single part. Matched mesh can then be colocated, merged or removed as directed.
-
-
-        Parameters
-        ----------
-        part_id : int
-            Id of the part.
-        source_face_zonelet_ids : Iterable[int]
-            Ids of source face zonelets to be mesh matched.
-        target_face_zonelet_ids : Iterable[int]
-            Ids of target face zonelets to be mesh matched.
-        params : MeshMatchParams
-            Parameters for mesh matching.
-
-        Returns
-        -------
-        MeshMatchResults
-            Returns the MeshMatchResults.
-
-
-        Examples
-        --------
-        connect = Connect(model = model)
-        connect.mesh_match_within_part_face_zonelets(part.id, source_face_zonelet_ids, target_face_zonelet_ids, match_mesh_params)
-
-        """
-        if not isinstance(part_id, int):
-            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
-        if not isinstance(source_face_zonelet_ids, Iterable):
-            raise TypeError("Invalid argument type passed for source_face_zonelet_ids, valid argument type is Iterable[int].")
-        if not isinstance(target_face_zonelet_ids, Iterable):
-            raise TypeError("Invalid argument type passed for target_face_zonelet_ids, valid argument type is Iterable[int].")
-        if not isinstance(params, MeshMatchParams):
-            raise TypeError("Invalid argument type passed for params, valid argument type is MeshMatchParams.")
-        args = {"part_id" : part_id,
-        "source_face_zonelet_ids" : source_face_zonelet_ids,
-        "target_face_zonelet_ids" : target_face_zonelet_ids,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::Connect/MeshMatchWithinPartFaceZonelets"
-        self._model._print_logs_before_command("mesh_match_within_part_face_zonelets", args)
-        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("mesh_match_within_part_face_zonelets", MeshMatchResults(model = self._model, json_data = result))
-        return MeshMatchResults(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connectstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connectstructs.py`

 * *Files 14% similar despite different names*

```diff
@@ -913,324 +913,7 @@
         """Stitch type depending on nature of surface boundary edges to be stitched.
         """
         return self._type
 
     @type.setter
     def type(self, value: StitchType):
         self._type = value
-
-class MeshMatchParams(CoreObject):
-    """Parameters to match surface mesh.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            use_absolute_tolerance: bool,
-            gap_tolerance: float,
-            side_tolerance: float,
-            check_interior: bool,
-            matched_mesh_option: MatchedMeshOption):
-        self._use_absolute_tolerance = use_absolute_tolerance
-        self._gap_tolerance = gap_tolerance
-        self._side_tolerance = side_tolerance
-        self._check_interior = check_interior
-        self._matched_mesh_option = MatchedMeshOption(matched_mesh_option)
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            use_absolute_tolerance: bool = None,
-            gap_tolerance: float = None,
-            side_tolerance: float = None,
-            check_interior: bool = None,
-            matched_mesh_option: MatchedMeshOption = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the MeshMatchParams.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a MeshMatchParams object with default parameters.
-        use_absolute_tolerance: bool, optional
-            When true, gap tolerance and side tolerance provided are absolute values.
-        gap_tolerance: float, optional
-            Gap tolerance between faces to be matched.
-        side_tolerance: float, optional
-            Side tolerance for matching to the side edges.
-        check_interior: bool, optional
-            When true, checks all nodes including boundary edge nodes and nodes inside the faces.
-        matched_mesh_option: MatchedMeshOption, optional
-            Option for treatment of matched mesh.
-        json_data: dict, optional
-            JSON dictionary to create a MeshMatchParams object with provided parameters.
-
-        Examples
-        --------
-        >>> mesh_match_params = prime.MeshMatchParams(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["useAbsoluteTolerance"] if "useAbsoluteTolerance" in json_data else None,
-                json_data["gapTolerance"] if "gapTolerance" in json_data else None,
-                json_data["sideTolerance"] if "sideTolerance" in json_data else None,
-                json_data["checkInterior"] if "checkInterior" in json_data else None,
-                MatchedMeshOption(json_data["matchedMeshOption"] if "matchedMeshOption" in json_data else None))
-        else:
-            all_field_specified = all(arg is not None for arg in [use_absolute_tolerance, gap_tolerance, side_tolerance, check_interior, matched_mesh_option])
-            if all_field_specified:
-                self.__initialize(
-                    use_absolute_tolerance,
-                    gap_tolerance,
-                    side_tolerance,
-                    check_interior,
-                    matched_mesh_option)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "MeshMatchParams")
-                    json_data = param_json["MeshMatchParams"] if "MeshMatchParams" in param_json else {}
-                    self.__initialize(
-                        use_absolute_tolerance if use_absolute_tolerance is not None else ( MeshMatchParams._default_params["use_absolute_tolerance"] if "use_absolute_tolerance" in MeshMatchParams._default_params else (json_data["useAbsoluteTolerance"] if "useAbsoluteTolerance" in json_data else None)),
-                        gap_tolerance if gap_tolerance is not None else ( MeshMatchParams._default_params["gap_tolerance"] if "gap_tolerance" in MeshMatchParams._default_params else (json_data["gapTolerance"] if "gapTolerance" in json_data else None)),
-                        side_tolerance if side_tolerance is not None else ( MeshMatchParams._default_params["side_tolerance"] if "side_tolerance" in MeshMatchParams._default_params else (json_data["sideTolerance"] if "sideTolerance" in json_data else None)),
-                        check_interior if check_interior is not None else ( MeshMatchParams._default_params["check_interior"] if "check_interior" in MeshMatchParams._default_params else (json_data["checkInterior"] if "checkInterior" in json_data else None)),
-                        matched_mesh_option if matched_mesh_option is not None else ( MeshMatchParams._default_params["matched_mesh_option"] if "matched_mesh_option" in MeshMatchParams._default_params else MatchedMeshOption(json_data["matchedMeshOption"] if "matchedMeshOption" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            use_absolute_tolerance: bool = None,
-            gap_tolerance: float = None,
-            side_tolerance: float = None,
-            check_interior: bool = None,
-            matched_mesh_option: MatchedMeshOption = None):
-        """Set the default values of MeshMatchParams.
-
-        Parameters
-        ----------
-        use_absolute_tolerance: bool, optional
-            When true, gap tolerance and side tolerance provided are absolute values.
-        gap_tolerance: float, optional
-            Gap tolerance between faces to be matched.
-        side_tolerance: float, optional
-            Side tolerance for matching to the side edges.
-        check_interior: bool, optional
-            When true, checks all nodes including boundary edge nodes and nodes inside the faces.
-        matched_mesh_option: MatchedMeshOption, optional
-            Option for treatment of matched mesh.
-        """
-        args = locals()
-        [MeshMatchParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of MeshMatchParams.
-
-        Examples
-        --------
-        >>> MeshMatchParams.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in MeshMatchParams._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._use_absolute_tolerance is not None:
-            json_data["useAbsoluteTolerance"] = self._use_absolute_tolerance
-        if self._gap_tolerance is not None:
-            json_data["gapTolerance"] = self._gap_tolerance
-        if self._side_tolerance is not None:
-            json_data["sideTolerance"] = self._side_tolerance
-        if self._check_interior is not None:
-            json_data["checkInterior"] = self._check_interior
-        if self._matched_mesh_option is not None:
-            json_data["matchedMeshOption"] = self._matched_mesh_option
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "use_absolute_tolerance :  %s\ngap_tolerance :  %s\nside_tolerance :  %s\ncheck_interior :  %s\nmatched_mesh_option :  %s" % (self._use_absolute_tolerance, self._gap_tolerance, self._side_tolerance, self._check_interior, self._matched_mesh_option)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def use_absolute_tolerance(self) -> bool:
-        """When true, gap tolerance and side tolerance provided are absolute values.
-        """
-        return self._use_absolute_tolerance
-
-    @use_absolute_tolerance.setter
-    def use_absolute_tolerance(self, value: bool):
-        self._use_absolute_tolerance = value
-
-    @property
-    def gap_tolerance(self) -> float:
-        """Gap tolerance between faces to be matched.
-        """
-        return self._gap_tolerance
-
-    @gap_tolerance.setter
-    def gap_tolerance(self, value: float):
-        self._gap_tolerance = value
-
-    @property
-    def side_tolerance(self) -> float:
-        """Side tolerance for matching to the side edges.
-        """
-        return self._side_tolerance
-
-    @side_tolerance.setter
-    def side_tolerance(self, value: float):
-        self._side_tolerance = value
-
-    @property
-    def check_interior(self) -> bool:
-        """When true, checks all nodes including boundary edge nodes and nodes inside the faces.
-        """
-        return self._check_interior
-
-    @check_interior.setter
-    def check_interior(self, value: bool):
-        self._check_interior = value
-
-    @property
-    def matched_mesh_option(self) -> MatchedMeshOption:
-        """Option for treatment of matched mesh.
-        """
-        return self._matched_mesh_option
-
-    @matched_mesh_option.setter
-    def matched_mesh_option(self, value: MatchedMeshOption):
-        self._matched_mesh_option = value
-
-class MeshMatchResults(CoreObject):
-    """Results associated with the mesh match operations.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            matched_area: float,
-            error_code: ErrorCode):
-        self._matched_area = matched_area
-        self._error_code = ErrorCode(error_code)
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            matched_area: float = None,
-            error_code: ErrorCode = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the MeshMatchResults.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a MeshMatchResults object with default parameters.
-        matched_area: float, optional
-            The total area of matched regions from both source and target faces.
-        error_code: ErrorCode, optional
-            Error Code associated with failure of mesh match operation.
-        json_data: dict, optional
-            JSON dictionary to create a MeshMatchResults object with provided parameters.
-
-        Examples
-        --------
-        >>> mesh_match_results = prime.MeshMatchResults(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["matchedArea"] if "matchedArea" in json_data else None,
-                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None))
-        else:
-            all_field_specified = all(arg is not None for arg in [matched_area, error_code])
-            if all_field_specified:
-                self.__initialize(
-                    matched_area,
-                    error_code)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "MeshMatchResults")
-                    json_data = param_json["MeshMatchResults"] if "MeshMatchResults" in param_json else {}
-                    self.__initialize(
-                        matched_area if matched_area is not None else ( MeshMatchResults._default_params["matched_area"] if "matched_area" in MeshMatchResults._default_params else (json_data["matchedArea"] if "matchedArea" in json_data else None)),
-                        error_code if error_code is not None else ( MeshMatchResults._default_params["error_code"] if "error_code" in MeshMatchResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            matched_area: float = None,
-            error_code: ErrorCode = None):
-        """Set the default values of MeshMatchResults.
-
-        Parameters
-        ----------
-        matched_area: float, optional
-            The total area of matched regions from both source and target faces.
-        error_code: ErrorCode, optional
-            Error Code associated with failure of mesh match operation.
-        """
-        args = locals()
-        [MeshMatchResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of MeshMatchResults.
-
-        Examples
-        --------
-        >>> MeshMatchResults.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in MeshMatchResults._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._matched_area is not None:
-            json_data["matchedArea"] = self._matched_area
-        if self._error_code is not None:
-            json_data["errorCode"] = self._error_code
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "matched_area :  %s\nerror_code :  %s" % (self._matched_area, self._error_code)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def matched_area(self) -> float:
-        """The total area of matched regions from both source and target faces.
-        """
-        return self._matched_area
-
-    @matched_area.setter
-    def matched_area(self, value: float):
-        self._matched_area = value
-
-    @property
-    def error_code(self) -> ErrorCode:
-        """Error Code associated with failure of mesh match operation.
-        """
-        return self._error_code
-
-    @error_code.setter
-    def error_code(self, value: ErrorCode):
-        self._error_code = value
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controldata.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controlstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controlstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/coreobject.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/coreobject.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetool.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetool.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetoolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextraction.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextraction.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextractionstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextractionstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileio.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileio.py`

 * *Files 10% similar despite different names*

```diff
@@ -459,113 +459,14 @@
         "export_fluent_mesh_params" : export_fluent_mesh_params._jsonify()}
         command_name = "PrimeMesh::FileIO/ExportFluentMeshingMesh"
         self._model._print_logs_before_command("export_fluent_meshing_mesh", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("export_fluent_meshing_mesh", FileWriteResults(model = self._model, json_data = result))
         return FileWriteResults(model = self._model, json_data = result)
 
-    def import_lsdyna_keyword_file(self, file_name : str, import_params : ImportLSDynaKeywordFileParams) -> FileReadResults:
-        """ Imports LS-DYNA Keyword file.
-
-
-        Parameters
-        ----------
-        file_name : str
-            Name of the file.
-        import_params : ImportLSDynaKeywordFileParams
-            Parameters for LS-DYNA Keyword file import.
-
-        Returns
-        -------
-        FileReadResults
-            Returns FileReadResults.
-
-        Examples
-        --------
-        >>> results = file_io.import_lsdyna_keyword_file(file_name, ImportLSDynaKeywordFileParams(model = model))
-
-        """
-        if not isinstance(file_name, str):
-            raise TypeError("Invalid argument type passed for file_name, valid argument type is str.")
-        if not isinstance(import_params, ImportLSDynaKeywordFileParams):
-            raise TypeError("Invalid argument type passed for import_params, valid argument type is ImportLSDynaKeywordFileParams.")
-        args = {"file_name" : file_name,
-        "import_params" : import_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ImportLSDynaKeywordFile"
-        self._model._print_logs_before_command("import_lsdyna_keyword_file", args)
-        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("import_lsdyna_keyword_file", FileReadResults(model = self._model, json_data = result))
-        return FileReadResults(model = self._model, json_data = result)
-
-    def export_lsdyna_keyword_file(self, file_name : str, export_params : ExportLSDynaKeywordFileParams) -> FileWriteResults:
-        """ Export FEA LS-DYNA Keyword file for solid, or surface mesh, or both.
-
-
-        Parameters
-        ----------
-        file_name : str
-            Name of the file.
-        export_params : ExportLSDynaKeywordFileParams
-            Parameters for FEA LS-DYNA Keyword file export.
-
-        Returns
-        -------
-        FileWriteResults
-            Returns FileWriteResults.
-
-        Examples
-        --------
-        >>> results = file_io.export_lsdyna_keyword_file(file_name, ExportLSDynaKeywordFileParams(model = model))
-
-        """
-        if not isinstance(file_name, str):
-            raise TypeError("Invalid argument type passed for file_name, valid argument type is str.")
-        if not isinstance(export_params, ExportLSDynaKeywordFileParams):
-            raise TypeError("Invalid argument type passed for export_params, valid argument type is ExportLSDynaKeywordFileParams.")
-        args = {"file_name" : file_name,
-        "export_params" : export_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ExportLSDynaKeywordFile"
-        self._model._print_logs_before_command("export_lsdyna_keyword_file", args)
-        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("export_lsdyna_keyword_file", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
-
-    def export_lsdyna_iga_keyword_file(self, file_name : str, export_params : ExportLSDynaIgaKeywordFileParams) -> FileWriteResults:
-        """ Export IGA LS-DYNA Keyword file for solid, or surface splines, or both.
-
-
-        Parameters
-        ----------
-        file_name : str
-            Name of the file.
-        export_params : ExportLSDynaIgaKeywordFileParams
-            Parameters for IGA LS-DYNA Keyword file export.
-
-        Returns
-        -------
-        FileWriteResults
-            Returns FileWriteResults.
-
-        Examples
-        --------
-        >>> results = file_io.export_lsdyna_iga_keyword_file(file_name, ExportLSDynaIgaKeywordFileParams(model = model))
-
-        """
-        if not isinstance(file_name, str):
-            raise TypeError("Invalid argument type passed for file_name, valid argument type is str.")
-        if not isinstance(export_params, ExportLSDynaIgaKeywordFileParams):
-            raise TypeError("Invalid argument type passed for export_params, valid argument type is ExportLSDynaIgaKeywordFileParams.")
-        args = {"file_name" : file_name,
-        "export_params" : export_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ExportLSDynaIgaKeywordFile"
-        self._model._print_logs_before_command("export_lsdyna_iga_keyword_file", args)
-        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("export_lsdyna_iga_keyword_file", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
-
     def export_boundary_fitted_spline_kfile(self, file_name : str, export_params : ExportBoundaryFittedSplineParams) -> FileWriteResults:
         """ Export IGA LS-DYNA Keyword file for boundary fitted spline.
 
 
         Parameters
         ----------
         file_name : str
@@ -654,16 +555,14 @@
 
         Notes
         -----
         This API does not support Unicode paths now.
 
         Examples
         --------
-        >>> import ansys.meshing.prime as prime
-        >>> model = prime.local_model()
         >>> fileio = prime.FileIO(model=model)
         >>> out_file_path = r"/tmp/output.stl"
         >>> part_ids = [part.id for part in model.parts]
         >>> export_stl_params=prime.ExportSTLParams(model=model,part_ids=part_ids)
         >>> results = fileio.export_stl(out_file_path,export_stl_params)
 
         """
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileiostructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileiostructs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2513,339 +2513,14 @@
         """
         return self._error_code
 
     @error_code.setter
     def error_code(self, value: ErrorCode):
         self._error_code = value
 
-class ImportLSDynaKeywordFileParams(CoreObject):
-    """Parameters to control LS-DYNA keyword file import settings.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            drop_mid_nodes: bool,
-            append: bool):
-        self._drop_mid_nodes = drop_mid_nodes
-        self._append = append
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            drop_mid_nodes: bool = None,
-            append: bool = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the ImportLSDynaKeywordFileParams.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a ImportLSDynaKeywordFileParams object with default parameters.
-        drop_mid_nodes: bool, optional
-            Option to import quadratic mesh elements as linear skipping the mid nodes.
-        append: bool, optional
-            Option to append imported k file into existing model.
-        json_data: dict, optional
-            JSON dictionary to create a ImportLSDynaKeywordFileParams object with provided parameters.
-
-        Examples
-        --------
-        >>> import_lsdyna_keyword_file_params = prime.ImportLSDynaKeywordFileParams(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["dropMidNodes"] if "dropMidNodes" in json_data else None,
-                json_data["append"] if "append" in json_data else None)
-        else:
-            all_field_specified = all(arg is not None for arg in [drop_mid_nodes, append])
-            if all_field_specified:
-                self.__initialize(
-                    drop_mid_nodes,
-                    append)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "ImportLSDynaKeywordFileParams")
-                    json_data = param_json["ImportLSDynaKeywordFileParams"] if "ImportLSDynaKeywordFileParams" in param_json else {}
-                    self.__initialize(
-                        drop_mid_nodes if drop_mid_nodes is not None else ( ImportLSDynaKeywordFileParams._default_params["drop_mid_nodes"] if "drop_mid_nodes" in ImportLSDynaKeywordFileParams._default_params else (json_data["dropMidNodes"] if "dropMidNodes" in json_data else None)),
-                        append if append is not None else ( ImportLSDynaKeywordFileParams._default_params["append"] if "append" in ImportLSDynaKeywordFileParams._default_params else (json_data["append"] if "append" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            drop_mid_nodes: bool = None,
-            append: bool = None):
-        """Set the default values of ImportLSDynaKeywordFileParams.
-
-        Parameters
-        ----------
-        drop_mid_nodes: bool, optional
-            Option to import quadratic mesh elements as linear skipping the mid nodes.
-        append: bool, optional
-            Option to append imported k file into existing model.
-        """
-        args = locals()
-        [ImportLSDynaKeywordFileParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of ImportLSDynaKeywordFileParams.
-
-        Examples
-        --------
-        >>> ImportLSDynaKeywordFileParams.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ImportLSDynaKeywordFileParams._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._drop_mid_nodes is not None:
-            json_data["dropMidNodes"] = self._drop_mid_nodes
-        if self._append is not None:
-            json_data["append"] = self._append
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "drop_mid_nodes :  %s\nappend :  %s" % (self._drop_mid_nodes, self._append)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def drop_mid_nodes(self) -> bool:
-        """Option to import quadratic mesh elements as linear skipping the mid nodes.
-        """
-        return self._drop_mid_nodes
-
-    @drop_mid_nodes.setter
-    def drop_mid_nodes(self, value: bool):
-        self._drop_mid_nodes = value
-
-    @property
-    def append(self) -> bool:
-        """Option to append imported k file into existing model.
-        """
-        return self._append
-
-    @append.setter
-    def append(self, value: bool):
-        self._append = value
-
-class ExportLSDynaKeywordFileParams(CoreObject):
-    """Parameters to control LS-DYNA keyword file export settings.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            part_ids: Iterable[int]):
-        self._part_ids = part_ids if isinstance(part_ids, np.ndarray) else np.array(part_ids, dtype=np.int32) if part_ids is not None else None
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            part_ids: Iterable[int] = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the ExportLSDynaKeywordFileParams.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a ExportLSDynaKeywordFileParams object with default parameters.
-        part_ids: Iterable[int], optional
-            Option to export only specified parts.
-        json_data: dict, optional
-            JSON dictionary to create a ExportLSDynaKeywordFileParams object with provided parameters.
-
-        Examples
-        --------
-        >>> export_lsdyna_keyword_file_params = prime.ExportLSDynaKeywordFileParams(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["partIds"] if "partIds" in json_data else None)
-        else:
-            all_field_specified = all(arg is not None for arg in [part_ids])
-            if all_field_specified:
-                self.__initialize(
-                    part_ids)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "ExportLSDynaKeywordFileParams")
-                    json_data = param_json["ExportLSDynaKeywordFileParams"] if "ExportLSDynaKeywordFileParams" in param_json else {}
-                    self.__initialize(
-                        part_ids if part_ids is not None else ( ExportLSDynaKeywordFileParams._default_params["part_ids"] if "part_ids" in ExportLSDynaKeywordFileParams._default_params else (json_data["partIds"] if "partIds" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            part_ids: Iterable[int] = None):
-        """Set the default values of ExportLSDynaKeywordFileParams.
-
-        Parameters
-        ----------
-        part_ids: Iterable[int], optional
-            Option to export only specified parts.
-        """
-        args = locals()
-        [ExportLSDynaKeywordFileParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of ExportLSDynaKeywordFileParams.
-
-        Examples
-        --------
-        >>> ExportLSDynaKeywordFileParams.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExportLSDynaKeywordFileParams._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._part_ids is not None:
-            json_data["partIds"] = self._part_ids
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "part_ids :  %s" % (self._part_ids)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def part_ids(self) -> Iterable[int]:
-        """Option to export only specified parts.
-        """
-        return self._part_ids
-
-    @part_ids.setter
-    def part_ids(self, value: Iterable[int]):
-        self._part_ids = value
-
-class ExportLSDynaIgaKeywordFileParams(CoreObject):
-    """Parameters for exporting LS-Dyna IGA keyword file.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            part_ids: Iterable[int]):
-        self._part_ids = part_ids if isinstance(part_ids, np.ndarray) else np.array(part_ids, dtype=np.int32) if part_ids is not None else None
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            part_ids: Iterable[int] = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the ExportLSDynaIgaKeywordFileParams.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a ExportLSDynaIgaKeywordFileParams object with default parameters.
-        part_ids: Iterable[int], optional
-        json_data: dict, optional
-            JSON dictionary to create a ExportLSDynaIgaKeywordFileParams object with provided parameters.
-
-        Examples
-        --------
-        >>> export_lsdyna_iga_keyword_file_params = prime.ExportLSDynaIgaKeywordFileParams(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["partIds"] if "partIds" in json_data else None)
-        else:
-            all_field_specified = all(arg is not None for arg in [part_ids])
-            if all_field_specified:
-                self.__initialize(
-                    part_ids)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "ExportLSDynaIgaKeywordFileParams")
-                    json_data = param_json["ExportLSDynaIgaKeywordFileParams"] if "ExportLSDynaIgaKeywordFileParams" in param_json else {}
-                    self.__initialize(
-                        part_ids if part_ids is not None else ( ExportLSDynaIgaKeywordFileParams._default_params["part_ids"] if "part_ids" in ExportLSDynaIgaKeywordFileParams._default_params else (json_data["partIds"] if "partIds" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            part_ids: Iterable[int] = None):
-        """Set the default values of ExportLSDynaIgaKeywordFileParams.
-
-        Parameters
-        ----------
-        part_ids: Iterable[int], optional
-        """
-        args = locals()
-        [ExportLSDynaIgaKeywordFileParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of ExportLSDynaIgaKeywordFileParams.
-
-        Examples
-        --------
-        >>> ExportLSDynaIgaKeywordFileParams.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExportLSDynaIgaKeywordFileParams._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._part_ids is not None:
-            json_data["partIds"] = self._part_ids
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "part_ids :  %s" % (self._part_ids)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def part_ids(self) -> Iterable[int]:
-        """
-        Option to export only specified parts.
-        """
-        return self._part_ids
-
-    @part_ids.setter
-    def part_ids(self, value: Iterable[int]):
-        self._part_ids = value
-
 class ExportBoundaryFittedSplineParams(CoreObject):
     """Parameters for exporting boundary fitted splines.
     """
     _default_params = {}
 
     def __initialize(
             self,
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/igastructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/igastructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanager.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanager.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfo.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfo.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfostructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfostructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/model.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/model.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/modelstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/modelstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpher.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpher.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpherbcsstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherbcsstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpherstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherstructs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,71 +26,59 @@
 
 class MorphSolveParams(CoreObject):
     """Morpher solve parameters.
     """
     _default_params = {}
 
     def __initialize(
-            self,
-            abs_purge_tol: float):
-        self._abs_purge_tol = abs_purge_tol
+            self):
+        pass
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            abs_purge_tol: float = None,
             json_data : dict = None,
              **kwargs):
         """Initializes the MorphSolveParams.
 
         Parameters
         ----------
         model: Model
             Model to create a MorphSolveParams object with default parameters.
-        abs_purge_tol: float, optional
-            Absolute purge tolerance.
         json_data: dict, optional
             JSON dictionary to create a MorphSolveParams object with provided parameters.
 
         Examples
         --------
         >>> morph_solve_params = prime.MorphSolveParams(model = model)
         """
         if json_data:
-            self.__initialize(
-                json_data["absPurgeTol"] if "absPurgeTol" in json_data else None)
+            self.__initialize()
         else:
-            all_field_specified = all(arg is not None for arg in [abs_purge_tol])
+            all_field_specified = all(arg is not None for arg in [])
             if all_field_specified:
-                self.__initialize(
-                    abs_purge_tol)
+                self.__initialize()
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "MorphSolveParams")
                     json_data = param_json["MorphSolveParams"] if "MorphSolveParams" in param_json else {}
-                    self.__initialize(
-                        abs_purge_tol if abs_purge_tol is not None else ( MorphSolveParams._default_params["abs_purge_tol"] if "abs_purge_tol" in MorphSolveParams._default_params else (json_data["absPurgeTol"] if "absPurgeTol" in json_data else None)))
+                    self.__initialize()
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
-    def set_default(
-            abs_purge_tol: float = None):
+    def set_default():
         """Set the default values of MorphSolveParams.
 
-        Parameters
-        ----------
-        abs_purge_tol: float, optional
-            Absolute purge tolerance.
         """
         args = locals()
         [MorphSolveParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
         """Print the default values of MorphSolveParams.
@@ -101,34 +89,22 @@
         """
         message = ""
         message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in MorphSolveParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._abs_purge_tol is not None:
-            json_data["absPurgeTol"] = self._abs_purge_tol
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "abs_purge_tol :  %s" % (self._abs_purge_tol)
+        message = "" % ()
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
-    @property
-    def abs_purge_tol(self) -> float:
-        """Absolute purge tolerance.
-        """
-        return self._abs_purge_tol
-
-    @abs_purge_tol.setter
-    def abs_purge_tol(self, value: float):
-        self._abs_purge_tol = value
-
 class MatchMorphParams(CoreObject):
     """MatchMorphParams describes the parameters required for match morphing.
     """
     _default_params = {}
 
     def __initialize(
             self):
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/part.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/part.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/partstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/partstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/primeconfig.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/primeconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     SCAFFOLDERBADINPUTPARAMS = 52
     """Incorrect input parameters."""
     SCAFFOLDERINVALIDABSOLUTEDISTOL = 53
     """Invalid absolute distance tolerance for scaffold operation."""
     SCAFFOLDERINVALIDCONSTANTMESHSIZE = 54
     """Invalid constant mesh size input for scaffold operation."""
     AUTOMESHFAILED = 100
-    """Auto mesh failed."""
+    """Auto meshing failed."""
     AITOVERLAPALONGMULTIFOUND = 101
     """Topology identification failed because of overlapping faces."""
     TRIANGULATIONFAILED = 102
     """Triangulation failed."""
     DUPLICATENODESFOUND = 103
     """Duplicate nodes found."""
     EDGEINTERSECTINGFACEFOUND = 104
@@ -94,14 +94,22 @@
     """No active size fields found."""
     AUTOMESHINVALIDMAXSIZE = 116
     """Invalid max size for auto volume meshing."""
     AUTOMESHHEXCOREFAILED = 117
     """Hex generation part of volume meshing failed."""
     INVALIDVOLUMECONTROLS = 118
     """Invalid volume controls specified for volume meshing."""
+    SOURCEFACINGCELLZONELETS = 119
+    """Source face zonelets facing existing volume mesh."""
+    TARGETWITHCELLZONELETS = 120
+    """Target face zonelets with volume mesh on both side."""
+    SIDEZONELETSNOTFIT = 121
+    """Side face zonelets are not sweepable for thin volume mesh."""
+    SOURCETARGETZONELETSNOTFIT = 122
+    """Source and target zonelets do not fit to thin volume mesh."""
     INVALIDPRISMCONTROLS_INCORRECTSCOPEENTITY = 123
     """Invalid scope entity."""
     INVALIDFIRSTASPECTRATIO = 124
     """Invalid first aspect ratio."""
     INVALIDLASTASPECTRATIO = 125
     """Invalid last aspect ratio."""
     INVALIDFIRSTHEIGHT = 126
@@ -122,14 +130,26 @@
     """Merge volumes failed."""
     DELETEVOLUMESFAILED = 134
     """Delete volumes failed."""
     PERIODICSURFACESNOTSUPPORTEDFORPRISMS = 135
     """Periodic surfaces selected for prism generation are not supported."""
     INVALIDNEIGHBORVOLUMES = 136
     """Invalid neighbor volumes selected to merge volumes."""
+    THINVOLUMEMESHFAILED = 137
+    """Thin volume meshing failed."""
+    PRISMMESHFAILED = 138
+    """Prism meshing failed."""
+    AUTOMESHINITFAILED = 139
+    """Auto mesh initialization failed."""
+    POLYMESHFAILED = 140
+    """Poly meshing failed."""
+    PYRAMIDMESHFAILED = 141
+    """Pyramid meshing failed."""
+    DELETEMESHFAILED = 142
+    """Deleting mesh failed."""
     OUTOFMEMORY = 200
     """Out of memory."""
     INTERRUPTED = 201
     """Method call interrupted."""
     GETSTATISTICSFAILED = 250
     """Failed to get mesh statistics."""
     GETELEMENTCOUNTFAILED = 251
@@ -534,30 +554,34 @@
     """Base face list input is invalid."""
     STACKER_NONSTACKABLEVOLUMESFOUND = 10109
     """Some volumes are not aligned in the stacking direction."""
     STACKER_INCORRECTBODYDEFINITION = 10110
     """Some bodies are intersecting or incorrectly defined."""
     STACKER_BASEFACEUNMESHED = 10111
     """Base face list input has unmeshed topofaces."""
-    INVALIDTHINVOLUMECONTROLS = 12010
-    """Invalid input provided. Invalid thin volume control."""
-    THINVOLUMECONTROLINVALIDSOURCESCOPE = 12020
-    """Invalid input provided. Source scope not found."""
-    THINVOLUMECONTROLINVALIDTARGETSCOPE = 12040
-    """Invalid input provided. Target scope not found."""
-    THINVOLUMECONTROLINVALIDSCOPE = 12060
-    """Invalid input provided. Source scope and target scope cannot be same."""
-    THINVOLUMECONTROLINVALIDSOURCESCOPEENTITY = 12080
-    """Invalid input provided. Invalid source scope entity."""
-    THINVOLUMECONTROLINVALIDTARGETSCOPEENTITY = 12100
-    """Invalid input provided. Invalid target scope entity."""
-    THINVOLUMECONTROLINVALIDNUMBEROFLAYER = 12120
-    """Invalid input provided. Number of layer in thin volume mesh should be greater than 0."""
-    THINVOLUMECONTROLTOPOLOGYNOTSUPPORTED = 12140
+    INVALIDTHINVOLUMECONTROLS = 12101
+    """Invalid input provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDSOURCESCOPE = 12102
+    """Invalid source scope provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDTARGETSCOPE = 12103
+    """Invalid target scope provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDSCOPE = 12104
+    """Same source and target scope provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDSOURCESCOPEENTITY = 12105
+    """Invalid source scope entity provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDTARGETSCOPEENTITY = 12106
+    """Invalid target scope entity provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDNUMBEROFLAYER = 12107
+    """Invalid number of layers provided for thin volume control."""
+    THINVOLUMECONTROLTOPOLOGYNOTSUPPORTED = 12108
     """Thin volume mesh controls not supported for part with topology data."""
+    THINVOLUMECONTROLINVALIDVOLUMESCOPE = 12109
+    """Invalid volume scope provided for thin volume control."""
+    THINVOLUMECONTROLINVALIDCONTROL = 12110
+    """Same face scope is set as target for multiple thin volume controls."""
     MICROSTRUCTUREINVALIDELEMENTTYPE = 13000
     """Invalid input provided. Invalid Element Type."""
 
 class WarningCode(enum.IntEnum):
     """Warning codes associated with the PyPrimeMesh operation.
     """
     NOWARNING = 0
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/quadtospline.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/quadtospline.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolder.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolder.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolderstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolderstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefield.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefield.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefieldstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefieldstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/splittoolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/splittoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearch.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearch.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearchstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilities.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfer.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surferstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surferstructs.py`

 * *Files 6% similar despite different names*

```diff
@@ -525,32 +525,38 @@
 class LocalSurferParams(CoreObject):
     """Parameters to perform local surface remeshing.
     """
     _default_params = {}
 
     def __initialize(
             self,
+            min_angle: float,
+            max_angle: float,
             size_field_type: SizeFieldType,
             min_size: float,
             max_size: float,
             growth_rate: float,
             constant_size: float,
             smooth_boundary: bool,
             n_rings: int):
+        self._min_angle = min_angle
+        self._max_angle = max_angle
         self._size_field_type = SizeFieldType(size_field_type)
         self._min_size = min_size
         self._max_size = max_size
         self._growth_rate = growth_rate
         self._constant_size = constant_size
         self._smooth_boundary = smooth_boundary
         self._n_rings = n_rings
 
     def __init__(
             self,
             model: CommunicationManager=None,
+            min_angle: float = None,
+            max_angle: float = None,
             size_field_type: SizeFieldType = None,
             min_size: float = None,
             max_size: float = None,
             growth_rate: float = None,
             constant_size: float = None,
             smooth_boundary: bool = None,
             n_rings: int = None,
@@ -558,14 +564,18 @@
              **kwargs):
         """Initializes the LocalSurferParams.
 
         Parameters
         ----------
         model: Model
             Model to create a LocalSurferParams object with default parameters.
+        min_angle: float, optional
+            Minimum feature angle limit used to identify and preserve features.
+        max_angle: float, optional
+            Maximum feature angle limit used to identify and preserve features.
         size_field_type: SizeFieldType, optional
             Size field type used to generate surface mesh.
         min_size: float, optional
             Minimum size to be used in sizing for the surfer.
         max_size: float, optional
             Maximum size to be used in sizing for the surfer.
         growth_rate: float, optional
@@ -581,39 +591,45 @@
 
         Examples
         --------
         >>> local_surfer_params = prime.LocalSurferParams(model = model)
         """
         if json_data:
             self.__initialize(
+                json_data["minAngle"] if "minAngle" in json_data else None,
+                json_data["maxAngle"] if "maxAngle" in json_data else None,
                 SizeFieldType(json_data["sizeFieldType"] if "sizeFieldType" in json_data else None),
                 json_data["minSize"] if "minSize" in json_data else None,
                 json_data["maxSize"] if "maxSize" in json_data else None,
                 json_data["growthRate"] if "growthRate" in json_data else None,
                 json_data["constantSize"] if "constantSize" in json_data else None,
                 json_data["smoothBoundary"] if "smoothBoundary" in json_data else None,
                 json_data["nRings"] if "nRings" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [size_field_type, min_size, max_size, growth_rate, constant_size, smooth_boundary, n_rings])
+            all_field_specified = all(arg is not None for arg in [min_angle, max_angle, size_field_type, min_size, max_size, growth_rate, constant_size, smooth_boundary, n_rings])
             if all_field_specified:
                 self.__initialize(
+                    min_angle,
+                    max_angle,
                     size_field_type,
                     min_size,
                     max_size,
                     growth_rate,
                     constant_size,
                     smooth_boundary,
                     n_rings)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "LocalSurferParams")
                     json_data = param_json["LocalSurferParams"] if "LocalSurferParams" in param_json else {}
                     self.__initialize(
+                        min_angle if min_angle is not None else ( LocalSurferParams._default_params["min_angle"] if "min_angle" in LocalSurferParams._default_params else (json_data["minAngle"] if "minAngle" in json_data else None)),
+                        max_angle if max_angle is not None else ( LocalSurferParams._default_params["max_angle"] if "max_angle" in LocalSurferParams._default_params else (json_data["maxAngle"] if "maxAngle" in json_data else None)),
                         size_field_type if size_field_type is not None else ( LocalSurferParams._default_params["size_field_type"] if "size_field_type" in LocalSurferParams._default_params else SizeFieldType(json_data["sizeFieldType"] if "sizeFieldType" in json_data else None)),
                         min_size if min_size is not None else ( LocalSurferParams._default_params["min_size"] if "min_size" in LocalSurferParams._default_params else (json_data["minSize"] if "minSize" in json_data else None)),
                         max_size if max_size is not None else ( LocalSurferParams._default_params["max_size"] if "max_size" in LocalSurferParams._default_params else (json_data["maxSize"] if "maxSize" in json_data else None)),
                         growth_rate if growth_rate is not None else ( LocalSurferParams._default_params["growth_rate"] if "growth_rate" in LocalSurferParams._default_params else (json_data["growthRate"] if "growthRate" in json_data else None)),
                         constant_size if constant_size is not None else ( LocalSurferParams._default_params["constant_size"] if "constant_size" in LocalSurferParams._default_params else (json_data["constantSize"] if "constantSize" in json_data else None)),
                         smooth_boundary if smooth_boundary is not None else ( LocalSurferParams._default_params["smooth_boundary"] if "smooth_boundary" in LocalSurferParams._default_params else (json_data["smoothBoundary"] if "smoothBoundary" in json_data else None)),
                         n_rings if n_rings is not None else ( LocalSurferParams._default_params["n_rings"] if "n_rings" in LocalSurferParams._default_params else (json_data["nRings"] if "nRings" in json_data else None)))
@@ -622,25 +638,31 @@
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
+            min_angle: float = None,
+            max_angle: float = None,
             size_field_type: SizeFieldType = None,
             min_size: float = None,
             max_size: float = None,
             growth_rate: float = None,
             constant_size: float = None,
             smooth_boundary: bool = None,
             n_rings: int = None):
         """Set the default values of LocalSurferParams.
 
         Parameters
         ----------
+        min_angle: float, optional
+            Minimum feature angle limit used to identify and preserve features.
+        max_angle: float, optional
+            Maximum feature angle limit used to identify and preserve features.
         size_field_type: SizeFieldType, optional
             Size field type used to generate surface mesh.
         min_size: float, optional
             Minimum size to be used in sizing for the surfer.
         max_size: float, optional
             Maximum size to be used in sizing for the surfer.
         growth_rate: float, optional
@@ -665,14 +687,18 @@
         """
         message = ""
         message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in LocalSurferParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
+        if self._min_angle is not None:
+            json_data["minAngle"] = self._min_angle
+        if self._max_angle is not None:
+            json_data["maxAngle"] = self._max_angle
         if self._size_field_type is not None:
             json_data["sizeFieldType"] = self._size_field_type
         if self._min_size is not None:
             json_data["minSize"] = self._min_size
         if self._max_size is not None:
             json_data["maxSize"] = self._max_size
         if self._growth_rate is not None:
@@ -683,19 +709,39 @@
             json_data["smoothBoundary"] = self._smooth_boundary
         if self._n_rings is not None:
             json_data["nRings"] = self._n_rings
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "size_field_type :  %s\nmin_size :  %s\nmax_size :  %s\ngrowth_rate :  %s\nconstant_size :  %s\nsmooth_boundary :  %s\nn_rings :  %s" % (self._size_field_type, self._min_size, self._max_size, self._growth_rate, self._constant_size, self._smooth_boundary, self._n_rings)
+        message = "min_angle :  %s\nmax_angle :  %s\nsize_field_type :  %s\nmin_size :  %s\nmax_size :  %s\ngrowth_rate :  %s\nconstant_size :  %s\nsmooth_boundary :  %s\nn_rings :  %s" % (self._min_angle, self._max_angle, self._size_field_type, self._min_size, self._max_size, self._growth_rate, self._constant_size, self._smooth_boundary, self._n_rings)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
+    def min_angle(self) -> float:
+        """Minimum feature angle limit used to identify and preserve features.
+        """
+        return self._min_angle
+
+    @min_angle.setter
+    def min_angle(self, value: float):
+        self._min_angle = value
+
+    @property
+    def max_angle(self) -> float:
+        """Maximum feature angle limit used to identify and preserve features.
+        """
+        return self._max_angle
+
+    @max_angle.setter
+    def max_angle(self, value: float):
+        self._max_angle = value
+
+    @property
     def size_field_type(self) -> SizeFieldType:
         """Size field type used to generate surface mesh.
         """
         return self._size_field_type
 
     @size_field_type.setter
     def size_field_type(self, value: SizeFieldType):
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         args = {"thin_volume_mesh_params" : thin_volume_mesh_params._jsonify()}
         command_name = "PrimeMesh::ThinVolumeControl/SetThinVolumeMeshParams"
         self._model._print_logs_before_command("set_thin_volume_mesh_params", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_thin_volume_mesh_params")
 
     def set_source_scope(self, entities : ScopeDefinition) -> SetScopeResults:
-        """ Sets the source of thin volume control scope.
+        """ Sets the source surface scope of thin volume control.
 
 
         Parameters
         ----------
         entities : ScopeDefinition
             Scope definition entities.
 
@@ -68,15 +68,15 @@
         command_name = "PrimeMesh::ThinVolumeControl/SetSourceScope"
         self._model._print_logs_before_command("set_source_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_source_scope", SetScopeResults(model = self._model, json_data = result))
         return SetScopeResults(model = self._model, json_data = result)
 
     def set_target_scope(self, entities : ScopeDefinition) -> SetScopeResults:
-        """ Sets the target of thin volume control scope.
+        """ Sets the target surface scope of thin volume control.
 
 
         Parameters
         ----------
         entities : ScopeDefinition
             Scope definition entities.
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topodata.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topodata.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilities.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilities.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilitystructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transform.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transform.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transformstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transformstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtool.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtool.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearch.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearch.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearchstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesweeper.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesweeperstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapper.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrappercontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapperstructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/controldata.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/fileio.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/fileio.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import ansys.meshing.prime.internals.utils as utils
 from ansys.meshing.prime.autogen.fileiostructs import (
     ExportBoundaryFittedSplineParams,
     ExportFluentCaseParams,
     ExportFluentMeshingMeshParams,
     ExportMapdlCdbParams,
     ExportMapdlCdbResults,
+    ExportSTLParams,
     FileReadParams,
     FileReadResults,
     FileWriteParams,
     FileWriteResults,
     ImportCadParams,
     ImportCadResults,
     ImportFluentCaseParams,
@@ -42,15 +43,15 @@
     """
 
     __doc__ = _FileIO.__doc__
 
     def __init__(self, model: Model):
         """Initialize model and parent class."""
         self._model = model
-        _FileIO.__init__(self, model)
+        super().__init__(model)
 
     def read_pmdat(self, file_name: str, file_read_params: FileReadParams) -> FileReadResults:
         """Read PyPrimeMesh data file.
 
         PyPrimeMesh data files have pmdat extension.
 
         Parameters
@@ -77,15 +78,15 @@
         >>> model = client.model
         >>> file_io = prime.FileIO(model=model)
         >>> file_read_params = prime.FileReadParams(model=model)
         >>> results = file_io.read_pmdat("/tmp/file.pmdat", file_read_params)
 
         """
         with utils.file_read_context(self._model, file_name) as temp_file_name:
-            result = _FileIO.read_pmdat(self, temp_file_name, file_read_params)
+            result = super().read_pmdat(temp_file_name, file_read_params)
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def write_pmdat(self, file_name: str, file_write_params: FileWriteParams) -> FileWriteResults:
         """Write PyPrimeMesh data file. PyPrimeMesh data files have .pmdat extension.
 
@@ -196,64 +197,85 @@
         >>> params = prime.WriteSizeFieldParams(model=model)
         >>> results = file_io.write_size_field("/tmp/my_prime_sizefield.psf", params)
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().write_size_field(temp_file_name, params)
         return result
 
-    def import_cad(self, file_name: str, params: ImportCadParams) -> ImportCadResults:
-        r"""Open CAD file.
-
-        Import CAD file from disk.
+    def import_mapdl_cdb(
+        self, file_name: str, params: ImportMapdlCdbParams
+    ) -> ImportMapdlCdbResults:
+        """Open MAPDL CDB file(cdb).
 
-        Supported formats on Windows are:
+        Parameters
+        ----------
+        file_name : str
+            Path to file on disk.
+        params : ImportMapdlCdbParams
+            Parameter to import a CDB file.
 
-        \*.scdoc \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
-        \*.dwg \*.dxf \*.model \*.exp \*.CATPart \*.CATProduct \*.cgr \*.3dxml \*.prt\* \*.asm\*
-        \*.iges \*.igs \*.ipt \*.iam \*.jt \*.prt \*.x_t \*.x_b \*.par \*.psm \*.asm \*.sldprt
-        \*.sldasm \*.step \*.stp \*.stl \*.plmxml \*.tgf
+        Returns
+        -------
+        ImportMapdlCdbResults
+            Return ImportMapdlCdbResults.
 
-        Supported formats on Linux are:
+        Notes
+        -----
+        This API does not support Unicode paths now.
 
-        \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
-        \*.CATPart \*.CATProduct \*.iges \*.igs \*.jt \*.x_t \*.x_b \*.step \*.stp
-        \*.stl \*.plmxml \*.tgf
+        Examples
+        --------
+        >>> import ansys.meshing.prime as prime
+        >>> # connect client to server and get model from it
+        >>> client = prime.Client(ip="localhost", port=50060)
+        >>> model = client.model
+        >>> file_io = prime.FileIO(model=model)
+        >>> params = prime.ImportMapdlCdbParams(model=model)
+        >>> results = file_io.import_mapdl_cdb("/tmp/file.cdb", params)
+        """
+        with utils.file_read_context(self._model, file_name) as temp_file_name:
+            result = super().import_mapdl_cdb(temp_file_name, params)
+            if result.error_code == ErrorCode.NOERROR:
+                self._model._sync_up_model()
+        return result
 
-        Refer documentation for detailed list of supported formats.
+    def export_mapdl_cdb(
+        self, file_name: str, params: ExportMapdlCdbParams
+    ) -> ExportMapdlCdbResults:
+        """Export MAPDL CDB file(cdb).
 
         Parameters
         ----------
         file_name : str
-             Path to file on disk.
-
-        params : ImportCadParams
-             Parameters to control CAD import options
+            Path to file on disk.
+        params : ExportMapdlCdbParams
+            Parameter to export a CDB file.
 
         Returns
         -------
-        ImportCadResults
-             Return ImportCadResults.
+        ExportMapdlCdbResults
+            Return ExportMapdlCdbResults.
+
+        Notes
+        -----
+        This API does not support Unicode paths now.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> #connect client to server and get model from it
         >>> client = prime.Client(ip="localhost", port=50060)
         >>> model = client.model
         >>> file_io = prime.FileIO(model=model)
-        >>> params = ImportCadParams(model=model)
-        >>> results = file_io.import_cad(
-                        "/tmp/my_cad.x_t", params=params)
-
+        >>> params = prime.ExportMapdlCdbParams(model=model)
+        >>> results = file_io.export_mapdl_cdb("/tmp/file.cdb", params)
         """
-        with utils.file_read_context(self._model, file_name) as temp_file_name:
-            import_result = _FileIO.import_cad(self, temp_file_name, params)
-            if import_result.error_code == ErrorCode.NOERROR:
-                self._model._sync_up_model()
-        return import_result
+        with utils.file_write_context(self._model, file_name) as temp_file_name:
+            result = super().export_mapdl_cdb(temp_file_name, params)
+        return result
 
     def import_fluent_meshing_meshes(
         self,
         file_names: List[str],
         import_fluent_meshing_mesh_params: ImportFluentMeshingMeshParams,
     ) -> ImportFluentMeshingMeshResults:
         """Import Fluent Meshing meshes of given files on disk.
@@ -283,16 +305,16 @@
         >>> params = prime.ImportFluentMeshingMeshParams(model=model)
         >>> results = file_io.import_fluent_meshing_meshes(
                         ["/tmp/mesh.msh", "/tmp/mesh1.msh"],
                         params)
 
         """
         with utils.file_read_context_list(self._model, file_names) as temp_file_names:
-            result = _FileIO.import_fluent_meshing_meshes(
-                self, temp_file_names, import_fluent_meshing_mesh_params
+            result = super().import_fluent_meshing_meshes(
+                temp_file_names, import_fluent_meshing_mesh_params
             )
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
 
     def import_fluent_case(
         self, file_name: str, import_fluent_case_params: ImportFluentCaseParams
@@ -322,15 +344,15 @@
         --------
         >>> file_io = prime.FileIO(model=model)
         >>> params = prime.ImportFluentCaseParams(model=model)
         >>> results = file_io.import_fluent_case("/tmp/fluent.cas", params)
 
         """
         with utils.file_read_context(self._model, file_name) as temp_file_name:
-            result = _FileIO.import_fluent_case(self, temp_file_name, import_fluent_case_params)
+            result = super().import_fluent_case(temp_file_name, import_fluent_case_params)
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def export_fluent_case(
         self, file_name: str, export_fluent_case_params: ExportFluentCaseParams
     ) -> FileWriteResults:
@@ -355,159 +377,147 @@
                         "/tmp/fluent.cas",
                         prime.ExportFluentCaseParams(model=model))
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().export_fluent_case(temp_file_name, export_fluent_case_params)
         return result
 
-    def import_mapdl_cdb(
-        self, file_name: str, params: ImportMapdlCdbParams
-    ) -> ImportMapdlCdbResults:
-        """Open MAPDL CDB file(cdb).
+    def export_fluent_meshing_mesh(
+        self, file_name: str, export_fluent_mesh_params: ExportFluentMeshingMeshParams
+    ) -> FileWriteResults:
+        """Export Fluent Meshing mesh file. Fluent Meshing mesh files have .msh extension.
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
-        params : ImportMapdlCdbParams
-            Parameter to import a CDB file.
+        export_fluent_mesh_params : ExportFluentMeshingMeshParams
+            Parameters to export Fluent Meshing mesh file.
 
         Returns
         -------
-        ImportMapdlCdbResults
-            Return ImportMapdlCdbResults.
-
-        Notes
-        -----
-        This API does not support Unicode paths now.
+        FileWriteResults
+            Return the FileWriteResults structure.
 
         Examples
         --------
-        >>> import ansys.meshing.prime as prime
-        >>> #connect client to server and get model from it
-        >>> client = prime.Client(ip="localhost", port=50060)
-        >>> model = client.model
-        >>> file_io = prime.FileIO(model=model)
-        >>> params = prime.ImportMapdlCdbParams(model=model)
-        >>> results = file_io.import_mapdl_cdb("/tmp/file.cdb", params)
+        >>> results = file_io.export_fluent_meshing_mesh(
+                        "/tmp/fluent_meshing.msh",
+                        ExportFluentMeshingMeshParams(model=model))
         """
-        with utils.file_read_context(self._model, file_name) as temp_file_name:
-            result = _FileIO.import_mapdl_cdb(self, temp_file_name, params)
-            if result.error_code == ErrorCode.NOERROR:
-                self._model._sync_up_model()
+        with utils.file_write_context(self._model, file_name) as temp_file_name:
+            result = super().export_fluent_meshing_mesh(temp_file_name, export_fluent_mesh_params)
         return result
 
-    def export_mapdl_cdb(
-        self, file_name: str, params: ExportMapdlCdbParams
-    ) -> ExportMapdlCdbResults:
-        """Export MAPDL CDB file(cdb).
+    def export_boundary_fitted_spline_kfile(
+        self, file_name: str, export_params: ExportBoundaryFittedSplineParams
+    ) -> FileWriteResults:
+        """Export IGA LS-DYNA Keyword file for boundary fitted spline.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
-        params : ExportMapdlCdbParams
-            Parameter to export a CDB file.
+            Name of the file.
+        export_params : ExportBoundaryFittedSplineParams
+            Parameters for IGA LS-DYNA Keyword file export.
 
         Returns
         -------
-        ExportMapdlCdbResults
-            Return ExportMapdlCdbResults.
-
-        Notes
-        -----
-        This API does not support Unicode paths now.
+        FileWriteResults
+            Return FileWriteResults.
 
         Examples
         --------
-        >>> import ansys.meshing.prime as prime
-        >>> #connect client to server and get model from it
-        >>> client = prime.Client(ip="localhost", port=50060)
-        >>> model = client.model
-        >>> file_io = prime.FileIO(model=model)
-        >>> params = prime.ExportMapdlCdbParams(model=model)
-        >>> results = file_io.export_mapdl_cdb("/tmp/file.cdb", params)
+        >>> results = file_io.export_boundary_fitted_spline_k_file(
+                        file_name,
+                        ExportBoundaryFittedSplineParams(model=model))
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
-            result = super().export_mapdl_cdb(temp_file_name, params)
+            result = super().export_boundary_fitted_spline_kfile(temp_file_name, export_params)
         return result
 
-    def export_fluent_case(
-        self, file_name: str, export_fluent_case_params: ExportFluentCaseParams
-    ) -> FileWriteResults:
-        """Export Fluent case file. Fluent case files have cas extension.
+    def import_cad(self, file_name: str, params: ImportCadParams) -> ImportCadResults:
+        r"""Open CAD file.
 
-        Parameters
-        ----------
-        file_name : str
-            Path to file on disk.
-        export_fluent_case_params : ExportFluentCaseParams
-            Parameters to export fluent case file.
+        Import CAD file from disk.
 
-        Returns
-        -------
-        FileWriteResults
-            Return the FileWriteResults structure.
+        Supported formats on Windows are:
 
-        Examples
-        --------
-        >>> file_io = FileIO(model=model)
-        >>> results = file_io.export_fluent_case("/tmp/fluent.cas",
-                                                 prime.ExportFluentCaseParams(model=model))
-        """
-        with utils.file_write_context(self._model, file_name) as temp_file_name:
-            result = super().export_fluent_case(temp_file_name, export_fluent_case_params)
-        return result
+        \*.scdoc \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
+        \*.dwg \*.dxf \*.model \*.exp \*.CATPart \*.CATProduct \*.cgr \*.3dxml \*.prt\* \*.asm\*
+        \*.iges \*.igs \*.ipt \*.iam \*.jt \*.prt \*.x_t \*.x_b \*.par \*.psm \*.asm \*.sldprt
+        \*.sldasm \*.step \*.stp \*.stl \*.plmxml \*.tgf
 
-    def export_fluent_meshing_mesh(
-        self, file_name: str, export_fluent_mesh_params: ExportFluentMeshingMeshParams
-    ) -> FileWriteResults:
-        """Export Fluent Meshing mesh file. Fluent Meshing mesh files have .msh extension.
+        Supported formats on Linux are:
+
+        \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
+        \*.CATPart \*.CATProduct \*.iges \*.igs \*.jt \*.x_t \*.x_b \*.step \*.stp
+        \*.stl \*.plmxml \*.tgf
+
+        Refer documentation for detailed list of supported formats.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
-        export_fluent_mesh_params : ExportFluentMeshingMeshParams
-            Parameters to export Fluent Meshing mesh file.
+             Path to file on disk.
+
+        params : ImportCadParams
+             Parameters to control CAD import options
 
         Returns
         -------
-        FileWriteResults
-            Return the FileWriteResults structure.
+        ImportCadResults
+             Return ImportCadResults.
 
         Examples
         --------
-        >>> results = file_io.export_fluent_meshing_mesh(
-                        "/tmp/fluent_meshing.msh",
-                        ExportFluentMeshingMeshParams(model=model))
+        >>> import ansys.meshing.prime as prime
+        >>> # connect client to server and get model from it
+        >>> client = prime.Client(ip="localhost", port=50060)
+        >>> model = client.model
+        >>> file_io = prime.FileIO(model=model)
+        >>> params = ImportCadParams(model=model)
+        >>> results = file_io.import_cad(
+                        "/tmp/my_cad.x_t", params=params)
+
         """
-        with utils.file_write_context(self._model, file_name) as temp_file_name:
-            result = super().export_fluent_meshing_mesh(temp_file_name, export_fluent_mesh_params)
-        return result
+        with utils.file_read_context(self._model, file_name) as temp_file_name:
+            import_result = super().import_cad(temp_file_name, params)
+            if import_result.error_code == ErrorCode.NOERROR:
+                self._model._sync_up_model()
+        return import_result
+
+    def export_stl(self, file_name: str, params: ExportSTLParams) -> FileWriteResults:
+        """Export STL file.
 
-    def export_boundary_fitted_spline_kfile(
-        self, file_name: str, export_params: ExportBoundaryFittedSplineParams
-    ) -> FileWriteResults:
-        """Export IGA LS-DYNA Keyword file for boundary fitted spline.
 
         Parameters
         ----------
         file_name : str
-            Name of the file.
-        export_params : ExportBoundaryFittedSplineParams
-            Parameters for IGA LS-DYNA Keyword file export.
+            Path to file on disk.
+        params : ExportSTLParams
+            Parameters for writing the file.
 
         Returns
         -------
         FileWriteResults
-            Return FileWriteResults.
+            Returns the FileWriteResults.
+
+
+        Notes
+        -----
+        This API does not support Unicode paths now.
 
         Examples
         --------
-        >>> results = file_io.export_boundary_fitted_spline_k_file(
-                        file_name,
-                        ExportBoundaryFittedSplineParams(model=model))
+        >>> import ansys.meshing.prime as prime
+        >>> model = prime.local_model()
+        >>> fileio = prime.FileIO(model=model)
+        >>> out_file_path = r"/tmp/output.stl"
+        >>> part_ids = [part.id for part in model.parts]
+        >>> export_stl_params=prime.ExportSTLParams(model=model,part_ids=part_ids)
+        >>> results = fileio.export_stl(out_file_path,export_stl_params)
+
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
-            result = super().export_boundary_fitted_spline_kfile(temp_file_name, export_params)
+            result = super().export_stl(temp_file_name, params)
         return result
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/model.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,16 @@
         ControlData
             Return the control data.
 
         Examples
         --------
             >>> control_data = model.control_data
         """
+        if self._control_data is None:
+            self._sync_up_model()
         return self._control_data
 
     @property
     def material_point_data(self) -> MaterialPointManager:
         """Get Material Point Data.
 
         MaterialPointManager is used to create, delete and manage material points.
@@ -339,14 +341,16 @@
         MaterialPointManager
             Return the material point manager.
 
         Examples
         --------
             >>> mpt_data = model.material_point_data
         """
+        if self._material_point_data is None:
+            self._sync_up_model()
         return self._material_point_data
 
     @property
     def python_logger(self):
         """Get PyPrimeMesh's Logger instance.
 
         PyPrimeMesh's Logger instance can be used to control the verbosity
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/part.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/part.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/periodiccontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/sizecontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfaceutilities.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfer.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/volumecontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/volumesweeper.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrapper.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrappercontrol.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/examples.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/examples.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,67 @@
 """Examples module for PyPrimeMesh
 """
 import os
 from enum import Enum
 from typing import Optional, Union
 
-from .download_utilities import download_file
+from .download_utilities import DownloadManager
 
-__all__ = ['clear_download_cache', 'get_file', 'Examples']
+__all__ = [
+    'get_file',
+    "download_bracket_dsco",
+    "download_bracket_fmd",
+    "download_bracket_scdoc",
+    "download_deformed_blade_dsco",
+    "download_deformed_blade_fmd",
+    "download_deformed_blade_scdoc",
+    "download_elbow_pmdat",
+    "download_elbow_fmd",
+    "download_elbow_scdoc",
+    "download_elbow_dsco",
+    "download_toy_car_fmd",
+    "download_toy_car_pmdat",
+    "download_toy_car_scdoc",
+    "download_toy_car_dsco",
+    "download_pipe_tee_fmd",
+    "download_pipe_tee_fmd",
+    "download_pipe_tee_dsco",
+    "download_toy_car_scdoc",
+    "download_pcb_pmdat",
+]
 
 
 class Examples(Enum):
     """Contains the available PyPrimeMesh examples to download."""
 
     ELBOW_PMDAT = {"filename": "mixing_elbow.pmdat", "git_folder": "mixing_elbow"}
     ELBOW_FMD = {"filename": "mixing_elbow.fmd", "git_folder": "mixing_elbow"}
     ELBOW_SCDOC = {"filename": "mixing_elbow.scdoc", "git_folder": "mixing_elbow"}
+    ELBOW_DSCO = {"filename": "mixing_elbow.dsco", "git_folder": "mixing_elbow"}
     BRACKET_FMD = {"filename": "bracket_mid_surface.fmd", "git_folder": "bracket_scaffold"}
     BRACKET_SCDOC = {"filename": "bracket_mid_surface.scdoc", "git_folder": "bracket_scaffold"}
+    BRACKET_DSCO = {"filename": "bracket_mid_surface.dsco", "git_folder": "bracket_scaffold"}
     TOY_CAR_PMDAT = {"filename": "toy_car.pmdat", "git_folder": "toy_car"}
     TOY_CAR_FMD = {"filename": "toy_car.fmd", "git_folder": "toy_car"}
     TOY_CAR_SCDOC = {"filename": "toy_car.scdoc", "git_folder": "toy_car"}
+    TOY_CAR_DSCO = {"filename": "toy_car.dsco", "git_folder": "toy_car"}
     PIPE_TEE_PMDAT = {"filename": "pipe_tee.pmdat", "git_folder": "pipe_tee"}
     PIPE_TEE_FMD = {"filename": "pipe_tee.fmd", "git_folder": "pipe_tee"}
     PIPE_TEE_SCDOC = {"filename": "pipe_tee.scdoc", "git_folder": "pipe_tee"}
+    PIPE_TEE_DSCO = {"filename": "pipe_tee.dsco", "git_folder": "pipe_tee"}
+    DEFORMED_BLADE_FMD = {"filename": "blade_deformed.fmd", "git_folder": "turbine_blade"}
+    DEFORMED_BLADE_SCDOC = {"filename": "blade_deformed.scdoc", "git_folder": "turbine_blade"}
+    DEFORMED_BLADE_DSCO = {"filename": "blade_deformed.dsco", "git_folder": "turbine_blade"}
+    TURBINE_BLADE_CDB = {"filename": "blade.cdb", "git_folder": "turbine_blade"}
+    PCB_PMDAT = {"filename": "pcb_stacker.pmdat", "git_folder": "pcb"}
 
 
 _DOWNLOADS = []
 
 
-def clear_download_cache():
-    """Clears the cache of downloaded files"""
-    [os.remove(_file) for _file in _DOWNLOADS]
-    _DOWNLOADS.clear()
-
-
 def get_file(
     example: Examples,
     destination: Optional[str] = None,
     force: bool = False,
 ) -> Union[str, os.PathLike]:
     """Downloads example files from git.
 
@@ -58,24 +82,25 @@
         Local path to the downloaded file
 
     Raises
     ------
     ValueError
         When the provided destination path does not exist on file
     """
+    download_manager = DownloadManager()
     if destination is not None and not os.path.isdir(destination):
         raise ValueError('destination directory provided does not exist')
-    file = download_file(
+    file = download_manager.download_file(
         example.value["filename"],
         'pyprimemesh',
         example.value["git_folder"],
         destination=destination,
         force=force,
     )
-    _DOWNLOADS.append(file)
+
     return file
 
 
 def download_elbow_pmdat(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download PMDAT file for the mixing elbow example
@@ -90,19 +115,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     elbow = prime_examples.download_elbow_pmdat()
@@ -129,19 +149,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     elbow = prime_examples.download_elbow_fmd()
@@ -169,19 +184,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     elbow = prime_examples.download_elbow_scdoc()
@@ -189,14 +199,48 @@
     >>>         _ = io.import_cad(elbow, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
     return get_file(Examples.ELBOW_SCDOC, destination, force)
 
 
+def download_elbow_dsco(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download DSCO file for the mixing elbow example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     elbow = prime_examples.download_elbow_dsco()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(elbow, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.ELBOW_DSCO, destination, force)
+
+
 def download_bracket_fmd(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download FMD file for the bracket scaffold example
 
     Parameters
     ----------
@@ -208,19 +252,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     bracket = prime_examples.download_bracket_fmd()
@@ -247,19 +286,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     bracket = prime_examples.download_bracket_scdoc()
@@ -267,14 +301,48 @@
     >>>         _ = io.import_cad(bracket, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
     return get_file(Examples.BRACKET_SCDOC, destination, force)
 
 
+def download_bracket_dsco(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download DSCO file for the bracket scaffold example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     bracket = prime_examples.download_bracket_dsco()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(bracket, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.BRACKET_DSCO, destination, force)
+
+
 def download_toy_car_pmdat(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download PMDAT file for the toy car example
 
     Parameters
     ----------
@@ -286,19 +354,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     toy_car = prime_examples.download_toy_car_pmdat()
@@ -325,19 +388,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     toy_car = prime_examples.download_toy_car_fmd()
@@ -364,19 +422,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     toy_car = prime_examples.download_toy_car_scdoc()
@@ -384,14 +437,48 @@
     >>>         _ = io.import_cad(toy_car, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
     return get_file(Examples.TOY_CAR_SCDOC, destination, force)
 
 
+def download_toy_car_dsco(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download DSCO file for the toy car example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     toy_car = prime_examples.download_toy_car_dsco()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(toy_car, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.TOY_CAR_DSCO, destination, force)
+
+
 def download_pipe_tee_pmdat(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download PMDAT file for the pipe tee example
 
     Parameters
     ----------
@@ -403,19 +490,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     pipe_tee = prime_examples.download_pipe_tee_pmdat()
@@ -442,19 +524,14 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     pipe_tee = prime_examples.download_pipe_tee_fmd()
@@ -481,25 +558,227 @@
         If false, an existing file in the cache may be re-used.
 
     Returns
     -------
     str
         Local path to the downloaded file
 
-    Raises
-    ------
-    ValueError
-        When the provided destination path does not exist on file
-
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     pipe_tee = prime_examples.download_pipe_tee_scdoc()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(pipe_tee, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
     return get_file(Examples.PIPE_TEE_SCDOC, destination, force)
+
+
+def download_pipe_tee_dsco(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download DSCO file for the pipe tee example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     pipe_tee = prime_examples.download_pipe_tee_dsco()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(pipe_tee, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.PIPE_TEE_DSCO, destination, force)
+
+
+def download_deformed_blade_fmd(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download FMD file for the turbine blade example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     deformed_blade = prime_examples.download_deformed_blade_fmd()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(deformed_blade, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.DEFORMED_BLADE_FMD, destination, force)
+
+
+def download_deformed_blade_scdoc(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download SCDOC file for the turbine blade example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     deformed_blade = prime_examples.download_deformed_blade_scdoc()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(deformed_blade, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.DEFORMED_BLADE_SCDOC, destination, force)
+
+
+def download_deformed_blade_dsco(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download DSCO file for the turbine blade example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     deformed_blade = prime_examples.download_deformed_blade_dsco()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(deformed_blade, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.DEFORMED_BLADE_DSCO, destination, force)
+
+
+def download_turbine_blade_cdb(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download CDB file for the turbine blade example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     turbine_blade_mesh = prime_examples.download_turbine_blade_cdb()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_mapdl_cdb(
+    >>>             turbine_blade_mesh,
+    >>>             params=prime.ImportMapdlCdbParams(model),
+    >>>         )
+    >>>     print(model)
+
+    """
+    return get_file(Examples.TURBINE_BLADE_CDB, destination, force)
+
+
+def download_pcb_pmdat(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download PMDAT file for the pcb example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     pcb = prime_examples.download_pcb_pmdat()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.read_pmdat(pcb, params=prime.FileReadParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.PCB_PMDAT, destination, force)
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/graphics.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import enum
 import os
 
 import numpy as np
 import pyvista as pv
-from pyvista import _vtk
+import vtk
 from pyvista.plotting.plotting import Plotter
 
 import ansys.meshing.prime as prime
+from ansys.meshing.prime.graphics.trame_gui import _HAS_TRAME, TrameVisualizer
 from ansys.meshing.prime.internals import defaults
 
 
 def compute_face_list_from_structured_nodes(nodes, dim):
     flist = []
     for w in range(dim[2]):
         for u in range(dim[0] - 1):
@@ -165,33 +166,41 @@
         [disp_mesh.select() for disp_mesh in self._selected_disp_mesh]
         return
 
 
 class Graphics(object):
     """ """
 
-    def __init__(self, model: prime.Model):
+    def __init__(self, model: prime.Model, use_trame: bool = False):
         """ """
         self._model = model
         self._display_data = {}
         self._display_spline_data = {}
         self._plotter = None
         self._picker = None
         self._color_by_type = ColorByType.ZONE
         self._parts = None
         self._facet_result = prime.FaceAndEdgeConnectivityResults(model=model)
         self._app = None
         self._ruler_visible = False
         self._ruler_actor = None
-        self._colorByTypeBt: _vtk.vtkButtonWidget = None
-        self._hideBt: _vtk.vtkButtonWidget = None
-        self._showEdgeBt: _vtk.vtkButtonWidget = None
-        self._printInfoBt: _vtk.vtkButtonWidget = None
-        self._showRulerBt: _vtk.vtkButtonWidget = None
+        self._colorByTypeBt: vtk.vtkButtonWidget = None
+        self._hideBt: vtk.vtkButtonWidget = None
+        self._showEdgeBt: vtk.vtkButtonWidget = None
+        self._printInfoBt: vtk.vtkButtonWidget = None
+        self._showRulerBt: vtk.vtkButtonWidget = None
         self._sphinx_build = defaults.get_sphinx_build()
+        self._use_trame = use_trame
+
+        if self._use_trame and not _HAS_TRAME:
+            warn_msg = (
+                "'use_trame' is active but Trame dependencies are not installed."
+                "Consider installing 'pyvista[trame]' to use this functionality."
+            )
+            self._model._logger.warning(warn_msg)
         if os.getenv('PRIME_APP_RUN'):
             self._app = __import__('PrimeApp')
         else:
             self.__update_display_data()
 
     def __update_display_data(self):
         """ """
@@ -356,15 +365,15 @@
             self.show(update)
 
     def __color_by_type_callback(self, flag):
         """ """
         vr = self._colorByTypeBt.GetRepresentation()
         state = vr.GetState()
         self._color_by_type = ColorByType(state)
-        r = _vtk.vtkPNGReader()
+        r = vtk.vtkPNGReader()
         color_by_type_icon_file = ""
         if self._color_by_type == ColorByType.ZONELET:
             color_by_type_icon_file = os.path.join(
                 os.path.dirname(__file__), 'images', 'surface_body.png'
             )
         elif self._color_by_type == ColorByType.ZONE:
             color_by_type_icon_file = os.path.join(os.path.dirname(__file__), 'images', 'bin.png')
@@ -439,14 +448,20 @@
         if os.getenv('PRIME_APP_RUN') and self._app is not None:
             app_g = self._app.Graphics().Get()
             app_g.DisplayModel()
             app_g.FitToScreen()
             return
         if update == True:
             self.__update_display_data()
+
+        # if we use trame, activate OFF_SCREEN before initializing plotter
+        pv_off_screen_original = None
+        if self._use_trame:
+            pv_off_screen_original = pv.OFF_SCREEN
+            pv.OFF_SCREEN = True
         self._plotter = pv.Plotter()
         self._plotter.show_axes()
         [
             disp_mesh.add_to_plotter(self._plotter)
             for part_id, data in self._display_data.items()
             for key, disp_mesh_data in data.items()
             for disp_mesh in disp_mesh_data
@@ -472,18 +487,28 @@
                 self.__print_callback, position=(10, 550), size=30, border_size=3
             )
             self._showRulerBt = self._plotter.add_checkbox_button_widget(
                 self.__show_ruler_callback, position=(10, 500), size=30, border_size=3
             )
         self._picker = Picker(self._plotter, self)
         self._plotter.track_click_position(self._picker, side='left')
-        # self._plotter.window_size = [1920, 1017]
         if self._sphinx_build == False:
             self.__update_bt_icons()
-        self._plotter.show()
+        self._show_selector()
+        if self._use_trame:
+            pv.OFF_SCREEN = pv_off_screen_original
+
+    def _show_selector(self):
+        """Chooses between using Trame or Python visualizer."""
+        if self._use_trame:
+            visualizer = TrameVisualizer()
+            visualizer.set_scene(self._plotter)
+            visualizer.show()
+        else:
+            self._plotter.show()
 
     def __draw_parts(self, parts=[], update=False, spline=False):
         """ """
         if os.getenv('PRIME_APP_RUN') and self._app is not None:
             app_g = self._app.Graphics().Get()
             app_g.Clear()
             [app_g.DrawPart(part) for part in parts]
@@ -537,15 +562,15 @@
                 self.__show_ruler_callback, position=(10, 500), size=30, border_size=3
             )
         self._picker = Picker(self._plotter, self)
         self._plotter.track_click_position(self._picker, side='left')
         # self._plotter.window_size = [1920, 1017]
         if self._sphinx_build == False:
             self.__update_bt_icons()
-        self._plotter.show()
+        self._show_selector()
 
     def __draw_scope_parts(self, update=False, scope: prime.ScopeDefinition = None):
         """ """
         self._plotter = pv.Plotter()
         self._plotter.show_axes()
         if os.getenv('PRIME_APP_RUN') and self._app is not None:
             app_g = self._app.Graphics().Get()
@@ -597,56 +622,56 @@
                 self.__show_ruler_callback, position=(10, 500), size=30, border_size=3
             )
         self._picker = Picker(self._plotter, self)
         self._plotter.track_click_position(self._picker, side='left')
         # self._plotter.window_size = [1920, 1017]
         if self._sphinx_build == False:
             self.__update_bt_icons()
-        self._plotter.show()
+        self._show_selector()
 
     def __update_bt_icons(self):
         vr = self._colorByTypeBt.GetRepresentation()
         vr.SetNumberOfStates(3)
-        r = _vtk.vtkPNGReader()
+        r = vtk.vtkPNGReader()
         color_by_zone_icon_file = os.path.join(os.path.dirname(__file__), 'images', 'bin.png')
         r.SetFileName(color_by_zone_icon_file)
         r.Update()
         image_1 = r.GetOutput()
         vr.SetButtonTexture(0, image_1)
         hide_vr = self._hideBt.GetRepresentation()
         hide_unhide_icon_file = os.path.join(
             os.path.dirname(__file__), 'images', 'invert_visibility.png'
         )
-        hide_r = _vtk.vtkPNGReader()
+        hide_r = vtk.vtkPNGReader()
         hide_r.SetFileName(hide_unhide_icon_file)
         hide_r.Update()
         image_2 = hide_r.GetOutput()
         hide_vr.SetButtonTexture(0, image_2)
         hide_vr.SetButtonTexture(1, image_2)
         show_edge_vr = self._showEdgeBt.GetRepresentation()
         show_edges_icon_file = os.path.join(os.path.dirname(__file__), 'images', 'show_edges.png')
-        show_edge_r = _vtk.vtkPNGReader()
+        show_edge_r = vtk.vtkPNGReader()
         show_edge_r.SetFileName(show_edges_icon_file)
         show_edge_r.Update()
         image_3 = show_edge_r.GetOutput()
         show_edge_vr.SetButtonTexture(0, image_3)
         show_edge_vr.SetButtonTexture(1, image_3)
         print_info_vr = self._printInfoBt.GetRepresentation()
         print_info_icon_file = os.path.join(
             os.path.dirname(__file__), 'images', 'selectioninfo.png'
         )
-        print_info_r = _vtk.vtkPNGReader()
+        print_info_r = vtk.vtkPNGReader()
         print_info_r.SetFileName(print_info_icon_file)
         print_info_r.Update()
         image_4 = print_info_r.GetOutput()
         print_info_vr.SetButtonTexture(0, image_4)
         print_info_vr.SetButtonTexture(1, image_4)
         show_ruler_vr = self._showRulerBt.GetRepresentation()
         show_ruler_icon_file = os.path.join(os.path.dirname(__file__), 'images', 'show_ruler.png')
-        show_ruler_r = _vtk.vtkPNGReader()
+        show_ruler_r = vtk.vtkPNGReader()
         show_ruler_r.SetFileName(show_ruler_icon_file)
         show_ruler_r.Update()
         image_5 = show_ruler_r.GetOutput()
         show_ruler_vr.SetButtonTexture(0, image_5)
         show_ruler_vr.SetButtonTexture(1, image_5)
 
     def get_color_by_type(self) -> ColorByType:
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/bin.png` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/bin.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/invert_visibility.png` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/invert_visibility.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/parts.png` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/parts.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/selectioninfo.png` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/selectioninfo.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/show_edges.png` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/show_edges.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/surface_body.png` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/surface_body.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/client.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,14 +117,15 @@
             utils.stop_prime_github_container(container_name)
         elif config.has_pim():
             self.remote_instance.delete()
             self.pim_client.close()
 
         clear_examples = bool(int(os.environ.get('PYPRIMEMESH_CLEAR_EXAMPLES', '1')))
         if clear_examples:
-            examples.clear_download_cache()
+            download_manager = examples.DownloadManager()
+            download_manager.clear_download_cache()
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.exit()
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/config.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/config.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/defaults.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/error_handling.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/error_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,28 @@
     ErrorCode.SCAFFOLDERBADINPUTEMPTYTOPO: "Empty Topology provided to scaffolder.",
     ErrorCode.SCAFFOLDERBADINPUTNOFREEFACES: "No free faces found in current topology.",
     ErrorCode.SCAFFOLDERBADINPUTPARAMS: "Invalid scaffolder parameters setup.",
     ErrorCode.SCAFFOLDERINVALIDABSOLUTEDISTOL: "Absolute distance tolerance must be a positive double and smaller than constant mesh size.",
     ErrorCode.SCAFFOLDERINVALIDCONSTANTMESHSIZE: "Constant mesh must be a positive double.",
     ErrorCode.OUTOFMEMORY: "Out of memory.",
     ErrorCode.INTERRUPTED: "Prime operation interrupted.",
-    ErrorCode.AUTOMESHFAILED: "Auto-Mesh failed.",
+    ErrorCode.AUTOMESHFAILED: "Auto meshing failed.",
+    ErrorCode.THINVOLUMEMESHFAILED: "Thin volume meshing failed.",
+    ErrorCode.PRISMMESHFAILED: "Prism meshing failed.",
+    ErrorCode.AUTOMESHINITFAILED: "Auto mesh initialization failed.",
+    ErrorCode.POLYMESHFAILED: "Poly meshing failed.",
+    ErrorCode.PYRAMIDMESHFAILED: "Pyramid meshing failed.",
+    ErrorCode.DELETEMESHFAILED: "Deleting mesh failed.",
     ErrorCode.INVALIDPRISMCONTROLS: "Conflict of prism settings on zonelets or invalid prism controls selected.",
     ErrorCode.PERIODICSURFACESNOTSUPPORTEDFORPRISMS: "Periodic surfaces selected for prism generation, not supported.",
     ErrorCode.ALREADYVOLUMEMESHED: "Already volume meshed.",
     ErrorCode.VOLUMESNOTUPTODATE: "Volumes are not up to date. Update volumes and try again.",
     ErrorCode.QUADRATICMESHSUPPORTEDONLYFORTETS: "Quadratic meshing is supported only for tetrahedrons.",
     ErrorCode.NOACTIVESFFOUND: "Active size fields are not available.",
-    ErrorCode.AITOVERLAPALONGMULTIFOUND: "Overlapping faces along mulit-connection found.",
+    ErrorCode.AITOVERLAPALONGMULTIFOUND: "Overlapping faces along multi-connection found.",
     ErrorCode.TRIANGULATIONFAILED: "Planar triangulation failed.",
     ErrorCode.TOPOFACESREMESHFAILED: "Failed to remesh some topofaces.",
     ErrorCode.PARTNOTFOUND: "Part not found.",
     ErrorCode.TOPODATANOTFOUND: "Topodata not found.",
     ErrorCode.SIZEFIELDNOTFOUND: "Size Field not found.",
     ErrorCode.CADGEOMETRYNOTFOUND: "CAD Geometry not found.",
     ErrorCode.VOLUMENOTFOUND: "Volume not found.",
@@ -255,25 +261,31 @@
     ErrorCode.SPLITINTERSECTINGBOUNDARYEDGESFAILED: "Splitting of intersecting boundary edges failed.",
     ErrorCode.MATCHINTERIORFAILED: "Matching of interior region of overlap failed.",
     ErrorCode.TOLERANCEVALUEINVALID: "Invalid tolerance value specified.",
     ErrorCode.INVALIDTHINVOLUMECONTROLS: "Invalid thin volume control.",
     ErrorCode.SOURCEORTARGETNOTSPECIFIED: "No target or source faces specified.",
     ErrorCode.THINVOLUMECONTROLINVALIDSOURCESCOPE: "Source scope not found.",
     ErrorCode.THINVOLUMECONTROLINVALIDTARGETSCOPE: "Target scope not found.",
+    ErrorCode.THINVOLUMECONTROLINVALIDVOLUMESCOPE: "Volume scope not found.",
     ErrorCode.THINVOLUMECONTROLINVALIDSCOPE: "Source scope and target scope cannot be same.",
     ErrorCode.THINVOLUMECONTROLINVALIDSOURCESCOPEENTITY: "Invalid source scope entity.",
     ErrorCode.THINVOLUMECONTROLINVALIDTARGETSCOPEENTITY: "Invalid target scope entity.",
     ErrorCode.THINVOLUMECONTROLINVALIDNUMBEROFLAYER: "Number of layer in thin volume mesh should be greater than 0.",
     ErrorCode.THINVOLUMECONTROLTOPOLOGYNOTSUPPORTED: "Thin volume mesh controls not supported for part with topology data.",
+    ErrorCode.THINVOLUMECONTROLINVALIDCONTROL: "Same face scope is set as target for multiple thin volume controls.",
     ErrorCode.EXPORTSTLFAILEDWITHTOPOLOGY: "Export STL not supported for part with topology data.",
     ErrorCode.EXPORTSTLFAILEDWITHQUADFACES: "Export STL not supported for mesh with quad faces.",
     ErrorCode.EXPORTSTLFAILEDWITHPOLYFACES: "Export STL not supported for mesh with poly faces.",
     ErrorCode.EXPORTSTLFAILEDWITHHIGHERORDERMESH: "Export STL not supported for higher order mesh.",
     ErrorCode.EXPORTSTLFAILEDWITHEMPTYPARTIDLIST: "Export STL failed. List of part ids is empty.",
     ErrorCode.EXPORTSTLFAILEDWITHINCORRECTPARTID: "Export STL failed. Part id is incorrect.",
+    ErrorCode.SOURCEFACINGCELLZONELETS: "Source face zonelets facing existing volume mesh.",
+    ErrorCode.TARGETWITHCELLZONELETS: "Target face zonelets with volume mesh on both sides.",
+    ErrorCode.SIDEZONELETSNOTFIT: "Side face zonelets are not sweepable for thin volume mesh.",
+    ErrorCode.SOURCETARGETZONELETSNOTFIT: "Source and target zonelets do not fit to thin volume mesh.",
 }
 
 prime_warning_messages = {
     WarningCode.NOWARNING: "Success.",
     WarningCode.UNKNOWN: "Unknown Warning.",
     WarningCode.SURFER_QUADCLEANUP_MULTITHREADINGNOTSUPPORTED: "Warning: Multithreading is skipped for quad cleanup.",
     WarningCode.SURFERLAYEREDQUADFAILED: "Surface Meshing Warning: Layered quad region has triangles.",
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/grpc_communicator.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/grpc_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/json_utils.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/json_utils.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/launcher.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/prime_communicator.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/prime_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/utils.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     mount_host: str = defaults.get_user_data_path(),
     mount_image: str = defaults.get_user_data_path_for_containers(),
     port: int = defaults.port(),
     name: str = 'ansys-prime-server',
     version: Optional[str] = None,
 ):
     license_file = os.environ.get('ANSYSLMD_LICENSE_FILE', None)
-    image_name = os.environ.get('PYPRIMEMESH_IMAGE_NAME', 'ghcr.io/pyansys/prime')
+    image_name = os.environ.get('PYPRIMEMESH_IMAGE_NAME', 'ghcr.io/ansys/prime')
     if license_file is None:
         raise ValueError('Licensing information to launch container not found')
     if version is None:
         version = os.environ.get('PYPRIMEMESH_IMAGE_TAG', 'latest')
     docker_command = [
         'docker',
         'run',
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/mesh_util.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/mesh_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,15 +744,15 @@
             for volume_zone in volume_zones_all:
                 if check_name_pattern(
                     scope._entity_expression, self._model.get_zone_name(volume_zone)
                 ):
                     volume_zones_to_mesh.append(volume_zone)
 
             volume_zones_to_avoid = [v for v in volume_zones_all if v not in volume_zones_to_mesh]
-            scope_str = ", ".join([self._model.get_zone_name(v) for v in volume_zones_to_avoid])
+            scope_str = ",".join([self._model.get_zone_name(v) for v in volume_zones_to_avoid])
 
             if len(scope_str) > 0:
                 volume_control_param_dead = prime.VolumeControlParams(
                     model=self._model, cell_zonelet_type=prime.CellZoneletType.DEAD
                 )
                 volume_control_scope_dead = prime.ScopeDefinition(
                     model=self._model,
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/scope.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/scope.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/utils.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,32 +38,26 @@
 
     Returns
     -------
     bool
         True if all found.
     """
     patterns = []
-    include_pattern = []
-    exclude_pattern = []
     a = name_patterns.split(",")
     for aa in a:
-        if len(aa) > 0:
-            b = aa.split(" ")
-            for bb in b:
-                if len(bb) > 0:
-                    patterns.append(bb)
-    for pattern in patterns:
-        pattern = pattern.strip()
-        if pattern.startswith("!"):
-            exclude_pattern.append(pattern[1:])
-        else:
-            include_pattern.append(pattern)
-
-    for pattern in exclude_pattern:
-        if match_pattern(pattern, name):
-            return False
+        patterns.append(aa)
 
-    for pattern in include_pattern:
-        if match_pattern(pattern, name):
-            return True
+    for pattern in patterns:
+        bb = pattern.split("!")
+        if match_pattern(bb[0].strip(), name):
+            if len(bb) > 1:
+                nv = False
+                for nvbb in bb[1:]:
+                    if match_pattern(nvbb.strip(), name):
+                        nv = True
+                        break
+                if not nv:
+                    return True
+            else:
+                return True
 
     return False
```

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/params/primestructs.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/params/primestructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/__init__.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/decoder.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/decoder.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/encoder.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/encoder.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/scanner.py` & `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/scanner.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev6/PKG-INFO` & `ansys_meshing_prime-0.4.0.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,115 @@
 Metadata-Version: 2.1
 Name: ansys-meshing-prime
-Version: 0.4.0.dev6
-Summary: PyPrimeMesh provides a python client to Ansys Prime Server. Ansys Prime Server delivers core Ansys meshing technology.
-Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
-Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
-Requires-Python: >=3.7,<4
+Version: 0.4.0.dev8
+Summary: PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology.
+Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
+Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansys-api-meshing-prime==0.1.1
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: pyvista>=0.32.0 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
 Requires-Dist: jupyter-sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.38.5 ; extra == "doc"
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
+Requires-Dist: Sphinx==6.2.0 ; extra == "doc"
+Requires-Dist: pyvista==0.38.6 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: pyvista>=0.32.0 ; extra == "graphics"
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest-pyvista==0.1.8 ; extra == "tests"
+Requires-Dist: pyvista[trame]==0.38.6 ; extra == "tests"
 Project-URL: Documentation, https://prime.docs.pyansys.com
-Project-URL: Source, https://github.com/pyansys/pyprimemesh
+Project-URL: Source, https://github.com/ansys/pyprimemesh
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: graphics
 Provides-Extra: tests
 
 # PyPrimeMesh
 
 [![pyansys](https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC)](https://docs.pyansys.com/)
-[![GH-CI](https://github.com/pyansys/pyprimemesh/actions/workflows/ci_cd.yml/badge.svg)](https://github.com/pyansys/pyprimemesh/actions/workflows/ci_cd.yml)
+[![GH-CI](https://github.com/ansys/pyprimemesh/actions/workflows/ci_cd.yml/badge.svg)](https://github.com/ansys/pyprimemesh/actions/workflows/ci_cd.yml)
 [![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
 
 ## Overview
 
-PyPrimeMesh provides a python client to Ansys Prime Server. Ansys Prime Server delivers core Ansys meshing technology.
+PyPrimeMesh is a Python client to Ansys Prime Server, which
+delivers core Ansys meshing technology.
 
 ## Documentation and Issues
 
 For information on PyPrimeMesh, refer to the latest [documentation](
 https://prime.docs.pyansys.com).
 
-For queries related to PyPrimeMesh, post on the [discussion](
-https://github.com/pyansys/pyprimemesh/discussions) page. 
+For queries related to PyPrimeMesh, post on the [PyPrimeMesh Discussions](
+https://github.com/ansys/pyprimemesh/discussions) page. 
 
-For bugs or enhancement requests, file an issue on our [issues](
-https://github.com/pyansys/pyprimemesh/issues) page. 
+For bugs or enhancement requests, post an issue on the [PyPrimeMesh Issues](
+https://github.com/ansys/pyprimemesh/issues) page. 
 
-For assistance, reach out to the PyAnsys
-Support team at [pyansys.support@ansys.com](mailto:pyansys.support@ansys.com).
+For assistance, reach out to the support team at
+[pyansys.core@ansys.com](mailto:pyansys.core@ansys.com).
 
 ## Installation
 
-The `ansys-meshing-prime` package supports Python 3.7 to Python 3.11 on Windows and Linux
-operating system.
+The `ansys-meshing-prime` package supports Python 3.8 to Python 3.11 on the Windows and Linux
+operating systems.
 
-PyPrimeMesh can be installed with all dependencies directly from PyPi as follows:
+
+PyPrimeMesh can be installed with all dependencies directly from PyPi by running
+this command:
 
 ```bash
 pip install ansys-meshing-prime[all]
 ```
 
 Alternatively, you can clone this repository and install the client using
+these commands:
 
 ```bash
-git clone https://github.com/pyansys/pyprimemesh
+git clone https://github.com/ansys/pyprimemesh
 cd pyprimemesh
 pip install -e .[all]
 ```
 
-The above command will install all functionality that is important to development.
-To install a basic version of the client, use the following command instead.
+The preceding commands install all functionality that is important to development.
+To install a basic version of the client, use this command instead:
 
 ```bash
 pip install -e .
 ```
 
 ## Dependencies
 
-You must have Ansys 2023 R1 or newer versions installed for Ansys Prime Server (optionally, CAD readers can be configured).  Ansys Prime Server requires a Preppost or CFD Preppost license to run.
+You must have Ansys 2023 R1 or later installed for access to Ansys Prime Server.
+Optionally, CAD readers can be configured. Ansys Prime Server requires
+an Ansys Mechanical PrepPost or Fluids PrepPost (CFD) license to run.
 
 ## Get Started
 
 ### Launching PyPrimeMesh
 
-To launch PyPrimeMesh:
+To launch PyPrimeMesh, use this code:
 
 ```python
 import ansys.meshing.prime as prime
 
 with prime.launch_prime() as prime_client:
     model = prime_client.model
 ```
@@ -110,9 +117,9 @@
 ## License and Acknowledgments
 
 PyPrimeMesh is licensed under the MIT license.
 
 PyPrimeMesh makes no commercial claim over Ansys whatsoever. This library extends the functionality of
 Ansys Prime Server by adding a Python interface without changing the core behavior or license
 of the original software. The use of Ansys Prime Server requires a legally licensed copy of Ansys
-Workbench.
+2023 or later.
```

