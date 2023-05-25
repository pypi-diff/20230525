# Comparing `tmp/endi_celery-6.5.9.tar.gz` & `tmp/endi_celery-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endi_celery-6.5.9.tar", last modified: Wed Mar  8 16:49:13 2023, max compression
+gzip compressed data, was "endi_celery-6.6.0.tar", last modified: Thu May 25 15:55:42 2023, max compression
```

## Comparing `endi_celery-6.5.9.tar` & `endi_celery-6.6.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-03-08 16:49:13.046133 endi_celery-6.5.9/
--rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-03-08 16:48:50.000000 endi_celery-6.5.9/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.5.9/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.5.9/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-03-08 16:49:13.046133 endi_celery-6.5.9/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-01-17 16:17:56.000000 endi_celery-6.5.9/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)     4726 2023-02-07 15:10:17.000000 endi_celery-6.5.9/development.ini
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-03-08 16:49:13.041133 endi_celery-6.5.9/endi_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4486 2023-01-11 11:00:06.000000 endi_celery-6.5.9/endi_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.5.9/endi_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.5.9/endi_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.5.9/endi_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.5.9/endi_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.5.9/endi_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.5.9/endi_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.5.9/endi_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-03-08 16:49:13.042133 endi_celery-6.5.9/endi_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.5.9/endi_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.5.9/endi_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2966 2023-01-11 11:02:40.000000 endi_celery-6.5.9/endi_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-03-07 14:08:09.000000 endi_celery-6.5.9/endi_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-03-08 16:49:13.043133 endi_celery-6.5.9/endi_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.5.9/endi_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.5.9/endi_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-03-08 16:49:13.045133 endi_celery-6.5.9/endi_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)     8087 2022-12-09 15:12:22.000000 endi_celery-6.5.9/endi_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39470 2023-02-08 16:49:51.000000 endi_celery-6.5.9/endi_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.5.9/endi_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.5.9/endi_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)     8649 2022-12-09 15:12:23.000000 endi_celery-6.5.9/endi_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.5.9/endi_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.5.9/endi_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.5.9/endi_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.5.9/endi_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-03-08 16:49:13.042133 endi_celery-6.5.9/endi_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-03-08 16:49:12.000000 endi_celery-6.5.9/endi_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1039 2023-03-08 16:49:13.000000 endi_celery-6.5.9/endi_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-03-08 16:49:12.000000 endi_celery-6.5.9/endi_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-03-08 16:49:12.000000 endi_celery-6.5.9/endi_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.5.9/endi_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-03-08 16:49:12.000000 endi_celery-6.5.9/endi_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-03-08 16:49:12.000000 endi_celery-6.5.9/endi_celery.egg-info/top_level.txt
--rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.5.9/prod_example.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.5.9/pytest.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.5.9/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-03-08 16:49:13.046133 endi_celery-6.5.9/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-01-17 16:18:35.000000 endi_celery-6.5.9/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.267074 endi_celery-6.6.0/
+-rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-05-25 15:55:13.000000 endi_celery-6.6.0/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.0/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.0/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-05-25 15:55:42.267074 endi_celery-6.6.0/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.0/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.0/development.ini
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.264074 endi_celery-6.6.0/endi_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.0/endi_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.0/endi_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.0/endi_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.0/endi_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.0/endi_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.0/endi_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.265075 endi_celery-6.6.0/endi_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.0/endi_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.0/endi_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.0/endi_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2966 2023-01-11 11:02:40.000000 endi_celery-6.6.0/endi_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.0/endi_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.265075 endi_celery-6.6.0/endi_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.0/endi_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.266075 endi_celery-6.6.0/endi_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)     8087 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39473 2023-05-25 15:25:03.000000 endi_celery-6.6.0/endi_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.0/endi_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.0/endi_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    13542 2023-05-25 15:32:59.000000 endi_celery-6.6.0/endi_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.0/endi_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.0/endi_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.0/endi_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.0/endi_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.0/endi_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.264074 endi_celery-6.6.0/endi_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-05-25 15:55:41.000000 endi_celery-6.6.0/endi_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-05-25 15:55:42.000000 endi_celery-6.6.0/endi_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-05-25 15:55:41.000000 endi_celery-6.6.0/endi_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-05-25 15:55:41.000000 endi_celery-6.6.0/endi_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.0/endi_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-05-25 15:55:42.000000 endi_celery-6.6.0/endi_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-05-25 15:55:42.000000 endi_celery-6.6.0/endi_celery.egg-info/top_level.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.0/prod_example.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.0/pytest.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.0/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-05-25 15:55:42.267074 endi_celery-6.6.0/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-01-17 16:18:35.000000 endi_celery-6.6.0/setup.py
```

### Comparing `endi_celery-6.5.9/LICENSE.txt` & `endi_celery-6.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/PKG-INFO` & `endi_celery-6.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi_celery
-Version: 6.5.9
+Version: 6.6.0
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.5.9/README.rst` & `endi_celery-6.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/development.ini` & `endi_celery-6.6.0/development.ini`

 * *Files 6% similar despite different names*

```diff
@@ -76,27 +76,38 @@
     endi_celery.tasks.csv_import
     endi_celery.tasks.export
     endi_celery.tasks.accounting_measure_compute
     endi_celery.tasks.accounting_parser
     endi.plugins.sap.celery_jobs
     endi.plugins.sap_urssaf3p.celery_jobs
     endi.plugins.sap.celery_jobs
