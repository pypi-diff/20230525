# Comparing `tmp/pygeoweaver-0.6.5.tar.gz` & `tmp/pygeoweaver-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.5.tar", last modified: Tue Apr 18 23:58:01 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.6.tar", last modified: Thu May 25 18:50:39 2023, max compression
```

## Comparing `pygeoweaver-0.6.5.tar` & `pygeoweaver-0.6.6.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:58:01.248442 pygeoweaver-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-18 23:58:01.248442 pygeoweaver-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:58:01.248442 pygeoweaver-0.6.5/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:58:01.248442 pygeoweaver-0.6.5/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-18 23:58:01.000000 pygeoweaver-0.6.5/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 23:58:01.000000 pygeoweaver-0.6.5/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:58:01.000000 pygeoweaver-0.6.5/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 23:58:01.000000 pygeoweaver-0.6.5/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 23:58:01.248442 pygeoweaver-0.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:58:01.248442 pygeoweaver-0.6.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-18 23:57:51.000000 pygeoweaver-0.6.5/test/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-25 18:50:39.015588 pygeoweaver-0.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/test/test_server.py
```

### Comparing `pygeoweaver-0.6.5/LICENSE` & `pygeoweaver-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/PKG-INFO` & `pygeoweaver-0.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.5
+Version: 0.6.6
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.5/README.md` & `pygeoweaver-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver/__main__.py` & `pygeoweaver-0.6.6/pygeoweaver/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The main function of pygeoweaver
 To run in CLI mode. 
 """
 from pygeoweaver import detail_host, detail_process, detail_workflow, export_workflow, \
     show_history, import_workflow, list_hosts, list_processes, list_workflows, \
     start, stop, reset_password, run_process, run_worklfow, helpwith, ui
+from pygeoweaver.server import show
 
 def main():
     # start geoweaver
     # start()
     # stop geoweaver
     # stop()
     # list resources
@@ -33,13 +34,13 @@
     #              environment_list="",)
     # run workflow by zip path
 
     # run workflow by folder path
 
     # reset localhost password for Geoweaver
     # reset_password()
-    ui()
-    helpwith()
+    show()
+    # helpwith()
 
 
 if __name__ == "__main__":
      main()
```

### Comparing `pygeoweaver-0.6.5/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.6/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.6/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver/sc_help.py` & `pygeoweaver-0.6.6/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.6/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.6/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.6/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.5/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.6/pygeoweaver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.5
+Version: 0.6.6
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.5/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.6.6/pygeoweaver.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 pygeoweaver/__init__.py
 pygeoweaver/__main__.py
+pygeoweaver/constants.py
 pygeoweaver/sc_detail.py
 pygeoweaver/sc_export.py
 pygeoweaver/sc_help.py
 pygeoweaver/sc_history.py
 pygeoweaver/sc_import.py
 pygeoweaver/sc_interface.py
 pygeoweaver/sc_list.py
@@ -16,8 +17,9 @@
 pygeoweaver/server.py
 pygeoweaver/utils.py
 pygeoweaver.egg-info/PKG-INFO
 pygeoweaver.egg-info/SOURCES.txt
 pygeoweaver.egg-info/dependency_links.txt
 pygeoweaver.egg-info/top_level.txt
 test/__init__.py
-test/test_all.py
+test/test_detail.py
+test/test_server.py
```

### Comparing `pygeoweaver-0.6.5/pyproject.toml` & `pygeoweaver-0.6.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.5"
+version = "0.6.6"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,19 +18,22 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.6.2"
+version = "0.6.6"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 setuptools = ">=61.0"
 requests = "2.28.2"
 
 [tool.poetry.scripts]
+
+[tool.pytest.ini_options]
+addopts = "-p no:warnings --cov=pygeoweaver --cov-report=html"
```

