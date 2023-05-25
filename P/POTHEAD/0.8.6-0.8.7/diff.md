# Comparing `tmp/POTHEAD-0.8.6.tar.gz` & `tmp/POTHEAD-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "POTHEAD-0.8.6.tar", last modified: Thu May  4 15:23:07 2023, max compression
+gzip compressed data, was "POTHEAD-0.8.7.tar", last modified: Thu May 25 16:40:09 2023, max compression
```

## Comparing `POTHEAD-0.8.6.tar` & `POTHEAD-0.8.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.6/LICENSE
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/PKG-INFO
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/POTHEAD.egg-info/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/PKG-INFO
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/SOURCES.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       76 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/requires.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/top_level.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.6/README.md
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/pothead/
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/__init__.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.6/pothead/cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.6/pothead/gating.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8198 2023-02-01 12:53:52.000000 POTHEAD-0.8.6/pothead/oob_response.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/resource_balancer.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/server.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11242 2023-04-04 15:05:09.000000 POTHEAD-0.8.6/pothead/subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.6/pothead/test_cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/test_resource_balancer.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    14323 2023-04-24 20:03:05.000000 POTHEAD-0.8.6/pothead/test_subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     9156 2023-04-24 20:03:18.000000 POTHEAD-0.8.6/pothead/test_worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.6/pothead/util.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14570 2023-04-24 20:03:05.000000 POTHEAD-0.8.6/pothead/worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.6/pothead/wsgi_typing.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/setup.cfg
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      876 2023-05-04 15:22:31.000000 POTHEAD-0.8.6/setup.py
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.7/LICENSE
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/PKG-INFO
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-25 16:40:09.133863 POTHEAD-0.8.7/POTHEAD.egg-info/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/PKG-INFO
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/SOURCES.txt
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       76 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/requires.txt
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/top_level.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.7/README.md
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/pothead/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/__init__.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.7/pothead/cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.7/pothead/gating.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8198 2023-05-25 14:08:42.000000 POTHEAD-0.8.7/pothead/oob_response.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/resource_balancer.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/server.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11308 2023-05-25 14:00:40.000000 POTHEAD-0.8.7/pothead/subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.7/pothead/test_cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/test_resource_balancer.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    14323 2023-05-25 16:38:51.000000 POTHEAD-0.8.7/pothead/test_subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     9156 2023-04-24 20:03:18.000000 POTHEAD-0.8.7/pothead/test_worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.7/pothead/util.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14570 2023-04-24 20:03:05.000000 POTHEAD-0.8.7/pothead/worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.7/pothead/wsgi_typing.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/setup.cfg
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      876 2023-05-25 16:39:27.000000 POTHEAD-0.8.7/setup.py
```

### Comparing `POTHEAD-0.8.6/LICENSE` & `POTHEAD-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/PKG-INFO` & `POTHEAD-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.6
+Version: 0.8.7
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.6/POTHEAD.egg-info/PKG-INFO` & `POTHEAD-0.8.7/POTHEAD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.6
+Version: 0.8.7
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.6/POTHEAD.egg-info/SOURCES.txt` & `POTHEAD-0.8.7/POTHEAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/README.md` & `POTHEAD-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/cgroups.py` & `POTHEAD-0.8.7/pothead/cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/gating.py` & `POTHEAD-0.8.7/pothead/gating.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/oob_response.py` & `POTHEAD-0.8.7/pothead/oob_response.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/resource_balancer.py` & `POTHEAD-0.8.7/pothead/resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/server.py` & `POTHEAD-0.8.7/pothead/server.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/subprocess_middleware.py` & `POTHEAD-0.8.7/pothead/subprocess_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,21 +302,24 @@
         proc.suspend()
     except psutil.NoSuchProcess:
         return []
 
     descendants = {proc}
     while True:
         prior_count = len(descendants)
-        for child in proc.children(recursive=True):
-            if child not in descendants:
-                try:
+        try:
+            for child in proc.children(recursive=True):
+                if child not in descendants:
                     child.suspend()
-                except psutil.NoSuchProcess:
-                    continue
                 descendants.add(child)
+        except psutil.NoSuchProcess:
+            if proc.is_running():
+                continue
+            else:
+                return []
         if len(descendants) == prior_count:
             break
 
     return descendants
 
 
 def _kill_process_and_its_descendants(process: multiprocessing.Process):
```

### Comparing `POTHEAD-0.8.6/pothead/test_cgroups.py` & `POTHEAD-0.8.7/pothead/test_cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/test_resource_balancer.py` & `POTHEAD-0.8.7/pothead/test_resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/test_subprocess_middleware.py` & `POTHEAD-0.8.7/pothead/test_subprocess_middleware.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/test_worker.py` & `POTHEAD-0.8.7/pothead/test_worker.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/util.py` & `POTHEAD-0.8.7/pothead/util.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/worker.py` & `POTHEAD-0.8.7/pothead/worker.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/pothead/wsgi_typing.py` & `POTHEAD-0.8.7/pothead/wsgi_typing.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.6/setup.py` & `POTHEAD-0.8.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 test_deps = ["aiohttp", "werkzeug", "tblib", "timeout-decorator"]
 
 setuptools.setup(
     name="POTHEAD",
-    version="0.8.6",
+    version="0.8.7",
     author="Ulrik Mikaelsson",
     author_email="ulrik.mikaelsson@gmail.com",
     description="A reverse-http proxy implementation for non-concurrent requests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/rawler/pothead",
     packages=setuptools.find_packages(),
```

