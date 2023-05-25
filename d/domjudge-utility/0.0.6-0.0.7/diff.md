# Comparing `tmp/domjudge_utility-0.0.6.tar.gz` & `tmp/domjudge_utility-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domjudge_utility-0.0.6.tar", max compression
+gzip compressed data, was "domjudge_utility-0.0.7.tar", max compression
```

## Comparing `domjudge_utility-0.0.6.tar` & `domjudge_utility-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-05-23 14:48:38.633285 domjudge_utility-0.0.6/LICENSE
--rw-r--r--   0        0        0      636 2023-05-23 14:48:38.633285 domjudge_utility-0.0.6/README.md
--rw-r--r--   0        0        0       71 2023-05-23 14:48:38.637285 domjudge_utility-0.0.6/domjudge_utility/__init__.py
--rw-r--r--   0        0        0    21894 2023-05-23 14:48:38.637285 domjudge_utility-0.0.6/domjudge_utility/dump.py
--rw-r--r--   0        0        0     3165 2023-05-23 14:48:38.637285 domjudge_utility-0.0.6/domjudge_utility/dump_config.py
--rw-r--r--   0        0        0      394 2023-05-23 14:48:38.637285 domjudge_utility-0.0.6/domjudge_utility/utils.py
--rw-r--r--   0        0        0       22 2023-05-23 14:48:38.637285 domjudge_utility-0.0.6/domjudge_utility/version.py
--rw-r--r--   0        0        0     1161 2023-05-23 14:48:38.637285 domjudge_utility-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-25 12:41:33.655414 domjudge_utility-0.0.7/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-25 12:41:33.655414 domjudge_utility-0.0.7/README.md
+-rw-r--r--   0        0        0       47 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/__init__.py
+-rw-r--r--   0        0        0    21911 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/dump.py
+-rw-r--r--   0        0        0     3165 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/dump_config.py
+-rw-r--r--   0        0        0      394 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/utils.py
+-rw-r--r--   0        0        0       22 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/version.py
+-rw-r--r--   0        0        0     1161 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.7/PKG-INFO
```

### Comparing `domjudge_utility-0.0.6/LICENSE` & `domjudge_utility-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.6/README.md` & `domjudge_utility-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.6/domjudge_utility/dump.py` & `domjudge_utility-0.0.7/domjudge_utility/dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,16 @@
                 charset = content_type.split("charset=")[1]
                 content = resp.content.decode(charset)
             else:
                 content = resp.content.decode()
 
             return content
         else:
-            file_path = os.path.join(self.config.base_file_path, "domjudge", "api", endpoint)
+            file_path = os.path.join(
+                self.config.base_file_path, "domjudge", "api", endpoint)
             self.logger.info('GET {}'.format(file_path))
             with open(file_path, 'r') as f:
                 return f.read()
 
     def image_download(self, img_url: str, dist: str):
         self.logger.info(
             "download image. [img_url=%s] [dist=%s]", img_url, dist)
```

### Comparing `domjudge_utility-0.0.6/domjudge_utility/dump_config.py` & `domjudge_utility-0.0.7/domjudge_utility/dump_config.py`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.6/pyproject.toml` & `domjudge_utility-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domjudge-utility"
-version = "0.0.6"
+version = "0.0.7"
 description = "DOMjudge Utility"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `domjudge_utility-0.0.6/PKG-INFO` & `domjudge_utility-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domjudge-utility
-Version: 0.0.6
+Version: 0.0.7
 Summary: DOMjudge Utility
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

