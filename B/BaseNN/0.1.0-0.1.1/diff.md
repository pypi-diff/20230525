# Comparing `tmp/BaseNN-0.1.0.tar.gz` & `tmp/BaseNN-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.0.tar", last modified: Wed May 24 09:09:25 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.1.tar", last modified: Thu May 25 08:16:34 2023, max compression
```

## Comparing `BaseNN-0.1.0.tar` & `BaseNN-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    37357 2023-05-24 07:46:21.000000 BaseNN-0.1.0/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.0/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-24 08:46:31.000000 BaseNN-0.1.0/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.0/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.0/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.0/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-24 09:08:59.000000 BaseNN-0.1.0/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.0/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-24 09:09:25.000000 BaseNN-0.1.0/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-24 09:09:25.000000 BaseNN-0.1.0/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-24 09:08:45.000000 BaseNN-0.1.0/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    38285 2023-05-25 08:15:44.000000 BaseNN-0.1.1/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.1/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-25 07:54:48.000000 BaseNN-0.1.1/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.1/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.1/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.1/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-25 08:16:14.000000 BaseNN-0.1.1/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.1/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:16:34.000000 BaseNN-0.1.1/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-25 08:16:34.000000 BaseNN-0.1.1/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-25 08:15:58.000000 BaseNN-0.1.1/setup.py
```

### Comparing `BaseNN-0.1.0/BaseNN/BaseNN.py` & `BaseNN-0.1.1/BaseNN/BaseNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
             data = Variable(torch.tensor(np.array(data)).to(torch.float32))
             self.model.eval()
             f = open(os.path.join(save_fold,'layer_data.txt'), "w")
             str_data = ""
             act_layer = 0
             tra_layer = 0
             for num, i in enumerate(self.model):
+                data = data.to(self.device)
                 data = i(data)
                 # print(num, i, data)
                 if isinstance(i, (type(torch.nn.ReLU()),type(torch.nn.Softmax()))): # 非传统层，不计数
                     act_layer+=0.1
                     str_data += str(tra_layer-1+act_layer) + "."+str(i) +"\n" + str(np.squeeze(data).tolist()) + "\n"
                 else:  #传统网络层
                     act_layer =0
@@ -379,36 +380,39 @@
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
             self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
             self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            return self.dataloader, self.val_dataloader
+
         else:
             self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
 
-        return self.dataloader
+            return self.dataloader
 
     def load_tab_data(self, data_path,batch_size=32, train_val_ratio=1.0, shuffle=True):
         from .load_data import TabularDataset
         dataset = TabularDataset(data_path)
         self.dataset_size = int(len(dataset))
         # print(self.dataset_size)
         # self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
             self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
             self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            return self.dataloader, self.val_dataloader
         else:
             self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
 
-        return self.dataloader
+            return self.dataloader
 
     def load_npz_data(self, data_path, batch_size=32, shuffle=True, classes=None,train_val_ratio=1.0):
         from .load_data import NpzDataset
         dataset = NpzDataset(data_path)
         self.dataset_size = int(len(dataset))
         self.img_classes = classes
 
@@ -683,14 +687,20 @@
             # torch.save([self.img_classes, self.model], model_path)
             print("保存模型{}成功！".format(model_path))
             return log
 
     def inference(self, data, show=False, checkpoint=None,hidden=None, label=False):
         if checkpoint is not None:
             self.rnn = torch.load(checkpoint)['para']['rnn']
+        if checkpoint:
+            self.model = torch.load(checkpoint)['state_dict']
+            try:
+                self.img_classes = torch.load(checkpoint)['meta']['CLASSES']
+            except:
+                pass
         if self.rnn:
             self.word2idx = torch.load(checkpoint)['meta']['word2idx']
             self.ix2word = {v:k for k, v in self.word2idx.items()}
             config = torch.load(checkpoint)['para']['config']
             self.model =  lstm(len(self.word2idx),config['para']['ed'],config['para']['hd'],config['para']['nl'])
             self.model.eval()
             self.model.to(self.device)
@@ -755,30 +765,39 @@
                         transform = torch.load(checkpoint)['meta']['transform']
                         if transform is not None:
                             img = np.array(transform(Image.fromarray(img)))
                         img_list.append(img)
                     
                     data = torch.from_numpy(np.array(img_list)).permute(0,3,1,2).to(torch.float32).to(self.device) 
                     # x = np.expand_dims(x, axis=1)
+            elif isinstance(data, DataLoader):  # 推理dataloader
+                res = torch.Tensor().to(self.device)
+                self.val_label = torch.Tensor().to(self.device)
+                for test_x, test_y in data:
+                    test_x = test_x.to(self.device)
+                    test_y = test_y.to(self.device)
+                    batch_res = self.model(test_x)
+                    res = torch.cat([res, batch_res], dim=0)
+                    self.val_label = torch.cat([self.val_label, test_y], dim=0)
+                self.val_label = self.val_label.cpu().detach().numpy()
+                res = res.cpu().detach().numpy()
+                if show:
+                    print("推理结果为：",res)
+                self. res = res
+                return res
 
             else:  # 推理numpy数组
                 data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
             # print(data.shape)
             # data  = Variable(torch.tensor(np.array(data)))
 
-            if checkpoint:
-                self.model = torch.load(checkpoint)['state_dict']
-                try:
-                    self.img_classes = torch.load(checkpoint)['meta']['CLASSES']
-                except:
-                    pass
             self.model.eval()
             with torch.no_grad():
                 res = self.model(data)
-            res = np.array(res.cpu())
+            res = res.cpu().detach().numpy()
             if show:
                 print("推理结果为：",res)
             self. res = res
             return res
     
     def _inference(self, data, show=False, checkpoint=None,hidden=None):
         data = data.to(self.device)
```

### Comparing `BaseNN-0.1.0/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.1/BaseNN/examples/BaseNN_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,18 +453,18 @@
     # iris_train_test()
 
     # mnist_train()
     # pth_info('mn_ckpt/basenn.pth')
     # mnist_test(True)
 
     # infer_9_demo()
-    # visual_feature_demo()
+    visual_feature_demo()
     # extract_feature_demo()
 
     # lstm_train_demo()
     # pth_info('model_lstm.pth')
     # lstm_infer_demo()
 
     # load_image_data_mn()
     # load_image_data_cd()
-    load_tab_data_iris()
+    # load_tab_data_iris()
     # load_npz_data_action()
```

### Comparing `BaseNN-0.1.0/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.1/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.0/BaseNN/load_data.py` & `BaseNN-0.1.1/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.0/BaseNN/version.py` & `BaseNN-0.1.1/BaseNN/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.0'
+__version__='0.1.1'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.0/setup.py` & `BaseNN-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.0',
+    version='0.1.1',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

