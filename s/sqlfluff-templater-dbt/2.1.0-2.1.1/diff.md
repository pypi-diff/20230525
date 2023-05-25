# Comparing `tmp/sqlfluff-templater-dbt-2.1.0.tar.gz` & `tmp/sqlfluff-templater-dbt-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-5j982rty/sqlfluff-templater-dbt-2.1.0.tar", last modified: Wed May  3 23:19:59 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-j4b_a0t4/sqlfluff-templater-dbt-2.1.1.tar", last modified: Thu May 25 16:29:33 2023, max compression
```

## Comparing `sqlfluff-templater-dbt-2.1.0.tar` & `sqlfluff-templater-dbt-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25159 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff-templater-dbt-2.1.0/LICENSE.md` & `sqlfluff-templater-dbt-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-2.1.0/PKG-INFO` & `sqlfluff-templater-dbt-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.1.0
+Version: 2.1.1
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-templater-dbt-2.1.0/setup.cfg` & `sqlfluff-templater-dbt-2.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 2.1.0
+version = 2.1.1
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -61,15 +61,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	sqlfluff==2.1.0
+	sqlfluff==2.1.1
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/templater.py` & `sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/templater.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from dataclasses import dataclass
 
 from dbt.version import get_installed_version
 from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
 from dbt.adapters.factory import register_adapter, get_adapter
 from dbt.compilation import Compiler as DbtCompiler
+from dbt.cli.resolvers import default_profiles_dir
 
 try:
     from dbt.exceptions import (
         CompilationException as DbtCompilationException,
         FailedToConnectException as DbtFailedToConnectException,
         DbtProjectError,
     )
@@ -178,26 +179,26 @@
             )
 
         return self.dbt_selector_method
 
     def _get_profiles_dir(self):
         """Get the dbt profiles directory from the configuration.
 
-        The default is `~/.dbt` in 0.17 but we use the
-        PROFILES_DIR variable from the dbt library to
+        The default is `~/.dbt` but we use the
+        default_profiles_dir from the dbt library to
         support a change of default in the future, as well
         as to support the same overwriting mechanism as
         dbt (currently an environment variable).
         """
         dbt_profiles_dir = os.path.abspath(
             os.path.expanduser(
                 self.sqlfluff_config.get_section(
                     (self.templater_selector, self.name, "profiles_dir")
                 )
-                or flags.PROFILES_DIR
+                or (os.getenv("DBT_PROFILES_DIR") or default_profiles_dir())
             )
         )
 
         if not os.path.exists(dbt_profiles_dir):
             templater_logger.error(
                 f"dbt_profiles_dir: {dbt_profiles_dir} could not be accessed. "
                 "Check it exists."
```

### Comparing `sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.1.0
+Version: 2.1.1
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

