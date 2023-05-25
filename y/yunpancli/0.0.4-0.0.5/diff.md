# Comparing `tmp/yunpancli-0.0.4.tar.gz` & `tmp/yunpancli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.4.tar", last modified: Wed May 24 10:42:14 2023, max compression
+gzip compressed data, was "yunpancli-0.0.5.tar", last modified: Thu May 25 02:49:48 2023, max compression
```

## Comparing `yunpancli-0.0.4.tar` & `yunpancli-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:42:14.633169 yunpancli-0.0.4/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.4/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-24 10:42:14.633245 yunpancli-0.0.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.4/README.md
--rw-r--r--   0 mac        (501) staff       (20)      125 2023-05-24 10:42:14.633542 yunpancli-0.0.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      692 2023-05-24 10:42:09.000000 yunpancli-0.0.4/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:42:14.632265 yunpancli-0.0.4/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.4/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.4/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     6868 2023-05-24 10:41:11.000000 yunpancli-0.0.4/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:42:14.633047 yunpancli-0.0.4/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-24 10:42:14.000000 yunpancli-0.0.4/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-05-24 10:42:14.000000 yunpancli-0.0.4/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-24 10:42:14.000000 yunpancli-0.0.4/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-24 10:42:14.000000 yunpancli-0.0.4/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-24 10:42:14.000000 yunpancli-0.0.4/yunpancli.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-24 10:42:14.000000 yunpancli-0.0.4/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 02:49:48.943761 yunpancli-0.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.5/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 02:49:48.943843 yunpancli-0.0.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.5/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      125 2023-05-25 02:49:48.944153 yunpancli-0.0.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      692 2023-05-25 02:49:25.000000 yunpancli-0.0.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 02:49:48.942712 yunpancli-0.0.5/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.5/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.5/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     7120 2023-05-25 02:49:01.000000 yunpancli-0.0.5/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 02:49:48.943642 yunpancli-0.0.5/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.4/LICENSE` & `yunpancli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.4/setup.py` & `yunpancli-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
     entry_points={"console_scripts": ["yunpancli=yunpancli:main"]},
-    version="0.0.4",
+    version="0.0.5",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
```

### Comparing `yunpancli-0.0.4/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.5/yunpancli/baidu_pan_sdk.py`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.4/yunpancli/base.py` & `yunpancli-0.0.5/yunpancli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,19 +92,24 @@
             return
         if os.path.isfile(src): # 上传单个文件
             pan_dest = os.path.join(pan_dest, os.path.basename(src))
             self.sdk.upload_file(src, pan_dest, self.account_info['accessToken'])
         else:       # 上传整个文件夹下的所有文件，空文件夹不上传
             last_len = len(os.path.split(src)[-1])
             prefix_len = len(src) - last_len
+            # 多于文件夹下存在文件数量过多的场景需要打印进度
+            trans_cnt = 0
             for root, dirs, files in os.walk(src):
                 for file in files:
                     file_path = os.path.join(root, file)
                     pan_file = os.path.join(pan_dest, file_path[prefix_len:])
                     self.sdk.upload_file(file_path, pan_file, self.account_info['accessToken'])
+                    trans_cnt += 1
+                    if trans_cnt > 100:
+                        print(f"transfered {trans_cnt} files ...")
             
     
     def handle_remote_cp(self, pan_src, pan_dest):
         print("not yet supported")
 
     def handle_cp(self, src, dest):
         pan_src = self._parse_pan_path(src)
```

