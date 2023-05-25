# Comparing `tmp/stockpy-learn-0.1.9.tar.gz` & `tmp/stockpy-learn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockpy-learn-0.1.9.tar", last modified: Sat Mar 25 11:36:42 2023, max compression
+gzip compressed data, was "stockpy-learn-0.2.1.tar", last modified: Thu May 25 17:54:23 2023, max compression
```

## Comparing `stockpy-learn-0.1.9.tar` & `stockpy-learn-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,47 @@
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     1076 2023-02-15 15:14:44.000000 stockpy-learn-0.1.9/LICENSE
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     7083 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/PKG-INFO
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     6457 2023-03-25 11:30:57.000000 stockpy-learn-0.1.9/README.md
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      140 2023-03-24 10:58:06.000000 stockpy-learn-0.1.9/pyproject.toml
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       38 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/setup.cfg
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     7360 2023-03-25 11:36:37.000000 stockpy-learn-0.1.9/setup.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       80 2023-03-24 12:12:27.000000 stockpy-learn-0.1.9/stockpy/__init__.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/neural_network/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      122 2023-03-24 12:12:44.000000 stockpy-learn-0.1.9/stockpy/neural_network/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    24214 2023-03-25 11:26:50.000000 stockpy-learn-0.1.9/stockpy/neural_network/_bigru.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21790 2023-03-25 11:26:55.000000 stockpy-learn-0.1.9/stockpy/neural_network/_bilstm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21831 2023-03-25 11:26:59.000000 stockpy-learn-0.1.9/stockpy/neural_network/_gru.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21892 2023-03-25 11:26:53.000000 stockpy-learn-0.1.9/stockpy/neural_network/_lstm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21005 2023-03-25 11:26:57.000000 stockpy-learn-0.1.9/stockpy/neural_network/_mlp.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/probabilistic/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       94 2023-03-24 12:13:22.000000 stockpy-learn-0.1.9/stockpy/probabilistic/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    24308 2023-03-25 11:02:45.000000 stockpy-learn-0.1.9/stockpy/probabilistic/_bnn.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    34370 2023-03-25 11:10:39.000000 stockpy-learn-0.1.9/stockpy/probabilistic/_dmm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    31088 2023-03-25 11:12:34.000000 stockpy-learn-0.1.9/stockpy/probabilistic/_ghmm.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/utils/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       67 2023-03-24 12:15:21.000000 stockpy-learn-0.1.9/stockpy/utils/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    11547 2023-03-24 15:37:54.000000 stockpy-learn-0.1.9/stockpy/utils/_dataset.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3090 2022-12-14 15:08:27.000000 stockpy-learn-0.1.9/stockpy/utils/_disk.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      607 2022-09-30 12:25:40.000000 stockpy-learn-0.1.9/stockpy/utils/_logconf.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     6018 2023-01-05 12:00:39.000000 stockpy-learn-0.1.9/stockpy/utils/_utils.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/stockpy/utils/prompt/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)        0 2022-12-29 19:04:34.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3664 2023-01-02 10:46:39.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/data.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3850 2023-01-05 16:33:37.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/ghmm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3570 2023-01-02 11:36:50.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/lstm.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/stockpy_learn.egg-info/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     7083 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/PKG-INFO
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      811 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/SOURCES.txt
--rw-rw-r--   0 silvio    (1000) silvio    (1000)        1 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/dependency_links.txt
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       43 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/requires.txt
--rw-rw-r--   0 silvio    (1000) silvio    (1000)        8 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/top_level.txt
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     1076 2023-02-15 15:14:44.000000 stockpy-learn-0.2.1/LICENSE
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    12031 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/PKG-INFO
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    11406 2023-05-18 09:39:54.000000 stockpy-learn-0.2.1/README.md
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      140 2023-03-24 10:58:06.000000 stockpy-learn-0.2.1/pyproject.toml
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)       38 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/setup.cfg
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     1141 2023-05-25 17:51:02.000000 stockpy-learn-0.2.1/setup.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      114 2023-05-19 10:46:51.000000 stockpy-learn-0.2.1/stockpy/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    19183 2023-05-25 17:35:18.000000 stockpy-learn-0.2.1/stockpy/base.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     1954 2023-05-19 10:48:32.000000 stockpy-learn-0.2.1/stockpy/config.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/metrics/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      115 2023-03-29 14:20:46.000000 stockpy-learn-0.2.1/stockpy/metrics/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     1002 2023-03-29 14:53:49.000000 stockpy-learn-0.2.1/stockpy/metrics/_base.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/neural_network/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      402 2023-05-25 14:11:06.000000 stockpy-learn-0.2.1/stockpy/neural_network/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    14969 2023-05-25 15:45:13.000000 stockpy-learn-0.2.1/stockpy/neural_network/_base.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7489 2023-05-25 15:37:19.000000 stockpy-learn-0.2.1/stockpy/neural_network/_bigru.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7594 2023-05-25 15:38:33.000000 stockpy-learn-0.2.1/stockpy/neural_network/_bilstm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7193 2023-05-25 15:39:34.000000 stockpy-learn-0.2.1/stockpy/neural_network/_cnn.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7102 2023-05-25 15:40:33.000000 stockpy-learn-0.2.1/stockpy/neural_network/_gru.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7545 2023-05-25 15:41:28.000000 stockpy-learn-0.2.1/stockpy/neural_network/_lstm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     5489 2023-05-25 16:29:55.000000 stockpy-learn-0.2.1/stockpy/neural_network/_mlp.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/preprocessing/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      303 2023-05-19 10:44:59.000000 stockpy-learn-0.2.1/stockpy/preprocessing/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     2310 2023-05-25 15:51:22.000000 stockpy-learn-0.2.1/stockpy/preprocessing/_base.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     9836 2023-05-25 17:14:46.000000 stockpy-learn-0.2.1/stockpy/preprocessing/_dataloader.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     5372 2023-05-25 17:12:59.000000 stockpy-learn-0.2.1/stockpy/preprocessing/_dataset.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    12265 2023-05-25 15:51:13.000000 stockpy-learn-0.2.1/stockpy/preprocessing/_scaler.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/probabilistic/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      201 2023-05-25 16:52:54.000000 stockpy-learn-0.2.1/stockpy/probabilistic/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    20973 2023-05-25 15:54:55.000000 stockpy-learn-0.2.1/stockpy/probabilistic/_base.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     9695 2023-05-25 16:48:01.000000 stockpy-learn-0.2.1/stockpy/probabilistic/_bcnn.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7674 2023-05-25 16:50:25.000000 stockpy-learn-0.2.1/stockpy/probabilistic/_bnn.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    10600 2023-05-25 16:48:11.000000 stockpy-learn-0.2.1/stockpy/probabilistic/_dmm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     8580 2023-05-25 16:48:17.000000 stockpy-learn-0.2.1/stockpy/probabilistic/_ghmm.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/probabilistic/utils/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      105 2023-05-12 15:18:42.000000 stockpy-learn-0.2.1/stockpy/probabilistic/utils/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7982 2023-05-12 14:37:44.000000 stockpy-learn-0.2.1/stockpy/probabilistic/utils/_hmm_utils.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy/utils/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)        0 2023-05-12 14:36:08.000000 stockpy-learn-0.2.1/stockpy/utils/__init__.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-05-25 17:54:23.643226 stockpy-learn-0.2.1/stockpy_learn.egg-info/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    12031 2023-05-25 17:54:23.000000 stockpy-learn-0.2.1/stockpy_learn.egg-info/PKG-INFO
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     1055 2023-05-25 17:54:23.000000 stockpy-learn-0.2.1/stockpy_learn.egg-info/SOURCES.txt
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)        1 2023-05-25 17:54:23.000000 stockpy-learn-0.2.1/stockpy_learn.egg-info/dependency_links.txt
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      155 2023-05-25 17:54:23.000000 stockpy-learn-0.2.1/stockpy_learn.egg-info/requires.txt
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)        8 2023-05-25 17:54:23.000000 stockpy-learn-0.2.1/stockpy_learn.egg-info/top_level.txt
```

### Comparing `stockpy-learn-0.1.9/LICENSE` & `stockpy-learn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.9/stockpy/neural_network/_bilstm.py` & `stockpy-learn-0.2.1/stockpy/probabilistic/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,622 +1,518 @@
-import datetime
-import hashlib
 import os