+    endi_celery.tasks.notification
 
 #    endi_edocsafe.tasks
 
 task_serializer = json
 accept_content=
                 json
                 yaml
 
 [celerybeat:accounting_parser]
 task = endi_celery.tasks.accounting_parser.handle_pool_task
 type = timedelta
 schedule = {"seconds": 180}
 
+[celerybeat:publish_pending_notifications]
+task = endi_celery.tasks.notification.publish_pending_notifications
+type = timedelta
+schedule = {"hours": 12}
+
+[celerybeat:clean_notifications]
+task = endi_celery.tasks.notification.clean_notifications
+type = timedelta
+schedule = {"days": 2}
+
 [server:main]
 use = egg:waitress#main
 host = 0.0.0.0
 #host= 0.0.0.0
 port = 8080
 
 [pshell]
```

### Comparing `endi_celery-6.5.9/endi_celery/__init__.py` & `endi_celery-6.6.0/endi_celery/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     """
     Includes some celery specific stuff in the main application
     """
     settings = config.get_settings()
     configure_accounting_parser_service(config, settings)
     config.add_directive("register_import_model", register_import_model)
     config.add_directive("register_export_model", register_export_model)
+    config.include("endi.views.invoices.routes")
     config.include("endi_celery.tasks")
 
 
 def worker(global_config, **settings):
     """
     Entry point for the pyramid celery stuff
     """
```

### Comparing `endi_celery-6.5.9/endi_celery/conf.py` & `endi_celery-6.6.0/endi_celery/conf.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/exception.py` & `endi_celery-6.6.0/endi_celery/exception.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/interfaces.py` & `endi_celery-6.6.0/endi_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/mail.py` & `endi_celery-6.6.0/endi_celery/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/models.py` & `endi_celery-6.6.0/endi_celery/models.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/parsers/__init__.py` & `endi_celery-6.6.0/endi_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/parsers/quadra.py` & `endi_celery-6.6.0/endi_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/parsers/sage.py` & `endi_celery-6.6.0/endi_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/parsers/sage_generation_expert.py` & `endi_celery-6.6.0/endi_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/tasks/__init__.py` & `endi_celery-6.6.0/endi_celery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/tasks/accounting_measure_compute.py` & `endi_celery-6.6.0/endi_celery/tasks/accounting_measure_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         """
         Update the category total value for a given measure type in the grid's
         cache
 
         :param obj measure: A child of BaseTreasuryMeasure
         """
         measure_type = measure.measure_type
-        if not measure_type.computed_total:
+        if not measure_type.is_computed_total:
             if measure_type.category_id not in self._category_totals:
                 self._category_totals[measure_type.category_id] = 0
             self._category_totals[measure_type.category_id] += measure.value
 
     def get_type_total(self, typ_id):
         """
         Get the total type for a given measure type
```

### Comparing `endi_celery-6.5.9/endi_celery/tasks/accounting_parser.py` & `endi_celery-6.6.0/endi_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/tasks/csv_import.py` & `endi_celery-6.6.0/endi_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/tasks/mail.py` & `endi_celery-6.6.0/endi_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/tasks/tasks.py` & `endi_celery-6.6.0/endi_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/tasks/utils.py` & `endi_celery-6.6.0/endi_celery/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery/transactional_task.py` & `endi_celery-6.6.0/endi_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/endi_celery.egg-info/PKG-INFO` & `endi_celery-6.6.0/endi_celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi-celery
-Version: 6.5.9
+Version: 6.6.0
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.5.9/endi_celery.egg-info/SOURCES.txt` & `endi_celery-6.6.0/endi_celery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 endi_celery.egg-info/SOURCES.txt
 endi_celery.egg-info/dependency_links.txt
 endi_celery.egg-info/entry_points.txt
 endi_celery.egg-info/not-zip-safe
 endi_celery.egg-info/requires.txt
 endi_celery.egg-info/top_level.txt
 endi_celery/parsers/__init__.py
+endi_celery/parsers/isacompta.py
 endi_celery/parsers/quadra.py
 endi_celery/parsers/sage.py
 endi_celery/parsers/sage_generation_expert.py
 endi_celery/schedulers/__init__.py
 endi_celery/schedulers/tasks.py
 endi_celery/tasks/__init__.py
 endi_celery/tasks/accounting_measure_compute.py
 endi_celery/tasks/accounting_parser.py
 endi_celery/tasks/csv_import.py
 endi_celery/tasks/export.py
 endi_celery/tasks/mail.py
+endi_celery/tasks/notification.py
 endi_celery/tasks/tasks.py
 endi_celery/tasks/utils.py
```

### Comparing `endi_celery-6.5.9/prod_example.ini` & `endi_celery-6.6.0/prod_example.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.5.9/setup.py` & `endi_celery-6.6.0/setup.py`

 * *Files identical despite different names*

