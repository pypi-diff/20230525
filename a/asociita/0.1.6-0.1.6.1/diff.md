# Comparing `tmp/asociita-0.1.6.tar.gz` & `tmp/asociita-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.6.tar", max compression
+gzip compressed data, was "asociita-0.1.6.1.tar", max compression
```

## Comparing `asociita-0.1.6.tar` & `asociita-0.1.6.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6/asociita/__init__.py
--rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    10709 2023-05-22 10:06:44.372395 asociita-0.1.6/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     8123 2023-05-20 18:23:51.699460 asociita-0.1.6/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     7959 2023-05-17 13:06:20.822173 asociita-0.1.6/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     4661 2023-05-12 12:28:36.608168 asociita-0.1.6/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    15498 2023-05-22 10:10:55.787158 asociita-0.1.6/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6/asociita/utils/computations.py
--rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6/asociita/utils/handlers.py
--rw-r--r--   0        0        0      484 2023-05-16 12:10:20.265814 asociita-0.1.6/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6/asociita/utils/loggers.py
--rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.6/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6/asociita/utils/showcase.py
--rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6/LICENSE
--rw-r--r--   0        0        0      669 2023-05-22 10:26:23.372950 asociita-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6/README.md
--rw-r--r--   0        0        0     3996 1970-01-01 00:00:00.000000 asociita-0.1.6/setup.py
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 asociita-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6.1/asociita/__init__.py
+-rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6.1/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6.1/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6.1/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6.1/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6.1/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6.1/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6.1/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    10709 2023-05-22 10:06:44.372395 asociita-0.1.6.1/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6.1/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     2699 2023-05-22 14:23:05.141330 asociita-0.1.6.1/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2654 2023-05-22 14:12:53.922859 asociita-0.1.6.1/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     6874 2023-05-22 14:12:25.240855 asociita-0.1.6.1/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     4661 2023-05-22 14:08:01.227174 asociita-0.1.6.1/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6.1/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6.1/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    15398 2023-05-22 14:25:35.473812 asociita-0.1.6.1/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6.1/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6.1/asociita/utils/computations.py
+-rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6.1/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6.1/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      585 2023-05-22 14:29:57.943413 asociita-0.1.6.1/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6.1/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.6.1/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6.1/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6.1/asociita/utils/showcase.py
+-rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6.1/LICENSE
+-rw-r--r--   0        0        0      671 2023-05-25 15:17:07.989704 asociita-0.1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6.1/README.md
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 asociita-0.1.6.1/setup.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 asociita-0.1.6.1/PKG-INFO
```

### Comparing `asociita-0.1.6/asociita/components/archiver/archive_manager.py` & `asociita-0.1.6.1/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.6.1/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.6.1/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.6.1/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/nodes/federated_node.py` & `asociita-0.1.6.1/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.6.1/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.6.1/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.6.1/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/datasets/fetch_data.py` & `asociita-0.1.6.1/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/datasets/load_cifar.py` & `asociita-0.1.6.1/asociita/datasets/shard_splits.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,160 +1,139 @@
 import datasets
 from datasets import load_dataset
 from asociita.datasets.shard_transformation import Shard_Transformation
-from asociita.utils.showcase import save_random
 from asociita.utils.handlers import Handler
+from asociita.utils.showcase import save_random
 import copy
-import pandas as pd
-import numpy as np
 
