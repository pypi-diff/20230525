# Comparing `tmp/dyn_libs-0.2.5.1.tar.gz` & `tmp/dyn_libs-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dyn_libs-0.2.5.1.tar", last modified: Thu Jun 23 03:53:29 2022, max compression
+gzip compressed data, was "dyn_libs-0.2.6.tar", last modified: Thu May 25 10:00:11 2023, max compression
```

## Comparing `dyn_libs-0.2.5.1.tar` & `dyn_libs-0.2.6.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/controllers/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)    13828 2022-06-23 03:49:51.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     9184 2022-06-15 03:40:51.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        0 2022-02-19 10:14:49.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/controllers/__init__.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1454 2022-02-23 11:30:57.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/es_paginate.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1257 2022-02-22 07:17:02.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/utils.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1777 2022-02-25 04:26:21.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/__init__.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        0 2022-02-10 07:09:45.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/__init__.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1773 2022-02-21 16:29:57.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1831 2022-02-25 04:22:27.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/base_model.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)      991 2022-02-21 07:12:46.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/field_history_model.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)      887 2019-12-01 16:02:42.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/db_manager.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     2912 2022-02-21 16:32:56.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/merchant_config.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        0 2022-02-10 07:23:26.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/__init__.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)      782 2022-02-21 07:13:00.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/elastic/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)      865 2022-02-23 11:30:57.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/elastic/base_model.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        0 2021-09-20 11:12:17.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/elastic/__init__.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        0 2019-12-01 15:37:28.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/__init__.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1655 2022-02-22 07:15:22.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/__init__.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/field_helper/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)    22327 2022-02-25 03:26:58.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/field_helper/base_field.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)      929 2022-02-25 03:19:04.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        0 2022-02-10 07:17:26.000000 dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/field_helper/__init__.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     5933 2022-06-23 03:51:59.000000 dyn_libs-0.2.5.1/README.md
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/dyn_libs.egg-info/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     8550 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/dyn_libs.egg-info/PKG-INFO
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)        1 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/dyn_libs.egg-info/dependency_links.txt
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)       88 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/dyn_libs.egg-info/requires.txt
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1294 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/dyn_libs.egg-info/SOURCES.txt
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)      283 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/dyn_libs.egg-info/top_level.txt
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     8550 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/PKG-INFO
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)       38 2022-06-23 03:53:29.000000 dyn_libs-0.2.5.1/setup.cfg
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     2375 2022-06-23 03:52:08.000000 dyn_libs-0.2.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.991696 dyn_libs-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-05-25 10:00:10.989696 dyn_libs-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.958695 dyn_libs-0.2.6/dyn_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-05-25 10:00:10.000000 dyn_libs-0.2.6/dyn_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-25 10:00:10.000000 dyn_libs-0.2.6/dyn_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:00:10.000000 dyn_libs-0.2.6/dyn_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 10:00:10.000000 dyn_libs-0.2.6/dyn_libs.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-25 10:00:10.000000 dyn_libs-0.2.6/dyn_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 10:00:10.000000 dyn_libs-0.2.6/dyn_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.947695 dyn_libs-0.2.6/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.961695 dyn_libs-0.2.6/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.962695 dyn_libs-0.2.6/mobio/libs/dynamic_field/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.966695 dyn_libs-0.2.6/mobio/libs/dynamic_field/common/
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/common/es_paginate.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.973695 dyn_libs-0.2.6/mobio/libs/dynamic_field/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py
+-rw-r--r--   0 root         (0) root         (0)    13828 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.974695 dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.978695 dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/field_helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/field_helper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22327 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/field_helper/base_field.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.979695 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.982695 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/elastic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/elastic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/elastic/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:00:10.987696 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/db_manager.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/field_history_model.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/merchant_config.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-25 09:58:38.000000 dyn_libs-0.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:00:10.991696 dyn_libs-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9279 2023-05-25 10:00:09.000000 dyn_libs-0.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/es_paginate.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/common/es_paginate.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/utils.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/common/utils.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/common/__init__.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/base_model.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/base_model.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/field_history_model.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/field_history_model.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/db_manager.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/db_manager.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/merchant_config.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/merchant_config.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/models/elastic/base_model.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/models/elastic/base_model.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/__init__.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/field_helper/base_field.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/field_helper/base_field.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py` & `dyn_libs-0.2.6/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.5.1/README.md` & `dyn_libs-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,16 @@
 [Elastic]
 index = dyn_test
 doc_type = df
 ```
 
 
 # Change logs
+* 0.2.6
+    - upgrade requests library
 * 0.2.5.1
     1) fix issue remove doc_type
     2) fix issue missing after_token
 * 0.2.5
     1) remove doc_type
 * 0.2.4
     1) upgrade elasticsearch_client to 7.17.4
```

