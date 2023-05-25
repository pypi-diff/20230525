# Comparing `tmp/Python-EasyGraph-0.2a8.tar.gz` & `tmp/Python-EasyGraph-0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Python-EasyGraph-0.2a8.tar", last modified: Thu Oct 15 09:38:14 2020, max compression
+gzip compressed data, was "dist/Python-EasyGraph-0.2a9.tar", last modified: Thu Oct 15 10:19:55 2020, max compression
```

## Comparing `Python-EasyGraph-0.2a8.tar` & `Python-EasyGraph-0.2a9.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/
--rw-r--r--   0 sds        (501) staff       (20)     3500 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/PKG-INFO
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/easygraph/
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/easygraph/classes/
--rw-r--r--   0 sds        (501) staff       (20)    23398 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/classes/directed_graph.py
--rw-r--r--   0 sds        (501) staff       (20)    19920 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/classes/graph.py
--rw-r--r--   0 sds        (501) staff       (20)       60 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/classes/__init__.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/easygraph/datasets/
--rw-r--r--   0 sds        (501) staff       (20)       49 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/datasets/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     6897 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/datasets/get_sample_graph.py
--rw-r--r--   0 sds        (501) staff       (20)      171 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/__init__.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/utils/
--rw-r--r--   0 sds        (501) staff       (20)     1445 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/utils/alias.py
--rw-r--r--   0 sds        (501) staff       (20)      294 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/utils/index_of_node.py
--rw-r--r--   0 sds        (501) staff       (20)      211 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/utils/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)      688 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/utils/convert_to_matrix.py
--rw-r--r--   0 sds        (501) staff       (20)     6040 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/utils/mapped_queue.py
--rw-r--r--   0 sds        (501) staff       (20)      427 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/utils/decorators.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/not_sorted/
--rw-r--r--   0 sds        (501) staff       (20)       48 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/not_sorted/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     1307 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/not_sorted/laplacian.py
--rw-r--r--   0 sds        (501) staff       (20)     1231 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/not_sorted/pagerank.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/drawing/
--rw-r--r--   0 sds        (501) staff       (20)     4806 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/drawing/positioning.py
--rw-r--r--   0 sds        (501) staff       (20)       26 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/drawing/__init__.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/centrality/
--rw-r--r--   0 sds        (501) staff       (20)       26 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/centrality/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     8485 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/centrality/centrality.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/path/
--rw-r--r--   0 sds        (501) staff       (20)       19 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/path/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     4355 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/path/path.py
--rw-r--r--   0 sds        (501) staff       (20)      362 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/__init__.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/components/
--rw-r--r--   0 sds        (501) staff       (20)     1055 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/components/ego_betweenness.py
--rw-r--r--   0 sds        (501) staff       (20)     3021 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/components/connected.py
--rw-r--r--   0 sds        (501) staff       (20)       82 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/components/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     7483 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/components/biconnected.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/
--rw-r--r--   0 sds        (501) staff       (20)     7884 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/sdne.py
--rw-r--r--   0 sds        (501) staff       (20)     8262 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/line.py
--rw-r--r--   0 sds        (501) staff       (20)       93 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     8591 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/node2vec.py
--rw-r--r--   0 sds        (501) staff       (20)     2942 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/deepwalk.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/community/
--rw-r--r--   0 sds        (501) staff       (20)     1874 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/community/modularity.py
--rw-r--r--   0 sds        (501) staff       (20)       65 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/community/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)     7449 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/community/modularity_max_detection.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/
--rw-r--r--   0 sds        (501) staff       (20)     4342 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/HIS.py
--rw-r--r--   0 sds        (501) staff       (20)     8069 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/HAM.py
--rw-r--r--   0 sds        (501) staff       (20)     8180 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/evaluation.py
--rw-r--r--   0 sds        (501) staff       (20)      109 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/__init__.py
--rw-r--r--   0 sds        (501) staff       (20)    11387 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/AP_Greedy.py
--rw-r--r--   0 sds        (501) staff       (20)     9701 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/MaxD.py
-drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/
--rw-r--r--   0 sds        (501) staff       (20)     3500 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/PKG-INFO
--rw-r--r--   0 sds        (501) staff       (20)     1794 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/SOURCES.txt
--rw-r--r--   0 sds        (501) staff       (20)       10 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/top_level.txt
--rw-r--r--   0 sds        (501) staff       (20)        1 2020-10-15 09:38:13.000000 Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/dependency_links.txt
--rw-r--r--   0 sds        (501) staff       (20)     1175 2020-10-15 09:37:58.000000 Python-EasyGraph-0.2a8/setup.py
--rw-r--r--   0 sds        (501) staff       (20)       38 2020-10-15 09:38:14.000000 Python-EasyGraph-0.2a8/setup.cfg
--rw-r--r--   0 sds        (501) staff       (20)     2600 2020-10-15 09:29:45.000000 Python-EasyGraph-0.2a8/README.rst
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/
+-rw-r--r--   0 sds        (501) staff       (20)     3500 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/PKG-INFO
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/classes/
+-rw-r--r--   0 sds        (501) staff       (20)    23398 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/classes/directed_graph.py
+-rw-r--r--   0 sds        (501) staff       (20)    19920 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/classes/graph.py
+-rw-r--r--   0 sds        (501) staff       (20)       60 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/classes/__init__.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/datasets/
+-rw-r--r--   0 sds        (501) staff       (20)       49 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/datasets/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     6897 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/datasets/get_sample_graph.py
+-rw-r--r--   0 sds        (501) staff       (20)      171 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/__init__.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/utils/
+-rw-r--r--   0 sds        (501) staff       (20)     1445 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/utils/alias.py
+-rw-r--r--   0 sds        (501) staff       (20)      294 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/utils/index_of_node.py
+-rw-r--r--   0 sds        (501) staff       (20)      211 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/utils/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)      688 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/utils/convert_to_matrix.py
+-rw-r--r--   0 sds        (501) staff       (20)     6040 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/utils/mapped_queue.py
+-rw-r--r--   0 sds        (501) staff       (20)      427 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/utils/decorators.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/not_sorted/
+-rw-r--r--   0 sds        (501) staff       (20)       48 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/not_sorted/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     1307 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/not_sorted/laplacian.py
+-rw-r--r--   0 sds        (501) staff       (20)     1231 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/not_sorted/pagerank.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/drawing/
+-rw-r--r--   0 sds        (501) staff       (20)     4806 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/drawing/positioning.py
+-rw-r--r--   0 sds        (501) staff       (20)       26 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/drawing/__init__.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/centrality/
+-rw-r--r--   0 sds        (501) staff       (20)       26 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/centrality/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     8485 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/centrality/centrality.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/path/
+-rw-r--r--   0 sds        (501) staff       (20)       19 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/path/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     4355 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/path/path.py
+-rw-r--r--   0 sds        (501) staff       (20)      362 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/__init__.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/components/
+-rw-r--r--   0 sds        (501) staff       (20)     1055 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/components/ego_betweenness.py
+-rw-r--r--   0 sds        (501) staff       (20)     3021 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/components/connected.py
+-rw-r--r--   0 sds        (501) staff       (20)       82 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/components/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     7483 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/components/biconnected.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/
+-rw-r--r--   0 sds        (501) staff       (20)     7884 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/sdne.py
+-rw-r--r--   0 sds        (501) staff       (20)     8262 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/line.py
+-rw-r--r--   0 sds        (501) staff       (20)       93 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     8591 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/node2vec.py
+-rw-r--r--   0 sds        (501) staff       (20)     2942 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/deepwalk.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/community/
+-rw-r--r--   0 sds        (501) staff       (20)     1874 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/community/modularity.py
+-rw-r--r--   0 sds        (501) staff       (20)       65 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/community/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)     7449 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/community/modularity_max_detection.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/
+-rw-r--r--   0 sds        (501) staff       (20)     4342 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/HIS.py
+-rw-r--r--   0 sds        (501) staff       (20)     8069 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/HAM.py
+-rw-r--r--   0 sds        (501) staff       (20)     8180 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/evaluation.py
+-rw-r--r--   0 sds        (501) staff       (20)      109 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/__init__.py
+-rw-r--r--   0 sds        (501) staff       (20)    11387 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/AP_Greedy.py
+-rw-r--r--   0 sds        (501) staff       (20)     9701 2020-10-15 09:25:50.000000 Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/MaxD.py
+drwxr-xr-x   0 sds        (501) staff       (20)        0 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/
+-rw-r--r--   0 sds        (501) staff       (20)     3500 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/PKG-INFO
+-rw-r--r--   0 sds        (501) staff       (20)     1833 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 sds        (501) staff       (20)      156 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/requires.txt
+-rw-r--r--   0 sds        (501) staff       (20)       10 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/top_level.txt
+-rw-r--r--   0 sds        (501) staff       (20)        1 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 sds        (501) staff       (20)     1174 2020-10-15 10:19:48.000000 Python-EasyGraph-0.2a9/setup.py
+-rw-r--r--   0 sds        (501) staff       (20)       38 2020-10-15 10:19:55.000000 Python-EasyGraph-0.2a9/setup.cfg
+-rw-r--r--   0 sds        (501) staff       (20)     2600 2020-10-15 10:17:23.000000 Python-EasyGraph-0.2a9/README.rst
```

### Comparing `Python-EasyGraph-0.2a8/PKG-INFO` & `Python-EasyGraph-0.2a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Python-EasyGraph
-Version: 0.2a8
+Version: 0.2a9
 Summary: Easy Graph
 Home-page: https://github.com/easy-graph/Easy-Graph
 Author: Fudan MSN Group
 Author-email: easygraph@163.com
 License: UNKNOWN
