# Comparing `tmp/BaseNN-0.1.1.tar.gz` & `tmp/BaseNN-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.1.tar", last modified: Thu May 25 08:16:34 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.2.tar", last modified: Thu May 25 08:41:03 2023, max compression
```

## Comparing `BaseNN-0.1.1.tar` & `BaseNN-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    38285 2023-05-25 08:15:44.000000 BaseNN-0.1.1/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.1/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-25 07:54:48.000000 BaseNN-0.1.1/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.1/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.1/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.1/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-25 08:16:14.000000 BaseNN-0.1.1/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-25 08:16:34.000000 BaseNN-0.1.1/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.1/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:16:34.000000 BaseNN-0.1.1/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-25 08:16:34.000000 BaseNN-0.1.1/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-25 08:15:58.000000 BaseNN-0.1.1/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    38381 2023-05-25 08:37:32.000000 BaseNN-0.1.2/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.2/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-25 07:54:48.000000 BaseNN-0.1.2/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.2/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.2/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.2/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-25 08:41:00.000000 BaseNN-0.1.2/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-25 08:41:03.000000 BaseNN-0.1.2/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.2/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 08:41:03.000000 BaseNN-0.1.2/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-25 08:41:03.000000 BaseNN-0.1.2/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-25 08:40:53.000000 BaseNN-0.1.2/setup.py
```

### Comparing `BaseNN-0.1.1/BaseNN/BaseNN.py` & `BaseNN-0.1.2/BaseNN/BaseNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,28 +236,30 @@
             data = Variable(torch.tensor(np.array(data)).to(torch.float32))
             self.model.eval()
             dir_name = os.path.abspath(save_fold)
             if not os.path.exists(dir_name):
                 os.mkdir(dir_name)
             if not in1img: # 每层分别画一张图，横向
                 for num, i in enumerate(self.model):
+                    data = data.to(self.device)
                     data = i(data)
                     self.show_one_layer(data, i, num+1, dir_name)
             else: # 所有层共画一张图，纵向
                 # fig, ax = plt.subplots(20, 20)
                 plt.figure(figsize=(18,10))
                 num_img = 0
                 for name, para in self.model.named_parameters():
                     if "Linear" not in name:
                         num_img = max(num_img, para.size()[0])
                 grid = plt.GridSpec(num_img+1,len(self.model)+1,wspace=0.5, hspace=0.5) #（ 单层最大图片数+1，层数）
                 tra_layer = 1
                 str_l = ""
                 act_layer = 0
                 for num, i in enumerate(self.model):
+                    data = data.to(self.device)
                     data = i(data)
                     tmp_data = data
                     # print(i,"data.shape", data.shape)
                     if len(data.shape) > 2 and data.shape[0] == 1:
                         tmp_data = np.squeeze(data)
 
                     for j in range(tmp_data.shape[0]): # 每一层
```

### Comparing `BaseNN-0.1.1/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.2/BaseNN/examples/BaseNN_demo.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.1/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.2/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.1/BaseNN/load_data.py` & `BaseNN-0.1.2/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.1/BaseNN/version.py` & `BaseNN-0.1.2/BaseNN/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.1'
+__version__='0.1.2'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.1/setup.py` & `BaseNN-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.1',
+    version='0.1.2',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

