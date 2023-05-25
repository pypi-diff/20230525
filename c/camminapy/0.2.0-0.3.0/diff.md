# Comparing `tmp/camminapy-0.2.0.tar.gz` & `tmp/camminapy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.2.0.tar", max compression
+gzip compressed data, was "camminapy-0.3.0.tar", max compression
```

## Comparing `camminapy-0.2.0.tar` & `camminapy-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.2.0/LICENSE
--rw-r--r--   0        0        0      254 2023-05-25 08:57:11.671705 camminapy-0.2.0/camminapy/__init__.py
--rw-r--r--   0        0        0     2543 2023-05-25 09:03:22.790041 camminapy-0.2.0/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.2.0/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.2.0/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.2.0/camminapy/utils/logger.py
--rw-r--r--   0        0        0      905 2023-05-25 09:13:08.058319 camminapy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 camminapy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.3.0/LICENSE
+-rw-r--r--   0        0        0      254 2023-05-25 08:57:11.671705 camminapy-0.3.0/camminapy/__init__.py
+-rw-r--r--   0        0        0     2543 2023-05-25 09:03:22.790041 camminapy-0.3.0/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.3.0/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.3.0/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.3.0/camminapy/utils/logger.py
+-rw-r--r--   0        0        0      905 2023-05-25 09:14:10.285985 camminapy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 camminapy-0.3.0/PKG-INFO
```

### Comparing `camminapy-0.2.0/LICENSE` & `camminapy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.2.0/camminapy/plot/footer.py` & `camminapy-0.3.0/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.2.0/camminapy/utils/config.py` & `camminapy-0.3.0/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.2.0/camminapy/utils/logger.py` & `camminapy-0.3.0/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.2.0/pyproject.toml` & `camminapy-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.2.0"
+version = "0.3.0"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 altair = "^5.0.0"
 gitpython = "^3.1.31"
```

