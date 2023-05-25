# Comparing `tmp/rscad-0.0.4.tar.gz` & `tmp/rscad-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rscad-0.0.4.tar", last modified: Thu Mar  9 20:34:52 2023, max compression
+gzip compressed data, was "rscad-0.0.5.tar", last modified: Thu May 25 13:08:28 2023, max compression
```

## Comparing `rscad-0.0.4.tar` & `rscad-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-03-09 20:34:52.034519 rscad-0.0.4/
--rw-r--r--   0 gws       (1000) users      (100)       75 2023-03-09 12:10:24.000000 rscad-0.0.4/Cargo.toml
--rw-r--r--   0 gws       (1000) users      (100)    26526 2023-03-02 14:10:13.000000 rscad-0.0.4/LICENSE
--rw-r--r--   0 gws       (1000) users      (100)       43 2023-02-13 08:52:19.000000 rscad-0.0.4/MANIFEST.in
--rw-r--r--   0 gws       (1000) users      (100)      141 2023-03-09 20:34:52.034519 rscad-0.0.4/PKG-INFO
--rw-r--r--   0 gws       (1000) users      (100)      825 2023-03-02 15:10:29.000000 rscad-0.0.4/README.md
-drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-03-09 20:34:52.032518 rscad-0.0.4/boolean/
--rw-r--r--   0 gws       (1000) users      (100)        0 2023-03-02 12:23:27.000000 rscad-0.0.4/boolean/__init__.py
--rw-r--r--   0 gws       (1000) users      (100)     1235 2023-03-02 12:23:27.000000 rscad-0.0.4/boolean/core.py
--rw-r--r--   0 gws       (1000) users      (100)      413 2023-03-02 12:23:27.000000 rscad-0.0.4/boolean/fun_tools.py
--rw-r--r--   0 gws       (1000) users      (100)     1527 2023-03-02 12:23:27.000000 rscad-0.0.4/boolean/polydata.py
-drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-03-09 20:34:52.033519 rscad-0.0.4/draft/
--rw-r--r--   0 gws       (1000) users      (100)        0 2023-03-09 12:15:56.000000 rscad-0.0.4/draft/__init__.py
--rw-r--r--   0 gws       (1000) users      (100)       58 2023-03-09 17:58:05.000000 rscad-0.0.4/draft/core.py
--rw-r--r--   0 gws       (1000) users      (100)      925 2023-03-09 20:34:04.000000 rscad-0.0.4/draft/polydata.py
-drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-03-09 20:34:52.031519 rscad-0.0.4/hello/
-drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-03-09 20:34:52.033519 rscad-0.0.4/hello/py/
--rw-r--r--   0 gws       (1000) users      (100)      149 2023-03-02 12:23:27.000000 rscad-0.0.4/hello/py/__init__.py
--rw-r--r--   0 gws       (1000) users      (100)       69 2023-03-02 14:50:37.000000 rscad-0.0.4/pyproject.toml
-drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-03-09 20:34:52.034519 rscad-0.0.4/rscad.egg-info/
--rw-r--r--   0 gws       (1000) users      (100)      141 2023-03-09 20:34:51.000000 rscad-0.0.4/rscad.egg-info/PKG-INFO
--rw-r--r--   0 gws       (1000) users      (100)      384 2023-03-09 20:34:51.000000 rscad-0.0.4/rscad.egg-info/SOURCES.txt
--rw-r--r--   0 gws       (1000) users      (100)        1 2023-03-09 20:34:51.000000 rscad-0.0.4/rscad.egg-info/dependency_links.txt
--rw-r--r--   0 gws       (1000) users      (100)        1 2023-03-02 10:25:51.000000 rscad-0.0.4/rscad.egg-info/not-zip-safe
--rw-r--r--   0 gws       (1000) users      (100)       14 2023-03-09 20:34:51.000000 rscad-0.0.4/rscad.egg-info/requires.txt
--rw-r--r--   0 gws       (1000) users      (100)        6 2023-03-09 20:34:51.000000 rscad-0.0.4/rscad.egg-info/top_level.txt
--rw-r--r--   0 gws       (1000) users      (100)       38 2023-03-09 20:34:52.034519 rscad-0.0.4/setup.cfg
--rw-r--r--   0 gws       (1000) users      (100)     1348 2023-03-09 19:37:13.000000 rscad-0.0.4/setup.py
+drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-05-25 13:08:28.848915 rscad-0.0.5/
+-rw-r--r--   0 gws       (1000) users      (100)       75 2023-05-25 11:51:27.000000 rscad-0.0.5/Cargo.toml
+-rw-r--r--   0 gws       (1000) users      (100)    26526 2023-03-02 14:10:13.000000 rscad-0.0.5/LICENSE
+-rw-r--r--   0 gws       (1000) users      (100)       59 2023-05-25 12:02:00.000000 rscad-0.0.5/MANIFEST.in
+-rw-r--r--   0 gws       (1000) users      (100)      141 2023-05-25 13:08:28.847915 rscad-0.0.5/PKG-INFO
+-rw-r--r--   0 gws       (1000) users      (100)      825 2023-03-02 15:10:29.000000 rscad-0.0.5/README.md
+-rw-r--r--   0 gws       (1000) users      (100)        6 2023-05-25 13:07:22.000000 rscad-0.0.5/VERSION
+drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-05-25 13:08:28.846915 rscad-0.0.5/boolean/
+-rw-r--r--   0 gws       (1000) users      (100)        0 2023-03-02 12:23:27.000000 rscad-0.0.5/boolean/__init__.py
+-rw-r--r--   0 gws       (1000) users      (100)     1235 2023-03-02 12:23:27.000000 rscad-0.0.5/boolean/core.py
+-rw-r--r--   0 gws       (1000) users      (100)      413 2023-03-02 12:23:27.000000 rscad-0.0.5/boolean/fun_tools.py
+-rw-r--r--   0 gws       (1000) users      (100)     1527 2023-03-02 12:23:27.000000 rscad-0.0.5/boolean/polydata.py
+drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-05-25 13:08:28.847915 rscad-0.0.5/draft/
+-rw-r--r--   0 gws       (1000) users      (100)        0 2023-03-09 12:15:56.000000 rscad-0.0.5/draft/__init__.py
+-rw-r--r--   0 gws       (1000) users      (100)       58 2023-03-09 17:58:05.000000 rscad-0.0.5/draft/core.py
+-rw-r--r--   0 gws       (1000) users      (100)      925 2023-03-09 20:34:04.000000 rscad-0.0.5/draft/polydata.py
+drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-05-25 13:08:28.845915 rscad-0.0.5/hello/
+drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-05-25 13:08:28.847915 rscad-0.0.5/hello/py/
+-rw-r--r--   0 gws       (1000) users      (100)      149 2023-03-02 12:23:27.000000 rscad-0.0.5/hello/py/__init__.py
+-rw-r--r--   0 gws       (1000) users      (100)       69 2023-03-02 14:50:37.000000 rscad-0.0.5/pyproject.toml
+drwxr-xr-x   0 gws       (1000) users      (100)        0 2023-05-25 13:08:28.847915 rscad-0.0.5/rscad.egg-info/
+-rw-r--r--   0 gws       (1000) users      (100)      141 2023-05-25 13:08:28.000000 rscad-0.0.5/rscad.egg-info/PKG-INFO
+-rw-r--r--   0 gws       (1000) users      (100)      392 2023-05-25 13:08:28.000000 rscad-0.0.5/rscad.egg-info/SOURCES.txt
+-rw-r--r--   0 gws       (1000) users      (100)        1 2023-05-25 13:08:28.000000 rscad-0.0.5/rscad.egg-info/dependency_links.txt
+-rw-r--r--   0 gws       (1000) users      (100)        1 2023-03-02 10:25:51.000000 rscad-0.0.5/rscad.egg-info/not-zip-safe
+-rw-r--r--   0 gws       (1000) users      (100)       14 2023-05-25 13:08:28.000000 rscad-0.0.5/rscad.egg-info/requires.txt
+-rw-r--r--   0 gws       (1000) users      (100)        6 2023-05-25 13:08:28.000000 rscad-0.0.5/rscad.egg-info/top_level.txt
+-rw-r--r--   0 gws       (1000) users      (100)       38 2023-05-25 13:08:28.848915 rscad-0.0.5/setup.cfg
+-rw-r--r--   0 gws       (1000) users      (100)     1348 2023-03-09 19:37:13.000000 rscad-0.0.5/setup.py
```

### Comparing `rscad-0.0.4/LICENSE` & `rscad-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rscad-0.0.4/README.md` & `rscad-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rscad-0.0.4/boolean/core.py` & `rscad-0.0.5/boolean/core.py`

 * *Files identical despite different names*

### Comparing `rscad-0.0.4/boolean/polydata.py` & `rscad-0.0.5/boolean/polydata.py`

 * *Files identical despite different names*

### Comparing `rscad-0.0.4/draft/polydata.py` & `rscad-0.0.5/draft/polydata.py`

 * *Files identical despite different names*

### Comparing `rscad-0.0.4/setup.py` & `rscad-0.0.5/setup.py`

 * *Files identical despite different names*

