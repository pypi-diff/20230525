# Comparing `tmp/textbsr-0.0.6.tar.gz` & `tmp/textbsr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.0.6.tar", last modified: Mon May 22 13:33:57 2023, max compression
+gzip compressed data, was "textbsr-0.0.7.tar", last modified: Thu May 25 13:28:45 2023, max compression
```

## Comparing `textbsr-0.0.6.tar` & `textbsr-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:33:57.000000 textbsr-0.0.6/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-22 13:33:57.000000 textbsr-0.0.6/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1169 2023-05-22 13:33:51.000000 textbsr-0.0.6/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:16:08.000000 textbsr-0.0.6/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.6/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.6/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.6/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6246 2023-05-22 13:33:41.000000 textbsr-0.0.6/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.6/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.6/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      349 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:28:45.000000 textbsr-0.0.7/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-25 13:28:45.000000 textbsr-0.0.7/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-25 13:28:45.000000 textbsr-0.0.7/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1276 2023-05-25 13:23:39.000000 textbsr-0.0.7/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:28:45.000000 textbsr-0.0.7/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:16:08.000000 textbsr-0.0.7/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:28:45.000000 textbsr-0.0.7/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.7/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:28:45.000000 textbsr-0.0.7/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.7/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.7/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6242 2023-05-25 13:03:22.000000 textbsr-0.0.7/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:28:45.000000 textbsr-0.0.7/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.7/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.7/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-25 13:28:45.000000 textbsr-0.0.7/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-25 13:28:44.000000 textbsr-0.0.7/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      383 2023-05-25 13:28:44.000000 textbsr-0.0.7/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-25 13:28:44.000000 textbsr-0.0.7/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       40 2023-05-25 13:28:44.000000 textbsr-0.0.7/textbsr.egg-info/entry_points.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-25 13:28:44.000000 textbsr-0.0.7/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-25 13:28:44.000000 textbsr-0.0.7/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.0.6/setup.py` & `textbsr-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,27 @@
     here = os.path.dirname(os.path.realpath(__file__))
     with open(os.path.join(here, filename), 'r') as f:
         requires = [line.replace('\n', '') for line in f.readlines()]
     return requires
 
 
 setup(name='textbsr',
-      version='0.0.6',
+      version='0.0.7',
       description='a simple version for blind text image super-resolution (current version is only for English and Chinese)',
       author='Xiaoming Li',
       author_email='csxmli@gmail.com',
       #requires= ['numpy','torch','cv2','time','argparse','torchvision'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
       license="S-Lab License 1.0",
       keywords='blind text image super-resolution',
       url='https://github.com/csxmli2016/MARCONet',
       include_package_data=True,
       install_requires=get_requirements(),
       python_requires='>=3.6',
+      entry_points = {
+        'console_scripts': [
+            'textbsr = textbsr:sr',
+        ],
+      }
       )
```

### Comparing `textbsr-0.0.6/textbsr/models/TextEnhancement.py` & `textbsr-0.0.7/textbsr/models/TextEnhancement.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.0.6/textbsr/textbsr.py` & `textbsr-0.0.7/textbsr/textbsr.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         filename = file_name
     cached_file = os.path.abspath(os.path.join(model_dir, filename))
     if not os.path.exists(cached_file):
         print(f'Downloading: "{url}" to {cached_file}\n')
         download_url_to_file(url, cached_file, hash_prefix=None, progress=progress)
     return cached_file
 
-def main(test_path, sr_path=None, save_path=None, is_aligned=False, save_text=False):
+def sr(test_path, sr_path=None, save_path=None, is_aligned=False, save_text=False):
     if save_path is None:
         TIMESTAMP = time.strftime("%m-%d_%H-%M", time.localtime())
         save_path = osp.join(test_path+'_'+TIMESTAMP+'_BSRGAN-Text')
     os.makedirs(save_path, exist_ok=True)
 
     
     lq_imgs = []
@@ -142,8 +142,8 @@
     parser.add_argument('-i', '--test_path', type=str, default='./testsets/LQ', help='the lr image path')
     parser.add_argument('-b', '--sr_path', type=str, default=None, help='the background sr path, default:None')
     parser.add_argument('-o', '--save_path', type=str, default=None, help='the text sr save path')
     parser.add_argument('-a', '--aligned', action='store_true', help='whether the input contains only text region, default:False')
     parser.add_argument('-p', '--save_text', action='store_true', help='whether save the LR and SR text layout, default:False')
     args = parser.parse_args()
 
-    main(args.test_path, args.sr_path, args.save_path, args.aligned, args.save_text)
+    sr(args.test_path, args.sr_path, args.save_path, args.aligned, args.save_text)
```

### Comparing `textbsr-0.0.6/textbsr/utils/utils_image.py` & `textbsr-0.0.7/textbsr/utils/utils_image.py`

 * *Files identical despite different names*

