# Comparing `tmp/RL_OM-0.0.3.tar.gz` & `tmp/RL_OM-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.0.3.tar", last modified: Sun May 21 18:08:11 2023, max compression
+gzip compressed data, was "RL_OM-0.0.4.tar", last modified: Thu May 25 09:41:48 2023, max compression
```

## Comparing `RL_OM-0.0.3.tar` & `RL_OM-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,63 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.786834 RL_OM-0.0.3/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.3/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.3/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-21 18:08:11.786661 RL_OM-0.0.3/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.3/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.781911 RL_OM-0.0.3/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    63135 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.783081 RL_OM-0.0.3/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.783330 RL_OM-0.0.3/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     4481 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.783928 RL_OM-0.0.3/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.784228 RL_OM-0.0.3/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     4476 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.785523 RL_OM-0.0.3/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14217 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.786356 RL_OM-0.0.3/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)    10585 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.782942 RL_OM-0.0.3/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      971 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.3/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-21 18:06:56.000000 RL_OM-0.0.3/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-21 18:08:11.786892 RL_OM-0.0.3/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.3/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.569265 RL_OM-0.0.4/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.4/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.4/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-25 09:41:48.569116 RL_OM-0.0.4/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.4/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.562805 RL_OM-0.0.4/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   129546 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.564144 RL_OM-0.0.4/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.564442 RL_OM-0.0.4/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5191 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.565072 RL_OM-0.0.4/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.565470 RL_OM-0.0.4/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4476 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.566328 RL_OM-0.0.4/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.567216 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.567965 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     4865 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5081 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16296 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4824 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.568641 RL_OM-0.0.4/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10669 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.568900 RL_OM-0.0.4/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4863 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.563981 RL_OM-0.0.4/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.4/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-25 09:39:45.000000 RL_OM-0.0.4/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-25 09:41:48.569308 RL_OM-0.0.4/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.4/setup.py
```

### Comparing `RL_OM-0.0.3/LICENSE` & `RL_OM-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/PKG-INFO` & `RL_OM-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.3/RL_OM/_modidx.py` & `RL_OM-0.0.4/RL_OM/_modidx.py`

 * *Files 27% similar despite different names*

```diff
@@ -47,14 +47,20 @@
                                                                                                              'RL_OM/agents/networks/critics.py'),
                                                'RL_OM.agents.networks.critics.CriticNetworkStateAction': ( 'agents/networks/critics.html#criticnetworkstateaction',
                                                                                                            'RL_OM/agents/networks/critics.py'),
                                                'RL_OM.agents.networks.critics.CriticNetworkStateAction.__init__': ( 'agents/networks/critics.html#criticnetworkstateaction.__init__',
                                                                                                                     'RL_OM/agents/networks/critics.py'),
                                                'RL_OM.agents.networks.critics.CriticNetworkStateAction.forward': ( 'agents/networks/critics.html#criticnetworkstateaction.forward',
                                                                                                                    'RL_OM/agents/networks/critics.py')},
