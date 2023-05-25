# Comparing `tmp/dbpyman-0.1.tar.gz` & `tmp/dbpyman-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbpyman-0.1.tar", last modified: Thu May 25 08:47:41 2023, max compression
+gzip compressed data, was "dbpyman-0.1.1.tar", last modified: Thu May 25 09:27:48 2023, max compression
```

## Comparing `dbpyman-0.1.tar` & `dbpyman-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 08:47:41.832795 dbpyman-0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1/LICENSE
--rw-rw-rw-   0        0        0      900 2023-05-25 08:47:41.832795 dbpyman-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-25 07:06:40.000000 dbpyman-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 08:47:41.816794 dbpyman-0.1/dbpyman.egg-info/
--rw-rw-rw-   0        0        0      900 2023-05-25 08:47:41.000000 dbpyman-0.1/dbpyman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-25 08:47:41.000000 dbpyman-0.1/dbpyman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 08:47:41.000000 dbpyman-0.1/dbpyman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-25 08:47:41.000000 dbpyman-0.1/dbpyman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 08:47:41.819247 dbpyman-0.1/py_discord_db_management/
--rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1/py_discord_db_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:47:41.825346 dbpyman-0.1/py_discord_db_management/classes/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1/py_discord_db_management/classes/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-05-25 08:18:49.000000 dbpyman-0.1/py_discord_db_management/classes/column.py
--rw-rw-rw-   0        0        0     2521 2023-05-25 07:54:11.000000 dbpyman-0.1/py_discord_db_management/classes/database.py
--rw-rw-rw-   0        0        0     1041 2023-05-25 08:02:05.000000 dbpyman-0.1/py_discord_db_management/classes/table.py
--rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1/py_discord_db_management/dbpyman.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:47:41.830238 dbpyman-0.1/py_discord_db_management/views/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1/py_discord_db_management/views/__init__.py
--rw-rw-rw-   0        0        0     3732 2023-05-25 07:44:53.000000 dbpyman-0.1/py_discord_db_management/views/table_add_data_view.py
--rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1/py_discord_db_management/views/table_categories_view.py
--rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1/py_discord_db_management/views/table_overview_view.py
--rw-rw-rw-   0        0        0      575 2023-05-25 08:47:21.000000 dbpyman-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 08:47:41.832795 dbpyman-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 09:27:48.561160 dbpyman-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3934 2023-05-25 09:27:48.558422 dbpyman-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3345 2023-05-25 09:27:25.000000 dbpyman-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:27:48.543831 dbpyman-0.1.1/dbpyman.egg-info/
+-rw-rw-rw-   0        0        0     3934 2023-05-25 09:27:48.000000 dbpyman-0.1.1/dbpyman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-25 09:27:48.000000 dbpyman-0.1.1/dbpyman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:27:48.000000 dbpyman-0.1.1/dbpyman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-25 09:27:48.000000 dbpyman-0.1.1/dbpyman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 09:27:48.546757 dbpyman-0.1.1/py_discord_db_management/
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1.1/py_discord_db_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:27:48.552711 dbpyman-0.1.1/py_discord_db_management/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1.1/py_discord_db_management/classes/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-05-25 08:18:49.000000 dbpyman-0.1.1/py_discord_db_management/classes/column.py
+-rw-rw-rw-   0        0        0     2521 2023-05-25 07:54:11.000000 dbpyman-0.1.1/py_discord_db_management/classes/database.py
+-rw-rw-rw-   0        0        0     1041 2023-05-25 08:02:05.000000 dbpyman-0.1.1/py_discord_db_management/classes/table.py
+-rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1.1/py_discord_db_management/dbpyman.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:27:48.558422 dbpyman-0.1.1/py_discord_db_management/views/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1.1/py_discord_db_management/views/__init__.py
+-rw-rw-rw-   0        0        0     3732 2023-05-25 07:44:53.000000 dbpyman-0.1.1/py_discord_db_management/views/table_add_data_view.py
+-rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1.1/py_discord_db_management/views/table_categories_view.py
+-rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1.1/py_discord_db_management/views/table_overview_view.py
+-rw-rw-rw-   0        0        0      577 2023-05-25 09:27:33.000000 dbpyman-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:27:48.561160 dbpyman-0.1.1/setup.cfg
```

### Comparing `dbpyman-0.1/LICENSE` & `dbpyman-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/dbpyman.egg-info/SOURCES.txt` & `dbpyman-0.1.1/dbpyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/classes/column.py` & `dbpyman-0.1.1/py_discord_db_management/classes/column.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/classes/database.py` & `dbpyman-0.1.1/py_discord_db_management/classes/database.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/classes/table.py` & `dbpyman-0.1.1/py_discord_db_management/classes/table.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/dbpyman.py` & `dbpyman-0.1.1/py_discord_db_management/dbpyman.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/views/table_add_data_view.py` & `dbpyman-0.1.1/py_discord_db_management/views/table_add_data_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/views/table_categories_view.py` & `dbpyman-0.1.1/py_discord_db_management/views/table_categories_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/py_discord_db_management/views/table_overview_view.py` & `dbpyman-0.1.1/py_discord_db_management/views/table_overview_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1/pyproject.toml` & `dbpyman-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbpyman"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="JanikCodes", email="janiksielaff@gmx.de" },
 ]
 description = "A package used to modify & view your MySQL database data dynamically"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

