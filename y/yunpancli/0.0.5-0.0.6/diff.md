# Comparing `tmp/yunpancli-0.0.5.tar.gz` & `tmp/yunpancli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.5.tar", last modified: Thu May 25 02:49:48 2023, max compression
+gzip compressed data, was "yunpancli-0.0.6.tar", last modified: Thu May 25 06:27:07 2023, max compression
```

## Comparing `yunpancli-0.0.5.tar` & `yunpancli-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 02:49:48.943761 yunpancli-0.0.5/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.5/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 02:49:48.943843 yunpancli-0.0.5/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.5/README.md
--rw-r--r--   0 mac        (501) staff       (20)      125 2023-05-25 02:49:48.944153 yunpancli-0.0.5/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      692 2023-05-25 02:49:25.000000 yunpancli-0.0.5/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 02:49:48.942712 yunpancli-0.0.5/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.5/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.5/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     7120 2023-05-25 02:49:01.000000 yunpancli-0.0.5/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 02:49:48.943642 yunpancli-0.0.5/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-25 02:49:48.000000 yunpancli-0.0.5/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 06:27:07.081769 yunpancli-0.0.6/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.6/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 06:27:07.081874 yunpancli-0.0.6/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.6/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      125 2023-05-25 06:27:07.082216 yunpancli-0.0.6/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      689 2023-05-25 06:26:26.000000 yunpancli-0.0.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 06:27:07.080568 yunpancli-0.0.6/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.6/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.6/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     7146 2023-05-25 03:04:58.000000 yunpancli-0.0.6/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 06:27:07.081623 yunpancli-0.0.6/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.5/LICENSE` & `yunpancli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.5/setup.py` & `yunpancli-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
-    entry_points={"console_scripts": ["yunpancli=yunpancli:main"]},
-    version="0.0.5",
+    entry_points={"console_scripts": ["pancli=yunpancli:main"]},
+    version="0.0.6",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
```

### Comparing `yunpancli-0.0.5/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.6/yunpancli/baidu_pan_sdk.py`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.5/yunpancli/base.py` & `yunpancli-0.0.6/yunpancli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             trans_cnt = 0
             for root, dirs, files in os.walk(src):
                 for file in files:
                     file_path = os.path.join(root, file)
                     pan_file = os.path.join(pan_dest, file_path[prefix_len:])
                     self.sdk.upload_file(file_path, pan_file, self.account_info['accessToken'])
                     trans_cnt += 1
-                    if trans_cnt > 100:
+                    if trans_cnt >= 100 and trans_cnt % 100 == 0:
                         print(f"transfered {trans_cnt} files ...")
             
     
     def handle_remote_cp(self, pan_src, pan_dest):
         print("not yet supported")
 
     def handle_cp(self, src, dest):
```