-def load_cifar(settings: dict) -> list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
-    """Loads the CIFAR dataset, splits it into the number of shards, pre-process selected
-    shards (subsets) and returns in a following format:
-    list[   
-        "Orchestrator Data"[
-            Dataset
-            ],   
-        "Agents Data"[
-            "Agent N"[
-                "Train Data"[
-                Dataset
-                ],
-                "Test Data"[
-                Dataset
-                ]
-            ]]]
-    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
-    ---------
-    Args:
-        settings (dict) : A dictionary containing all the dataset settings.
-    Returns:
-        list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
-    
-    # Using the 'test' data as a orchestrator validaiton set.
-    orchestrator_data = load_dataset('cifar10', split='test')
-    # Using the 'train' data as a dataset reserved for agents
-    dataset = load_dataset('cifar10', split='train')
 
-    # List datasets for all nodes.
-    nodes_data = []
-    
-    
-    # Type: Random Uniform (Sharding) -> Same size, random distribution
-    if settings['split_type'] == 'random_uniform':
+
+class Shard_Splits:
+    """a common class for creating various splits among the clients"""
+
+    @staticmethod
+    def random_uniform(dataset: datasets.arrow_dataset.Dataset,
+                       settings: dict):
+        nodes_data = []
         for shard in range(settings['shards']): # Each shard corresponds to one
             agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
             
             # Shard transformation
             if shard in settings['transformations'].keys():
                 if settings['save_transformations']:
                     original_imgs = copy.deepcopy(agent_data['image'])
                 agent_data = Shard_Transformation.transform(agent_data, preferences=settings['transformations'][shard]) # CALL SHARD_TRANSFORMATION CLASS
                 if settings['save_transformations']:
                     save_random(original_imgs, agent_data['image'], settings['transformations'][shard])
 
             # In-shard split between test and train data.
             agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
             nodes_data.append([agent_data['train'], agent_data['test']])
+        return nodes_data
     
 
-    # # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
-    # if settings['split_type'] == 'random_imbalanced':
-    #     no_agents = settings['agents']
-    #     imbalanced_agents = settings['imbalanced_clients']
-    #     agents = [agent for agent in range(no_agents)]
-    #     pandas_df = dataset.to_pandas().drop('image', axis=1)
-    #     labels = sorted(pandas_df.label.unique())
+    @staticmethod
+    def random_imbalanced(dataset: datasets.arrow_dataset.Dataset,
+                          settings: dict):
+        nodes_data = []
+        no_agents = settings['agents']
+        imbalanced_agents = settings['imbalanced_clients']
+        agents = [agent for agent in range(no_agents)]
+        pandas_df = dataset.to_pandas().drop('image', axis=1)
+        labels = sorted(pandas_df.label.unique())
 
-    #     save_distribution = False
-    #     print_distribution = False
+        save_distribution = False
+        print_distribution = False
         
-    #     if settings.get('save_distribution'):
-    #         distribution_blueprint = []
-    #         save_distribution = True
-    #     if settings.get('print_distribution'):
-    #         print_distribution = True
-    #     if settings.get('custom_sample_size'):
-    #         sample_size = settings['custom_sample_size']
-    #     else:
-    #         sample_size = int(len(dataset) / no_agents)
-    
-
-    #     # I) Sampling dominant clients
-    #     for agent in agents:
-    #         if agent in imbalanced_agents:
-    #             # 1. Sampling indexes
-    #             sampling_weights = {key: (1 - imbalanced_agents[agent][1]) / (len(labels) - 1) for key in labels}
-    #             sampling_weights[imbalanced_agents[agent][0]] = imbalanced_agents[agent][1]
+        if settings.get('save_distribution'):
+            distribution_blueprint = []
+            save_distribution = True
+        if settings.get('print_distribution'):
+            print_distribution = True
+        if settings.get('custom_sample_size'):
+            sample_size = settings['custom_sample_size']
+        else:
+            sample_size = int(len(dataset) / no_agents)
+    
+
+        # I) Sampling dominant clients
+        for agent in agents:
+            if agent in imbalanced_agents:
+                # 1. Sampling indexes
+                sampling_weights = {key: (1 - imbalanced_agents[agent][1]) / (len(labels) - 1) for key in labels}
+                sampling_weights[imbalanced_agents[agent][0]] = imbalanced_agents[agent][1]
                 
-    #             # Additional step, checking the availability of every label TODO
-    #             # required_samples = (np.array(list(sampling_weights.values())) * sample_size).astype('int')
-    #             # counts = pandas_df['label'].value_counts()[pandas_df['label'].value_counts() > required_samples]
+                # Additional step, checking the availability of every label TODO
+                # required_samples = (np.array(list(sampling_weights.values())) * sample_size).astype('int')
+                # counts = pandas_df['label'].value_counts()[pandas_df['label'].value_counts() > required_samples]
                 
-    #             # 2. Apllying weights
-    #             pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
-    #             sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
+                # 2. Apllying weights
+                pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
+                sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
                 
-    #             counts = sample['label'].value_counts().sort_index()
-    #             if print_distribution:
-    #                 print(f"Distribution of client {agent} is : {counts}")
-    #             if save_distribution:
-    #                 ag = counts.to_dict()
-    #                 distribution = {'agent':agent}
-    #                 distribution.update(ag)
-    #                 distribution_blueprint.append(distribution)
-    #             # 3. Selecting indexes and performing test - train split.
-    #             sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
-    #             agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
-    #             nodes_data.append([agent_data['train'], agent_data['test']])
+                counts = sample['label'].value_counts().sort_index()
+                if print_distribution:
+                    print(f"Distribution of client {agent} is : {counts}")
+                if save_distribution:
+                    ag = counts.to_dict()
+                    distribution = {'agent':agent}
+                    distribution.update(ag)
+                    distribution_blueprint.append(distribution)
+                # 3. Selecting indexes and performing test - train split.
+                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
+                agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
+                nodes_data.append([agent_data['train'], agent_data['test']])
                 
-    #             # 4. Removing samples indexes
-    #             pandas_df.drop(sample.index, inplace=True)
-    #         else:
-    #             nodes_data.append([]) # Inserting placeholder to preserve in-list order.
-
-
-    #     # II) Sampling balanced clients
-    #     for agent in agents:
-    #         if agent not in imbalanced_agents:
-    #             # 1. Sampling indexes
-    #             sample = pandas_df.sample(n = sample_size, random_state=42)
-    #             counts = sample['label'].value_counts().sort_index()
-    #             if print_distribution:
-    #                 print(f"Distribution of client {agent} is : {counts}")
-    #             if save_distribution:
-    #                 ag = counts.to_dict()
-    #                 distribution = {'agent':agent}
-    #                 distribution.update(ag)
-    #                 distribution_blueprint.append(distribution)
-    #             # 2. Selecting indexes and performing test - train split.
-    #             sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
-    #             agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
-    #             nodes_data[agent] = ([agent_data['train'], agent_data['test']])
-    #             # 3. Removing samples indexes
-    #             pandas_df.drop(sample.index, inplace=True)
+                # 4. Removing samples indexes
+                pandas_df.drop(sample.index, inplace=True)
+            else:
+                nodes_data.append([]) # Inserting placeholder to preserve in-list order.
+
+
+        # II) Sampling balanced clients
+        for agent in agents:
+            if agent not in imbalanced_agents:
+                # 1. Sampling indexes
+                sample = pandas_df.sample(n = sample_size, random_state=42)
+                counts = sample['label'].value_counts().sort_index()
+                if print_distribution:
+                    print(f"Distribution of client {agent} is : {counts}")
+                if save_distribution:
+                    ag = counts.to_dict()
+                    distribution = {'agent':agent}
+                    distribution.update(ag)
+                    distribution_blueprint.append(distribution)
+                # 2. Selecting indexes and performing test - train split.
+                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
+                agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
+                nodes_data[agent] = ([agent_data['train'], agent_data['test']])
+                # 3. Removing samples indexes
+                pandas_df.drop(sample.index, inplace=True)
         
-    #     if save_distribution:
-    #         Handler.save_csv_file(file = distribution_blueprint,
-    #                               saving_path=settings['save_path'],
-    #                               file_name='distribution_blueprint.csv')
-
-    # # Type: Same Dataset -> One dataset copied n times.
-    # elif settings['split_type'] == 'same_dataset':
-    #     agent_data = dataset.shard(num_shards=1, index=0)
-    #     agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
-    #     for _ in range(settings['agents']):
-    #         nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
+        if save_distribution:
+            Handler.save_csv_file(file = distribution_blueprint,
+                                  saving_path=settings['save_path'],
+                                  file_name='distribution_blueprint.csv')
+        return nodes_data
+
+    @staticmethod
+    def replicate_same_dataset(dataset: datasets.arrow_dataset.Dataset,
+                               settings: dict):
+        nodes_data = []
+        agent_data = dataset.shard(num_shards=1, index=0)
+        agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
+        for _ in range(settings['agents']):
+            nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
+        
+        return nodes_data
     
 
-    # # Type: Blocks - One dataset copied inside one block (cluster)
-    # elif settings['split_type'] == 'blocks':
-    #     for shard in range(settings['shards']):
-    #         agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
-    #         agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
-    #         for _ in range((int(settings['agents'] / settings['shards']))):
-    #             nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
-
-    return [orchestrator_data, nodes_data]
-            
+    @staticmethod
+    def split_in_blocks(dataset: datasets.arrow_dataset.Dataset,
+                        settings: dict):
+        nodes_data = []
+        for shard in range(settings['shards']):
+            agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
+            agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
+            for _ in range((int(settings['agents'] / settings['shards']))):
+                nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
+        return nodes_data
```

### Comparing `asociita-0.1.6/asociita/datasets/shard_transformation.py` & `asociita-0.1.6.1/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/models/pytorch/cifar10.py` & `asociita-0.1.6.1/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/models/pytorch/federated_model.py` & `asociita-0.1.6.1/asociita/models/pytorch/federated_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         assert settings, "Could not find settings, please ensure that a valid dictionary containing settings was passed in a function call."
         assert net, "Could not find net object, please ensure that a valid nn.Module was passed in a function call."
         assert local_dataset, "Could not find local dataset that should be used with that model. Pleasure ensure that local dataset was passed in a function call."
         
         self.net = net
         self.settings = settings
         self.node_name = node_name
-        self.features_name = settings["features_name"]
         # If both, train and test data were provided
         if len(local_dataset) == 2:
             self.trainloader, self.testloader = self.prepare_data(local_dataset)
         # If only a test dataset was provided.
         elif len(local_dataset) == 1:
             self.testloader = self.prepare_data(local_dataset, only_test=True)
         else:
@@ -265,15 +264,15 @@
         running_loss = 0.0
         total_correct = 0
         total = 0
         #self.net = self.net.to(self.device)
 
         self.net.train()
         for _, dic in enumerate(self.trainloader):
-            data = dic[self.features_name]
+            data = dic['image']
             target = dic['label']
 
             self.optimizer.zero_grad()
 
             if isinstance(data, list):
                 data = data[0]
 
@@ -323,15 +322,15 @@
                 correct = 0
                 total = 0
                 y_pred = []
                 y_true = []
                 losses = []
                 with torch.no_grad():
                     for _, dic in enumerate(self.testloader):
-                        data = dic[self.features_name]
+                        data = dic['image']
                         target = dic['label']
                         data, target = data.to(self.device), target.to(self.device)
                         output = self.net(data)
                         total += target.size(0)
                         test_loss = criterion(output, target).item()
                         losses.append(test_loss)
                         pred = output.argmax(dim=1, keepdim=True)
@@ -387,9 +386,9 @@
                     false_positive_rate
                 )
 
 
     def transform_func(self,
                        data):
         convert_tensor = transforms.ToTensor()
-        data[self.features_name] = [convert_tensor(img) for img in data[self.features_name]]
+        data['image'] = [convert_tensor(img) for img in data['image']]
         return data
```

### Comparing `asociita-0.1.6/asociita/models/pytorch/mnist.py` & `asociita-0.1.6.1/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/computations.py` & `asociita-0.1.6.1/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/custom_transformations.py` & `asociita-0.1.6.1/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/handlers.py` & `asociita-0.1.6.1/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/loggers.py` & `asociita-0.1.6.1/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/optimizers.py` & `asociita-0.1.6.1/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/orchestrations.py` & `asociita-0.1.6.1/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/asociita/utils/showcase.py` & `asociita-0.1.6.1/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/LICENSE` & `asociita-0.1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/pyproject.toml` & `asociita-0.1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.6"
+version = "0.1.6.1"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.6/README.md` & `asociita-0.1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6/setup.py` & `asociita-0.1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'numpy>=1.24.1,<2.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
  'torch>=1.13.1,<2.0.0',
  'torchvision>=0.14.1,<0.15.0']
 
 setup_kwargs = {
     'name': 'asociita',
-    'version': '0.1.6',
+    'version': '0.1.6.1',
     'description': "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.",
     'long_description': '### Setting Configuration\n\nIn order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.\n\n```\n{\n    "orchestrator":{\n        "iterations": int,\n        "number_of_nodes": int,\n        "local_warm_start": bool,\n        "sample_size": int,\n        "evaluation": "none" | "full"\n        "save_metrics": bool,\n\t"save_models": bool,\n\t"save_path": str\n\t"nodes": [0,\n\t1,\n\t2]\n    },\n    "nodes":{\n    "local_epochs": int,\n    "model_settings": {\n        "optimizer": "RMS",\n        "batch_size": int,\n        "learning_rate": float}\n        }\n}\n```\n\nThe `settings` contains two dictionaries: `orchestrator` and `nodes`.\n\n`orchestrator` contains all the settings necessary details of the training:\n\n* `iterations` is the number of rounds to be performed. Example: `iterations:12`\n* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`\n* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.\n* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`\n* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`\n* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`\n* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.\n* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.\n* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.\n\n`nodes` contains all the necessary configuration for nodes.\n\n* `"local_epochs":` the number of local epochs to be performed on the local nodes.\n* `"model_settings"` is a dictionary containing all the parameters for training the model.\n  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`\n  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`\n  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`\n',
     'author': 'Maciej Zuziak',
     'author_email': 'maciejkrzysztof.zuziak@isti.cnr.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Scolpe/Asociita',
```

### Comparing `asociita-0.1.6/PKG-INFO` & `asociita-0.1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

