# Comparing `tmp/ttrace-0.1.8.tar.gz` & `tmp/ttrace-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttrace-0.1.8.tar", max compression
+gzip compressed data, was "ttrace-0.1.9.tar", max compression
```

## Comparing `ttrace-0.1.8.tar` & `ttrace-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2778 2023-04-26 09:09:07.923462 ttrace-0.1.8/Readme.md
--rw-r--r--   0        0        0     1753 2023-05-15 14:05:27.274856 ttrace-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0    25572 2023-05-15 14:05:12.615100 ttrace-0.1.8/ttrace/__init__.py
--rw-r--r--   0        0        0        0 2023-03-01 06:28:10.240369 ttrace-0.1.8/ttrace/utils/__init__.py
--rw-r--r--   0        0        0     4941 2023-05-15 13:57:36.053811 ttrace-0.1.8/ttrace/utils/treestuff.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 ttrace-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5767 2023-05-25 11:30:47.164522 ttrace-0.1.9/Readme.md
+-rw-r--r--   0        0        0     1753 2023-05-25 11:31:01.256582 ttrace-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0    25572 2023-05-25 11:28:06.211838 ttrace-0.1.9/ttrace/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-01 06:28:10.240369 ttrace-0.1.9/ttrace/utils/__init__.py
+-rw-r--r--   0        0        0     4941 2023-05-15 13:57:36.053811 ttrace-0.1.9/ttrace/utils/treestuff.py
+-rw-r--r--   0        0        0     6350 1970-01-01 00:00:00.000000 ttrace-0.1.9/PKG-INFO
```

### Comparing `ttrace-0.1.8/pyproject.toml` & `ttrace-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ttrace"
-version = "0.1.8"
+version = "0.1.9"
 description = "Makes use of strace"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/ttrace.git"
 readme = "Readme.md"
 packages = [
   {include = "ttrace"}
 ]
```

### Comparing `ttrace-0.1.8/ttrace/__init__.py` & `ttrace-0.1.9/ttrace/__init__.py`

 * *Files identical despite different names*

### Comparing `ttrace-0.1.8/ttrace/utils/treestuff.py` & `ttrace-0.1.9/ttrace/utils/treestuff.py`

 * *Files identical despite different names*

