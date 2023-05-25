# Comparing `tmp/neurodeploy-0.0.8.tar.gz` & `tmp/neurodeploy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurodeploy-0.0.8.tar", last modified: Fri Mar 31 23:41:47 2023, max compression
+gzip compressed data, was "neurodeploy-0.0.9.tar", last modified: Fri Mar 31 23:52:09 2023, max compression
```

## Comparing `neurodeploy-0.0.8.tar` & `neurodeploy-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.650369 neurodeploy-0.0.8/
--rw-r--r--   0 maher.naija   (502) staff       (20)     1900 2023-03-31 23:41:47.650193 neurodeploy-0.0.8/PKG-INFO
--rw-r--r--   0 maher.naija   (502) staff       (20)     3967 2023-03-30 21:36:23.000000 neurodeploy-0.0.8/README.md
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.646140 neurodeploy-0.0.8/display/
--rw-r--r--   0 maher.naija   (502) staff       (20)        0 2023-03-21 14:48:57.000000 neurodeploy-0.0.8/display/__init__.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     2532 2023-03-30 22:45:07.000000 neurodeploy-0.0.8/display/rich_demo.py
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.647004 neurodeploy-0.0.8/neurodeploy/
--rw-r--r--   0 maher.naija   (502) staff       (20)      191 2023-03-30 22:41:33.000000 neurodeploy-0.0.8/neurodeploy/__init__.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1820 2023-03-29 22:34:53.000000 neurodeploy-0.0.8/neurodeploy/credentials.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     3961 2023-03-30 22:12:44.000000 neurodeploy-0.0.8/neurodeploy/model.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1029 2023-03-31 23:41:33.000000 neurodeploy-0.0.8/neurodeploy/user.py
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.650009 neurodeploy-0.0.8/neurodeploy.egg-info/
--rw-r--r--   0 maher.naija   (502) staff       (20)     1900 2023-03-31 23:41:47.000000 neurodeploy-0.0.8/neurodeploy.egg-info/PKG-INFO
--rw-r--r--   0 maher.naija   (502) staff       (20)      556 2023-03-31 23:41:47.000000 neurodeploy-0.0.8/neurodeploy.egg-info/SOURCES.txt
--rw-r--r--   0 maher.naija   (502) staff       (20)        1 2023-03-31 23:41:47.000000 neurodeploy-0.0.8/neurodeploy.egg-info/dependency_links.txt
--rw-r--r--   0 maher.naija   (502) staff       (20)       42 2023-03-31 23:41:47.000000 neurodeploy-0.0.8/neurodeploy.egg-info/top_level.txt
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.647791 neurodeploy-0.0.8/process/
--rw-r--r--   0 maher.naija   (502) staff       (20)       79 2023-03-27 17:53:37.000000 neurodeploy-0.0.8/process/__init__.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1581 2023-03-29 23:00:47.000000 neurodeploy-0.0.8/process/nd_config.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1021 2023-03-31 23:02:15.000000 neurodeploy-0.0.8/process/nd_credentials.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1419 2023-03-31 23:37:27.000000 neurodeploy-0.0.8/process/nd_token.py
--rw-r--r--   0 maher.naija   (502) staff       (20)       38 2023-03-31 23:41:47.650416 neurodeploy-0.0.8/setup.cfg
--rw-r--r--   0 maher.naija   (502) staff       (20)     1033 2023-03-31 23:41:44.000000 neurodeploy-0.0.8/setup.py
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.648796 neurodeploy-0.0.8/sub_cmd/
--rw-r--r--   0 maher.naija   (502) staff       (20)       90 2023-03-27 17:02:02.000000 neurodeploy-0.0.8/sub_cmd/__init__.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1157 2023-03-29 23:03:43.000000 neurodeploy-0.0.8/sub_cmd/config.py
--rw-r--r--   0 maher.naija   (502) staff       (20)      923 2023-03-25 00:22:08.000000 neurodeploy-0.0.8/sub_cmd/credentials.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     1464 2023-03-29 22:10:17.000000 neurodeploy-0.0.8/sub_cmd/model.py
--rw-r--r--   0 maher.naija   (502) staff       (20)      456 2023-03-25 00:28:39.000000 neurodeploy-0.0.8/sub_cmd/user.py
-drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:41:47.649442 neurodeploy-0.0.8/utils/
--rw-r--r--   0 maher.naija   (502) staff       (20)       38 2023-03-27 18:42:02.000000 neurodeploy-0.0.8/utils/__init__.py
--rw-r--r--   0 maher.naija   (502) staff       (20)      555 2023-03-31 23:05:07.000000 neurodeploy-0.0.8/utils/files.py
--rw-r--r--   0 maher.naija   (502) staff       (20)     2066 2023-03-21 14:48:57.000000 neurodeploy-0.0.8/utils/query.py
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.044004 neurodeploy-0.0.9/
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1900 2023-03-31 23:52:09.043838 neurodeploy-0.0.9/PKG-INFO
+-rw-r--r--   0 maher.naija   (502) staff       (20)     3967 2023-03-30 21:36:23.000000 neurodeploy-0.0.9/README.md
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.038827 neurodeploy-0.0.9/display/
+-rw-r--r--   0 maher.naija   (502) staff       (20)        0 2023-03-21 14:48:57.000000 neurodeploy-0.0.9/display/__init__.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     2532 2023-03-30 22:45:07.000000 neurodeploy-0.0.9/display/rich_demo.py
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.040111 neurodeploy-0.0.9/neurodeploy/
+-rw-r--r--   0 maher.naija   (502) staff       (20)      191 2023-03-30 22:41:33.000000 neurodeploy-0.0.9/neurodeploy/__init__.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1820 2023-03-29 22:34:53.000000 neurodeploy-0.0.9/neurodeploy/credentials.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     3961 2023-03-30 22:12:44.000000 neurodeploy-0.0.9/neurodeploy/model.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1021 2023-03-31 23:51:02.000000 neurodeploy-0.0.9/neurodeploy/user.py
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.043649 neurodeploy-0.0.9/neurodeploy.egg-info/
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1900 2023-03-31 23:52:08.000000 neurodeploy-0.0.9/neurodeploy.egg-info/PKG-INFO
+-rw-r--r--   0 maher.naija   (502) staff       (20)      556 2023-03-31 23:52:08.000000 neurodeploy-0.0.9/neurodeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 maher.naija   (502) staff       (20)        1 2023-03-31 23:52:08.000000 neurodeploy-0.0.9/neurodeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 maher.naija   (502) staff       (20)       42 2023-03-31 23:52:08.000000 neurodeploy-0.0.9/neurodeploy.egg-info/top_level.txt
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.041231 neurodeploy-0.0.9/process/
+-rw-r--r--   0 maher.naija   (502) staff       (20)       79 2023-03-27 17:53:37.000000 neurodeploy-0.0.9/process/__init__.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1581 2023-03-29 23:00:47.000000 neurodeploy-0.0.9/process/nd_config.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1021 2023-03-31 23:02:15.000000 neurodeploy-0.0.9/process/nd_credentials.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1419 2023-03-31 23:37:27.000000 neurodeploy-0.0.9/process/nd_token.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)       38 2023-03-31 23:52:09.044056 neurodeploy-0.0.9/setup.cfg
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1033 2023-03-31 23:51:59.000000 neurodeploy-0.0.9/setup.py
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.042368 neurodeploy-0.0.9/sub_cmd/
+-rw-r--r--   0 maher.naija   (502) staff       (20)       90 2023-03-27 17:02:02.000000 neurodeploy-0.0.9/sub_cmd/__init__.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1157 2023-03-29 23:03:43.000000 neurodeploy-0.0.9/sub_cmd/config.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)      923 2023-03-25 00:22:08.000000 neurodeploy-0.0.9/sub_cmd/credentials.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     1464 2023-03-29 22:10:17.000000 neurodeploy-0.0.9/sub_cmd/model.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)      456 2023-03-25 00:28:39.000000 neurodeploy-0.0.9/sub_cmd/user.py
+drwxr-xr-x   0 maher.naija   (502) staff       (20)        0 2023-03-31 23:52:09.043088 neurodeploy-0.0.9/utils/
+-rw-r--r--   0 maher.naija   (502) staff       (20)       38 2023-03-27 18:42:02.000000 neurodeploy-0.0.9/utils/__init__.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)      555 2023-03-31 23:05:07.000000 neurodeploy-0.0.9/utils/files.py
+-rw-r--r--   0 maher.naija   (502) staff       (20)     2066 2023-03-21 14:48:57.000000 neurodeploy-0.0.9/utils/query.py
```

### Comparing `neurodeploy-0.0.8/PKG-INFO` & `neurodeploy-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurodeploy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neuro deploy SDK
 Author: maher_naija
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neurodeploy-0.0.8/README.md` & `neurodeploy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/display/rich_demo.py` & `neurodeploy-0.0.9/display/rich_demo.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/neurodeploy/credentials.py` & `neurodeploy-0.0.9/neurodeploy/credentials.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/neurodeploy/model.py` & `neurodeploy-0.0.9/neurodeploy/model.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/neurodeploy/user.py` & `neurodeploy-0.0.9/neurodeploy/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     headers = {}
     headers["username"] = username
     headers["password"] = password
     data = None
     response_data = query.post(url, data, headers)
     resp = nd_token.save_token(response_data)
     if resp == 1:
