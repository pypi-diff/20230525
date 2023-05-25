# Comparing `tmp/dbpyman-0.1.21.tar.gz` & `tmp/dbpyman-0.1.211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbpyman-0.1.21.tar", last modified: Thu May 25 09:56:32 2023, max compression
+gzip compressed data, was "dbpyman-0.1.211.tar", last modified: Thu May 25 12:03:47 2023, max compression
```

## Comparing `dbpyman-0.1.21.tar` & `dbpyman-0.1.211.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.310547 dbpyman-0.1.21/
--rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1.21/LICENSE
--rw-rw-rw-   0        0        0     3935 2023-05-25 09:56:32.310547 dbpyman-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0     3345 2023-05-25 09:27:25.000000 dbpyman-0.1.21/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.295664 dbpyman-0.1.21/dbpyman.egg-info/
--rw-rw-rw-   0        0        0     3935 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-25 09:56:32.000000 dbpyman-0.1.21/dbpyman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.298507 dbpyman-0.1.21/py_discord_db_management/
--rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1.21/py_discord_db_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.303041 dbpyman-0.1.21/py_discord_db_management/classes/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1.21/py_discord_db_management/classes/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-05-25 08:18:49.000000 dbpyman-0.1.21/py_discord_db_management/classes/column.py
--rw-rw-rw-   0        0        0     2521 2023-05-25 07:54:11.000000 dbpyman-0.1.21/py_discord_db_management/classes/database.py
--rw-rw-rw-   0        0        0     1041 2023-05-25 08:02:05.000000 dbpyman-0.1.21/py_discord_db_management/classes/table.py
--rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1.21/py_discord_db_management/dbpyman.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:56:32.307879 dbpyman-0.1.21/py_discord_db_management/views/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1.21/py_discord_db_management/views/__init__.py
--rw-rw-rw-   0        0        0     3732 2023-05-25 07:44:53.000000 dbpyman-0.1.21/py_discord_db_management/views/table_add_data_view.py
--rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1.21/py_discord_db_management/views/table_categories_view.py
--rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1.21/py_discord_db_management/views/table_overview_view.py
--rw-rw-rw-   0        0        0      578 2023-05-25 09:56:18.000000 dbpyman-0.1.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 09:56:32.310547 dbpyman-0.1.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 12:03:47.427592 dbpyman-0.1.211/
+-rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1.211/LICENSE
+-rw-rw-rw-   0        0        0     3936 2023-05-25 12:03:47.427592 dbpyman-0.1.211/PKG-INFO
+-rw-rw-rw-   0        0        0     3345 2023-05-25 12:02:42.000000 dbpyman-0.1.211/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:03:47.412774 dbpyman-0.1.211/dbpyman.egg-info/
+-rw-rw-rw-   0        0        0     3936 2023-05-25 12:03:47.000000 dbpyman-0.1.211/dbpyman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-25 12:03:47.000000 dbpyman-0.1.211/dbpyman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:03:47.000000 dbpyman-0.1.211/dbpyman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-25 12:03:47.000000 dbpyman-0.1.211/dbpyman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 12:03:47.412774 dbpyman-0.1.211/py_discord_db_management/
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1.211/py_discord_db_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:03:47.418597 dbpyman-0.1.211/py_discord_db_management/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1.211/py_discord_db_management/classes/__init__.py
+-rw-rw-rw-   0        0        0     1560 2023-05-25 11:55:34.000000 dbpyman-0.1.211/py_discord_db_management/classes/column.py
+-rw-rw-rw-   0        0        0     3134 2023-05-25 11:55:56.000000 dbpyman-0.1.211/py_discord_db_management/classes/database.py
+-rw-rw-rw-   0        0        0     1043 2023-05-25 11:55:56.000000 dbpyman-0.1.211/py_discord_db_management/classes/table.py
+-rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1.211/py_discord_db_management/dbpyman.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:03:47.424685 dbpyman-0.1.211/py_discord_db_management/views/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1.211/py_discord_db_management/views/__init__.py
+-rw-rw-rw-   0        0        0     3785 2023-05-25 11:57:33.000000 dbpyman-0.1.211/py_discord_db_management/views/table_add_data_view.py
+-rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1.211/py_discord_db_management/views/table_categories_view.py
+-rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1.211/py_discord_db_management/views/table_overview_view.py
+-rw-rw-rw-   0        0        0      579 2023-05-25 12:03:33.000000 dbpyman-0.1.211/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:03:47.427592 dbpyman-0.1.211/setup.cfg
```

### Comparing `dbpyman-0.1.21/LICENSE` & `dbpyman-0.1.211/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.21/PKG-INFO` & `dbpyman-0.1.211/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.21
+Version: 0.1.211
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,19 @@
 License-File: LICENSE
 
 ## Discord Mysql Management Framework
 This package is used to dynamically **add new data** to your existing Mysql tables.<br>
 You're also able to **delete** or **view** data.<br>
 It'll return you an embed & a view for you to send back.
 
