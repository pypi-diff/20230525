# Comparing `tmp/Metage2Metabo-1.5.3.tar.gz` & `tmp/Metage2Metabo-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Metage2Metabo-1.5.3.tar", last modified: Mon Sep 26 17:31:02 2022, max compression
+gzip compressed data, was "dist/Metage2Metabo-1.5.4.tar", last modified: Thu May 25 16:00:54 2023, max compression
```

## Comparing `Metage2Metabo-1.5.3.tar` & `Metage2Metabo-1.5.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/Metage2Metabo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18771 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/metage2metabo/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19943 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11875 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/__main_analysis__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/community_addedvalue.py
--rw-r--r--   0 runner    (1001) docker     (121)     4362 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/community_scope.py
--rw-r--r--   0 runner    (1001) docker     (121)     9747 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/individual_scope.py
--rw-r--r--   0 runner    (1001) docker     (121)    11122 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/m2m_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/minimal_community.py
--rw-r--r--   0 runner    (1001) docker     (121)    20215 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m/reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4919 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/enumeration.py
--rw-r--r--   0 runner    (1001) docker     (121)    22242 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/graph_compression.py
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/m2m_analysis_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    10355 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/solution_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6082 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/sbml_management.py
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/metage2metabo/workflow_data/
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/workflow_data/seeds_workflow.sbml
--rwxr-xr-x   0 runner    (1001) docker     (121)  4782536 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/metage2metabo/workflow_data/workflow_genomes.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 17:31:02.000000 Metage2Metabo-1.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_addedvalue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7075 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_cscope.py
--rw-r--r--   0 runner    (1001) docker     (121)    22779 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_iscope.py
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_metacom.py
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_mincom.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2415 2022-09-26 17:30:01.000000 Metage2Metabo-1.5.3/test/test_m2m_recon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/Metage2Metabo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/metage2metabo/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/__main_analysis__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/community_addedvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/community_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/individual_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/m2m_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/minimal_community.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20215 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m/reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/graph_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/m2m_analysis_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/solution_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/sbml_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/metage2metabo/workflow_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/workflow_data/seeds_workflow.sbml
+-rwxr-xr-x   0 runner    (1001) docker     (123)  4782536 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/metage2metabo/workflow_data/workflow_genomes.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:00:54.000000 Metage2Metabo-1.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_addedvalue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7075 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_cscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_iscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_metacom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_mincom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2415 2023-05-25 16:00:05.000000 Metage2Metabo-1.5.4/test/test_m2m_recon.py
```

### Comparing `Metage2Metabo-1.5.3/Metage2Metabo.egg-info/PKG-INFO` & `Metage2Metabo-1.5.4/Metage2Metabo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: Metage2Metabo
-Version: 1.5.3
+Version: 1.5.4
 Summary: Automatic reconstruction of draft metabolic networks with Pathway Tools and graph-based metabolic analysis
 Home-page: https://github.com/aureme/metage2metabo
 Author: AuReMe
 Author-email: gem-aureme@inria.fr
 License: GPLv3+
 Description: metage2metabo is a Python3 workflow to perform graph-based metabolic analysis starting from annotated genomes. It uses Pathway Tools in a automatic and parallel way to reconstruct metabolic networks for a large number of genomes. The obtained metabolic networks are then analyzed individually and collectively in order to get the added value of cooperation in microbiota over individual metabolism, and to identify and screen interesting organisms among all. More information on usage and troubleshooting on Github: https://github.com/aureme/metage2metabo
 Platform: UNKNOWN
```

### Comparing `Metage2Metabo-1.5.3/Metage2Metabo.egg-info/SOURCES.txt` & `Metage2Metabo-1.5.4/Metage2Metabo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/PKG-INFO` & `Metage2Metabo-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: Metage2Metabo
-Version: 1.5.3
+Version: 1.5.4
 Summary: Automatic reconstruction of draft metabolic networks with Pathway Tools and graph-based metabolic analysis
 Home-page: https://github.com/aureme/metage2metabo
 Author: AuReMe
 Author-email: gem-aureme@inria.fr
 License: GPLv3+
 Description: metage2metabo is a Python3 workflow to perform graph-based metabolic analysis starting from annotated genomes. It uses Pathway Tools in a automatic and parallel way to reconstruct metabolic networks for a large number of genomes. The obtained metabolic networks are then analyzed individually and collectively in order to get the added value of cooperation in microbiota over individual metabolism, and to identify and screen interesting organisms among all. More information on usage and troubleshooting on Github: https://github.com/aureme/metage2metabo
 Platform: UNKNOWN
