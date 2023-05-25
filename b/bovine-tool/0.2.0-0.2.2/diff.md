# Comparing `tmp/bovine_tool-0.2.0.tar.gz` & `tmp/bovine_tool-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_tool-0.2.0.tar", max compression
+gzip compressed data, was "bovine_tool-0.2.2.tar", max compression
```

## Comparing `bovine_tool-0.2.0.tar` & `bovine_tool-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      952 2023-05-22 14:17:04.678842 bovine_tool-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-22 14:17:04.678842 bovine_tool-0.2.0/bovine_tool/__init__.py
--rw-r--r--   0        0        0      495 2023-05-22 14:17:04.678842 bovine_tool-0.2.0/bovine_tool/cleanup.py
--rw-r--r--   0        0        0      277 2023-05-22 14:17:04.678842 bovine_tool-0.2.0/bovine_tool/create.py
--rw-r--r--   0        0        0     2014 2023-05-22 14:17:04.682842 bovine_tool-0.2.0/bovine_tool/manage.py
--rw-r--r--   0        0        0      770 2023-05-22 14:17:04.682842 bovine_tool-0.2.0/bovine_tool/register.py
--rw-r--r--   0        0        0      557 2023-05-22 14:17:04.682842 bovine_tool-0.2.0/bovine_tool/store.py
--rw-r--r--   0        0        0      479 2023-05-22 14:26:40.230579 bovine_tool-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 bovine_tool-0.2.0/setup.py
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 bovine_tool-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      952 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/bovine_tool/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/bovine_tool/cleanup.py
+-rw-r--r--   0        0        0      277 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/bovine_tool/create.py
+-rw-r--r--   0        0        0     2014 2023-05-22 14:17:04.682842 bovine_tool-0.2.2/bovine_tool/manage.py
+-rw-r--r--   0        0        0      770 2023-05-22 14:17:04.682842 bovine_tool-0.2.2/bovine_tool/register.py
+-rw-r--r--   0        0        0      557 2023-05-22 14:17:04.682842 bovine_tool-0.2.2/bovine_tool/store.py
+-rw-r--r--   0        0        0      520 2023-05-25 18:44:02.806690 bovine_tool-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 bovine_tool-0.2.2/setup.py
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 bovine_tool-0.2.2/PKG-INFO
```

### Comparing `bovine_tool-0.2.0/README.md` & `bovine_tool-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.0/bovine_tool/manage.py` & `bovine_tool-0.2.2/bovine_tool/manage.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.0/bovine_tool/register.py` & `bovine_tool-0.2.2/bovine_tool/register.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.0/bovine_tool/store.py` & `bovine_tool-0.2.2/bovine_tool/store.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.0/setup.py` & `bovine_tool-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 {'': ['*']}
 
 install_requires = \
 ['bovine-store>=0.2.1,<0.3.0']
 
 setup_kwargs = {
     'name': 'bovine-tool',
-    'version': '0.2.0',
-    'description': '',
+    'version': '0.2.2',
+    'description': 'Basic tools to administrate a bovine herd',
     'long_description': '# bovine_tool\n\nbovine_tool provides a CLI interface to manage bovine.\n\n## Configuration\n\nThe default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".\n\n## Quick start\n\nTo register a new user with a FediVerse handle use\n\n```bash\npython -m bovine_tool.register fediverse_handle [--domain DOMAIN]\n```\n\nthe domain must be specified.\n\n## Managing users\n\n```bash\npython -m bovine_tool.manage bovine_name\n```\n\ndisplays the user.\n\nTo add a did key for [the Moo Client Registration Flow](https://blog.mymath.rocks/2023-03-25/BIN2_Moo_Client_Registration_Flow) with a BovineClient use\n\n```bash\npython -m bovine_tool.manage bovine_name --did_key key_name did_key\n```\n\nFurthermore, using `--properties` the properties can be over written.\n\n## Todo\n\n- [ ] Add ability to delete stale data, e.g. remote data older than X days\n- [ ] Add ability to import/export all data associated with an actor\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
     'packages': packages,
```

### Comparing `bovine_tool-0.2.0/PKG-INFO` & `bovine_tool-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bovine-tool
-Version: 0.2.0
-Summary: 
+Version: 0.2.2
+Summary: Basic tools to administrate a bovine herd
 Home-page: https://codeberg.org/bovine/bovine
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

