# Comparing `tmp/deamons-0.0.5.tar.gz` & `tmp/deamons-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deamons-0.0.5.tar", last modified: Tue May 23 21:59:01 2023, max compression
+gzip compressed data, was "deamons-0.0.6.tar", last modified: Thu May 25 15:15:21 2023, max compression
```

## Comparing `deamons-0.0.5.tar` & `deamons-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 21:59:01.792888 deamons-0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-05-23 21:49:01.000000 deamons-0.0.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-05-23 19:16:59.000000 deamons-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      510 2023-05-23 21:59:01.791885 deamons-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-05-23 21:49:01.000000 deamons-0.0.5/README.md
--rw-rw-rw-   0        0        0      101 2023-05-23 21:56:02.000000 deamons-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 21:59:01.792888 deamons-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1272 2023-05-23 21:58:37.000000 deamons-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 21:59:01.772885 deamons-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 21:59:01.789886 deamons-0.0.5/src/deamons.egg-info/
--rw-rw-rw-   0        0        0      510 2023-05-23 21:59:01.000000 deamons-0.0.5/src/deamons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-05-23 21:59:01.000000 deamons-0.0.5/src/deamons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 21:59:01.000000 deamons-0.0.5/src/deamons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 21:59:01.000000 deamons-0.0.5/src/deamons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 15:15:21.163477 deamons-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 21:49:01.000000 deamons-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:16:59.000000 deamons-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      510 2023-05-25 15:15:21.163477 deamons-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-05-23 21:49:01.000000 deamons-0.0.6/README.md
+-rw-rw-rw-   0        0        0      101 2023-05-23 21:56:02.000000 deamons-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:15:21.164476 deamons-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2023-05-25 15:12:38.000000 deamons-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:15:21.143477 deamons-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:15:21.161477 deamons-0.0.6/src/deamons.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-05-25 15:15:21.000000 deamons-0.0.6/src/deamons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-05-25 15:15:21.000000 deamons-0.0.6/src/deamons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:15:21.000000 deamons-0.0.6/src/deamons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:15:21.000000 deamons-0.0.6/src/deamons.egg-info/top_level.txt
```

### Comparing `deamons-0.0.5/LICENSE` & `deamons-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deamons-0.0.5/setup.py` & `deamons-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 here = Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="deamons",
-    version="0.0.5",
+    version="0.0.6",
     description="Fridrich deamon",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lukas Krahbichler",
     author_email="melonenbuby@proton.me",
     url="https://github.com/FridrichDerGosse/Fridrich",
     classifiers=[
```

