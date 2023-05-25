# Comparing `tmp/noise2read-0.1.0.tar.gz` & `tmp/noise2read-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.1.0.tar", last modified: Sun May 21 07:25:03 2023, max compression
+gzip compressed data, was "noise2read-0.1.2.tar", last modified: Wed May 24 05:02:29 2023, max compression
```

## Comparing `noise2read-0.1.0.tar` & `noise2read-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.836815 noise2read-0.1.0/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.1.0/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-21 07:25:03.839256 noise2read-0.1.0/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.1.0/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.1.0/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-21 07:25:03.846093 noise2read-0.1.0/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.583385 noise2read-0.1.0/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.735572 noise2read-0.1.0/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      181 2023-05-21 00:25:03.000000 noise2read-0.1.0/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.1.0/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17309 2023-05-21 04:58:20.000000 noise2read-0.1.0/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    56606 2023-05-21 06:40:27.000000 noise2read-0.1.0/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11566 2023-05-21 07:12:51.000000 noise2read-0.1.0/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.1.0/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.1.0/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26118 2023-05-21 07:18:05.000000 noise2read-0.1.0/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    39127 2023-05-20 01:49:53.000000 noise2read-0.1.0/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    20359 2023-05-21 07:14:27.000000 noise2read-0.1.0/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.799466 noise2read-0.1.0/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.1.0/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.829330 noise2read-0.1.0/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.1.0/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.1.0/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-24 05:02:29.969142 noise2read-0.1.2/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.1.2/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-24 05:02:29.970525 noise2read-0.1.2/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.1.2/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.1.2/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-24 05:02:29.973667 noise2read-0.1.2/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-24 05:02:29.827251 noise2read-0.1.2/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-24 05:02:29.918427 noise2read-0.1.2/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      181 2023-05-24 05:01:33.000000 noise2read-0.1.2/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.1.2/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17762 2023-05-23 11:26:07.000000 noise2read-0.1.2/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.1.2/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.1.2/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    56303 2023-05-24 04:48:03.000000 noise2read-0.1.2/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11566 2023-05-21 07:12:51.000000 noise2read-0.1.2/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.1.2/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.1.2/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.1.2/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26117 2023-05-24 05:01:15.000000 noise2read-0.1.2/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    39224 2023-05-23 08:52:23.000000 noise2read-0.1.2/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    20495 2023-05-23 11:26:58.000000 noise2read-0.1.2/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.1.2/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.1.2/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-24 05:02:29.949641 noise2read-0.1.2/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-24 05:02:29.000000 noise2read-0.1.2/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-24 05:02:29.000000 noise2read-0.1.2/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-24 05:02:29.000000 noise2read-0.1.2/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-24 05:02:29.000000 noise2read-0.1.2/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.1.2/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-24 05:02:29.000000 noise2read-0.1.2/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-24 05:02:29.000000 noise2read-0.1.2/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-24 05:02:29.964521 noise2read-0.1.2/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.1.2/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.1.2/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.1.2/tests/test_utils.py
```

### Comparing `noise2read-0.1.0/LICENSE` & `noise2read-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/PKG-INFO` & `noise2read-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.1.0
+Version: 0.1.2
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.1.0/README.rst` & `noise2read-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/setup.cfg` & `noise2read-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/classifier.py` & `noise2read-0.1.2/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/config.py` & `noise2read-0.1.2/src/noise2read/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-19 10:56:38
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-21 14:58:20
+# @Last Modified time: 2023-05-23 21:26:07
 
 import configparser
 import os
 
 class Config(object):
     def __init__(self, config_file, logger):
         conf = configparser.ConfigParser()
@@ -122,14 +122,19 @@
             else:
                 self.high_ambiguous = True        
             if conf.has_option("AmbiguousSetup", "proba_deviation"):
                 self.proba_deviation = conf.getfloat("AmbiguousSetup", "proba_deviation")
             else:
                 self.proba_deviation = 0.95 # default 
 
+            if conf.has_option("AmbiguousSetup", "iso_neg_high"):
+                self.iso_neg_high = conf.getboolean("AmbiguousSetup", "iso_neg_high")
+            else:
+                self.iso_neg_high = True    
+
             # ModelTuningSetup
             if conf.has_option("ModelTuningSetup", "n_trials"):
                 self.n_trials = conf.getint("ModelTuningSetup", "n_trials")
             else:
                 self.n_trials = 30
                 
             if conf.has_option("ModelTuningSetup", "n_estimators"):