-Description: EasyGraph(v0.2a8)
+Description: EasyGraph(v0.2a9)
         ==================
         
         Copyright (C) <2020> by Mobile Systems and Networking Group, Fudan University
         
         .. image:: https://img.shields.io/pypi/v/Python-EasyGraph.svg
           :target: https://pypi.org/project/Python-EasyGraph/
```

### Comparing `Python-EasyGraph-0.2a8/easygraph/classes/directed_graph.py` & `Python-EasyGraph-0.2a9/easygraph/classes/directed_graph.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/classes/graph.py` & `Python-EasyGraph-0.2a9/easygraph/classes/graph.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/datasets/get_sample_graph.py` & `Python-EasyGraph-0.2a9/easygraph/datasets/get_sample_graph.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/utils/alias.py` & `Python-EasyGraph-0.2a9/easygraph/utils/alias.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/utils/convert_to_matrix.py` & `Python-EasyGraph-0.2a9/easygraph/utils/convert_to_matrix.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/utils/mapped_queue.py` & `Python-EasyGraph-0.2a9/easygraph/utils/mapped_queue.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/not_sorted/laplacian.py` & `Python-EasyGraph-0.2a9/easygraph/functions/not_sorted/laplacian.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/not_sorted/pagerank.py` & `Python-EasyGraph-0.2a9/easygraph/functions/not_sorted/pagerank.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/drawing/positioning.py` & `Python-EasyGraph-0.2a9/easygraph/functions/drawing/positioning.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/centrality/centrality.py` & `Python-EasyGraph-0.2a9/easygraph/functions/centrality/centrality.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/path/path.py` & `Python-EasyGraph-0.2a9/easygraph/functions/path/path.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/components/ego_betweenness.py` & `Python-EasyGraph-0.2a9/easygraph/functions/components/ego_betweenness.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/components/connected.py` & `Python-EasyGraph-0.2a9/easygraph/functions/components/connected.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/components/biconnected.py` & `Python-EasyGraph-0.2a9/easygraph/functions/components/biconnected.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/sdne.py` & `Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/sdne.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/line.py` & `Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/line.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/node2vec.py` & `Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/node2vec.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/graph_embedding/deepwalk.py` & `Python-EasyGraph-0.2a9/easygraph/functions/graph_embedding/deepwalk.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/community/modularity.py` & `Python-EasyGraph-0.2a9/easygraph/functions/community/modularity.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/community/modularity_max_detection.py` & `Python-EasyGraph-0.2a9/easygraph/functions/community/modularity_max_detection.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/HIS.py` & `Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/HIS.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/HAM.py` & `Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/HAM.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/evaluation.py` & `Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/evaluation.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/AP_Greedy.py` & `Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/AP_Greedy.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/easygraph/functions/structural_holes/MaxD.py` & `Python-EasyGraph-0.2a9/easygraph/functions/structural_holes/MaxD.py`

 * *Files identical despite different names*

### Comparing `Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/PKG-INFO` & `Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Python-EasyGraph
-Version: 0.2a8
+Version: 0.2a9
 Summary: Easy Graph
 Home-page: https://github.com/easy-graph/Easy-Graph
 Author: Fudan MSN Group
 Author-email: easygraph@163.com
 License: UNKNOWN
