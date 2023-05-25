# Comparing `tmp/dbpyman-0.1.2.tar.gz` & `tmp/dbpyman-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbpyman-0.1.2.tar", last modified: Thu May 25 09:46:02 2023, max compression
+gzip compressed data, was "dbpyman-0.1.21.tar", last modified: Thu May 25 09:56:32 2023, max compression
```

## Comparing `dbpyman-0.1.2.tar` & `dbpyman-0.1.21.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:46:02.214996 dbpyman-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3934 2023-05-25 09:46:02.214976 dbpyman-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3345 2023-05-25 09:27:25.000000 dbpyman-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 09:46:02.199494 dbpyman-0.1.2/dbpyman.egg-info/
--rw-rw-rw-   0        0        0     3934 2023-05-25 09:46:02.000000 dbpyman-0.1.2/dbpyman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-25 09:46:02.000000 dbpyman-0.1.2/dbpyman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:46:02.000000 dbpyman-0.1.2/dbpyman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-25 09:46:02.000000 dbpyman-0.1.2/dbpyman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 09:46:02.202192 dbpyman-0.1.2/py_discord_db_management/
--rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1.2/py_discord_db_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:46:02.207682 dbpyman-0.1.2/py_discord_db_management/classes/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1.2/py_discord_db_management/classes/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-05-25 08:18:49.000000 dbpyman-0.1.2/py_discord_db_management/classes/column.py
--rw-rw-rw-   0        0        0     2521 2023-05-25 07:54:11.000000 dbpyman-0.1.2/py_discord_db_management/classes/database.py
--rw-rw-rw-   0        0        0     1041 2023-05-25 08:02:05.000000 dbpyman-0.1.2/py_discord_db_management/classes/table.py
--rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1.2/py_discord_db_management/dbpyman.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:46:02.212543 dbpyman-0.1.2/py_discord_db_management/views/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1.2/py_discord_db_management/views/__init__.py
--rw-rw-rw-   0        0        0     3732 2023-05-25 07:44:53.000000 dbpyman-0.1.2/py_discord_db_management/views/table_add_data_view.py
--rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1.2/py_discord_db_management/views/table_categories_view.py
--rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1.2/py_discord_db_management/views/table_overview_view.py
--rw-rw-rw-   0        0        0      756 2023-05-25 09:45:23.000000 dbpyman-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 09:46:02.214996 dbpyman-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.310547 dbpyman-0.1.21/
+-rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1.21/LICENSE
+-rw-rw-rw-   0        0        0     3935 2023-05-25 09:56:32.310547 dbpyman-0.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0     3345 2023-05-25 09:27:25.000000 dbpyman-0.1.21/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.295664 dbpyman-0.1.21/dbpyman.egg-info/
+-rw-rw-rw-   0        0        0     3935 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.298507 dbpyman-0.1.21/py_discord_db_management/
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1.21/py_discord_db_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.303041 dbpyman-0.1.21/py_discord_db_management/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1.21/py_discord_db_management/classes/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-05-25 08:18:49.000000 dbpyman-0.1.21/py_discord_db_management/classes/column.py
+-rw-rw-rw-   0        0        0     2521 2023-05-25 07:54:11.000000 dbpyman-0.1.21/py_discord_db_management/classes/database.py
+-rw-rw-rw-   0        0        0     1041 2023-05-25 08:02:05.000000 dbpyman-0.1.21/py_discord_db_management/classes/table.py
+-rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1.21/py_discord_db_management/dbpyman.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.307879 dbpyman-0.1.21/py_discord_db_management/views/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1.21/py_discord_db_management/views/__init__.py
+-rw-rw-rw-   0        0        0     3732 2023-05-25 07:44:53.000000 dbpyman-0.1.21/py_discord_db_management/views/table_add_data_view.py
+-rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1.21/py_discord_db_management/views/table_categories_view.py
+-rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1.21/py_discord_db_management/views/table_overview_view.py
+-rw-rw-rw-   0        0        0      578 2023-05-25 09:56:18.000000 dbpyman-0.1.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:56:32.310547 dbpyman-0.1.21/setup.cfg
```

### Comparing `dbpyman-0.1.2/LICENSE` & `dbpyman-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/PKG-INFO` & `dbpyman-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.2
+Version: 0.1.21
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.2/README.md` & `dbpyman-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/dbpyman.egg-info/PKG-INFO` & `dbpyman-0.1.21/dbpyman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.2
+Version: 0.1.21
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.2/dbpyman.egg-info/SOURCES.txt` & `dbpyman-0.1.21/dbpyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/classes/column.py` & `dbpyman-0.1.21/py_discord_db_management/classes/column.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/classes/database.py` & `dbpyman-0.1.21/py_discord_db_management/classes/database.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/classes/table.py` & `dbpyman-0.1.21/py_discord_db_management/classes/table.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/dbpyman.py` & `dbpyman-0.1.21/py_discord_db_management/dbpyman.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/views/table_add_data_view.py` & `dbpyman-0.1.21/py_discord_db_management/views/table_add_data_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/views/table_categories_view.py` & `dbpyman-0.1.21/py_discord_db_management/views/table_categories_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.2/py_discord_db_management/views/table_overview_view.py` & `dbpyman-0.1.21/py_discord_db_management/views/table_overview_view.py`

 * *Files identical despite different names*