### Comparing `dyn_libs-0.2.5.1/dyn_libs.egg-info/PKG-INFO` & `dyn_libs-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: dyn-libs
-Version: 0.2.5.1
+Name: dyn_libs
+Version: 0.2.6
 Summary: Mobio Dynamic Fields
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
+Project-URL: Source, https://github.com/mobiovn
 Description: # install_requires
         <pre>
         m-singleton==0.3 
         pymongo==3.7.2
         requests==2.25.1
         unidecode==1.1.1
         elasticsearch==7.17.4
@@ -186,14 +187,16 @@
         [Elastic]
         index = dyn_test
         doc_type = df
         ```
         
         
         # Change logs
+        * 0.2.6
+            - upgrade requests library
         * 0.2.5.1
             1) fix issue remove doc_type
             2) fix issue missing after_token
         * 0.2.5
             1) remove doc_type
         * 0.2.4
             1) upgrade elasticsearch_client to 7.17.4
@@ -215,22 +218,21 @@
             2) change function args <b>add_els_config</b>
             <pre>
             def add_els_config(self, index, doc_type):
                 self.index = index
                 self.doc_type = doc_type
             </pre>
         
+Keywords: mobio,dyn_libs
 Platform: UNKNOWN
-Classifier: Topic :: Software Development
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `dyn_libs-0.2.5.1/dyn_libs.egg-info/SOURCES.txt` & `dyn_libs-0.2.6/dyn_libs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 README.md
+pyproject.toml
 setup.py
 dyn_libs.egg-info/PKG-INFO
 dyn_libs.egg-info/SOURCES.txt
 dyn_libs.egg-info/dependency_links.txt
+dyn_libs.egg-info/namespace_packages.txt
 dyn_libs.egg-info/requires.txt
 dyn_libs.egg-info/top_level.txt
+mobio/libs/__init__.py
 mobio/libs/dynamic_field/__init__.py
 mobio/libs/dynamic_field/common/__init__.py
 mobio/libs/dynamic_field/common/es_paginate.py
 mobio/libs/dynamic_field/common/utils.py
 mobio/libs/dynamic_field/controllers/__init__.py
 mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py
 mobio/libs/dynamic_field/controllers/i_base_filter_controller.py
```

### Comparing `dyn_libs-0.2.5.1/PKG-INFO` & `dyn_libs-0.2.6/dyn_libs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: dyn_libs
-Version: 0.2.5.1
+Name: dyn-libs
+Version: 0.2.6
 Summary: Mobio Dynamic Fields
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
+Project-URL: Source, https://github.com/mobiovn
 Description: # install_requires
         <pre>
         m-singleton==0.3 
         pymongo==3.7.2
         requests==2.25.1
         unidecode==1.1.1
         elasticsearch==7.17.4
@@ -186,14 +187,16 @@
         [Elastic]
         index = dyn_test
         doc_type = df
         ```
         
         
         # Change logs
+        * 0.2.6
+            - upgrade requests library
         * 0.2.5.1
             1) fix issue remove doc_type
             2) fix issue missing after_token
         * 0.2.5
             1) remove doc_type
         * 0.2.4
             1) upgrade elasticsearch_client to 7.17.4
@@ -215,22 +218,21 @@
             2) change function args <b>add_els_config</b>
             <pre>
             def add_els_config(self, index, doc_type):
                 self.index = index
                 self.doc_type = doc_type
             </pre>
         
+Keywords: mobio,dyn_libs
 Platform: UNKNOWN
-Classifier: Topic :: Software Development
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3
 Description-Content-Type: text/markdown
```