-import shutil
-import sys
 import glob
-
-import numpy as np
-import pandas as pd
-
 import torch
-import torch.nn as nn
-from torch.optim import SGD, Adam
-from torch.utils.data import DataLoader
-from torch.autograd import Variable
-import torch.optim.lr_scheduler as lr_scheduler
-
-from ..utils import StockDataset, normalize
-import pandas as pd
-import matplotlib.pyplot as plt
-from tqdm.auto import tqdm, trange
-
-# set style of graphs
-plt.style.use('ggplot')
-from pylab import rcParams
-plt.rcParams['figure.dpi'] = 100
+from pyro.nn import PyroModule
+from pyro.infer import Predictive
+import pyro.distributions as dist
+import torch.nn.functional as F
+
+import pyro
+from pyro.nn import PyroModule
+from pyro.infer import (
+    SVI,
+    Trace_ELBO,
+    TraceMeanField_ELBO
+)
+from pyro.optim import ClippedAdam
+from pyro.optim import PyroLRScheduler
+from torch.optim.lr_scheduler import StepLR
+from sklearn.metrics import f1_score
+from tqdm.auto import tqdm
+from abc import abstractmethod, ABCMeta
+from ..base import BaseEstimator
+from ..base import ClassifierMixin
+from ..base import RegressorMixin
+from ..config import Config as cfg
 
-# TODO Implement forecasting function and plotting
-# TODO Implement interface 
+class CombinedMeta(ABCMeta, type(PyroModule)):
+    pass
 
-class Net(nn.Module):
+class BaseProb(BaseEstimator, PyroModule, metaclass=CombinedMeta):
     """
-    A class representing a neural network model for time series prediction.
+    This is an abstract base class for all probabilistic models. It extends both the BaseEstimator and PyroModule classes to provide 
+    the basic functionalities required by any probabilistic model.
 
-    Parameters:
-        input_size (int): the number of input features
-        hidden_size (int): the number of hidden units in the GRU layer
-        num_layers (int): the number of GRU layers
-        output_dim (int): the number of output units
+    Methods:
+        _initComponent():
+            Initializes the model, optimizer, and scheduler.
+        _initOptimizer() -> torch.optim.Optimizer:
+            Initializes the optimizer used to train the model.
+        _initScheduler() -> torch.optim.lr_scheduler.StepLR:
+            Initializes a learning rate scheduler to control the learning rate during training.
+        _initSVI() -> pyro.infer.svi.SVI:
+            Initializes a Stochastic Variational Inference (SVI) instance to optimize the model and guide.
+        _log_build_file_path():
+            Constructs the configuration for the file path for logging.
+        _log_model_state():
+            Retrieves the state of the model for logging purposes.
     """
-    def __init__(self, 
-                input_size=4,  
-                hidden_size=32, 
-                num_layers=2, 
-                output_dim=1
-                ):
-
-        super().__init__()
-        self.input_size = input_size # this is the number of features
-        self.hidden_size = hidden_size
-        self.num_layers = num_layers
-
-        self.lstm = nn.LSTM(input_size, 
-                            hidden_size, 
-                            num_layers, 
-                            bidirectional=True,
-                            batch_first=True
-                            )
-        self.fc = nn.Linear(hidden_size*2, output_dim)
-        # self.dropout = nn.Dropout(dropout)
-        self.relu = nn.ReLU()
 