+            'RL_OM.agents.processors.eoq_preprocessors': { 'RL_OM.agents.processors.eoq_preprocessors.GetInventory': ( 'agents/processors/eoq_preprocessors.html#getinventory',
+                                                                                                                       'RL_OM/agents/processors/eoq_preprocessors.py'),
+                                                           'RL_OM.agents.processors.eoq_preprocessors.GetInventory.__call__': ( 'agents/processors/eoq_preprocessors.html#getinventory.__call__',
+                                                                                                                                'RL_OM/agents/processors/eoq_preprocessors.py'),
+                                                           'RL_OM.agents.processors.eoq_preprocessors.GetInventory.__init__': ( 'agents/processors/eoq_preprocessors.html#getinventory.__init__',
+                                                                                                                                'RL_OM/agents/processors/eoq_preprocessors.py')},
             'RL_OM.agents.processors.processors': { 'RL_OM.agents.processors.processors.ClipNegative': ( 'agents/processors/processors.html#clipnegative',
                                                                                                          'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.ClipNegative.__call__': ( 'agents/processors/processors.html#clipnegative.__call__',
                                                                                                                   'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.DiscreteToContinuous': ( 'agents/processors/processors.html#discretetocontinuous',
                                                                                                                  'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.DiscreteToContinuous.__call__': ( 'agents/processors/processors.html#discretetocontinuous.__call__',
@@ -81,14 +87,308 @@
                                                                                                                       'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.RoundAction': ( 'agents/processors/processors.html#roundaction',
                                                                                                         'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.RoundAction.__call__': ( 'agents/processors/processors.html#roundaction.__call__',
                                                                                                                  'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.RoundAction.__init__': ( 'agents/processors/processors.html#roundaction.__init__',
                                                                                                                  'RL_OM/agents/processors/processors.py')},
+            'RL_OM.agents.rl_agents.algorithms.sac_discrete': { 'RL_OM.agents.rl_agents.algorithms.sac_discrete.GumbelSoftmax': ( 'agents/rl_agents/algorithms/sac_discrete.html#gumbelsoftmax',
+                                                                                                                                  'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.GumbelSoftmax.entropy': ( 'agents/rl_agents/algorithms/sac_discrete.html#gumbelsoftmax.entropy',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.GumbelSoftmax.log_prob': ( 'agents/rl_agents/algorithms/sac_discrete.html#gumbelsoftmax.log_prob',
+                                                                                                                                           'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.GumbelSoftmax.rsample': ( 'agents/rl_agents/algorithms/sac_discrete.html#gumbelsoftmax.rsample',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.GumbelSoftmax.sample': ( 'agents/rl_agents/algorithms/sac_discrete.html#gumbelsoftmax.sample',
+                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy',
+                                                                                                                                        'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.__call__': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.__call__',
+                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.__init__': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.__init__',
+                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.compute_action_and_log_prob': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.compute_action_and_log_prob',
+                                                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.compute_action_and_log_prob_t': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.compute_action_and_log_prob_t',
+                                                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.distribution': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.distribution',
+                                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.draw_action': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.draw_action',
+                                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.entropy': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.entropy',
+                                                                                                                                                'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.get_weights': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.get_weights',
+                                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.parameters': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.parameters',
+                                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.reset': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.reset',
+                                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.set_weights': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.set_weights',
+                                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_Discrete_Policy.use_cuda': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete_policy.use_cuda',
+                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete',
+                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete.__init__': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete.__init__',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete._alpha': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete._alpha',
+                                                                                                                                        'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete._alpha_np': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete._alpha_np',
+                                                                                                                                           'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete._loss': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete._loss',
+                                                                                                                                       'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete._next_q': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete._next_q',
+                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete._post_load': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete._post_load',
+                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete._update_alpha': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete._update_alpha',
+                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_discrete.py'),
+                                                                'RL_OM.agents.rl_agents.algorithms.sac_discrete.SAC_discrete.fit': ( 'agents/rl_agents/algorithms/sac_discrete.html#sac_discrete.fit',
+                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_discrete.py')},
+            'RL_OM.agents.rl_agents.algorithms.sac_gumbel': { 'RL_OM.agents.rl_agents.algorithms.sac_gumbel.GumbelSoftmax': ( 'agents/rl_agents/algorithms/sac_gumbel.html#gumbelsoftmax',
+                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.GumbelSoftmax.entropy': ( 'agents/rl_agents/algorithms/sac_gumbel.html#gumbelsoftmax.entropy',
+                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.GumbelSoftmax.log_prob': ( 'agents/rl_agents/algorithms/sac_gumbel.html#gumbelsoftmax.log_prob',
+                                                                                                                                       'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.GumbelSoftmax.rsample': ( 'agents/rl_agents/algorithms/sac_gumbel.html#gumbelsoftmax.rsample',
+                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.GumbelSoftmax.sample': ( 'agents/rl_agents/algorithms/sac_gumbel.html#gumbelsoftmax.sample',
+                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel',
+                                                                                                                           'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel.__init__': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel.__init__',
+                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel._alpha': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel._alpha',
+                                                                                                                                  'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel._alpha_np': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel._alpha_np',
+                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel._loss': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel._loss',
+                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel._next_q': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel._next_q',
+                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel._post_load': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel._post_load',
+                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel._update_alpha': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel._update_alpha',
+                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbel.fit': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbel.fit',
+                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy',
+                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.__call__': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.__call__',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.__init__': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.__init__',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.compute_action_and_log_prob': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.compute_action_and_log_prob',
+                                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.compute_action_and_log_prob_t': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.compute_action_and_log_prob_t',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.distribution': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.distribution',
+                                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.draw_action': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.draw_action',
+                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.entropy': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.entropy',
+                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.get_weights': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.get_weights',
+                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.parameters': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.parameters',
+                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.reset': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.reset',
+                                                                                                                                       'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.set_weights': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.set_weights',
+                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_gumbel.SAC_gumbelPolicy.use_cuda': ( 'agents/rl_agents/algorithms/sac_gumbel.html#sac_gumbelpolicy.use_cuda',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_gumbel.py')},
+            'RL_OM.agents.rl_agents.algorithms.sac_hybrid': { 'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid',
+                                                                                                                           'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid.__init__': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid.__init__',
+                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid._alpha': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid._alpha',
+                                                                                                                                  'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid._alpha_np': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid._alpha_np',
+                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid._loss': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid._loss',
+                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid._next_q': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid._next_q',
+                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid._post_load': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid._post_load',
+                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid._update_alpha': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid._update_alpha',
+                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybrid.fit': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybrid.fit',
+                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy',
+                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.__call__': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.__call__',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.__init__': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.__init__',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.compute_action_and_log_prob': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.compute_action_and_log_prob',
+                                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.compute_action_and_log_prob_t': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.compute_action_and_log_prob_t',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.cont_distribution': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.cont_distribution',
+                                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.discrete_distribution': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.discrete_distribution',
+                                                                                                                                                       'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.draw_action': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.draw_action',
+                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.draw_action_mean_and_logits': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.draw_action_mean_and_logits',
+                                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.draw_noisy_action': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.draw_noisy_action',
+                                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.entropy': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.entropy',
+                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.get_weights': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.get_weights',
+                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.parameters': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.parameters',
+                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.reset': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.reset',
+                                                                                                                                       'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.set_weights': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.set_weights',
+                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py'),
+                                                              'RL_OM.agents.rl_agents.algorithms.sac_hybrid.SAC_hybridPolicy.use_cuda': ( 'agents/rl_agents/algorithms/sac_hybrid.html#sac_hybridpolicy.use_cuda',
+                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_hybrid.py')},
+            'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed': { 'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy',
+                                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.__call__': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.__call__',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.__init__': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.__init__',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.compute_action_and_log_prob': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.compute_action_and_log_prob',
+                                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.compute_action_and_log_prob_t': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.compute_action_and_log_prob_t',
+                                                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.cont_distribution': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.cont_distribution',
+                                                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.discrete_distribution': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.discrete_distribution',
+                                                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.draw_action': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.draw_action',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.draw_action_mean_and_logits': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.draw_action_mean_and_logits',
+                                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.draw_noisy_action': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.draw_noisy_action',
+                                                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.entropy': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.entropy',
+                                                                                                                                                           'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.get_weights': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.get_weights',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.parameters': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.parameters',
+                                                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.reset': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.reset',
+                                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.set_weights': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.set_weights',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybridPolicy.use_cuda': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybridpolicy.use_cuda',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed',
+                                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed.__init__': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed.__init__',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed._alpha': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed._alpha',
+                                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed._alpha_np': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed._alpha_np',
+                                                                                                                                                                'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed._loss': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed._loss',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed._next_q': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed._next_q',
+                                                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed._post_load': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed._post_load',
+                                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed._update_alpha': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed._update_alpha',
+                                                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_reversed.SAC_hybrid_reversed.fit': ( 'agents/rl_agents/algorithms/sac_hybrid_reversed.html#sac_hybrid_reversed.fit',
+                                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py')},
+            'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate': { 'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy',
+                                                                                                                                                   'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.__call__': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.__call__',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.__init__': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.__init__',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.compute_action_and_log_prob': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.compute_action_and_log_prob',
+                                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.compute_action_and_log_prob_t': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.compute_action_and_log_prob_t',
+                                                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.cont_distribution': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.cont_distribution',
+                                                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.discrete_distribution': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.discrete_distribution',
+                                                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.draw_action': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.draw_action',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.draw_action_mean_and_logits': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.draw_action_mean_and_logits',
+                                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.draw_noisy_action': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.draw_noisy_action',
+                                                                                                                                                                     'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.entropy': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.entropy',
+                                                                                                                                                           'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.get_weights': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.get_weights',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.parameters': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.parameters',
+                                                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.reset': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.reset',
+                                                                                                                                                         'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.set_weights': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.set_weights',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybridPolicy.use_cuda': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybridpolicy.use_cuda',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate',
+                                                                                                                                                      'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate.__init__': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate.__init__',
+                                                                                                                                                               'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate._alpha': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate._alpha',
+                                                                                                                                                             'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate._alpha_np': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate._alpha_np',
+                                                                                                                                                                'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate._loss': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate._loss',
+                                                                                                                                                            'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate._next_q': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate._next_q',
+                                                                                                                                                              'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate._post_load': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate._post_load',
+                                                                                                                                                                 'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate._update_alpha': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate._update_alpha',
+                                                                                                                                                                    'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py'),
+                                                                       'RL_OM.agents.rl_agents.algorithms.sac_hybrid_separate.SAC_hybrid_separate.fit': ( 'agents/rl_agents/algorithms/sac_hybrid_separate.html#sac_hybrid_separate.fit',
+                                                                                                                                                          'RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py')},
+            'RL_OM.agents.rl_agents.pre_specified_agents.SAC_discrete': { 'RL_OM.agents.rl_agents.pre_specified_agents.SAC_discrete.SACDiscrete': ( 'agents/rl_agents/pre_specified_agents/sac_discrete.html#sacdiscrete',
+                                                                                                                                                    'RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py'),
+                                                                          'RL_OM.agents.rl_agents.pre_specified_agents.SAC_discrete.SACDiscrete.__getattr__': ( 'agents/rl_agents/pre_specified_agents/sac_discrete.html#sacdiscrete.__getattr__',
+                                                                                                                                                                'RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py'),
+                                                                          'RL_OM.agents.rl_agents.pre_specified_agents.SAC_discrete.SACDiscrete.__init__': ( 'agents/rl_agents/pre_specified_agents/sac_discrete.html#sacdiscrete.__init__',
+                                                                                                                                                             'RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py')},
+            'RL_OM.agents.rl_agents.pre_specified_agents.SAC_gumbel': { 'RL_OM.agents.rl_agents.pre_specified_agents.SAC_gumbel.SACGumbel': ( 'agents/rl_agents/pre_specified_agents/sac_gumbel.html#sacgumbel',
+                                                                                                                                              'RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py'),
+                                                                        'RL_OM.agents.rl_agents.pre_specified_agents.SAC_gumbel.SACGumbel.__getattr__': ( 'agents/rl_agents/pre_specified_agents/sac_gumbel.html#sacgumbel.__getattr__',
+                                                                                                                                                          'RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py'),
+                                                                        'RL_OM.agents.rl_agents.pre_specified_agents.SAC_gumbel.SACGumbel.__init__': ( 'agents/rl_agents/pre_specified_agents/sac_gumbel.html#sacgumbel.__init__',
+                                                                                                                                                       'RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py')},
+            'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel': { 'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbel': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbel',
+                                                                                                                                                                  'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbel.__getattr__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbel.__getattr__',
+                                                                                                                                                                              'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbel.__init__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbel.__init__',
+                                                                                                                                                                           'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbelReversed': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbelreversed',
+                                                                                                                                                                          'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbelReversed.__getattr__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbelreversed.__getattr__',
+                                                                                                                                                                                      'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbelReversed.__init__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbelreversed.__init__',
+                                                                                                                                                                                   'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbelSeparate': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbelseparate',
+                                                                                                                                                                          'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbelSeparate.__getattr__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbelseparate.__getattr__',
+                                                                                                                                                                                      'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py'),
+                                                                               'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_gumbel.SACHybridGumbelSeparate.__init__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_gumbel.html#sachybridgumbelseparate.__init__',
+                                                                                                                                                                                   'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py')},
+            'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_naive': { 'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_naive.SACHybridNaive': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_naive.html#sachybridnaive',
+                                                                                                                                                               'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py'),
+                                                                              'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_naive.SACHybridNaive.__getattr__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_naive.html#sachybridnaive.__getattr__',
+                                                                                                                                                                           'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py'),
+                                                                              'RL_OM.agents.rl_agents.pre_specified_agents.SAC_hybrid_naive.SACHybridNaive.__init__': ( 'agents/rl_agents/pre_specified_agents/sac_hybrid_naive.html#sachybridnaive.__init__',
+                                                                                                                                                                        'RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py')},
             'RL_OM.agents.rl_agents.sac_discrete': { 'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax',
                                                                                                             'RL_OM/agents/rl_agents/sac_discrete.py'),
                                                      'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.entropy': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.entropy',
                                                                                                                     'RL_OM/agents/rl_agents/sac_discrete.py'),
                                                      'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.log_prob': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.log_prob',
                                                                                                                      'RL_OM/agents/rl_agents/sac_discrete.py'),
                                                      'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.rsample': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.rsample',
@@ -344,21 +644,29 @@
                                                             'RL_OM.agents.rl_agents.sac_hybrid_separate.SAC_hybrid_separate.fit': ( 'agents/rl_agents/sac_hybrid_separate.html#sac_hybrid_separate.fit',
                                                                                                                                     'RL_OM/agents/rl_agents/sac_hybrid_separate.py')},
             'RL_OM.core': {'RL_OM.core.foo': ('core.html#foo', 'RL_OM/core.py')},
             'RL_OM.environments.calculation_functions': { 'RL_OM.environments.calculation_functions.eoq_rq_calculations': ( 'environments/calculation_functions.html#eoq_rq_calculations',
                                                                                                                             'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.get_fixed_ordering_cost': ( 'environments/calculation_functions.html#get_fixed_ordering_cost',
                                                                                                                                 'RL_OM/environments/calculation_functions.py')},
+            'RL_OM.environments.data_generators': { 'RL_OM.environments.data_generators.make_binary': ( 'environments/data_generators.html#make_binary',
+                                                                                                        'RL_OM/environments/data_generators.py'),
+                                                    'RL_OM.environments.data_generators.make_regular_binary': ( 'environments/data_generators.html#make_regular_binary',
+                                                                                                                'RL_OM/environments/data_generators.py')},
+            'RL_OM.environments.feature_converters': { 'RL_OM.environments.feature_converters.feature_oracle': ( 'environments/feature_converters.html#feature_oracle',
+                                                                                                                 'RL_OM/environments/feature_converters.py')},
             'RL_OM.environments.multi_period_inventory': { 'RL_OM.environments.multi_period_inventory.MultiPeriodEnv': ( 'environments/multi_period_inventory.html#multiperiodenv',
                                                                                                                          'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.__init__': ( 'environments/multi_period_inventory.html#multiperiodenv.__init__',
                                                                                                                                   'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.render': ( 'environments/multi_period_inventory.html#multiperiodenv.render',
                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.reset': ( 'environments/multi_period_inventory.html#multiperiodenv.reset',
                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_space': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_space',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_state': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_state',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.step': ( 'environments/multi_period_inventory.html#multiperiodenv.step',
-                                                                                                                              'RL_OM/environments/multi_period_inventory.py')}}}
+                                                                                                                              'RL_OM/environments/multi_period_inventory.py')},
+            'RL_OM.experiment_functions.run_experiment': { 'RL_OM.experiment_functions.run_experiment.experiment_stepwise': ( 'experiment_functions/run_experiment.html#experiment_stepwise',
+                                                                                                                              'RL_OM/experiment_functions/run_experiment.py')}}}
```

### Comparing `RL_OM-0.0.3/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.0.4/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,44 +9,56 @@
 
 # Mushroom libraries
 from mushroom_rl.core import Agent
 
 # %% ../../../nbs/agents/benchmark_agents/01_EOQ.ipynb 6
 class EOQAgent(Agent):
 
+    train_directly=True
+
     """
     Agent implementing the Economic Order Quantity (EOQ) policy.
 
     Args:
         mdp_info (MDPInfo): Information about the Markov Decision Process (MDP).
         s (numpy.ndarray): The fixed ordering cost.
         h (numpy.ndarray): The holding cost per unit per period.
+        preprocessors (list): List of preprocessors to be applied to the state.
         postprocessors (list): List of postprocessors to be applied to the policy.
+        agent_name (str): Name of the agent. If set to None will use some default name.
 
     Attributes:
         mdp_info (MDPInfo): Information about the Markov Decision Process (MDP).
         policy (EOQPolicy): The EOQ policy implemented by the agent.
 
     """
 
 
     def __init__(self,
                   mdp_info,
                   s, # fixed ordering cost
                   h, # holding cost per unit per period
-                  postprocessors = None
+                  preprocessors = None,
+                  postprocessors = None,
+                  agent_name = None
         ):
 
         policy = EOQPolicy(
             d = None,
             s = s,
             h = h,
+            preprocessors = preprocessors,
             postprocessors = postprocessors
         )
 
+        if agent_name is None:
+            self.name = 'EOQAgent'
+        else:
+            self.name = agent_name
+
         super().__init__(mdp_info, policy)
 
     def fit(self, demand):
 
         """ 
         Fit the EOQ policy to the given demand.
 
@@ -91,21 +103,26 @@
 
     """
 
     def __init__(self,
                  d, 
                  s, 
                  h, 
+                 preprocessors = None,
                  postprocessors = None
                  ):
         self.d = d
         self.s = s
         self.h = h
         self.num_products = len(s)
         self.q_star = None
+        if preprocessors is None:
+            self.preprocessors = []
+        else:
+            self.preprocessors = (preprocessors)
         if postprocessors is None:
             self.postprocessors = []
         else:
             self.postprocessors = (postprocessors)
 
     def set_q_star(self):
         
@@ -136,14 +153,17 @@
 
         """
 
         assert self.q_star is not None, "q_star is not set"
 
         action = np.zeros(self.num_products)
 
+        for preprocessor in self.preprocessors:
+            inventory_level = preprocessor(inventory_level)
+
         # TODO account for lead time
         action = np.where(inventory_level >= self.d, 0, self.q_star)
 
         for postprocessor in self.postprocessors:
             action = postprocessor(action)
 
         return action
```

### Comparing `RL_OM-0.0.3/RL_OM/agents/networks/actors.py` & `RL_OM-0.0.4/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/networks/base.py` & `RL_OM-0.0.4/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/networks/critics.py` & `RL_OM-0.0.4/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/processors/processors.py` & `RL_OM-0.0.4/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
     def _loss(self, state, probs, log_probs): #change
         q_0 = self._critic_approximator(state,
                                         output_tensor=True, idx=0)
         
         q_1 = self._critic_approximator(state,
                                         output_tensor=True, idx=1)
 
-        q = torch.min(q_0, q_1) #! check if this element-wise min is correct
+        q = torch.min(q_0, q_1) 
 
         return ((self._alpha * log_probs - q)*probs).sum(dim=1).mean() #! check if this is correct
 
     def _update_alpha(self, probs, log_probs):
         alpha_loss = - ((self._log_alpha * (log_probs + self._target_entropy))*probs).sum(dim=1).mean()#! check if this is correct
         self._alpha_optim.zero_grad()
         alpha_loss.backward()
```

### Comparing `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/environments/calculation_functions.py` & `RL_OM-0.0.4/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.3/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.0.4/RL_OM/environments/multi_period_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,17 @@
         self.start_inventory = start_inventory
         self.inventory_cap = inventory_cap
 
         if not self.inventory_allowed:
             assert holding_cost is None, "If inventory is not allowed, holding_cost must be None"
         self.holding_cost = holding_cost
 
+        if np.all(lead_time == 0):
+            self.use_order_pipeline = False
+
         self.lead_time = lead_time
         self.lead_time_variance = lead_time_variance
 
         if np.all(lead_time_variance == 0):
             self.max_lead_time = self.lead_time
         else:
             self.max_lead_time = max_lead_time
@@ -222,15 +225,15 @@
 
         if self.num_features > 0:
             self.observation_state[:self.num_features] = self.features[self.period]
 
         if self.inventory_allowed:
             self.observation_state[self.num_features:self.num_features+self.num_products] = self.inventory
 
-        if self.order_pipeline:
+        if self.use_order_pipeline:
             slots_occupied = 0
             for product in range(self.num_products):
                 self.observation_state[self.num_features+self.num_products+slots_occupied:self.num_features+self.num_products+slots_occupied+self.max_lead_time[product]] = self.order_pipeline[product]
                 slots_occupied += self.max_lead_time[product]
 
         if self.max_demand_backlog > 0:
             self.observation_state[self.num_features+self.num_products+np.sum(self.num_products * self.lead_time):] = self.demand_backlog
```

### Comparing `RL_OM-0.0.3/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.0.4/RL_OM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.3/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.0.4/RL_OM.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,33 @@
 RL_OM/agents/benchmark_agents/__init__.py
 RL_OM/agents/benchmark_agents/eoq.py
 RL_OM/agents/networks/__init__.py
 RL_OM/agents/networks/actors.py
 RL_OM/agents/networks/base.py
 RL_OM/agents/networks/critics.py
 RL_OM/agents/processors/__init__.py
+RL_OM/agents/processors/eoq_preprocessors.py
 RL_OM/agents/processors/processors.py
 RL_OM/agents/rl_agents/__init__.py
 RL_OM/agents/rl_agents/sac_discrete.py
 RL_OM/agents/rl_agents/sac_gumbel.py
 RL_OM/agents/rl_agents/sac_hybrid.py
 RL_OM/agents/rl_agents/sac_hybrid_reversed.py
 RL_OM/agents/rl_agents/sac_hybrid_separate.py
+RL_OM/agents/rl_agents/algorithms/__init__.py
+RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
 RL_OM/environments/__init__.py
 RL_OM/environments/calculation_functions.py
-RL_OM/environments/multi_period_inventory.py
+RL_OM/environments/data_generators.py
+RL_OM/environments/feature_converters.py
+RL_OM/environments/multi_period_inventory.py
+RL_OM/experiment_functions/__init__.py
+RL_OM/experiment_functions/run_experiment.py
```

### Comparing `RL_OM-0.0.3/settings.ini` & `RL_OM-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.0.3/setup.py` & `RL_OM-0.0.4/setup.py`

 * *Files identical despite different names*

