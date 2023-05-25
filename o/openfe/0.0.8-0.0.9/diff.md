# Comparing `tmp/openfe-0.0.8.tar.gz` & `tmp/openfe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfe-0.0.8.tar", last modified: Sun Feb 12 11:44:10 2023, max compression
+gzip compressed data, was "openfe-0.0.9.tar", last modified: Wed Feb 22 08:55:30 2023, max compression
```

## Comparing `openfe-0.0.8.tar` & `openfe-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 11:44:10.439477 openfe-0.0.8/
--rw-rw-rw-   0        0        0     1075 2022-11-21 11:12:13.000000 openfe-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3464 2023-02-12 11:44:10.438479 openfe-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2022-11-29 02:57:38.000000 openfe-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-12 11:44:10.429479 openfe-0.0.8/openfe/
--rw-rw-rw-   0        0        0     6195 2022-12-07 08:52:43.000000 openfe-0.0.8/openfe/FeatureGenerator.py
--rw-rw-rw-   0        0        0      408 2022-11-23 14:07:47.000000 openfe-0.0.8/openfe/__init__.py
--rw-rw-rw-   0        0        0    37659 2023-02-12 11:41:32.000000 openfe-0.0.8/openfe/openfe.py
--rw-rw-rw-   0        0        0     6003 2022-12-19 02:47:19.000000 openfe-0.0.8/openfe/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-12 11:44:10.438479 openfe-0.0.8/openfe.egg-info/
--rw-rw-rw-   0        0        0     3464 2023-02-12 11:44:10.000000 openfe-0.0.8/openfe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-02-12 11:44:10.000000 openfe-0.0.8/openfe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 11:44:10.000000 openfe-0.0.8/openfe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-02-12 11:44:10.000000 openfe-0.0.8/openfe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-12 11:44:10.000000 openfe-0.0.8/openfe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-12 11:44:10.439477 openfe-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      889 2023-02-12 11:43:19.000000 openfe-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-22 08:55:30.611690 openfe-0.0.9/
+-rw-rw-rw-   0        0        0     1075 2022-11-21 11:12:13.000000 openfe-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3593 2023-02-22 08:55:30.611690 openfe-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-02-20 08:15:34.000000 openfe-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-22 08:55:30.597213 openfe-0.0.9/openfe/
+-rw-rw-rw-   0        0        0     6195 2022-12-07 08:52:43.000000 openfe-0.0.9/openfe/FeatureGenerator.py
+-rw-rw-rw-   0        0        0      408 2022-11-23 14:07:47.000000 openfe-0.0.9/openfe/__init__.py
+-rw-rw-rw-   0        0        0    38369 2023-02-22 08:42:17.000000 openfe-0.0.9/openfe/openfe.py
+-rw-rw-rw-   0        0        0     6003 2022-12-19 02:47:19.000000 openfe-0.0.9/openfe/utils.py
+drwxrwxrwx   0        0        0        0 2023-02-22 08:55:30.610682 openfe-0.0.9/openfe.egg-info/
+-rw-rw-rw-   0        0        0     3593 2023-02-22 08:55:30.000000 openfe-0.0.9/openfe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-02-22 08:55:30.000000 openfe-0.0.9/openfe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-22 08:55:30.000000 openfe-0.0.9/openfe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-02-22 08:55:30.000000 openfe-0.0.9/openfe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-02-22 08:55:30.000000 openfe-0.0.9/openfe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-22 08:55:30.611690 openfe-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      889 2023-02-22 08:55:26.000000 openfe-0.0.9/setup.py
```

### Comparing `openfe-0.0.8/LICENSE` & `openfe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openfe-0.0.8/PKG-INFO` & `openfe-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfe
-Version: 0.0.8
+Version: 0.0.9
 Summary: OpenFE: automated feature generation beyond expert-level performance
 Home-page: https://github.com/IIIS-Li-Group/OpenFE/
 Author: Tianping Zhang
 Author-email: ztp18@mails.tsinghua.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,15 @@
 
 OpenFE is a new framework for automated feature generation for tabular data. 
 OpenFE is easy-to-use, effective, and efficient with following advantages:
 - OpenFE can discover effective candidate features for improving the learning performance of both GBDT and neural networks.
 - OpenFE is efficient and supports parallel computing.
 - OpenFE covers 23 useful and effective operators for generating candidate features.
 - OpenFE supports binary-classification, multi-classification, and regression tasks.
