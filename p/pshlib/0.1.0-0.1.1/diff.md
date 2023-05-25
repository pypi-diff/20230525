# Comparing `tmp/pshlib-0.1.0.tar.gz` & `tmp/pshlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pshlib-0.1.0.tar", max compression
+gzip compressed data, was "pshlib-0.1.1.tar", max compression
```

## Comparing `pshlib-0.1.0.tar` & `pshlib-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-05-25 20:19:40.765285 pshlib-0.1.0/LICENSE
--rw-r--r--   0        0        0      622 2023-05-25 21:17:50.914732 pshlib-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-25 20:42:55.090454 pshlib-0.1.0/pshlib/__init__.py
--rw-r--r--   0        0        0     1615 2023-05-25 21:08:03.262649 pshlib-0.1.0/pshlib/psh.py
--rw-r--r--   0        0        0     5521 2023-05-25 21:09:19.754160 pshlib-0.1.0/pshlib/shcmd.py
--rw-r--r--   0        0        0      335 2023-05-25 21:28:03.303837 pshlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 pshlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 20:19:40.765285 pshlib-0.1.1/LICENSE
+-rw-r--r--   0        0        0      622 2023-05-25 21:17:50.914732 pshlib-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 20:42:55.090454 pshlib-0.1.1/pshlib/__init__.py
+-rw-r--r--   0        0        0     1615 2023-05-25 21:08:03.262649 pshlib-0.1.1/pshlib/psh.py
+-rw-r--r--   0        0        0     5521 2023-05-25 21:09:19.754160 pshlib-0.1.1/pshlib/shcmd.py
+-rw-r--r--   0        0        0      381 2023-05-25 21:35:17.900207 pshlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 pshlib-0.1.1/PKG-INFO
```

### Comparing `pshlib-0.1.0/LICENSE` & `pshlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pshlib-0.1.0/README.md` & `pshlib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pshlib-0.1.0/pshlib/psh.py` & `pshlib-0.1.1/pshlib/psh.py`

 * *Files identical despite different names*

### Comparing `pshlib-0.1.0/pshlib/shcmd.py` & `pshlib-0.1.1/pshlib/shcmd.py`

 * *Files identical despite different names*