```

### Comparing `Metage2Metabo-1.5.3/README.md` & `Metage2Metabo-1.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/workflows/Python%20package/badge.svg)](https://github.com/AuReMe/metage2metabo/actions) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
 # M2M - metage2metabo
-Metage2metabo is a Python3 (Python >= 3.6, tested with 3.6 and 3.7) tool to perform graph-based metabolic analysis starting from annotated genomes (**reference genomes or metagenome-assembled genomes**). It uses *Pathway Tools* in a automatic and parallel way to **reconstruct metabolic networks** for a large number of genomes. The obtained metabolic networks are then **analyzed individually and collectively** in order to get the **added value of metabolic cooperation in microbiota over individual metabolism** and to **identify and screen interesting organisms** among all. 
+Metage2metabo is a Python3 (Python >= 3.7, tested with 3.7 and 3.8) tool to perform graph-based metabolic analysis starting from annotated genomes (**reference genomes or metagenome-assembled genomes**). It uses *Pathway Tools* in a automatic and parallel way to **reconstruct metabolic networks** for a large number of genomes. The obtained metabolic networks are then **analyzed individually and collectively** in order to get the **added value of metabolic cooperation in microbiota over individual metabolism** and to **identify and screen interesting organisms** among all.
 
 
 m2m can be used as a whole workflow (``` m2m workflow ```, ``` m2m metacom ```) or steps can be performed individually (``` m2m recon ``` , ``` m2m iscope ``` , ``` m2m cscope ```, ``` m2m addedvalue ```, ``` m2m mincom ```, ``` m2m seeds ```).
 
 A dedicated pipeline for the analysis of minimal community solution and their visualisation in power graphs is available with `m2m analysis`. More details in the [documentation](https://metage2metabo.readthedocs.io/en/latest/m2m_analysis.html).
 
 **If you use M2M, please cite:**
@@ -75,15 +75,15 @@
 Also, m2m_analysis relies on other packages:
 * [networkx](https://github.com/networkx/networkx) to create graph from miscoto results
 * [ete3](https://github.com/etetoolkit/ete) to add taxonomy information on the graph if you used mpwt taxon file
 * [powergrasp](https://github.com/Aluriak/PowerGrASP) to compress networkx graph
 
 ## Requirements
 
-* [Pathway Tools](http://bioinformatics.ai.sri.com/ptools/) version 23.0 or higher (free for [academic users](https://biocyc.org/download-bundle.shtml)) is **required for m2m workflow and m2m recon**
+* [Pathway Tools](http://bioinformatics.ai.sri.com/ptools/) version 23.0 or higher (free for [academic users](https://biocyc.org/download-bundle.shtml)) is **required for m2m workflow and m2m recon**.  Metage2Metabo uses mpwt for multiprocessing and mpwt is not usable on Windows. Therefore, the reconstruction step of Metage2Metabo **is not available on Windows**.
     * Pathway Tools requirements
         * **Linux**: Gnome terminal and Libxm4
         ```sh
         apt-get update && apt-get install gnome-terminal libxm4
          ```
         * **All OS**: [NCBI Blast](https://www.ncbi.nlm.nih.gov/books/NBK279671/) and a ncbirc file in user's home directory
             * Install with apt-get
@@ -114,17 +114,17 @@
         echo 'export PATH="$PATH:your/install/directory/pathway-tools:"' >> ~/.bashrc
         ````
 
 * [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
 
 ## Installation
 
-Developed and tested on Linux (Ubuntu, Fedora, Debian) and MacOs (version 10.14) with Python3.6.
+Developed and tested on Linux (Ubuntu, Fedora, Debian) and MacOs (version 10.14) with Python3.7.
 
-Continuous Integration using GitHub Actions with Python3.6 and Python3.7 on ubuntu-latest, macos-latest and windows-latest ([corresponding virtual environment](https://docs.github.com/en/free-pro-team@latest/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources)).
+Continuous Integration using GitHub Actions with Python3.7 and Python3.8 on ubuntu-latest, macos-latest and windows-latest ([corresponding virtual environment](https://docs.github.com/en/free-pro-team@latest/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources)).
 
 ### Installation with pip
 
 ```
 pip install Metage2Metabo
 ```
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/__init__.py` & `Metage2Metabo-1.5.4/metage2metabo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -10,10 +10,10 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
 from metage2metabo import m2m, m2m_analysis
 
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 """ version of the package
 """
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/__main__.py` & `Metage2Metabo-1.5.4/metage2metabo/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/__main_analysis__.py` & `Metage2Metabo-1.5.4/metage2metabo/__main_analysis__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/__init__.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/community_addedvalue.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/community_addedvalue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/community_scope.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/community_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/individual_scope.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/individual_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/m2m_workflow.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/m2m_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/minimal_community.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/minimal_community.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m/reconstruction.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m/reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/__init__.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/enumeration.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/enumeration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/graph_compression.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/graph_compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-import csv
 import logging
 import networkx as nx
 import os
+import re
 import shutil
 import subprocess
 import sys
 import time
 import zipfile
 
 from bubbletools import convert
@@ -148,14 +148,15 @@
         compression(gml_input_path, bbl_output)
         logger.info('######### PowerGraph visualization: ' + target_name + ' #########')
 
         # Read gml file with networkx and extract the essential and alternative symbionts using the note of each node (organism).
         graph = nx.read_gml(gml_input_path)
         essentials = [organism for organism in graph.nodes if graph.nodes[organism]['note'] == 'ES']
         alternatives = [organism for organism in graph.nodes if graph.nodes[organism]['note'] == 'AS']
+
         if taxon_file:
             key_species = essentials + alternatives
             taxon_key_species = set([organism.split('__')[0] for organism in key_species])
             if len(set(all_taxons).intersection(taxon_key_species)) == 0:
                 logger.critical('Difference of taxonomy level between gml file ('+gml_input_path+') compared to '+taxonomy_output_file+'.')
                 sys.exit(1)
 
@@ -209,14 +210,15 @@
         gml_input (str): gml file
         bbl_output (str): bbl output file
     """
     starttime = time.time()
     with open('powergrasp.cfg', 'w') as config_file:
         config_file.write('[powergrasp options]\n')
         config_file.write('SHOW_STORY = no\n')
+        config_file.write('SHOW_DEBUG = no\n')
 
     import powergrasp
     from bubbletools import BubbleTree
 
     with open(bbl_output, 'w') as fd:
         for line in powergrasp.compress_by_cc(gml_input):
             fd.write(line + '\n')
@@ -294,14 +296,33 @@
     if check_oog:
         logger.info('######### Creation of the powergraph svg accessible at ' + svg_output + ' #########')
         oog_cmds = ["java", "-jar", oog_jar, "-inputfiles=" + bbl_input, "-img", "-outputdir=" + svg_output]
         subproc = subprocess.Popen(oog_cmds)
         subproc.wait()
 
 
+def convert_taxon_id(taxon_id):
+    """Some taxon IDs are converted by powergrasp.
+    Especially some strings are replaced by their Unicode ints.
+    This function replaces these codes by the corresponding string.
+
+    Args:
+        taxon_id (str): taxon ID with potential Unicode int.
+
+    Returns:
+        taxon_id (str): converted taxon ID
+    """
+    matches = re.findall('_c\d*_', taxon_id)
+    for match in matches:
+        convert_match = chr(int(match.strip('_c').strip('_')))
+        taxon_id = taxon_id.replace(match, convert_match)
+
+    return taxon_id
+
+
 def update_js(html_output, essentials, alternatives):
     """Update graph.js to add colors for essential and alternative symbionts.
 
     Args:
         html_output (str): path to html folder (containing js subfolder with gaph.js)
         essentials (list): list of essential symbionts
         alternatives (list): list of alternative symbionts
@@ -329,15 +350,22 @@
 
     js_folder = os.path.join(html_output, 'js')
     graph_js = os.path.join(js_folder, 'graph.js')
     new_graph_sj = ''
     with open(graph_js, 'r') as input_js:
         for line in input_js:
             if "data: { 'id'" in line:
-                species_id = line.split("'id':")[1].split(',')[0].split("'")[1]
+                species_id = line.split("'id':")[1].split("'")[1].strip("'| ")
+
+                # Fix issue with converted str into Unicode int.
+                if '_c' in species_id:
+                    unconvert_species_id = species_id
+                    species_id = convert_taxon_id(species_id)
+                    line = line.replace(unconvert_species_id, species_id)
+
                 if species_id in essentials:
                     line = line.replace(" } },", ", 'type': 'essential' } },")
                 if species_id in alternatives:
                     line = line.replace(" } },", ", 'type': 'alternative' } },")
             new_graph_sj += line
             if 'style: [' in line:
                 new_graph_sj += selector_color
@@ -372,16 +400,23 @@
 
     js_folder = os.path.join(html_output, 'js')
     graph_js = os.path.join(js_folder, 'graph.js')
     new_graph_sj = ''
     with open(graph_js, 'r') as input_js:
         for line in input_js:
             if "data: { 'id'" in line:
-                species_names = line.split("'id':")[1].split(',')[0].strip("'| ")
+                species_names = line.split("'id':")[1].split("'")[1].strip("'| ")
+
+                # Fix issue with converted str into Unicode int.
+                if '_c' in species_names:
+                    unconvert_species_names = species_names
+                    species_names = convert_taxon_id(species_names)
+                    line = line.replace(unconvert_species_names, species_names)
                 species_taxon_id = species_names.split('__')[0]
+
                 if species_taxon_id in taxon_colors:
                     if species_names in essentials:
                         line = line.replace(" } },", ", 'type': '"+species_taxon_id+"' } },")
                     if species_names in alternatives:
                         line = line.replace(" } },", ", 'type': '"+species_taxon_id+"' }, css: {'shape': 'rectangle'} },")
 
             new_graph_sj += line
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/m2m_analysis_workflow.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/m2m_analysis_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/solution_graph.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/solution_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/m2m_analysis/taxonomy.py` & `Metage2Metabo-1.5.4/metage2metabo/m2m_analysis/taxonomy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/sbml_management.py` & `Metage2Metabo-1.5.4/metage2metabo/sbml_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/utils.py` & `Metage2Metabo-1.5.4/metage2metabo/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/metage2metabo/workflow_data/seeds_workflow.sbml` & `Metage2Metabo-1.5.4/metage2metabo/workflow_data/seeds_workflow.sbml`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/metage2metabo/workflow_data/workflow_genomes.tar.gz` & `Metage2Metabo-1.5.4/metage2metabo/workflow_data/workflow_genomes.tar.gz`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/setup.py` & `Metage2Metabo-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (C) 2019-2021 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
+# Copyright (C) 2019-2023 Clémence Frioux & Arnaud Belcour - Inria Dyliss - Pleiade
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_addedvalue.py` & `Metage2Metabo-1.5.4/test/test_m2m_addedvalue.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_analysis.py` & `Metage2Metabo-1.5.4/test/test_m2m_analysis.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_cscope.py` & `Metage2Metabo-1.5.4/test/test_m2m_cscope.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_iscope.py` & `Metage2Metabo-1.5.4/test/test_m2m_iscope.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_metacom.py` & `Metage2Metabo-1.5.4/test/test_m2m_metacom.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_mincom.py` & `Metage2Metabo-1.5.4/test/test_m2m_mincom.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.5.3/test/test_m2m_recon.py` & `Metage2Metabo-1.5.4/test/test_m2m_recon.py`

 * *Files identical despite different names*