+- OpenFE can automatically handle missing values and categorical features.
 
 For further details, please refer to [the paper](https://arxiv.org/abs/2211.12507). 
 
 Extensive comparison experiments on public datasets show that OpenFE outperforms existing feature generation methods on both effectiveness and efficiency.
 Moreover, we validate OpenFE on the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/ieee-fraud-detection)
 Kaggle competition, and show that a simple XGBoost model with features generated by OpenFE 
 beats 99.3% of 6351 data science teams. The features generated by OpenFE results in larger performance
@@ -66,8 +67,8 @@
 train_x, test_x = transform(train_x, test_x, features, n_jobs=n_jobs) # transform the train and test data according to generated features.
 ```
 
 We provide an example using the standard california_housing dataset in 
 [this link](<https://github.com/IIIS-Li-Group/OpenFE/blob/master/examples/california_housing.py>). 
 A more complicated example demonstrating OpenFE can outperform machine learning experts in the IEEE-CIS Fraud Detection 
 Kaggle competition is provided in [this link](<https://github.com/IIIS-Li-Group/OpenFE/blob/master/examples/IEEE-CIS-Fraud-Detection/>).
-Users can also refer to our [documentation] for more advanced usage of OpenFE and FAQ about feature generation.
+Users can also refer to our [documentation](<https://openfe-document.readthedocs.io/en/latest/>) for more advanced usage of OpenFE and FAQ about feature generation.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openfe Version: 0.0.8 Summary: OpenFE: automated
+Metadata-Version: 2.1 Name: openfe Version: 0.0.9 Summary: OpenFE: automated
 feature generation beyond expert-level performance Home-page: https://
 github.com/IIIS-Li-Group/OpenFE/ Author: Tianping Zhang Author-email:
 ztp18@mails.tsinghua.edu.cn Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE
   [https://github.com/IIIS-Li-Group/OpenFE/blob/master/docs/logo/openfe.svg]
@@ -11,21 +11,22 @@
                  **** |Paper | Documentation | Examples | ****
 OpenFE is a new framework for automated feature generation for tabular data.
 OpenFE is easy-to-use, effective, and efficient with following advantages: -
 OpenFE can discover effective candidate features for improving the learning
 performance of both GBDT and neural networks. - OpenFE is efficient and
 supports parallel computing. - OpenFE covers 23 useful and effective operators
 for generating candidate features. - OpenFE supports binary-classification,
-multi-classification, and regression tasks. For further details, please refer
-to [the paper](https://arxiv.org/abs/2211.12507). Extensive comparison
-experiments on public datasets show that OpenFE outperforms existing feature
-generation methods on both effectiveness and efficiency. Moreover, we validate
-OpenFE on the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/
-ieee-fraud-detection) Kaggle competition, and show that a simple XGBoost model
-with features generated by OpenFE beats 99.3% of 6351 data science teams. The
+multi-classification, and regression tasks. - OpenFE can automatically handle
+missing values and categorical features. For further details, please refer to
+[the paper](https://arxiv.org/abs/2211.12507). Extensive comparison experiments
+on public datasets show that OpenFE outperforms existing feature generation
+methods on both effectiveness and efficiency. Moreover, we validate OpenFE on
+the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/ieee-fraud-
+detection) Kaggle competition, and show that a simple XGBoost model with
+features generated by OpenFE beats 99.3% of 6351 data science teams. The
 features generated by OpenFE results in larger performance improvement than the
 features provided by the first-place team in the competition. Get Started and
 Documentation ----------------------------- **Installation** It is recommended
 to use **pip** for installation. ``` pip install openfe ``` Please do not use
 **conda install openfe** for installation. It will install another python
 package different from ours. **A Quick Example** It only takes four lines of
 codes to generate features by OpenFE. First, we generate features by OpenFE.
@@ -36,9 +37,10 @@
 test data according to generated features. ``` We provide an example using the
 standard california_housing dataset in [this link](
 github.com/IIIS-Li-Group/OpenFE/blob/master/examples/california_housing.py>). A
 more complicated example demonstrating OpenFE can outperform machine learning
 experts in the IEEE-CIS Fraud Detection Kaggle competition is provided in [this
 link](
 github.com/IIIS-Li-Group/OpenFE/blob/master/examples/IEEE-CIS-Fraud-Detection/
->). Users can also refer to our [documentation] for more advanced usage of
-OpenFE and FAQ about feature generation.
+>). Users can also refer to our [documentation](
+openfe-document.readthedocs.io/en/latest/>) for more advanced usage of OpenFE
+and FAQ about feature generation.
```

### Comparing `openfe-0.0.8/README.md` & `openfe-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 OpenFE is a new framework for automated feature generation for tabular data. 
 OpenFE is easy-to-use, effective, and efficient with following advantages:
 - OpenFE can discover effective candidate features for improving the learning performance of both GBDT and neural networks.
 - OpenFE is efficient and supports parallel computing.
 - OpenFE covers 23 useful and effective operators for generating candidate features.
 - OpenFE supports binary-classification, multi-classification, and regression tasks.
