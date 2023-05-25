# Comparing `tmp/deamons-0.0.7.tar.gz` & `tmp/deamons-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deamons-0.0.7.tar", last modified: Thu May 25 15:20:34 2023, max compression
+gzip compressed data, was "deamons-0.0.8.tar", last modified: Thu May 25 15:24:52 2023, max compression
```

## Comparing `deamons-0.0.7.tar` & `deamons-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:20:34.222655 deamons-0.0.7/
--rw-rw-rw-   0        0        0    35823 2023-05-23 21:49:01.000000 deamons-0.0.7/LICENSE
--rw-rw-rw-   0        0        0        0 2023-05-23 19:16:59.000000 deamons-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      510 2023-05-25 15:20:34.221656 deamons-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-05-23 21:49:01.000000 deamons-0.0.7/README.md
--rw-rw-rw-   0        0        0      101 2023-05-23 21:56:02.000000 deamons-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 15:20:34.222655 deamons-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1304 2023-05-25 15:20:08.000000 deamons-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:20:34.198692 deamons-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 15:20:34.220698 deamons-0.0.7/src/deamons.egg-info/
--rw-rw-rw-   0        0        0      510 2023-05-25 15:20:34.000000 deamons-0.0.7/src/deamons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-05-25 15:20:34.000000 deamons-0.0.7/src/deamons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:20:34.000000 deamons-0.0.7/src/deamons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:20:34.000000 deamons-0.0.7/src/deamons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 15:24:52.264647 deamons-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 21:49:01.000000 deamons-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:16:59.000000 deamons-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      510 2023-05-25 15:24:52.263649 deamons-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-05-23 21:49:01.000000 deamons-0.0.8/README.md
+-rw-rw-rw-   0        0        0      101 2023-05-23 21:56:02.000000 deamons-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:24:52.264647 deamons-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2023-05-25 15:24:27.000000 deamons-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:24:52.240647 deamons-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:24:52.248647 deamons-0.0.8/src/deamons/
+-rw-rw-rw-   0        0        0      117 2023-05-25 15:12:38.000000 deamons-0.0.8/src/deamons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:24:52.262647 deamons-0.0.8/src/deamons.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-05-25 15:24:52.000000 deamons-0.0.8/src/deamons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-25 15:24:52.000000 deamons-0.0.8/src/deamons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:24:52.000000 deamons-0.0.8/src/deamons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 15:24:52.000000 deamons-0.0.8/src/deamons.egg-info/top_level.txt
```

### Comparing `deamons-0.0.7/LICENSE` & `deamons-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deamons-0.0.7/setup.py` & `deamons-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 here = Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="deamons",
-    version="0.0.7",
+    version="0.0.8",
     description="Fridrich deamon",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lukas Krahbichler",
     author_email="melonenbuby@proton.me",
     url="https://github.com/FridrichDerGosse/Fridrich",
     classifiers=[
```