-        print("[bold green]you are logged succesful[/bold green]")
+        print("[bold green]Login Successful[/bold green]")
     else:
         print("[bold red]login error[/bold red]")
```

### Comparing `neurodeploy-0.0.8/neurodeploy.egg-info/PKG-INFO` & `neurodeploy-0.0.9/neurodeploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurodeploy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neuro deploy SDK
 Author: maher_naija
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neurodeploy-0.0.8/neurodeploy.egg-info/SOURCES.txt` & `neurodeploy-0.0.9/neurodeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/process/nd_config.py` & `neurodeploy-0.0.9/process/nd_config.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/process/nd_credentials.py` & `neurodeploy-0.0.9/process/nd_credentials.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/process/nd_token.py` & `neurodeploy-0.0.9/process/nd_token.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/setup.py` & `neurodeploy-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_SDK.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="neurodeploy",  # This is the name of the package
-    version="0.0.8",  # The initial release version
+    version="0.0.9",  # The initial release version
     author="maher_naija",  # Full name of the author
     description="Neuro deploy SDK",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `neurodeploy-0.0.8/sub_cmd/config.py` & `neurodeploy-0.0.9/sub_cmd/config.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/sub_cmd/credentials.py` & `neurodeploy-0.0.9/sub_cmd/credentials.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/sub_cmd/model.py` & `neurodeploy-0.0.9/sub_cmd/model.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/utils/files.py` & `neurodeploy-0.0.9/utils/files.py`

 * *Files identical despite different names*

### Comparing `neurodeploy-0.0.8/utils/query.py` & `neurodeploy-0.0.9/utils/query.py`

 * *Files identical despite different names*

