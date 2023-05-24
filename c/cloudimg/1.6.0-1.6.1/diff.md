# Comparing `tmp/cloudimg-1.6.0.tar.gz` & `tmp/cloudimg-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudimg-1.6.0.tar", last modified: Sun Mar 19 23:33:55 2023, max compression
+gzip compressed data, was "cloudimg-1.6.1.tar", last modified: Wed May 24 03:05:00 2023, max compression
```

## Comparing `cloudimg-1.6.0.tar` & `cloudimg-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:33:55.063777 cloudimg-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-19 23:33:44.000000 cloudimg-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-19 23:33:44.000000 cloudimg-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-19 23:33:55.063777 cloudimg-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-19 23:33:44.000000 cloudimg-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:33:55.063777 cloudimg-1.6.0/cloudimg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 23:33:44.000000 cloudimg-1.6.0/cloudimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25702 2023-03-19 23:33:44.000000 cloudimg-1.6.0/cloudimg/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-03-19 23:33:44.000000 cloudimg-1.6.0/cloudimg/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-03-19 23:33:44.000000 cloudimg-1.6.0/cloudimg/ms_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:33:55.063777 cloudimg-1.6.0/cloudimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-19 23:33:54.000000 cloudimg-1.6.0/cloudimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-19 23:33:54.000000 cloudimg-1.6.0/cloudimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 23:33:54.000000 cloudimg-1.6.0/cloudimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-19 23:33:54.000000 cloudimg-1.6.0/cloudimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-19 23:33:54.000000 cloudimg-1.6.0/cloudimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-19 23:33:44.000000 cloudimg-1.6.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-19 23:33:44.000000 cloudimg-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 23:33:55.063777 cloudimg-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-19 23:33:44.000000 cloudimg-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:33:55.063777 cloudimg-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-03-19 23:33:44.000000 cloudimg-1.6.0/tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-03-19 23:33:44.000000 cloudimg-1.6.0/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-19 23:33:44.000000 cloudimg-1.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:05:00.804285 cloudimg-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-24 03:04:47.000000 cloudimg-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 03:04:47.000000 cloudimg-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 03:05:00.804285 cloudimg-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 03:04:47.000000 cloudimg-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:05:00.804285 cloudimg-1.6.1/cloudimg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:04:47.000000 cloudimg-1.6.1/cloudimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-05-24 03:04:47.000000 cloudimg-1.6.1/cloudimg/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-24 03:04:47.000000 cloudimg-1.6.1/cloudimg/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19119 2023-05-24 03:04:47.000000 cloudimg-1.6.1/cloudimg/ms_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:05:00.804285 cloudimg-1.6.1/cloudimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 03:05:00.000000 cloudimg-1.6.1/cloudimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 03:05:00.000000 cloudimg-1.6.1/cloudimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:05:00.000000 cloudimg-1.6.1/cloudimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 03:05:00.000000 cloudimg-1.6.1/cloudimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 03:05:00.000000 cloudimg-1.6.1/cloudimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 03:04:47.000000 cloudimg-1.6.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 03:04:47.000000 cloudimg-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:05:00.804285 cloudimg-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-24 03:04:47.000000 cloudimg-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:05:00.804285 cloudimg-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-05-24 03:04:47.000000 cloudimg-1.6.1/tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-05-24 03:04:47.000000 cloudimg-1.6.1/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-24 03:04:47.000000 cloudimg-1.6.1/tox.ini
```

### Comparing `cloudimg-1.6.0/LICENSE` & `cloudimg-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.0/PKG-INFO` & `cloudimg-1.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cloudimg
-Version: 1.6.0
+Version: 1.6.1
 Summary: Services for building and releasing products in cloud environments
 Home-page: https://github.com/release-engineering/cloudimg
 Author: Alex Misstear
 Author-email: amisstea@redhat.com
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudimg-1.6.0/README.md` & `cloudimg-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.0/cloudimg/aws.py` & `cloudimg-1.6.1/cloudimg/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,28 +416,28 @@
         if image_path.lower().startswith('http'):
             # Stream the upload from a remote URL
             log.info('Opening stream to: %s', image_path)
             resp = requests.get(image_path, stream=True, timeout=30)
             resp.raise_for_status()
             stream = resp.iter_content(chunk_size)
             callback = UploadProgress(container_name, object_name)
-            if object_name.endswith(".xz"):
+            if image_path.endswith(".xz"):
                 raise NotImplementedError(
                     "LZMA decompression is not implemented "
                     "for S3 content from an HTTP source")
             self.s3.meta.client.upload_fileobj(stream,
                                                container_name,
                                                object_name,
                                                Callback=callback)
-        elif object_name.endswith(".xz"):
+        elif image_path.endswith(".xz"):
             # Stream the decompression to the container file
             # Can take a few minutes to load into memory
-            object_name = object_name.rstrip(".xz")
             callback = UploadProgress(container_name, object_name)
-            log.info("Processing a LZMA compressed file: %s.", object_name)
+            log.info("Processing a LZMA compressed file: %s.",
+                     os.path.basename(image_path))
             with lzma.open(image_path, "rb") as data:
                 self.s3.meta.client.upload_fileobj(data,
                                                    container_name,
                                                    object_name,
                                                    Callback=callback)
         else:
             callback = UploadProgress(container_name, object_name,
```

### Comparing `cloudimg-1.6.0/cloudimg/common.py` & `cloudimg-1.6.1/cloudimg/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     @property
     def _default_snapshot_name(self):
         return os.path.splitext(self.object_name)[0]
 
     @property
     def object_name(self):
-        return os.path.basename(self.image_path)
+        return os.path.basename(self.image_path).rstrip(".xz")
 
 
 class DeleteMetadata(object):
     """
     A collection of metadata necessary for deleting a disk image and its
     dependent objects from a cloud provider.
```

### Comparing `cloudimg-1.6.0/cloudimg/ms_azure.py` & `cloudimg-1.6.1/cloudimg/ms_azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,17 +375,17 @@
         container_client = self.get_container_by_name(
             name=container_name,
             create=True
         )
 
         # Azure can't handle compressed images on marketplaces so we need to
         # send the decompressed data to its storage account.
-        if object_name.endswith(".xz"):
-            log.info("Processing a LZMA compressed file: %s.", object_name)
-            object_name = object_name.rstrip(".xz")
+        if image_path.endswith(".xz"):
+            log.info("Processing a LZMA compressed file: %s.",
+                     os.path.basename(image_path))
             open_func = lzma.open
         else:
             open_func = open
 
         # Check the image tags
         log.info("Checking whether the image was already uploaded.")
         if self.are_tags_present(container_client, tags):
```

### Comparing `cloudimg-1.6.0/cloudimg.egg-info/PKG-INFO` & `cloudimg-1.6.1/cloudimg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cloudimg
-Version: 1.6.0
+Version: 1.6.1
 Summary: Services for building and releasing products in cloud environments
 Home-page: https://github.com/release-engineering/cloudimg
 Author: Alex Misstear
 Author-email: amisstea@redhat.com
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudimg-1.6.0/setup.py` & `cloudimg-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cloudimg',
-    version='1.6.0',
+    version='1.6.1',
     author='Alex Misstear',
     author_email='amisstea@redhat.com',
     description=('Services for building and releasing products in cloud '
                  'environments'),
     license='GPLv3',
     url='https://github.com/release-engineering/cloudimg',
     packages=find_packages(),
```

### Comparing `cloudimg-1.6.0/tests/test_aws.py` & `cloudimg-1.6.1/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.0/tests/test_azure.py` & `cloudimg-1.6.1/tests/test_azure.py`

 * *Files identical despite different names*

