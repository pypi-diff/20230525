# Comparing `tmp/spswarehouse-0.3.0.tar.gz` & `tmp/spswarehouse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.3.0.tar", last modified: Thu May 25 16:11:54 2023, max compression
+gzip compressed data, was "spswarehouse-0.3.1.tar", last modified: Thu May 25 16:20:38 2023, max compression
```

## Comparing `spswarehouse-0.3.0.tar` & `spswarehouse-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.461835 spswarehouse-0.3.0/
--rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8200 2023-05-25 16:11:54.459868 spswarehouse-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 16:11:54.461835 spswarehouse-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-05-25 16:11:09.000000 spswarehouse-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.439070 spswarehouse-0.3.0/spswarehouse/
--rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.3.0/spswarehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.450861 spswarehouse-0.3.0/spswarehouse/calpads/
--rw-rw-rw-   0        0        0        0 2023-05-17 18:23:32.000000 spswarehouse-0.3.0/spswarehouse/calpads/__init__.py
--rw-rw-rw-   0        0        0    40625 2023-05-25 16:11:09.000000 spswarehouse-0.3.0/spswarehouse/calpads/calpads.py
--rw-rw-rw-   0        0        0     6136 2023-05-25 16:11:09.000000 spswarehouse-0.3.0/spswarehouse/calpads/calpads_config.py
--rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.3.0/spswarehouse/credentials.py.template
--rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.3.0/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.3.0/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.3.0/spswarehouse/googleslides.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.456868 spswarehouse-0.3.0/spswarehouse/powerschool/
--rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.3.0/spswarehouse/powerschool/__init__.py
--rw-rw-rw-   0        0        0    21622 2023-05-17 17:25:10.000000 spswarehouse-0.3.0/spswarehouse/powerschool/powerschool.py
--rw-rw-rw-   0        0        0    29877 2023-05-15 20:19:39.000000 spswarehouse-0.3.0/spswarehouse/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0      302 2023-05-17 18:23:32.000000 spswarehouse-0.3.0/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.3.0/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.3.0/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.446273 spswarehouse-0.3.0/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8200 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.537935 spswarehouse-0.3.1/
+-rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2023-05-25 16:20:38.534528 spswarehouse-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 16:20:38.537935 spswarehouse-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-25 16:20:09.000000 spswarehouse-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.498908 spswarehouse-0.3.1/spswarehouse/
+-rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.3.1/spswarehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.521589 spswarehouse-0.3.1/spswarehouse/calpads/
+-rw-rw-rw-   0        0        0        0 2023-05-17 18:23:32.000000 spswarehouse-0.3.1/spswarehouse/calpads/__init__.py
+-rw-rw-rw-   0        0        0    40625 2023-05-25 16:11:09.000000 spswarehouse-0.3.1/spswarehouse/calpads/calpads.py
+-rw-rw-rw-   0        0        0     6136 2023-05-25 16:11:09.000000 spswarehouse-0.3.1/spswarehouse/calpads/calpads_config.py
+-rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.3.1/spswarehouse/credentials.py.template
+-rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.3.1/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.3.1/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.3.1/spswarehouse/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.530139 spswarehouse-0.3.1/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.3.1/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    21618 2023-05-25 16:20:04.000000 spswarehouse-0.3.1/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    29877 2023-05-15 20:19:39.000000 spswarehouse-0.3.1/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0      302 2023-05-17 18:23:32.000000 spswarehouse-0.3.1/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.3.1/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.3.1/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.511771 spswarehouse-0.3.1/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.3.0/LICENSE` & `spswarehouse-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/PKG-INFO` & `spswarehouse-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.3.0/README.md` & `spswarehouse-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/__init__.py` & `spswarehouse-0.3.1/spswarehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/calpads/calpads.py` & `spswarehouse-0.3.1/spswarehouse/calpads/calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/calpads/calpads_config.py` & `spswarehouse-0.3.1/spswarehouse/calpads/calpads_config.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/credentials.py.template` & `spswarehouse-0.3.1/spswarehouse/credentials.py.template`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/googledrive.py` & `spswarehouse-0.3.1/spswarehouse/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/googlesheets.py` & `spswarehouse-0.3.1/spswarehouse/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/googleslides.py` & `spswarehouse-0.3.1/spswarehouse/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/powerschool/powerschool.py` & `spswarehouse-0.3.1/spswarehouse/powerschool/powerschool.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             logging.info("School Picker found. Click it.")
 
             elem.click()
 
             time.sleep(1)
 
             logging.info("Waiting for School Search Field")
-            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
+            elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 
                 'schoolSearchField_value')))
             logging.info("Found School Search Field. Typing in school name.")
 
             elem.send_keys(school_name)
 
             time.sleep(1)
```

### Comparing `spswarehouse-0.3.0/spswarehouse/powerschool/powerschool_calpads.py` & `spswarehouse-0.3.1/spswarehouse/powerschool/powerschool_calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/table_names.py` & `spswarehouse-0.3.1/spswarehouse/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/table_utils.py` & `spswarehouse-0.3.1/spswarehouse/table_utils.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse/warehouse.py` & `spswarehouse-0.3.1/spswarehouse/warehouse.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.0/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.3.1/spswarehouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.3.0/spswarehouse.egg-info/SOURCES.txt` & `spswarehouse-0.3.1/spswarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