@@ -274,20 +279,20 @@
                 self.indels = conf.getboolean("Simulation", "indels")
             else:
                 self.indels = False
 
             if conf.has_option("Simulation", "error_rate1"):
                 self.error_rate1 = conf.getfloat("Simulation", "error_rate1")
             else:
-                self.error_rate1 = 0.03 # default
+                self.error_rate1 = 0.1 # default
 
             if conf.has_option("Simulation", "error_rate2"):
                 self.error_rate2 = conf.getfloat("Simulation", "error_rate2")
             else:
-                self.error_rate2 = 0.005 # default
+                self.error_rate2 = 0.05 # default
 
             if conf.has_option("Simulation", "sim_seed"):
                 self.sim_seed = conf.getint("Simulation", "sim_seed")
             else:
                 self.sim_seed = 42 # default
                 
             # # Evaluation
@@ -297,14 +302,15 @@
             #     self.delta = 10 # default
 
         if config_file == None:
             # path
             self.result_dir = os.path.join(base_path, 'result/')
             # input
             self.ground_truth_data = None  
+
             # general
             self.num_workers = -1 
             self.chunks_num = 100
             self.min_iters = 1000
             self.verbose = True 
             self.iso_change_detail = False     
             self.top_n = 100      
@@ -326,14 +332,15 @@
             self.read_type = 'DNA'
 
             # AmbiguousSetup
             self.high_ambiguous = True 
             # high ambiguous predict probability difference
             self.proba_deviation = 0.95      # for base editing and lncRNA quant datasets 0.75 others 0.6 
             # self.ambiguous_error_node_degree = 4   # for base editing and lncRNA quant datasets 3 others 4 
+            self.iso_neg_high = True # if True, the high frequency isolated nodes aslso included as negative samples for high ambiguous prediction. This will use quite a lot computational resources (memory) for embeeding and model training
 
             # ModelTuningSetup
             self.n_trials = 30
             self.n_estimators = 400
             self.test_size = 0.1 # default 
             # random state for SMOTE and train_test_split       
             self.random_state = 42 # default  
@@ -369,16 +376,16 @@
             # self.amplicon_error_node_degree = 4
 
             # simulation
             self.min_freq = 4
             self.min_read_count = 30
             self.substations = True
             self.indels = False
-            self.error_rate1 = 0.03
-            self.error_rate2 = 0.005
+            self.error_rate1 = 0.1
+            self.error_rate2 = 0.05
             self.sim_seed = 42
 
             # # Evaluation
             # self.delta = 1
 
             # # coverage
             # self.library_layout = 'PE'
```

### Comparing `noise2read-0.1.0/src/noise2read/coverage.py` & `noise2read-0.1.2/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/data_analysis.py` & `noise2read-0.1.2/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/data_generation.py` & `noise2read-0.1.2/src/noise2read/data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-21 16:40:27
+# @Last Modified time: 2023-05-24 14:48:03
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -764,33 +764,31 @@
         self.logger.info("Constructing 2nt-edit-distance based graph.")
         graph, unique_seqs = self.generate_graph(data_set, edit_dis=2)
         self.graph_summary(graph)
         genuine_df, negative_df, ambiguous_df = self.extract_err_samples(graph, edit_dis=2)
         del graph
         return genuine_df, negative_df, ambiguous_df, unique_seqs
 
-    def extract_amplicon_err_samples(self, data_set, amplicon_low_freq=50, amplicon_high_freq=1500):
+    def extract_amplicon_err_samples(self, data_set):
         """
         extract amplicon sequencing errors from read graph
 
         Args:
             data_set (str): The filename including path for further errors correction for amplicon sequencing data.
-            amplicon_low_freq (int, optional): The threshold of low frquency determining a read for further rectification for amplicon sequencing ddata. Defaults to 50.
-            amplicon_high_freq (int, optional): The threshold of high frquency for amplicon sequencing error correction. Defaults to 1500.
 
         Returns:
             DataFrame: amplicon_df, a dataframe saving the amplicon sequencing errors
             List: unique_seqs, a list saving unique reads of input dataset
         """
         self.logger.debug(data_set)
         self.logger.info("Constructing the second 1nt-edit-distance based graph for further amplicon sequencing data correction.")
         graph, seq_lens_set, seqs2id_dict, unique_seqs = self.generate_graph(data_set, edit_dis=1)
         self.graph_summary(graph)
         