-    def forward(self, x):
+    @abstractmethod
+    def __init__(self, **kwargs):
         """
-        Defines the forward pass of the neural network.
+        Initializes the probabilistic model.
+        This method is abstract and must be overridden in subclasses.
 
         Parameters:
-            x (torch.Tensor): the input tensor
+            kwargs (dict): A dictionary of keyword arguments.
+        """
 
-        Returns:
-            out (torch.Tensor): the output tensor
+        PyroModule.__init__(self)
+        BaseEstimator.__init__(self, **kwargs)
+
+    def _initComponent(self):
+        """
+        Initializes the model, optimizer, and scheduler.
         """
-        
-        batch_size = x.size(0)
-        h0 = Variable(torch.zeros(self.num_layers*2, batch_size, self.hidden_size))
-        c0 = Variable(torch.zeros(self.num_layers*2, batch_size, self.hidden_size))
-        
-        out, _ = self.lstm(x, (h0, c0))
-        out = self.fc(out[:, -1, :]) #Final Output
-       
-        out = out.view(-1,1)
-
-        return out
-
-class BiLSTM():
-
-    def __init__(self,
-                input_size=4,
-                hidden_size=32, 
-                num_layers=2,
-                output_dim=1,
-                pretrained=False
-                ):
-        
-        self._input_size = input_size
-        self._hidden_size = hidden_size
-        self._num_layers = num_layers
-        self._pretrained = pretrained
-        self._output_dim = output_dim
-        self.use_cuda = torch.cuda.is_available()
-  
-        self._initModel()
-        self.name = "bidirectional LSTM neural network"
 
-    def _initOptimizer(self):
+        self.optimizer = self._initOptimizer()
+        # self._initScheduler()
+        self.svi = self._initSVI()
+
+    def _initOptimizer(self) -> torch.optim.Optimizer:
         """
-        Initializes the optimizer for the neural network model.
-        
+        Initializes the optimizer used to train the model.
+
         Returns:
-            optimizer (torch.optim.Adam): the Adam optimizer for the model
+            torch.optim.Optimizer: The optimizer instance used to train the model.
         """
-        return torch.optim.Adam(self._model.parameters(), lr=1e-3)
-        
-    def _initTrainDl(self, 
-                     x_train, 
-                     batch_size, 
-                     num_workers, 
-                     sequence_length
-                     ):
-        """
-        Initializes the training data loader.
 
-        Parameters:
-            x_train (numpy.ndarray or pandas dataset): the training dataset
-            batch_size (int): the batch size to use for training
-            num_workers (int): the number of workers to use for data loading
-            sequence_length (int): the length of the input sequence
+        adam_params = {"lr": cfg.training.lr, 
+                            "betas": cfg.training.betas,
+                            "lrd": cfg.training.lrd,
+                            "weight_decay": cfg.training.weight_decay
+                        }
+        return ClippedAdam(adam_params)
+    
+    def _initScheduler(self) -> torch.optim.lr_scheduler.StepLR:
+        """
+        Initializes a learning rate scheduler to control the learning rate during training.
 
         Returns:
-            train_dl (torch.utils.data.DataLoader): the training data loader
+            torch.optim.lr_scheduler.StepLR: The learning rate scheduler used to control the learning rate during training.
         """
-        train_dl = StockDataset(x_train, sequence_length=sequence_length)
 
-        train_dl = DataLoader(train_dl, 
-                            batch_size=batch_size * (torch.cuda.device_count() \
-                                                                   if self.use_cuda else 1),  
-                            num_workers=num_workers,
-                            pin_memory=self.use_cuda,
-                            shuffle=True
-                            )
+        step_lr = StepLR(self.optimizer, step_size=cfg.training.step_size, gamma=cfg.training.gamma)
+        scheduler = PyroLRScheduler(step_lr, self.optimizer)
+        return scheduler
+    
+    @abstractmethod
+    def _initSVI(self) -> pyro.infer.svi.SVI:
+        """
+        Initializes a Stochastic Variational Inference (SVI) instance to optimize the model and guide.
 
-        self._batch_size = batch_size
-        self._num_workers = num_workers
-        self._sequence_length = sequence_length
+        Returns:
+            pyro.infer.svi.SVI: The SVI instance used to optimize the model and guide.
+        """
 
-        return train_dl
+        pass
 
-    def _initValDl(self, 
-                   x_test
-                   ):
+    def _log_build_file_path(self):
         """
-        Initializes the validation data loader.
-
-        Parameters:
-            x_test (numpy.ndarray or pandas dataset): the validation dataset
+        Constructs the configuration for the file path for logging.
 
         Returns:
-            val_dl (torch.utils.data.DataLoader): the validation data loader
+            dict: The configuration dictionary for the file path for logging.
         """
-        val_dl = StockDataset(x_test, 
-                                sequence_length=self._sequence_length
-                                )
-
-        val_dl = DataLoader(val_dl, 
-                            batch_size=self._batch_size * (torch.cuda.device_count() \
-                                                    if self.use_cuda else 1), 
-                            num_workers=self._num_workers,
-                            pin_memory=self.use_cuda,
-                            shuffle=False
-                            )
-        
-        return val_dl
+
+        file_path_configs = {
+            "file_format": self.name + '_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}.state',
+            "args": (self.input_size, cfg.prob.hidden_size, self.output_size,
+                    cfg.prob.rnn_dim, cfg.prob.z_dim, cfg.prob.emission_dim,
+                    cfg.prob.transition_dim, cfg.prob.variance, cfg.comm.dropout, 
+                    cfg.training.lr, cfg.training.weight_decay)
+        }
+
+        return file_path_configs
     
-    def _initTrainValData(self, 
-                          x_train,
-                          validation_sequence,
-                          batch_size,
-                          num_workers,
-                          sequence_length
-                          ):
+    def _log_model_state(self):
         """