+### Built With
+[![Python][python]][python-url]
+[![MySQL][mysql]][mysql-url]
+![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)
+
 ### How to get started
 1. Install the package
 ```py
 pip install dbpyman
 ```
 2. Create a new command for your discord Bot and create a `database` object inside that.
 ```py
@@ -82,17 +87,12 @@
 embed, view = dbpyman.create_db_management(database)
 ```
 
 ### Contribute
 Feel free to contribute to the project, it's open source.<br>
 It's probably possible to *not only* support MySQL and work with inheritance to allow other database types.
 
-### Built With
-[![Python][python]][python-url]
-[![MySQL][mysql]][mysql-url]
-![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)
-
 <!-- MARKDOWN LINKS & IMAGES -->
 [python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
 [mysql]: https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white
 [mysql-url]: https://www.mysql.com/
 [python-url]: https://www.python.org/
```

### Comparing `dbpyman-0.1.21/README.md` & `dbpyman-0.1.211/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 ## Discord Mysql Management Framework
 This package is used to dynamically **add new data** to your existing Mysql tables.<br>
 You're also able to **delete** or **view** data.<br>
 It'll return you an embed & a view for you to send back.
 
+### Built With
+[![Python][python]][python-url]
+[![MySQL][mysql]][mysql-url]
+![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)
+
 ### How to get started
 1. Install the package
 ```py
 pip install dbpyman
 ```
 2. Create a new command for your discord Bot and create a `database` object inside that.
 ```py
@@ -68,17 +73,12 @@
 embed, view = dbpyman.create_db_management(database)
 ```
 
 ### Contribute
 Feel free to contribute to the project, it's open source.<br>
 It's probably possible to *not only* support MySQL and work with inheritance to allow other database types.
 
-### Built With
-[![Python][python]][python-url]
-[![MySQL][mysql]][mysql-url]
-![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)
-
 <!-- MARKDOWN LINKS & IMAGES -->
 [python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
 [mysql]: https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white
 [mysql-url]: https://www.mysql.com/
 [python-url]: https://www.python.org/
```

### Comparing `dbpyman-0.1.21/dbpyman.egg-info/PKG-INFO` & `dbpyman-0.1.211/dbpyman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.21
+Version: 0.1.211
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,19 @@
 License-File: LICENSE
 
 ## Discord Mysql Management Framework
 This package is used to dynamically **add new data** to your existing Mysql tables.<br>
 You're also able to **delete** or **view** data.<br>
 It'll return you an embed & a view for you to send back.
 
+### Built With
+[![Python][python]][python-url]
+[![MySQL][mysql]][mysql-url]
+![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)
+
 ### How to get started
 1. Install the package
 ```py
 pip install dbpyman
 ```
 2. Create a new command for your discord Bot and create a `database` object inside that.
 ```py
@@ -82,17 +87,12 @@
 embed, view = dbpyman.create_db_management(database)
 ```
 
 ### Contribute
 Feel free to contribute to the project, it's open source.<br>
 It's probably possible to *not only* support MySQL and work with inheritance to allow other database types.
 
-### Built With
-[![Python][python]][python-url]
-[![MySQL][mysql]][mysql-url]
-![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)
-
 <!-- MARKDOWN LINKS & IMAGES -->
 [python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
 [mysql]: https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white
 [mysql-url]: https://www.mysql.com/
 [python-url]: https://www.python.org/
```

### Comparing `dbpyman-0.1.21/dbpyman.egg-info/SOURCES.txt` & `dbpyman-0.1.211/dbpyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.21/py_discord_db_management/classes/column.py` & `dbpyman-0.1.211/py_discord_db_management/classes/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,21 @@
         self.__null = null
         self.__key = key
         self.__default = default
         self.__extra = extra
 
         # variable that is used to attach values to that specific column
         self.__attached_data = None
+        self.__hidden = False
+
+    def get_hidden(self):
+        return self.__hidden
+
+    def set_hidden(self, new_visibility):
+        self.__hidden = new_visibility
 
     def set_attached_data(self, attached_data):
         # value is empty
         if not attached_data:
             self.__attached_data = self.__default
         else:
             self.__attached_data = attached_data
```

### Comparing `dbpyman-0.1.21/py_discord_db_management/classes/database.py` & `dbpyman-0.1.211/py_discord_db_management/classes/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,27 @@
         for table in self.tables:
             if table.get_table_name().lower() == table_name.lower():
                 # we found the table
                 table.set_hidden(True)
                 return
 
         warnings.warn(f"Couldn't find table with name: {table_name}")
+
+    def set_column_hidden(self, table_name, column_name):
+        for table in self.tables:
+            if table.get_table_name().lower() == table_name.lower():
+                # we found the table
+                for column in table.get_columns():
+                    if column.get_field().lower() == column_name.lower():
+                        # we found the column
+                        column.set_hidden(True)
+                        return
+
+                warnings.warn(f"Couldn't find column with name: {column_name}")
+        warnings.warn(f"Couldn't find table with name: {table_name}")
     def set_column_default_value(self, table_name, column_name, value):
         for table in self.tables:
             if table.get_table_name().lower() == table_name.lower():
                 # we found the table
                 for column in table.get_columns():
                     if column.get_field().lower() == column_name.lower():
                         # we found the column
```

### Comparing `dbpyman-0.1.21/py_discord_db_management/classes/table.py` & `dbpyman-0.1.211/py_discord_db_management/classes/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from py_discord_db_management.classes.column import Column
 
 
 class Table:
     def __init__(self, database, table_name):
         self.__table_name = table_name
         self.__columns = self.get_columns_from_table(database, table_name)
+
         self.__hidden = False
 
     def set_hidden(self, new_visibility):
         self.__hidden = new_visibility
 
     def get_hidden(self):
         return self.__hidden
```

### Comparing `dbpyman-0.1.21/py_discord_db_management/dbpyman.py` & `dbpyman-0.1.211/py_discord_db_management/dbpyman.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.21/py_discord_db_management/views/table_add_data_view.py` & `dbpyman-0.1.211/py_discord_db_management/views/table_add_data_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
                 # style=discord.TextStyle.paragraph
                 column_counter = self.column_index
 
                 # create individual input based on column
                 for index, column in itertools.islice(enumerate(self.columns[self.column_index:], start=self.column_index), 5):
                     # increase counter
                     column_counter += 1
-                    self.add_item(discord.ui.TextInput(label=f"{column.get_field()}", required=not column.get_nullable(), placeholder=str(column.get_default()) ))
+                    if not column.get_hidden():
+                        self.add_item(discord.ui.TextInput(label=f"{column.get_field()}", required=not column.get_nullable(), placeholder=str(column.get_default()) ))
 
                 self.column_index = column_counter
 
             async def on_submit(self, interaction: discord.Interaction):
                 await interaction.response.defer()
 
                 # retrieve the data from each input
```

### Comparing `dbpyman-0.1.21/py_discord_db_management/views/table_categories_view.py` & `dbpyman-0.1.211/py_discord_db_management/views/table_categories_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.21/py_discord_db_management/views/table_overview_view.py` & `dbpyman-0.1.211/py_discord_db_management/views/table_overview_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.21/pyproject.toml` & `dbpyman-0.1.211/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbpyman"
-version = "0.1.21"
+version = "0.1.211"
 authors = [
   { name="JanikCodes", email="janiksielaff@gmx.de" },
 ]
 description = "A package used to modify & view your MySQL database data dynamically"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

