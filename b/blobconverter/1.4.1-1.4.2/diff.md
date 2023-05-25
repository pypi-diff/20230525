# Comparing `tmp/blobconverter-1.4.1.tar.gz` & `tmp/blobconverter-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blobconverter-1.4.1.tar", last modified: Mon May  8 18:04:45 2023, max compression
+gzip compressed data, was "dist\blobconverter-1.4.2.tar", last modified: Thu May 25 18:14:19 2023, max compression
```

## Comparing `blobconverter-1.4.1.tar` & `blobconverter-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 18:04:45.150584 blobconverter-1.4.1/
--rw-rw-rw-   0        0        0     9241 2023-05-08 18:04:45.149584 blobconverter-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6520 2023-05-08 16:19:16.000000 blobconverter-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 18:04:45.110583 blobconverter-1.4.1/blobconverter/
--rw-rw-rw-   0        0        0    21893 2023-05-08 18:04:39.000000 blobconverter-1.4.1/blobconverter/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-08 16:19:16.000000 blobconverter-1.4.1/blobconverter/__main__.py
--rw-rw-rw-   0        0        0     5577 2023-05-08 16:19:16.000000 blobconverter-1.4.1/blobconverter/test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 18:04:45.145587 blobconverter-1.4.1/blobconverter.egg-info/
--rw-rw-rw-   0        0        0     9241 2023-05-08 18:04:44.000000 blobconverter-1.4.1/blobconverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-05-08 18:04:45.000000 blobconverter-1.4.1/blobconverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 18:04:44.000000 blobconverter-1.4.1/blobconverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-08 18:04:44.000000 blobconverter-1.4.1/blobconverter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-05-08 18:04:44.000000 blobconverter-1.4.1/blobconverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-08 18:04:44.000000 blobconverter-1.4.1/blobconverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 18:04:45.151584 blobconverter-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1429 2023-05-08 18:04:35.000000 blobconverter-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:14:19.598013 blobconverter-1.4.2/
+-rw-rw-rw-   0        0        0     9241 2023-05-25 18:14:19.596010 blobconverter-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6520 2023-05-08 16:19:16.000000 blobconverter-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 18:14:19.547995 blobconverter-1.4.2/blobconverter/
+-rw-rw-rw-   0        0        0    21942 2023-05-10 21:01:24.000000 blobconverter-1.4.2/blobconverter/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:19:16.000000 blobconverter-1.4.2/blobconverter/__main__.py
+-rw-rw-rw-   0        0        0     5577 2023-05-08 16:19:16.000000 blobconverter-1.4.2/blobconverter/test.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:14:19.593029 blobconverter-1.4.2/blobconverter.egg-info/
+-rw-rw-rw-   0        0        0     9241 2023-05-25 18:14:19.000000 blobconverter-1.4.2/blobconverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-05-25 18:14:19.000000 blobconverter-1.4.2/blobconverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 18:14:19.000000 blobconverter-1.4.2/blobconverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-25 18:14:19.000000 blobconverter-1.4.2/blobconverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-05-25 18:14:19.000000 blobconverter-1.4.2/blobconverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 18:14:19.000000 blobconverter-1.4.2/blobconverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 18:14:19.599023 blobconverter-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2023-05-25 18:12:41.000000 blobconverter-1.4.2/setup.py
```

### Comparing `blobconverter-1.4.1/PKG-INFO` & `blobconverter-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobconverter
-Version: 1.4.1
+Version: 1.4.2
 Summary: The tool that allows you to convert neural networks to MyriadX blob
 Home-page: https://github.com/luxonis/blobconverter
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/luxonis/blobconverter/issues
 Project-URL: Source Code, https://github.com/luxonis/blobconverter/tree/master/cli
```

### Comparing `blobconverter-1.4.1/README.md` & `blobconverter-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `blobconverter-1.4.1/blobconverter/__init__.py` & `blobconverter-1.4.2/blobconverter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,22 +480,23 @@
     }
     files = {
         'config': path,
     }
     return compile_blob(blob_name=name, req_data=body, req_files=files, **kwargs)
 
 
-def zoo_list(version=None, url=None):
+def zoo_list(version=None, url=None, zoo_type='intel'):
     if url is None:
         url = __defaults["url"]
     if version is None:
         version = __defaults["version"]
 
     url_params = {
-        'version': version
+        'version': version,
+        'zoo_type': zoo_type
     }
 
     response = requests.get("{}/zoo_models?{}".format(url, urllib.parse.urlencode(url_params)))
     response.raise_for_status()
     return response.json()['available']
```

### Comparing `blobconverter-1.4.1/blobconverter/test.py` & `blobconverter-1.4.2/blobconverter/test.py`

 * *Files identical despite different names*

### Comparing `blobconverter-1.4.1/blobconverter.egg-info/PKG-INFO` & `blobconverter-1.4.2/blobconverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobconverter
-Version: 1.4.1
+Version: 1.4.2
 Summary: The tool that allows you to convert neural networks to MyriadX blob
 Home-page: https://github.com/luxonis/blobconverter
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/luxonis/blobconverter/issues
 Project-URL: Source Code, https://github.com/luxonis/blobconverter/tree/master/cli
```

### Comparing `blobconverter-1.4.1/setup.py` & `blobconverter-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup
 
 setup(
     name='blobconverter',
-    version='1.4.1',
+    version='1.4.2',
     description='The tool that allows you to convert neural networks to MyriadX blob',
     long_description=io.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/luxonis/blobconverter',
     keywords="blobconverter blob converter myriadx openvino tensorflow caffe ir",
     author='Luxonis',
     author_email='support@luxonis.com',
```

