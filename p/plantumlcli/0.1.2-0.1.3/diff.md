# Comparing `tmp/plantumlcli-0.1.2.tar.gz` & `tmp/plantumlcli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantumlcli-0.1.2.tar", last modified: Sun May  7 08:00:23 2023, max compression
+gzip compressed data, was "plantumlcli-0.1.3.tar", last modified: Thu May 25 05:12:34 2023, max compression
```

## Comparing `plantumlcli-0.1.2.tar` & `plantumlcli-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli/entry/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/plantumlcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/plantumlcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-pdf.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.747515 plantumlcli-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-25 05:12:34.747515 plantumlcli-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.743515 plantumlcli-0.1.3/plantumlcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.743515 plantumlcli-0.1.3/plantumlcli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.747515 plantumlcli-0.1.3/plantumlcli/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/entry/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/entry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/entry/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.747515 plantumlcli-0.1.3/plantumlcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/models/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/models/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.747515 plantumlcli-0.1.3/plantumlcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/plantumlcli/utils/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:12:34.743515 plantumlcli-0.1.3/plantumlcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-25 05:12:34.000000 plantumlcli-0.1.3/plantumlcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 05:12:34.000000 plantumlcli-0.1.3/plantumlcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:12:34.000000 plantumlcli-0.1.3/plantumlcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 05:12:34.000000 plantumlcli-0.1.3/plantumlcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 05:12:34.000000 plantumlcli-0.1.3/plantumlcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 05:12:34.000000 plantumlcli-0.1.3/plantumlcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/requirements-pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 05:12:34.747515 plantumlcli-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-25 05:12:02.000000 plantumlcli-0.1.3/setup.py
```

### Comparing `plantumlcli-0.1.2/LICENSE` & `plantumlcli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/PKG-INFO` & `plantumlcli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
@@ -19,18 +19,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: pdf
 Provides-Extra: doc
 Provides-Extra: lint
+Provides-Extra: pdf
+Provides-Extra: test
 License-File: LICENSE
 
 # plantumlcli
 
 [![PyPI](https://img.shields.io/pypi/v/plantumlcli)](https://pypi.org/project/plantumlcli/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plantumlcli)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/plantumlcli)
```

### Comparing `plantumlcli-0.1.2/README.md` & `plantumlcli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/entry/base.py` & `plantumlcli-0.1.3/plantumlcli/entry/base.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/entry/cli.py` & `plantumlcli-0.1.3/plantumlcli/entry/cli.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/entry/general.py` & `plantumlcli-0.1.3/plantumlcli/entry/general.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/entry/local.py` & `plantumlcli-0.1.3/plantumlcli/entry/local.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/entry/remote.py` & `plantumlcli-0.1.3/plantumlcli/entry/remote.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/models/base.py` & `plantumlcli-0.1.3/plantumlcli/models/base.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/models/local.py` & `plantumlcli-0.1.3/plantumlcli/models/local.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/models/remote.py` & `plantumlcli-0.1.3/plantumlcli/models/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,20 +117,21 @@
                     if self._get_server_version() < (1, 2023):
                         raise ValueError(f'Resource type {type_!r} not supported for '
                                          f'plantuml server site lower than 1.2023 - {self._get_server_version()!r}.')
 
     def _get_version(self) -> str:
         if not self._is_official():
             r = self.__get_homepage()
-            return PyQuery(r.content.decode()).find('#footer').text().strip()
+            page = PyQuery(r.content.decode())
+            return (page.find('#footer') or page.find('.footer')).text().strip()
         else:
             return 'Official Site'
 
     def _get_server_version(self) -> Tuple[int, int, int]:
-        (major, year, v), = re.findall(r'version\s*(?P<major>\d)(?P<year>\d{4})(?P<v>\d{2})',
+        (major, year, v), = re.findall(r'version\s*(?P<major>\d)[.\-]?(?P<year>\d{4})[.\-]?(?P<v>\d{1,2})',
                                        self._get_version(), re.IGNORECASE)
 
         return int(major), int(year), int(v.lstrip('0') or '0')
 
     def __get_uml_path(self, type_: str, code: str):
         return f"{type_}/{self.__compress(code)}"
```

### Comparing `plantumlcli-0.1.2/plantumlcli/utils/concurrent.py` & `plantumlcli-0.1.3/plantumlcli/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/utils/decorator.py` & `plantumlcli-0.1.3/plantumlcli/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/utils/encoding.py` & `plantumlcli-0.1.3/plantumlcli/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/utils/execute.py` & `plantumlcli-0.1.3/plantumlcli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli/utils/file.py` & `plantumlcli-0.1.3/plantumlcli/utils/file.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli.egg-info/PKG-INFO` & `plantumlcli-0.1.3/plantumlcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
@@ -19,18 +19,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: pdf
 Provides-Extra: doc
 Provides-Extra: lint
+Provides-Extra: pdf
+Provides-Extra: test
 License-File: LICENSE
 
 # plantumlcli
 
 [![PyPI](https://img.shields.io/pypi/v/plantumlcli)](https://pypi.org/project/plantumlcli/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plantumlcli)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/plantumlcli)
```

### Comparing `plantumlcli-0.1.2/plantumlcli.egg-info/SOURCES.txt` & `plantumlcli-0.1.3/plantumlcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/plantumlcli.egg-info/requires.txt` & `plantumlcli-0.1.3/plantumlcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.2/setup.py` & `plantumlcli-0.1.3/setup.py`

 * *Files identical despite different names*

