# Comparing `tmp/BaseNN-0.1.2.tar.gz` & `tmp/BaseNN-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.2.tar", last modified: Thu May 25 08:41:03 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.3.tar", last modified: Thu May 25 08:56:33 2023, max compression
```

## Comparing `BaseNN-0.1.2.tar` & `BaseNN-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    38381 2023-05-25 08:37:32.000000 BaseNN-0.1.2/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.2/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-25 07:54:48.000000 BaseNN-0.1.2/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.2/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.2/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.2/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-25 08:41:00.000000 BaseNN-0.1.2/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.2/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:41:03.000000 BaseNN-0.1.2/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-25 08:41:03.000000 BaseNN-0.1.2/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-25 08:40:53.000000 BaseNN-0.1.2/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:56:33.000000 BaseNN-0.1.3/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    38760 2023-05-25 08:56:07.000000 BaseNN-0.1.3/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.3/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-25 07:54:48.000000 BaseNN-0.1.3/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.3/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.3/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.3/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-25 08:56:27.000000 BaseNN-0.1.3/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-25 08:56:33.000000 BaseNN-0.1.3/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.3/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:56:33.000000 BaseNN-0.1.3/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-25 08:56:33.000000 BaseNN-0.1.3/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-25 08:56:23.000000 BaseNN-0.1.3/setup.py
```

### Comparing `BaseNN-0.1.2/BaseNN/BaseNN.py` & `BaseNN-0.1.3/BaseNN/BaseNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                     tmp_data = data
                     # print(i,"data.shape", data.shape)
                     if len(data.shape) > 2 and data.shape[0] == 1:
                         tmp_data = np.squeeze(data)
 
                     for j in range(tmp_data.shape[0]): # 每一层
                         # print("num+1",num+1, "j", j)
-                        img = tmp_data[j].detach().numpy()
+                        img = tmp_data[j].cpu().detach().numpy()
                         if len(img.shape) == 1:
                             img = np.reshape(img, (img.shape[0],1))
                         # w, c = img.shape
                         # print(w, c)
                         # img = np.reshape(img, (w, c))
                         # plt.subplot(tmp_data.shape[0],num+1, j+1)
                         if tmp_data.shape[0] == 1:
@@ -353,15 +353,15 @@
         return out
 
     def show_one_layer(self, data, layer_name, num, dir_name):
         if len(data.shape) > 2 and data.shape[0] == 1:
             data = np.squeeze(data)
 
         for i in range(data.shape[0]):
-            img = data[i].detach().numpy()
+            img = data[i].cpu().detach().numpy()
             if len(img.shape) == 1:
                 img = np.reshape(img, (1, img.shape[0]))
             # w, c = img.shape
             # print(w, c)
             # img = np.reshape(img, (w, c))
             plt.subplot(1,data.shape[0], i+1)
             plt.imshow(img)
@@ -386,15 +386,21 @@
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
             self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
             self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
             return self.dataloader, self.val_dataloader
 
         else:
             self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
-
+            self.label = torch.Tensor()
+            for train_x, train_y in self.dataloader:
+                # test_x = test_x.to(self.device)
+                # test_y = test_y.to(self.device)
+                # batch_res = self.model(test_x)
+                self.label = torch.cat([self.label, train_y], dim=0)
+                self.label = self.label.cpu().detach().numpy()
             return self.dataloader
 
     def load_tab_data(self, data_path,batch_size=32, train_val_ratio=1.0, shuffle=True):
         from .load_data import TabularDataset
         dataset = TabularDataset(data_path)
         self.dataset_size = int(len(dataset))
         # print(self.dataset_size)
@@ -791,15 +797,15 @@
                 data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
             # print(data.shape)
             # data  = Variable(torch.tensor(np.array(data)))
 
             self.model.eval()
             with torch.no_grad():
                 res = self.model(data)
-            res = res.cpu().detach().numpy()
+            res = res.detach().numpy()
             if show:
                 print("推理结果为：",res)
             self. res = res
             return res
     
     def _inference(self, data, show=False, checkpoint=None,hidden=None):
         data = data.to(self.device)
```

### Comparing `BaseNN-0.1.2/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.3/BaseNN/examples/BaseNN_demo.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.2/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.3/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.2/BaseNN/load_data.py` & `BaseNN-0.1.3/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.2/BaseNN/version.py` & `BaseNN-0.1.3/BaseNN/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.2'
+__version__='0.1.3'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.2/setup.py` & `BaseNN-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.2',
+    version='0.1.3',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