+- OpenFE can automatically handle missing values and categorical features.
 
 For further details, please refer to [the paper](https://arxiv.org/abs/2211.12507). 
 
 Extensive comparison experiments on public datasets show that OpenFE outperforms existing feature generation methods on both effectiveness and efficiency.
 Moreover, we validate OpenFE on the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/ieee-fraud-detection)
 Kaggle competition, and show that a simple XGBoost model with features generated by OpenFE 
 beats 99.3% of 6351 data science teams. The features generated by OpenFE results in larger performance
@@ -52,8 +53,8 @@
 train_x, test_x = transform(train_x, test_x, features, n_jobs=n_jobs) # transform the train and test data according to generated features.
 ```
 
 We provide an example using the standard california_housing dataset in 
 [this link](<https://github.com/IIIS-Li-Group/OpenFE/blob/master/examples/california_housing.py>). 
 A more complicated example demonstrating OpenFE can outperform machine learning experts in the IEEE-CIS Fraud Detection 
 Kaggle competition is provided in [this link](<https://github.com/IIIS-Li-Group/OpenFE/blob/master/examples/IEEE-CIS-Fraud-Detection/>).
-Users can also refer to our [documentation] for more advanced usage of OpenFE and FAQ about feature generation.
+Users can also refer to our [documentation](<https://openfe-document.readthedocs.io/en/latest/>) for more advanced usage of OpenFE and FAQ about feature generation.
```

#### html2text {}

```diff
@@ -4,21 +4,22 @@
                  **** |Paper | Documentation | Examples | ****
 OpenFE is a new framework for automated feature generation for tabular data.
 OpenFE is easy-to-use, effective, and efficient with following advantages: -
 OpenFE can discover effective candidate features for improving the learning
 performance of both GBDT and neural networks. - OpenFE is efficient and
 supports parallel computing. - OpenFE covers 23 useful and effective operators
 for generating candidate features. - OpenFE supports binary-classification,
-multi-classification, and regression tasks. For further details, please refer
-to [the paper](https://arxiv.org/abs/2211.12507). Extensive comparison
-experiments on public datasets show that OpenFE outperforms existing feature
-generation methods on both effectiveness and efficiency. Moreover, we validate
-OpenFE on the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/
-ieee-fraud-detection) Kaggle competition, and show that a simple XGBoost model
-with features generated by OpenFE beats 99.3% of 6351 data science teams. The
+multi-classification, and regression tasks. - OpenFE can automatically handle
+missing values and categorical features. For further details, please refer to
+[the paper](https://arxiv.org/abs/2211.12507). Extensive comparison experiments
+on public datasets show that OpenFE outperforms existing feature generation
+methods on both effectiveness and efficiency. Moreover, we validate OpenFE on
+the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/ieee-fraud-
+detection) Kaggle competition, and show that a simple XGBoost model with
+features generated by OpenFE beats 99.3% of 6351 data science teams. The
 features generated by OpenFE results in larger performance improvement than the
 features provided by the first-place team in the competition. Get Started and
 Documentation ----------------------------- **Installation** It is recommended
 to use **pip** for installation. ``` pip install openfe ``` Please do not use
 **conda install openfe** for installation. It will install another python
 package different from ours. **A Quick Example** It only takes four lines of
 codes to generate features by OpenFE. First, we generate features by OpenFE.
@@ -29,9 +30,10 @@
 test data according to generated features. ``` We provide an example using the
 standard california_housing dataset in [this link](
 github.com/IIIS-Li-Group/OpenFE/blob/master/examples/california_housing.py>). A
 more complicated example demonstrating OpenFE can outperform machine learning
 experts in the IEEE-CIS Fraud Detection Kaggle competition is provided in [this
 link](
 github.com/IIIS-Li-Group/OpenFE/blob/master/examples/IEEE-CIS-Fraud-Detection/
->). Users can also refer to our [documentation] for more advanced usage of
-OpenFE and FAQ about feature generation.
+>). Users can also refer to our [documentation](
+openfe-document.readthedocs.io/en/latest/>) for more advanced usage of OpenFE
+and FAQ about feature generation.
```

### Comparing `openfe-0.0.8/openfe/FeatureGenerator.py` & `openfe-0.0.9/openfe/FeatureGenerator.py`

 * *Files identical despite different names*

### Comparing `openfe-0.0.8/openfe/openfe.py` & `openfe-0.0.9/openfe/openfe.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .utils import tree_to_formula, check_xor, formula_to_tree
 from sklearn.inspection import permutation_importance
 from sklearn.feature_selection import mutual_info_regression, mutual_info_classif
 from sklearn.metrics import mean_squared_error, log_loss, roc_auc_score
 import scipy.special
 from copy import deepcopy
 from tqdm import tqdm