-        Initializes the training and validation data loaders.
-
-        Parameters:
-            x_train (numpy.ndarray): the training dataset
-            validation_sequence (int): the number of time steps to reserve for validation during training
-            batch_size (int): the batch size to use during training
-            num_workers (int): the number of workers to use for data loading
-            sequence_length (int): the length of the input sequence
+        Retrieves the state of the model for logging purposes.
 
         Returns:
-            train_dl (torch.utils.data.DataLoader): the training data loader
-            val_dl (torch.utils.data.DataLoader): the validation data loader
+            dict: The dictionary containing the state of the model for logging.
         """
 
-        scaler = normalize(x_train)
-
-        x_train = scaler.fit_transform()
-        val_dl = x_train[-validation_sequence:]
-        x_train = x_train[:len(x_train)-len(val_dl)]
-
-        train_dl = self._initTrainDl(x_train, 
-                                        batch_size=batch_size,
-                                        num_workers=num_workers,
-                                        sequence_length=sequence_length
-                                        )
+        state = {
+            'model_state': self.state_dict(),
+            'model_name': type(self).__name__,
+            'optimizer_state': self.optimizer.get_state(),
+            'optimizer_name': type(self.optimizer).__name__,
+        }
 
-        val_dl = self._initValDl(val_dl)
+        return state
+    
+class ClassifierProb(BaseProb, ClassifierMixin, metaclass=ABCMeta):
+    """
+    This is an abstract class for a probabilistic classifier model. It inherits from the `BaseProb` class, 
+    the `ClassifierMixin` class, and uses the `ABCMeta` metaclass.
 
-        return train_dl, val_dl
+    Methods:
+        __init__(self, **kwargs):
+            Initializes the classifier by calling the super() function to inherit methods and properties 
+            from the parent classes.
+    
+        _initSVI(self):
+            This is an abstract method and needs to be implemented in any child class. This method is 
+            responsible for initializing the Stochastic Variational Inference (SVI) instance used for 
+            optimization.
+
+        _doTraining(self, train_dl: torch.utils.data.DataLoader) -> float:
+            Trains the model on the training data for the specified number of epochs. The method computes 
+            the total training loss, and the F1-score using the true and predicted labels. The model is 
+            set to training mode and the SVI optimizer is used for training.
+
+        _doValidation(self, val_dl: torch.utils.data.DataLoader) -> float:
+            Validates the model on the validation data. The method computes the total validation loss, and 
+            the F1-score using the true and predicted labels. The model is set to evaluation mode and the 
+            SVI optimizer is used for validation.
+    """
 
-    def fit(self, 
-            x_train,
-            epochs=10,
-            sequence_length=30,
-            batch_size=8, 
-            num_workers=4,
-            validation_sequence=30, 
-            validation_cadence=5,
-            patience=5
-            ):
+    @abstractmethod
+    def __init__(self, **kwargs):
         """
-        Fits the neural network model to a given dataset.
+        Initializes the classifier by calling the super() function to inherit methods and properties 
+        from the parent classes.
 
         Parameters:
-            x_train (numpy.ndarray): the training dataset
-            epochs (int): the number of epochs to train the model for
-            sequence_length (int): the length of the input sequence
-            batch_size (int): the batch size to use during training
-            num_workers (int): the number of workers to use for data loading
-            validation_sequence (int): the number of time steps to reserve for validation during training
-            validation_cadence (int): how often to run validation during training
-            patience (int): how many epochs to wait for improvement in validation loss before stopping early
-
-        Returns:
-            None
-        """
-
-        train_dl, val_dl = self._initTrainValData(x_train,
-                                                  validation_sequence,
-                                                  batch_size,
-                                                  num_workers,
-                                                  sequence_length
-                                                  )
-        
-        self._train(epochs,
-                    train_dl,
-                    val_dl,
-                    validation_cadence,
-                    patience
-                    )
-        
-    def _train(self, 
-               epochs,
-               train_dl,
-               val_dl,
-               validation_cadence,
-               patience
-               ):
+            kwargs (dict): A dictionary of keyword arguments.
         """
-        Trains the neural network model on the training dataset.
+        super().__init__(**kwargs)
 
