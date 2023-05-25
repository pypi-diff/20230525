# Comparing `tmp/disklru-1.0.5.tar.gz` & `tmp/disklru-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disklru-1.0.5.tar", last modified: Fri May 19 02:03:57 2023, max compression
+gzip compressed data, was "disklru-1.0.6.tar", last modified: Thu May 25 02:16:44 2023, max compression
```

## Comparing `disklru-1.0.5.tar` & `disklru-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.551477 disklru-1.0.5/
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.543245 disklru-1.0.5/.github/
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.548302 disklru-1.0.5/.github/workflows/
--rw-r--r--   0 niteris    (501) staff       (20)      855 2023-05-18 22:37:02.000000 disklru-1.0.5/.github/workflows/lint.yml
--rw-r--r--   0 niteris    (501) staff       (20)      801 2023-05-18 22:37:02.000000 disklru-1.0.5/.github/workflows/push_macos.yml
--rw-r--r--   0 niteris    (501) staff       (20)      803 2023-05-18 22:37:02.000000 disklru-1.0.5/.github/workflows/push_ubuntu.yml
--rw-r--r--   0 niteris    (501) staff       (20)      800 2023-05-18 22:37:02.000000 disklru-1.0.5/.github/workflows/push_win.yml
--rw-r--r--   0 niteris    (501) staff       (20)     1914 2023-05-18 22:37:02.000000 disklru-1.0.5/.gitignore
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.549013 disklru-1.0.5/.vscode/
--rw-r--r--   0 niteris    (501) staff       (20)     1354 2023-05-18 22:37:02.000000 disklru-1.0.5/.vscode/launch.json
--rw-r--r--   0 niteris    (501) staff       (20)      819 2023-05-18 22:37:02.000000 disklru-1.0.5/.vscode/settings.json
--rw-r--r--   0 niteris    (501) staff       (20)     1109 2023-05-18 22:37:02.000000 disklru-1.0.5/.vscode/tasks.json
--rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-05-18 22:37:02.000000 disklru-1.0.5/LICENSE
--rw-r--r--   0 niteris    (501) staff       (20)      102 2023-05-18 22:37:02.000000 disklru-1.0.5/MANIFEST.in
--rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 02:03:57.551260 disklru-1.0.5/PKG-INFO
--rw-r--r--   0 niteris    (501) staff       (20)      862 2023-05-18 22:37:02.000000 disklru-1.0.5/README.md
--rwxr-xr-x   0 niteris    (501) staff       (20)      400 2023-05-19 00:59:49.000000 disklru-1.0.5/activate.sh
--rwxr-xr-x   0 niteris    (501) staff       (20)      435 2023-05-18 22:37:02.000000 disklru-1.0.5/lint.sh
--rw-r--r--   0 niteris    (501) staff       (20)     2138 2023-05-18 22:37:02.000000 disklru-1.0.5/make_venv.py
--rw-r--r--   0 niteris    (501) staff       (20)      712 2023-05-19 02:02:40.000000 disklru-1.0.5/pyproject.toml
--rw-r--r--   0 niteris    (501) staff       (20)       47 2023-05-19 01:11:14.000000 disklru-1.0.5/requirements.testing.txt
--rw-r--r--   0 niteris    (501) staff       (20)       38 2023-05-19 02:03:57.551542 disklru-1.0.5/setup.cfg
--rw-r--r--   0 niteris    (501) staff       (20)     1090 2023-05-18 22:37:02.000000 disklru-1.0.5/setup.py
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.543625 disklru-1.0.5/src/
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.549595 disklru-1.0.5/src/disklru/
--rw-r--r--   0 niteris    (501) staff       (20)       92 2023-05-19 01:11:14.000000 disklru-1.0.5/src/disklru/__init__.py
--rw-r--r--   0 niteris    (501) staff       (20)     3641 2023-05-19 02:02:19.000000 disklru-1.0.5/src/disklru/disklru.py
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.550662 disklru-1.0.5/src/disklru.egg-info/
--rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 02:03:57.000000 disklru-1.0.5/src/disklru.egg-info/PKG-INFO
--rw-r--r--   0 niteris    (501) staff       (20)      543 2023-05-19 02:03:57.000000 disklru-1.0.5/src/disklru.egg-info/SOURCES.txt
--rw-r--r--   0 niteris    (501) staff       (20)        1 2023-05-19 02:03:57.000000 disklru-1.0.5/src/disklru.egg-info/dependency_links.txt
--rw-r--r--   0 niteris    (501) staff       (20)        8 2023-05-19 02:03:57.000000 disklru-1.0.5/src/disklru.egg-info/top_level.txt
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 02:03:57.550860 disklru-1.0.5/tests/
--rw-r--r--   0 niteris    (501) staff       (20)     3163 2023-05-19 01:11:27.000000 disklru-1.0.5/tests/test_disklru.py
--rw-r--r--   0 niteris    (501) staff       (20)      498 2023-05-19 01:11:14.000000 disklru-1.0.5/tox.ini
--rwxr-xr-x   0 niteris    (501) staff       (20)      291 2023-05-18 22:37:02.000000 disklru-1.0.5/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.925649 disklru-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.881650 disklru-1.0.6/.github/
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.903648 disklru-1.0.6/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      801 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      803 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      800 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     1914 2023-05-25 00:48:35.000000 disklru-1.0.6/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.907649 disklru-1.0.6/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-25 00:48:35.000000 disklru-1.0.6/.vscode/launch.json
+-rw-rw-rw-   0        0        0      819 2023-05-25 00:48:35.000000 disklru-1.0.6/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-25 00:48:35.000000 disklru-1.0.6/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-25 00:48:35.000000 disklru-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      102 2023-05-25 00:48:35.000000 disklru-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2764 2023-05-25 02:16:44.924648 disklru-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2045 2023-05-25 00:48:35.000000 disklru-1.0.6/README.md
+-rw-rw-rw-   0        0        0      400 2023-05-25 00:48:35.000000 disklru-1.0.6/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-25 00:48:35.000000 disklru-1.0.6/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-25 00:48:35.000000 disklru-1.0.6/make_venv.py
+-rw-rw-rw-   0        0        0      712 2023-05-25 02:16:25.000000 disklru-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2023-05-25 00:48:35.000000 disklru-1.0.6/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 02:16:44.926649 disklru-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-05-25 00:48:35.000000 disklru-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.883649 disklru-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.909649 disklru-1.0.6/src/disklru/
+-rw-rw-rw-   0        0        0       92 2023-05-25 00:48:35.000000 disklru-1.0.6/src/disklru/__init__.py
+-rw-rw-rw-   0        0        0     3641 2023-05-25 00:48:35.000000 disklru-1.0.6/src/disklru/disklru.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.922649 disklru-1.0.6/src/disklru.egg-info/
+-rw-rw-rw-   0        0        0     2764 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.923649 disklru-1.0.6/tests/
+-rw-rw-rw-   0        0        0     3163 2023-05-25 00:48:35.000000 disklru-1.0.6/tests/test_disklru.py
+-rw-rw-rw-   0        0        0      498 2023-05-25 00:48:35.000000 disklru-1.0.6/tox.ini
+-rw-rw-rw-   0        0        0      312 2023-05-25 02:15:29.000000 disklru-1.0.6/upload_package.sh
```

### Comparing `disklru-1.0.5/.github/workflows/lint.yml` & `disklru-1.0.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.github/workflows/push_macos.yml` & `disklru-1.0.6/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.github/workflows/push_ubuntu.yml` & `disklru-1.0.6/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.github/workflows/push_win.yml` & `disklru-1.0.6/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.gitignore` & `disklru-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.vscode/launch.json` & `disklru-1.0.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.vscode/settings.json` & `disklru-1.0.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/.vscode/tasks.json` & `disklru-1.0.6/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/LICENSE` & `disklru-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/make_venv.py` & `disklru-1.0.6/make_venv.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/pyproject.toml` & `disklru-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
 ]
 # Change this with the version number bump.
 # Also make the change in zcmds/version.py
-version = "1.0.5"
+version = "1.0.6"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `disklru-1.0.5/setup.py` & `disklru-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/src/disklru/disklru.py` & `disklru-1.0.6/src/disklru/disklru.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/src/disklru.egg-info/SOURCES.txt` & `disklru-1.0.6/src/disklru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disklru-1.0.5/tests/test_disklru.py` & `disklru-1.0.6/tests/test_disklru.py`

 * *Files identical despite different names*