+# import tracemalloc
 from datetime import datetime
 
 
 def _enumerate(current_order_num_features, lower_order_num_features,
                current_order_cat_features, lower_order_cat_features):
     num_candidate_features = []
     cat_candidate_features = []
@@ -307,14 +308,19 @@
         gc.collect()
         return self.new_features_list
 
     def myprint(self, s):
         if self.verbose:
             print(s)
 
+    # def monitor_memory(self):
+    #     peak_memory = tracemalloc.get_traced_memory()
+    #     print(peak_memory)
+    #     self.myprint(f"Peak memory usage: {peak_memory[1] / 1024 / 1024:.2f} MB")
+
     def process_and_save_data(self):
         self.data.index.name = 'openfe_index'
         self.data.reset_index().to_feather(self.tmp_save_path)
 
     def get_index(self, train_index, val_index):
         if train_index is None or val_index is None:
             if self.task == 'classification':
@@ -477,44 +483,51 @@
                 self.myprint("Meet early-stopping in successive feature-wise halving.")
             candidate_features_list = [item[0] for item in candidate_features_scores[:n_reserved_features]]
             del candidate_features_scores[n_reserved_features:]; gc.collect()
 
             results = self._calculate_and_evaluate(candidate_features_list, train_idx, val_idx)
             candidate_features_scores = sorted(results, key=lambda x: x[1], reverse=True)
 
-        return_results = [item for item in candidate_features_scores if item[1] > 0]
+        return_results = [item[0] for item in candidate_features_scores if item[1] > 0]
         if not return_results:
-            return_results = [item for item in candidate_features_scores[:100]]
+            return_results = [item[0] for item in candidate_features_scores[:100]]
         return return_results
 
     def stage2_select(self):
         data_new = []
         new_features = []
-        for feature, score in self.candidate_features_list:
+        self.candidate_features_list = self._calculate(self.candidate_features_list,
+                                                       self.train_index.to_list(),
+                                                       self.val_index.to_list())
+        index_tmp = self.candidate_features_list[0].data.index
+        for feature in self.candidate_features_list:
             new_features.append(tree_to_formula(feature))
             data_new.append(feature.data.values)
+            feature.delete()
+        gc.collect()
         data_new = np.vstack(data_new)