-        Parameters:
-            epochs (int): the number of epochs to train the model for
-            train_dl (torch.utils.data.DataLoader): the training data loader
-            val_dl (torch.utils.data.DataLoader): the validation data loader
-            validation_cadence (int): how often to run validation during training
-            patience (int): how many epochs to wait for improvement in validation loss before stopping early
-
-        Returns:
-            None
+    @abstractmethod
+    def _initSVI(self):
         """
-        
-        self._model.train()
-        best_loss = float('inf')
-        counter = 0
-
-        for epoch_ndx in tqdm((range(1, epochs + 1)), position=0, leave=True):
-            epoch_loss = 0.0
-            for x_batch, y_batch in train_dl:   
-                self._optimizer.zero_grad()  
-                loss = self._computeBatchLoss(x_batch, y_batch)
-                loss.backward()     
-                self._optimizer.step()
-                epoch_loss += loss
-
-            if epoch_ndx % validation_cadence != 0:                
-                print(f"Epoch {epoch_ndx}, Loss: {epoch_loss / len(train_dl)}")
-
-            else:
-                total_loss = self._doValidation(val_dl)
-
-                print(f"Epoch {epoch_ndx}, Val Loss {total_loss}")
-
-                # Early stopping
-                stop, best_loss, counter = self._earlyStopping(total_loss, 
-                                                               best_loss, 
-                                                               counter, 
-                                                               patience,
-                                                               epoch_ndx
-                                                               )
-                if stop:
-                    break
-
-    def _computeBatchLoss(self, 
-                         x_batch, 
-                         y_batch
-                         ):     
+        This is an abstract method and needs to be implemented in any child class. This method is 
+        responsible for initializing the Stochastic Variational Inference (SVI) instance used for 
+        optimization.
+        """
+        pass
+    
+    def _doTraining(self, train_dl: torch.utils.data.DataLoader) -> float:
         """
-        Computes the loss for a given batch of data.
+        Trains the model on the training data for the specified number of epochs.
 
         Parameters:
-            x_batch (torch.Tensor): the input data
-            y_batch (torch.Tensor): the target data
+            train_dl (torch.utils.data.DataLoader): The training data.
 
         Returns:
-            torch.Tensor: the loss for the given batch of data
-        """  
+            float: The training loss.
+            float: The F1-score of the training data.
+            list: The true labels of the training data.
+            list: The predicted labels of the training data.
+        """
+        # Initialize variables for tracking loss, correct predictions, total samples, and labels
+        train_loss = 0.0
+        correct = 0
+        total = 0
+        true_labels = []
+        pred_labels = []
+
+        # Switch the model to training mode. This has any effect only on certain modules like Dropout or BatchNorm.
+        self.train()
 
-        output = self._model(x_batch)
-        loss_function = nn.MSELoss()
-        loss = loss_function(output, y_batch)
+        # Iterate over the training data loader
+        for x_batch, y_batch in train_dl:
+            # The Stochastic Variational Inference (SVI) optimizer takes a step using the data and labels, and the loss is computed
+            loss = self.svi.step(x_batch, y_batch)
+            # Add the loss to the total training loss
+            train_loss += loss
+         
+            # Make predictions using the current batch of data
+            output = self.forward(x_batch)
+            # Get the predicted class by finding the maximum value of the output
+            _, predicted = torch.max(output.data, 1)
+            # Add the number of data points in the batch to the total number of data points
+            total += y_batch.size(0)
+            # Add the number of correct predictions in the batch to the total number of correct predictions
+            correct += (predicted == y_batch).sum().item()
 
-        return loss.mean() 
+            # Extend the list of true labels and predicted labels
+            true_labels.extend(y_batch.tolist())
+            pred_labels.extend(predicted.tolist())
 
-    def _doValidation(self, val_dl):
+        # Compute the average training loss
+        train_loss /= len(train_dl)
+        # Compute the weighted F1-score, a measure of the model's performance
+        train_f1 = f1_score(true_labels, pred_labels, average='weighted') * 100
+
+        # Return the training loss, F1-score, true labels, and predicted labels
+        return train_loss, train_f1, true_labels, pred_labels
+
+    def _doValidation(self, val_dl: torch.utils.data.DataLoader) -> float:
         """
-        Performs validation on a given validation data loader.
+        Validates the model on the validation data.
 
         Parameters:
-            val_dl (torch.utils.data.DataLoader): the validation data loader
+            val_dl (torch.utils.data.DataLoader): The validation data.
 
         Returns:
-            float: the total loss over the validation set
+            float: The validation loss.
+            float: The F1-score of the validation data.
+            list: The true labels of the validation data.
+            list: The predicted labels of the validation data.
         """
 
-        total_loss = 0
-        self._model.eval()
-        with torch.no_grad():  
+        # Initialize variables for tracking loss, correct predictions, total samples, and labels
+        val_loss = 0.0
+        correct = 0
+        total = 0
+        true_labels = []
+        pred_labels = []
+
+        # Set the model to evaluation mode (disables gradient computation and dropout)
+        self.eval()
+        # Disable gradient tracking for efficiency
+        with torch.no_grad():
+            # Iterate over the validation data loader
             for x_batch, y_batch in val_dl:
-                loss_var = self._computeBatchLoss(x_batch, y_batch)
-                total_loss += loss_var / val_dl.batch_size
+                # Compute the loss for the batch
+                loss = self.svi.evaluate_loss(x_batch, y_batch)
+                val_loss += loss
+
+                # Forward pass to obtain model predictions
+                output = self.forward(x_batch)
+                # Get the predicted labels by selecting the maximum value along the second dimension
+                _, predicted = torch.max(output.data, 1)
+                # Update the count of total samples and correct predictions
+                total += y_batch.size(0)
+                correct += (predicted == y_batch).sum().item()
+
+                # Extend the true and predicted labels lists
+                true_labels.extend(y_batch.tolist())
+                pred_labels.extend(predicted.tolist())
+
+        # Compute the average validation loss
+        val_loss /= len(val_dl)
+        # Calculate the weighted F1 score for the true and predicted labels
+        val_f1 = f1_score(true_labels, pred_labels, average='weighted') * 100
+
+        # Return the validation loss, F1 score, true labels, and predicted labels
+        return val_loss, val_f1, true_labels, pred_labels
 
-        self._model.train()
+class RegressorProb(BaseProb, RegressorMixin, metaclass=ABCMeta):
+    """
+    This is an abstract class for a probabilistic regression model. It inherits from the `BaseProb` and 
+    `RegressorMixin` classes, and uses the `ABCMeta` metaclass.
 
-        return total_loss 
+    Methods:
+        __init__(self, **kwargs):
+            Initializes the regressor by calling the super() function to inherit methods and properties 
+            from the parent classes.
     
-    def _earlyStopping(self,
-                       total_loss,
-                       best_loss,
-                       counter,
-                       patience,
-                       epoch_ndx
-                       ):
+        _initSVI(self):
+            This is an abstract method and needs to be implemented in any child class. This method is 
+            responsible for initializing the Stochastic Variational Inference (SVI) instance used for 
+            optimization.
+
+        _doTraining(self, train_dl: torch.utils.data.DataLoader) -> float:
+            Trains the model on the training data. The method computes the total training loss. The model 
+            is set to training mode and the SVI optimizer is used for training.
+
+        _doValidation(self, val_dl: torch.utils.data.DataLoader) -> float:
+            Validates the model on the validation data. The method computes the total validation loss. 
+            The model is set to evaluation mode and the SVI optimizer is used for validation.
+        
+        _predictNN(self, test_dl: torch.utils.data.DataLoader) -> torch.Tensor:
+            Makes a prediction using a neural network model. The data is passed through the model and the 
+            output is returned.
+        
+        _predictHMM(self, test_dl: torch.utils.data.DataLoader) -> torch.Tensor:
+            Makes a prediction using a Hidden Markov Model. The data is passed through the model and the 
+            output is returned.
+
+        _predict(self, test_dl: torch.utils.data.DataLoader) -> torch.Tensor:
+            This is an abstract method and needs to be implemented in any child class. This method is 
+            responsible for making predictions.
+    """
+
+    @abstractmethod
+    def __init__(self, **kwargs):
         """
