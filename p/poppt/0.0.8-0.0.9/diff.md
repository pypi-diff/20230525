# Comparing `tmp/poppt-0.0.8.tar.gz` & `tmp/poppt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppt-0.0.8.tar", last modified: Fri Apr 14 16:29:12 2023, max compression
+gzip compressed data, was "poppt-0.0.9.tar", last modified: Fri Apr 14 16:36:57 2023, max compression
```

## Comparing `poppt-0.0.8.tar` & `poppt-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.895310 poppt-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5248 2023-04-14 16:29:12.895310 poppt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.854309 poppt-0.0.8/poppt/
--rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.8/poppt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.879313 poppt-0.0.8/poppt/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.8/poppt/api/__init__.py
--rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.8/poppt/api/ppt.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.885318 poppt-0.0.8/poppt/core/
--rw-rw-rw-   0        0        0     2407 2023-04-14 16:28:38.000000 poppt-0.0.8/poppt/core/PPTType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.8/poppt/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.886312 poppt-0.0.8/poppt/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.8/poppt/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.889309 poppt-0.0.8/poppt/lib/ppt/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.8/poppt/lib/ppt/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.8/poppt/lib/ppt/ppt2pdf_service.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.875309 poppt-0.0.8/poppt.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-04-14 16:29:12.000000 poppt-0.0.8/poppt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-14 16:29:12.000000 poppt-0.0.8/poppt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:29:12.000000 poppt-0.0.8/poppt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.8/poppt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-04-14 16:29:12.000000 poppt-0.0.8/poppt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 16:29:12.000000 poppt-0.0.8/poppt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      722 2023-04-14 16:29:12.898310 poppt-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:29:12.893308 poppt-0.0.8/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2023-04-13 14:34:22.000000 poppt-0.0.8/tests/test_ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.710880 poppt-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5248 2023-04-14 16:36:57.711880 poppt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.676244 poppt-0.0.9/poppt/
+-rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.9/poppt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.698246 poppt-0.0.9/poppt/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.9/poppt/api/__init__.py
+-rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.9/poppt/api/ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.702268 poppt-0.0.9/poppt/core/
+-rw-rw-rw-   0        0        0     2363 2023-04-14 16:35:31.000000 poppt-0.0.9/poppt/core/PPTType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.9/poppt/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.704259 poppt-0.0.9/poppt/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.9/poppt/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.706885 poppt-0.0.9/poppt/lib/ppt/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.9/poppt/lib/ppt/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.9/poppt/lib/ppt/ppt2pdf_service.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.695245 poppt-0.0.9/poppt.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-04-14 16:36:57.000000 poppt-0.0.9/poppt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-14 16:36:57.000000 poppt-0.0.9/poppt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:36:57.000000 poppt-0.0.9/poppt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.9/poppt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-04-14 16:36:57.000000 poppt-0.0.9/poppt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 16:36:57.000000 poppt-0.0.9/poppt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      722 2023-04-14 16:36:57.712880 poppt-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:36:57.709880 poppt-0.0.9/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-04-13 14:34:22.000000 poppt-0.0.9/tests/test_ppt.py
```

### Comparing `poppt-0.0.8/LICENSE` & `poppt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poppt-0.0.8/PKG-INFO` & `poppt-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.0.8/README.md` & `poppt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `poppt-0.0.8/poppt/api/ppt.py` & `poppt-0.0.9/poppt/api/ppt.py`

 * *Files identical despite different names*

### Comparing `poppt-0.0.8/poppt/core/PPTType.py` & `poppt-0.0.9/poppt/core/PPTType.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,39 +20,38 @@
             # 判断文件的类型，对所有的ppt文件进行处理(ppt文件以ppt或者pptx结尾的)
             if filename.endswith('ppt') or filename.endswith('pptx'):
                 new_pdf_name = Path(filename).stem + '.pdf'  # PPT素材1.pdf
                 output_pdf_filename = Path(abs_output_path).absolute() / new_pdf_name
                 ppt2pdf_single(filename, str(output_pdf_filename))
                 # time.sleep(3)
 
-    def ppt2img(self, input_path, output_path, img_type, suffix1='ppt', suffix2='pptx'):
+    def ppt2img(self, input_path, output_path, img_type):
         '''将PPT另存为图片格式
           arguments:
               pptFullName: 要转换的ppt文件，
               pptName：转换后的存放JPG文件的目录
               imgType: 图片类型
         '''
-        filenames_ppt = get_files(input_path, suffix=suffix1)
-        filenames_pptx = get_files(input_path, suffix=suffix2)
-        filenames = filenames_pptx + filenames_ppt
+        filenames = get_files(input_path)
         # 启动PPT
         pptClient = win32com.client.Dispatch('PowerPoint.Application')
         # 设置为0表示后台运行，不显示，1则显示
         pptClient.Visible = True
         for ppt_file in filenames:
-            # Python路径操作模块pathlib，看这篇就够了！ https://zhuanlan.zhihu.com/p/475661402
-            output_dir = Path(output_path).absolute() / str(Path(ppt_file).stem)
-            exsit, output_dir = mkdir(output_dir)
-            # JPG是17
-            img_type_jpg = 17
-            # PNG是18
-            img_type_png = 18
+            if ppt_file.endswith('ppt') or ppt_file.endswith('pptx'):
+                # Python路径操作模块pathlib，看这篇就够了！ https://zhuanlan.zhihu.com/p/475661402
+                output_dir = Path(output_path).absolute() / str(Path(ppt_file).stem)
+                exsit, output_dir = mkdir(output_dir)
+                # JPG是17
+                img_type_jpg = 17
+                # PNG是18
+                img_type_png = 18
 
-            # 打开PPT文件
-            ppt = pptClient.Presentations.Open(ppt_file, WithWindow=False, ReadOnly=1)
-            # 另存为图片
-            if img_type == 'jpg':
-                ppt.SaveAs(output_dir, img_type_jpg)
-            else:
-                ppt.SaveAs(output_dir, img_type_png)
-            # 退出
+                # 打开PPT文件
+                ppt = pptClient.Presentations.Open(ppt_file, WithWindow=False, ReadOnly=1)
+                # 另存为图片
+                if img_type == 'jpg':
+                    ppt.SaveAs(output_dir, img_type_jpg)
+                else:
+                    ppt.SaveAs(output_dir, img_type_png)
+        # 退出
         pptClient.Quit()
```

### Comparing `poppt-0.0.8/poppt/lib/ppt/ppt2pdf_service.py` & `poppt-0.0.9/poppt/lib/ppt/ppt2pdf_service.py`

 * *Files identical despite different names*

### Comparing `poppt-0.0.8/poppt.egg-info/PKG-INFO` & `poppt-0.0.9/poppt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.0.8/setup.cfg` & `poppt-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 7074 0d0a 7665 7273 696f   = poppt..versio
-00000020: 6e20 3d20 302e 302e 380d 0a64 6573 6372  n = 0.0.8..descr
+00000020: 6e20 3d20 302e 302e 390d 0a64 6573 6372  n = 0.0.9..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 7074 0d0a 6c6f 6e67  tall poppt..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poppt-0.0.8/tests/test_ppt.py` & `poppt-0.0.9/tests/test_ppt.py`

 * *Files identical despite different names*