-        data_new = pd.DataFrame(data_new.T, index=self.candidate_features_list[0][0].data.index,
+        data_new = pd.DataFrame(data_new.T, index=index_tmp,
                                 columns=['autoFE-%d' % i for i in range(len(new_features))])
         data_new = pd.concat([data_new, self.data], axis=1)
         for f in self.categorical_features:
             data_new[f] = data_new[f].astype('category')
             data_new[f] = data_new[f].cat.codes
             data_new[f] = data_new[f].astype('category')
         data_new = data_new.replace([np.inf, -np.inf], np.nan)
         if self.drop_columns is not None:
             data_new = data_new.drop(self.drop_columns, axis=1)
         train_y = self.label.loc[self.train_index]
         val_y = self.label.loc[self.val_index]
         train_init = self.init_scores.loc[self.train_index]
         val_init = self.init_scores.loc[self.val_index]
 
-        train_x = data_new.loc[self.train_index]
-        val_x = data_new.loc[self.val_index]
-
+        train_x = data_new.loc[self.train_index].copy()
+        val_x = data_new.loc[self.val_index].copy()
+        del data_new
+        gc.collect()
         self.myprint("Finish data processing.")
         if self.stage2_params is None:
             params = {"n_estimators": 1000, "importance_type": "gain", "num_leaves": 16,
                       "seed": 1, "n_jobs": self.n_jobs}
         else:
             params = self.stage2_params
         if self.metric is not None:
@@ -624,27 +637,28 @@
             data = pd.read_feather(self.tmp_save_path, columns=list(base_features)).set_index('openfe_index')
             data_temp = data.loc[train_idx + val_idx]
             del data
             gc.collect()
 
             for candidate_feature in candidate_features:
                 candidate_feature.calculate(data_temp, is_root=True)
+                candidate_feature.f_delete()
                 results.append(candidate_feature)
             return results
         except:
             print(traceback.format_exc())
             exit()
 
     def _calculate(self, candidate_features, train_idx, val_idx):
         results = []
         length = int(np.ceil(len(candidate_features) / self.n_jobs / 4))
         n = int(np.ceil(len(candidate_features) / length))
         random.shuffle(candidate_features)
-        for f in candidate_features:
-            f.delete()
+        # for f in candidate_features:
+        #     f.delete()
         with ProcessPoolExecutor(max_workers=self.n_jobs) as ex:
             with tqdm(total=n) as progress:
                 for i in range(n):
                     if i == (n - 1):
                         future = ex.submit(self._calculate_multiprocess,
                                            candidate_features[i * length:],
                                            train_idx, val_idx)
@@ -675,14 +689,15 @@
             val_y = self.label.loc[val_idx]
             train_init = self.init_scores.loc[train_idx]
             val_init = self.init_scores.loc[val_idx]
             init_metric = self.get_init_metric(val_init, val_y)
             for candidate_feature in candidate_features:
                 candidate_feature.calculate(data_temp, is_root=True)
                 score = self._evaluate(candidate_feature, train_y, val_y, train_init, val_init, init_metric)
+                candidate_feature.delete()
                 results.append([candidate_feature, score])
             return results
         except:
             print(traceback.format_exc())
             exit()
 
     def _calculate_and_evaluate(self, candidate_features, train_idx, val_idx):
```

### Comparing `openfe-0.0.8/openfe/utils.py` & `openfe-0.0.9/openfe/utils.py`

 * *Files identical despite different names*

### Comparing `openfe-0.0.8/openfe.egg-info/PKG-INFO` & `openfe-0.0.9/openfe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfe
-Version: 0.0.8
+Version: 0.0.9
 Summary: OpenFE: automated feature generation beyond expert-level performance
 Home-page: https://github.com/IIIS-Li-Group/OpenFE/
 Author: Tianping Zhang
 Author-email: ztp18@mails.tsinghua.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,15 @@
 
 OpenFE is a new framework for automated feature generation for tabular data. 
 OpenFE is easy-to-use, effective, and efficient with following advantages:
 - OpenFE can discover effective candidate features for improving the learning performance of both GBDT and neural networks.
 - OpenFE is efficient and supports parallel computing.
 - OpenFE covers 23 useful and effective operators for generating candidate features.
 - OpenFE supports binary-classification, multi-classification, and regression tasks.
+- OpenFE can automatically handle missing values and categorical features.
 
 For further details, please refer to [the paper](https://arxiv.org/abs/2211.12507). 
 
 Extensive comparison experiments on public datasets show that OpenFE outperforms existing feature generation methods on both effectiveness and efficiency.
 Moreover, we validate OpenFE on the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/ieee-fraud-detection)
 Kaggle competition, and show that a simple XGBoost model with features generated by OpenFE 
 beats 99.3% of 6351 data science teams. The features generated by OpenFE results in larger performance
@@ -66,8 +67,8 @@
 train_x, test_x = transform(train_x, test_x, features, n_jobs=n_jobs) # transform the train and test data according to generated features.
 ```
 
 We provide an example using the standard california_housing dataset in 
 [this link](<https://github.com/IIIS-Li-Group/OpenFE/blob/master/examples/california_housing.py>). 
 A more complicated example demonstrating OpenFE can outperform machine learning experts in the IEEE-CIS Fraud Detection 
 Kaggle competition is provided in [this link](<https://github.com/IIIS-Li-Group/OpenFE/blob/master/examples/IEEE-CIS-Fraud-Detection/>).
-Users can also refer to our [documentation] for more advanced usage of OpenFE and FAQ about feature generation.
+Users can also refer to our [documentation](<https://openfe-document.readthedocs.io/en/latest/>) for more advanced usage of OpenFE and FAQ about feature generation.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openfe Version: 0.0.8 Summary: OpenFE: automated
+Metadata-Version: 2.1 Name: openfe Version: 0.0.9 Summary: OpenFE: automated
 feature generation beyond expert-level performance Home-page: https://
 github.com/IIIS-Li-Group/OpenFE/ Author: Tianping Zhang Author-email:
 ztp18@mails.tsinghua.edu.cn Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE
   [https://github.com/IIIS-Li-Group/OpenFE/blob/master/docs/logo/openfe.svg]
@@ -11,21 +11,22 @@
                  **** |Paper | Documentation | Examples | ****
 OpenFE is a new framework for automated feature generation for tabular data.
 OpenFE is easy-to-use, effective, and efficient with following advantages: -
 OpenFE can discover effective candidate features for improving the learning
 performance of both GBDT and neural networks. - OpenFE is efficient and
 supports parallel computing. - OpenFE covers 23 useful and effective operators
 for generating candidate features. - OpenFE supports binary-classification,
-multi-classification, and regression tasks. For further details, please refer
-to [the paper](https://arxiv.org/abs/2211.12507). Extensive comparison
-experiments on public datasets show that OpenFE outperforms existing feature
-generation methods on both effectiveness and efficiency. Moreover, we validate
-OpenFE on the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/
-ieee-fraud-detection) Kaggle competition, and show that a simple XGBoost model
-with features generated by OpenFE beats 99.3% of 6351 data science teams. The
+multi-classification, and regression tasks. - OpenFE can automatically handle
+missing values and categorical features. For further details, please refer to
+[the paper](https://arxiv.org/abs/2211.12507). Extensive comparison experiments
+on public datasets show that OpenFE outperforms existing feature generation
+methods on both effectiveness and efficiency. Moreover, we validate OpenFE on
+the [IEEE-CIS Fraud Detection](https://www.kaggle.com/competitions/ieee-fraud-
+detection) Kaggle competition, and show that a simple XGBoost model with
+features generated by OpenFE beats 99.3% of 6351 data science teams. The
 features generated by OpenFE results in larger performance improvement than the
 features provided by the first-place team in the competition. Get Started and
 Documentation ----------------------------- **Installation** It is recommended
 to use **pip** for installation. ``` pip install openfe ``` Please do not use
 **conda install openfe** for installation. It will install another python
 package different from ours. **A Quick Example** It only takes four lines of
 codes to generate features by OpenFE. First, we generate features by OpenFE.
@@ -36,9 +37,10 @@
 test data according to generated features. ``` We provide an example using the
 standard california_housing dataset in [this link](
 github.com/IIIS-Li-Group/OpenFE/blob/master/examples/california_housing.py>). A
 more complicated example demonstrating OpenFE can outperform machine learning
 experts in the IEEE-CIS Fraud Detection Kaggle competition is provided in [this
 link](
 github.com/IIIS-Li-Group/OpenFE/blob/master/examples/IEEE-CIS-Fraud-Detection/
->). Users can also refer to our [documentation] for more advanced usage of
-OpenFE and FAQ about feature generation.
+>). Users can also refer to our [documentation](
+openfe-document.readthedocs.io/en/latest/>) for more advanced usage of OpenFE
+and FAQ about feature generation.
```

### Comparing `openfe-0.0.8/setup.py` & `openfe-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name="openfe",
-  version="0.0.8",
+  version="0.0.9",
   author="Tianping Zhang",
   author_email="ztp18@mails.tsinghua.edu.cn",
   description="OpenFE: automated feature generation beyond expert-level performance",
   long_description=long_description,
   long_description_content_type="text/markdown",
   python_requires='>=3.6',
   install_requires=[
```