-        Implements early stopping during training.
+        Initializes the regressor by calling the super() function to inherit methods and properties 
+        from the parent classes.
 
         Parameters:
-            total_loss (float): the total validation loss
-            best_loss (float): the best validation loss seen so far
-            counter (int): the number of epochs without improvement in validation loss
-            patience (int): how many epochs to wait for improvement in validation loss before stopping early
-            epoch_ndx (int): the current epoch number
-
-        Returns:
-            tuple: a tuple containing a bool indicating whether to stop early, the best loss seen so far, and the current counter value
-        """
-
-        if total_loss < best_loss:
-            best_loss = total_loss
-            best_epoch_ndx = epoch_ndx
-            self._saveModel('bilstm', best_epoch_ndx)
-            counter = 0
-        else:
-            counter += 1
-
-        if counter >= patience:
-            print(f"No improvement after {patience} epochs. Stopping early.")
-            return True, best_loss, counter
-        else:
-            return False, best_loss, counter
-
-    def predict(self, 
-                x_test
-                ):
+            kwargs (dict): A dictionary of keyword arguments.
+        """
+        super().__init__(**kwargs)
+
+    @abstractmethod
+    def _initSVI(self):
+        """
+        This is an abstract method and needs to be implemented in any child class. This method is 
+        responsible for initializing the Stochastic Variational Inference (SVI) instance used for 
+        optimization.
+        """
+        pass
+    
+    def _doTraining(self, train_dl: torch.utils.data.DataLoader) -> float:
         """
-        Make predictions on a given test set.
+        Trains the model on the training data for the specified number of epochs.
 
         Parameters:
-            x_test (np.ndarray): the test set to make predictions on
+            train_dl (torch.utils.data.DataLoader): The training data.
 
         Returns:
-            np.ndarray: the predicted values for the given test set
+            float: The training loss.
+            None: Additional metrics (not used in regression).
+            None: Additional metrics (not used in regression).
+            None: Additional metrics (not used in regression).
         """
+        # Initialize the variable for tracking the training loss
+        train_loss = 0.0
+        # Set the model to training mode (enables gradient computation and dropout)
+        self.train()
+        # Iterate over the training data loader
+        for x_batch, y_batch in train_dl:
+            # Move the batch to the appropriate device
+            x_batch = x_batch.to(cfg.training.device)
+            y_batch = y_batch.to(cfg.training.device)
 
-        scaler = normalize(x_test)
-        x_test = scaler.fit_transform()
-        val_dl = self._initValDl(x_test)
-        batch_iter = enumerate(val_dl)
-
-        output = torch.tensor([])
-        self._model.eval()
-        
-        with torch.no_grad():
-            for _, batch_tup in batch_iter:
-                y_star = self._model(batch_tup[0])
-                output = torch.cat((output, y_star), 0)
+            # Compute the loss and perform a single optimization step
+            loss = self.svi.step(x_batch, y_batch)
+            # Accumulate the training loss
+            train_loss += loss
 
-        output = output.detach().numpy() * scaler.std() + scaler.mean()
-                    
-        return output
+        # Compute the average training loss
+        train_loss /= len(train_dl)
+        # Return the training loss and None values for additional metrics
+        return train_loss, None, None, None
 
-    def _initModel(self):
+    def _doValidation(self, val_dl: torch.utils.data.DataLoader) -> float:
         """
-        Initializes the neural network model.
+        Validates the model on the validation data.
+
+        Parameters:
+            val_dl (torch.utils.data.DataLoader): The validation data.
 
         Returns:
-            None
+            float: The validation loss.
+            None: Additional metrics (not used in regression).
+            None: Additional metrics (not used in regression).
+            None: Additional metrics (not used in regression).
         """
+        # Initialize the variable for tracking the validation loss
+        val_loss = 0.0
+        # Set the model to evaluation mode (disables gradient computation and dropout)
+        self.eval()
+        # Disable gradient tracking for efficiency
+        with torch.no_grad():
+            # Iterate over the validation data loader
+            for x_batch, y_batch in val_dl:
+                # Move the batch to the appropriate device
+                x_batch = x_batch.to(cfg.training.device)
+                y_batch = y_batch.to(cfg.training.device)
+
+                # Compute the loss for the batch
+                loss = self.svi.evaluate_loss(x_batch, y_batch)
+                # Accumulate the validation loss
+                val_loss += loss
 
-        model = Net(input_size=self._input_size,
-                    hidden_size=self._hidden_size,
-                    output_dim=self._output_dim
-                    )
-        
-        if self._pretrained:
-            path = self._initModelPath('bilstm')
-            model_dict = torch.load(path)
-            model.load_state_dict(model_dict['model_state'])
-
-        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+        # Compute the average validation loss
+        val_loss /= len(val_dl)
 
-        if self.use_cuda:
-            if torch.cuda.device_count() > 1:
-                model = nn.DataParallel(model)
-            self._model = model.to(device)
+        # Return the validation loss and None values for additional metrics
+        return val_loss, None, None, None
+    
+    def _predictNN(self, test_dl: torch.utils.data.DataLoader) -> torch.Tensor:
+        """
+        Makes predictions on the test data using the model's forward method and Pyro's Predictive class. 
+        This method is suitable for Neural Network models.
 
-        self._model = model
+        Parameters:
+            test_dl (torch.utils.data.DataLoader): DataLoader object that contains the test data in batches.
 
-        self._optimizer = self._initOptimizer()
+        Returns:
+            torch.Tensor: Tensor containing the model's predictions.
+        """
+        # Initializes an empty tensor to store the output
+        output = torch.tensor([])
 