-        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2]
         
         amplicon_df = pd.DataFrame(columns=["idx", "StartRead","StartReadCount", "StartDegree", "ErrorTye", "ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
         for sub_graph in subgraphs:
             edges_lst = [e for e in sub_graph.edges()]
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
@@ -820,21 +818,21 @@
             nx.write_gexf(group_G, file_name)
             gexf_files.append(file_name)
 
         amplicon_lst = []
         idx = 0
         for gexf_file in gexf_files:
             cur_graph = nx.read_gexf(gexf_file)
-            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
+            sub_graphs = [cur_graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
             
             cur_lst, cur_idx = self.extract_amplicon_errs(sub_graphs, idx)
             amplicon_lst.extend(cur_lst)
             idx = cur_idx + 1
             os.remove(gexf_file)
-            del graph, sub_graphs
+            del cur_graph, sub_graphs
 
         for item in amplicon_lst:
             amplicon_df.loc[len(amplicon_df)] = item
         if self.config.verbose:
             amplicon_df.to_csv(self.config.result_dir + "amplicon.csv", index=False)  
         return amplicon_df
         
@@ -844,33 +842,33 @@
             edges_lst = [e for e in sub_graph.edges()]
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
                     node_count = sub_graph.nodes[node]['count']
                     node_degree = sub_graph.degree[node]
                     line = []
-                    if node_count < amplicon_low_freq and not sub_graph.nodes[node]['flag']:# and node_degree <= self.config.amplicon_error_node_degree:
+                    if node_count < self.config.amplicon_low_freq and not sub_graph.nodes[node]['flag']:# and node_degree <= self.config.amplicon_error_node_degree:
                         node_neis = [n for n in sub_graph.neighbors(node)]
                         # nei2count = []
                         nei_degree_count = []
                         for nei in node_neis:
                             nei_count = sub_graph.nodes[nei]['count']
                             nei_degree = sub_graph.degree[nei]
-                            if nei_count > amplicon_high_freq:
+                            if nei_count > self.config.amplicon_high_freq:
                                 line = [nei, nei_count, nei_degree, node, node_count, node_degree]
                                 new_line = self.err_type_classification(line) 
                                 new_line.insert(0, idx) 
                                 # writer.writerow(new_line)
                                 # amplicon_df.loc[len(amplicon_df)] = new_line
                                 amplicon_errs_lst.append(new_line)
                         idx += 1
                         sub_graph.nodes[node]['flag'] = True
                     else:
                         continue     
-        return amplicon_errs_lst
+        return amplicon_errs_lst, idx
   
     def draw_graph(self, graph, sub_dir, drawing_graph_num = 50):
         """
         draw subgraphs from edit-distance-based read graph
 
         Args:
             graph (object): A graph constructed using NetworkX.
```

### Comparing `noise2read-0.1.0/src/noise2read/data_preprocessing.py` & `noise2read-0.1.2/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/encoding.py` & `noise2read-0.1.2/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/error_orrection.py` & `noise2read-0.1.2/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/isolates_correction.py` & `noise2read-0.1.2/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/noise2read.py` & `noise2read-0.1.2/src/noise2read/noise2read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2022-12-29 23:04:12
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-21 17:18:05
+# @Last Modified time: 2023-05-24 15:01:15
 
 from noise2read.config import Config
 import sys, getopt
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 from noise2read.data_analysis import DataAnalysis
 import os
@@ -233,16 +233,16 @@
                     else:
                         corrected_file, new_negative_df = EC.all_in_one_correction(isolates_file, non_isolates_file, unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df =None) 
                     if read_min_len > config.min_read_len:
                         genuine_df2, negative_df2, ambiguous_df2, unique_seqs2 = DG.extract_ed2_errors(corrected_file)
                         mid_result = EC.all_in_one_ed2_correction(corrected_file, unique_seqs2, genuine_df2, negative_df2, ambiguous_df2)
                     else:
                         mid_result = corrected_file
-
-                    amplicon_df = DG.extract_amplicon_err_samples(mid_result, config.amplicon_low_freq, config.amplicon_high_freq)
+                    # mid_result = config.input_file
+                    amplicon_df = DG.extract_amplicon_err_samples(mid_result)
                     config.correct_data = EC.correct_amplicon_err(mid_result, genuine_df, negative_df, new_negative_df, amplicon_df, config.amplicon_threshold_proba)
                 
                     DataAnalysis(logger, config).evaluation()
                     # delete bcool result
                     bcool_dir = os.path.join(config.result_dir, 'bcool/')
                     if os.path.exists(bcool_dir):
                         os.system("rm -rf %s" % bcool_dir)
```

### Comparing `noise2read-0.1.0/src/noise2read/reads2vectors.py` & `noise2read-0.1.2/src/noise2read/reads2vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-20 11:49:53
+# @Last Modified time: 2023-05-23 18:52:23
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
@@ -572,29 +572,30 @@
             cur_kmer2 = row['EndErrKmer']
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
             # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
             negative_feature_lst.append((row['StartRead'], row['EndRead'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
         # isolates negative
-        for idx, row in negative_df.iterrows():
-            read = row['StartRead']
-            pos_reads = enumerate_ed1_seqs(read)
-            for read2 in pos_reads:
-                # negative_feature_lst.append(read) 
-                # negative_feature_lst.append(read2)  
-                cur_err_tye_kmers = error_type_classification(read, read2)
-                cur_err_tye = cur_err_tye_kmers[0]
-                cur_kmer1 = cur_err_tye_kmers[1]
-                cur_kmer2 = cur_err_tye_kmers[2]
-                cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-                cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-                cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-                # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
-                negative_feature_lst.append((read, read2, cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
+        if self.config.iso_neg_high:
+            for idx, row in negative_df.iterrows():
+                read = row['StartRead']
+                pos_reads = enumerate_ed1_seqs(read)
+                for read2 in pos_reads:
+                    # negative_feature_lst.append(read) 
+                    # negative_feature_lst.append(read2)  
+                    cur_err_tye_kmers = error_type_classification(read, read2)
+                    cur_err_tye = cur_err_tye_kmers[0]
+                    cur_kmer1 = cur_err_tye_kmers[1]
+                    cur_kmer2 = cur_err_tye_kmers[2]
+                    cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
+                    cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
+                    cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
+                    # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
+                    negative_feature_lst.append((read, read2, cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
         
         negative_fea = self.read2vec(negative_feature_lst)
         del negative_feature_lst
         ###############################################################
         ambiguous_feature_lst = []
         for idx, row in ambiguous_df.iterrows():
             # ambiguous_feature_lst.append(row['StartRead'])
```

### Comparing `noise2read-0.1.0/src/noise2read/simulation.py` & `noise2read-0.1.2/src/noise2read/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:04:45
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-21 17:14:27
+# @Last Modified time: 2023-05-23 21:26:58
 
 import collections
 from Bio import SeqIO
 # import gzip
 from Bio.SeqRecord import SeqRecord
 from Bio.Seq import Seq
 from tqdm import tqdm
@@ -147,15 +147,19 @@
             correct_data = EC.all_in_one_ed2_correction(corrected_file, unique_seqs2, genuine_df2, negative_df2, ambiguous_df2)
         else:
             correct_data = corrected_file
         return correct_data        
 
     def simulation(self):
         # step 1 correct errors using noise2read
-        corrected_data = self.error_correction(self.config)
+        # 
+        if os.path.exists(self.config.correct_data):
+            corrected_data = self.config.correct_data
+        else:
+            corrected_data = self.error_correction(self.config)
         # inject errors
         raw_data, true_data = self.error_injection(corrected_data)
         # raw_data, true_data = self.error_injection(self.config.input_file)
         DP = DataProcessing( 
             self.logger,
             self.config)
         umi_raw_dataset, umi_true_dataset = DP.write_mimic_umis(raw_data, true_data)
```

### Comparing `noise2read-0.1.0/src/noise2read/umitest.py` & `noise2read-0.1.2/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read/utils.py` & `noise2read-0.1.2/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.1.2/src/noise2read.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.1.0
+Version: 0.1.2
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.1.0/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.1.2/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/tests/test_data_generation.py` & `noise2read-0.1.2/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/tests/test_reads2vector.py` & `noise2read-0.1.2/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.0/tests/test_utils.py` & `noise2read-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