-Description: EasyGraph(v0.2a8)
+Description: EasyGraph(v0.2a9)
         ==================
         
         Copyright (C) <2020> by Mobile Systems and Networking Group, Fudan University
         
         .. image:: https://img.shields.io/pypi/v/Python-EasyGraph.svg
           :target: https://pypi.org/project/Python-EasyGraph/
```

### Comparing `Python-EasyGraph-0.2a8/Python_EasyGraph.egg-info/SOURCES.txt` & `Python-EasyGraph-0.2a9/Python_EasyGraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.rst
 setup.py
 Python_EasyGraph.egg-info/PKG-INFO
 Python_EasyGraph.egg-info/SOURCES.txt
 Python_EasyGraph.egg-info/dependency_links.txt
+Python_EasyGraph.egg-info/requires.txt
 Python_EasyGraph.egg-info/top_level.txt
 easygraph/__init__.py
 easygraph/classes/__init__.py
 easygraph/classes/directed_graph.py
 easygraph/classes/graph.py
 easygraph/datasets/__init__.py
 easygraph/datasets/get_sample_graph.py
```

### Comparing `Python-EasyGraph-0.2a8/setup.py` & `Python-EasyGraph-0.2a9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Python-EasyGraph",                                     
-    version="0.2a8",                                        
+    version="0.2a9",                                        
     author="Fudan MSN Group",                                       
     author_email="easygraph@163.com",                      
     description="Easy Graph",                            
     long_description=long_description,                      
     long_description_content_type="text/x-rst",          
     url="https://github.com/easy-graph/Easy-Graph",                              
     packages=setuptools.find_packages(),                    
     classifiers=[                                           
         "Programming Language :: Python :: 3",              
         "License :: OSI Approved :: BSD License",           
         "Operating System :: OS Independent",               
     ],
-    iinstall_requires=parse_requirements("requirements.txt"),
+    install_requires=parse_requirements("requirements.txt"),
 )
```

### Comparing `Python-EasyGraph-0.2a8/README.rst` & `Python-EasyGraph-0.2a9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-EasyGraph(v0.2a8)
+EasyGraph(v0.2a9)
 ==================
 
 Copyright (C) <2020> by Mobile Systems and Networking Group, Fudan University
 
 .. image:: https://img.shields.io/pypi/v/Python-EasyGraph.svg
   :target: https://pypi.org/project/Python-EasyGraph/
```