-    def _saveModel(self, type_str, epoch_ndx):
+        # Iterates over the test data loader
+        for x_batch in test_dl:
+            # Moves the batch data to the specified device (CPU or GPU)
+            x_batch = x_batch.to(cfg.training.device)
+            
+            # Initializes a Predictive instance using the model's forward method, the guide, 
+            # the number of samples (equal to the batch size), and the sites to return
+            predictive = Predictive(model=self.forward, 
+                                    guide=self.guide, 
+                                    num_samples=cfg.training.batch_size,
+                                    return_sites=("linear.weight", "obs", "_RETURN")
+                                    )
+            
+            # Makes predictions on the batch data
+            samples = predictive(x_batch)
+            
+            # Initializes a dictionary to store the statistics of the sites
+            site_stats = {}
+            for k, v in samples.items():
+                # Stores the mean of the samples for each site
+                site_stats[k] = {"mean": torch.mean(v, 0)}
+
+            # Gets the mean prediction of the '_RETURN' site
+            y_pred = site_stats['_RETURN']['mean']
+            
+            # Concatenates the prediction to the output tensor
+            output = torch.cat((output, y_pred), 0)
+            
+        return output
+    
+    def _predictHMM(self, test_dl: torch.utils.data.DataLoader) -> torch.Tensor:
         """
-        Saves the model to disk.
+        Makes predictions on the test data using the model's guide and emitter methods. 
+        This method is suitable for Hidden Markov Models.
 
         Parameters:
-            type_str (str): a string indicating the type of model
-            epoch_ndx (int): the epoch index
+            test_dl (torch.utils.data.DataLoader): DataLoader object that contains the test data in batches.
 
         Returns:
-            None
-        """
+            torch.Tensor: Tensor containing the model's predictions.
+        """
+        # Creates a list to store the predicted y values
+        output = []
+
+        # Iterates over the test data in batches
+        for x_batch in test_dl:
+            # Makes predictions for the current batch
+            with torch.no_grad():
+                # Computes the location and scale parameters of the latent variable distribution at each time step
+                *_, z_loc, z_scale = self.guide(x_batch)
+                
+                # Applies the softplus function to the scale parameter to ensure its positivity
+                z_scale = F.softplus(z_scale)
+                
+                # Samples from the normal distribution specified by the location and scale parameters
+                z_t = dist.Normal(z_loc, z_scale).rsample()
+                
+                # Passes the latent variable and the data through the emitter to obtain the mean of the emission distribution at each time step
+                mean_t, _ = self.emitter(z_t, x_batch)
+                    
+                # Gets the mean of the emission distribution at the last time step
+                mean_last = mean_t[:, -1, :]
 
-        file_path = os.path.join(
-            '..',
-            '..',
-            'models',
-            'BiLSTM',
-            '{}_{}_{}_{}.state'.format(
-                    type_str,
-                    self._input_size,
-                    self._hidden_size,
-                    self._num_layers,
-            )
-        )
-
-        os.makedirs(os.path.dirname(file_path), mode=0o755, exist_ok=True)
-
-        model = self._model
-        if isinstance(model, torch.nn.DataParallel):
-            model = model.module
+            # Adds the predicted y values for the current batch to the list
+            output.append(mean_last)
 
-        state = {
-            'model_state': model.state_dict(),
-            'model_name': type(model).__name__,
-            'optimizer_state': self._optimizer.state_dict(),
-            'optimizer_name': type(self._optimizer).__name__,
-            'epoch': epoch_ndx
-        }
-
-        torch.save(state, file_path)
+        # Concatenates the predicted y values for all batches into a single tensor
+        output = torch.cat(output)
 
-        with open(file_path, 'rb') as f:
-            hashlib.sha1(f.read()).hexdigest()
+        # Reshapes the tensor to get an array of shape [number_of_samples, 1]
+        output = output.reshape(-1, 1)
 
-    def _initModelPath(self, type_str):
+        # Returns the predicted y values as a tensor
+        return output
+    
+    @abstractmethod
+    def _predict(self, test_dl: torch.utils.data.DataLoader) -> torch.Tensor:
         """
-        Initializes the model path.
+        Makes predictions on the test data.
 
         Parameters:
-            type_str (str): a string indicating the type of model
+            test_dl (torch.utils.data.DataLoader): The test data.
 
         Returns:
-            str: the path to the initialized model
+            torch.Tensor: The predicted output.
         """
-
-        model_dir = '../../models/BiLSTM'
-        if not os.path.exists(model_dir):
-            os.makedirs(model_dir)
-
-        local_path = os.path.join(
-            '..', 
-            '..', 
-            'models', 
-            'BiLSTM', 
-            type_str + '_{}_{}_{}.state'.format(self._input_size,
-                                                self._hidden_size,
-                                                self._num_layers
-                                                ),
-            )
-
-        file_list = glob.glob(local_path)
-        
-        if not file_list:
-            raise ValueError(f"No matching model found in {local_path} for the given parameters.")
-        
-        # Return the most recent matching file
-        return file_list[0]
-
-    def trading(self, 
-                predicted, 
-                real, 
-                shares=0, 
-                stop_loss=0.0, 
-                initial_balance=10000, 
-                threshold=0.0, 
-                plot=True
-                ):
-        """
-        Simulate trading based on predicted and real stock prices.
-
-        Args:
-            predicted (np.ndarray): Array of predicted stock prices.
-            real (np.ndarray): Array of real stock prices.
-            shares (int): Number of shares held at the start of the simulation. Default is 0.
-            stop_loss (float): Stop loss percentage. If the stock price falls below this percentage of the initial price,
-                            all shares will be sold. Default is 0.0.
-            initial_balance (float): Initial balance to start trading with. Default is 10000.
-            threshold (float): Buy/Sell threshold. Default is 0.0.
-            plot (bool): Whether to plot the trading simulation or not. Default is True.
-
-        Returns:
-            tuple: A tuple containing balance (float), total profit/loss (float), percentage increase (float), 
-            and transactions (list of tuples). The transactions are of the form (timestamp, price, action, shares, balance).
-        """
-
-        assert predicted.shape == real.shape, "predicted and real must have the same shape"
-        assert shares >= 0, "shares cannot be negative"
-        assert initial_balance >= 0, "initial_balance cannot be negative"
-        assert 0 <= stop_loss <= 1, "stop_loss must be between 0 and 1"
-
-        transactions = []
-        balance = initial_balance
-        num_shares = shares
-        total_profit_loss = 0
-
-        if num_shares == 0 and balance >= real[0]:
-            num_shares = int(balance / real[0])
-            balance -= num_shares * real[0]
-            transactions.append((0, real[0], "BUY", num_shares, balance))
-
-        for i in range(1, len(predicted)):
-            if predicted[i] > real[i-1] * (1 + threshold):
-                if num_shares == 0:
-                    num_shares = int(balance / real[i])
-                    balance -= num_shares * real[i]
-                    transactions.append((i, real[i], "BUY", num_shares, balance))
-                elif num_shares > 0:
-                    balance += num_shares * real[i]
-                    total_profit_loss += (real[i] - real[i-1]) * num_shares
-                    transactions.append((i, real[i], "SELL", num_shares, balance))
-                    num_shares = 0
-            elif predicted[i] < real[i-1] * (1 - threshold):
-                if num_shares == 0:
-                    continue
-                elif num_shares > 0:
-                    balance += num_shares * real[i]
-                    total_profit_loss += (real[i] - real[i-1]) * num_shares
-                    transactions.append((i, real[i], "SELL", num_shares, balance))
-                    num_shares = 0
-
-            if stop_loss > 0 and num_shares > 0 and real[i] < (real[0] - stop_loss):
-                balance += num_shares * real[i]
-                total_profit_loss += (real[i] - real[i-1]) * num_shares
-                transactions.append((i, real[i], "SELL", num_shares, balance))
-                num_shares = 0
-
-        if num_shares > 0:
-            balance += num_shares * real[-1]
-            total_profit_loss += (real[-1] - real[-2]) * num_shares
-            transactions.append((len(predicted)-1, real[-1], "SELL", num_shares, balance))
-            num_shares = 0
-
-        percentage_increase = (balance - initial_balance) / initial_balance * 100
-
-        if plot:
-            fig, ax = plt.subplots(figsize=(12, 6))
-            ax.plot(real, label='Real')
-            ax.plot(predicted, label='Predicted')
-            buy_scatter = ax.scatter([], [], c='g', marker='^', s=100)
-            sell_scatter = ax.scatter([], [], c='r', marker='v', s=100)
-            for transaction in transactions:
-                timestamp, price, action, shares, balance = transaction
-                if action == 'BUY':
-                    buy_scatter = ax.scatter(timestamp, predicted[timestamp], c='g', marker='^', s=100)
-                elif action == 'SELL':
-                    sell_scatter = ax.scatter(timestamp, predicted[timestamp], c='r', marker='v', s=100)
-            ax.set_xlabel('Time')
-            ax.set_ylabel('Price')
-            ax.set_title('Trading Simulation')
-            fig.autofmt_xdate()
-            ax.legend((ax.plot([], label='Real')[0], ax.plot([], label='Predicted')[0], buy_scatter, sell_scatter),
-                    ('Real', 'Predicted', 'Buy', 'Sell'))
-            ax.text(0.05, 0.05, 
-                    'Percentage increase: ${:.2f}%'.format(percentage_increase[0]), 
-                    ha='left', va='center',
-                      transform=ax.transAxes, 
-                      bbox=dict(facecolor='white', alpha=0.5)
-                      )
-            plt.show()
-        
-        return balance, total_profit_loss, percentage_increase, transactions
+        pass
```

### Comparing `stockpy-learn-0.1.9/stockpy_learn.egg-info/SOURCES.txt` & `stockpy-learn-0.2.1/stockpy_learn.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 stockpy/__init__.py
+stockpy/base.py
+stockpy/config.py
+stockpy/metrics/__init__.py
+stockpy/metrics/_base.py
 stockpy/neural_network/__init__.py
+stockpy/neural_network/_base.py
 stockpy/neural_network/_bigru.py
 stockpy/neural_network/_bilstm.py
+stockpy/neural_network/_cnn.py
 stockpy/neural_network/_gru.py
 stockpy/neural_network/_lstm.py
 stockpy/neural_network/_mlp.py
+stockpy/preprocessing/__init__.py
+stockpy/preprocessing/_base.py
+stockpy/preprocessing/_dataloader.py
+stockpy/preprocessing/_dataset.py
+stockpy/preprocessing/_scaler.py
 stockpy/probabilistic/__init__.py
+stockpy/probabilistic/_base.py
+stockpy/probabilistic/_bcnn.py
 stockpy/probabilistic/_bnn.py
 stockpy/probabilistic/_dmm.py
 stockpy/probabilistic/_ghmm.py
+stockpy/probabilistic/utils/__init__.py
+stockpy/probabilistic/utils/_hmm_utils.py
 stockpy/utils/__init__.py
-stockpy/utils/_dataset.py
-stockpy/utils/_disk.py
-stockpy/utils/_logconf.py
-stockpy/utils/_utils.py
-stockpy/utils/prompt/__init__.py
-stockpy/utils/prompt/data.py
-stockpy/utils/prompt/ghmm.py
-stockpy/utils/prompt/lstm.py
 stockpy_learn.egg-info/PKG-INFO
 stockpy_learn.egg-info/SOURCES.txt
 stockpy_learn.egg-info/dependency_links.txt
 stockpy_learn.egg-info/requires.txt
 stockpy_learn.egg-info/top_level.txt
```

