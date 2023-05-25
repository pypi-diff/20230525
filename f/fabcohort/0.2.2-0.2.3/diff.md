# Comparing `tmp/fabcohort-0.2.2.tar.gz` & `tmp/fabcohort-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabcohort-0.2.2.tar", last modified: Fri May 19 14:55:00 2023, max compression
+gzip compressed data, was "fabcohort-0.2.3.tar", last modified: Thu May 25 16:08:19 2023, max compression
```

## Comparing `fabcohort-0.2.2.tar` & `fabcohort-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:55:00.784223 fabcohort-0.2.2/
--rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:55:00.784052 fabcohort-0.2.2/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      337 2023-05-18 20:13:13.000000 fabcohort-0.2.2/README.md
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:55:00.783250 fabcohort-0.2.2/fab_cohort/
--rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.2.2/fab_cohort/__init__.py
--rw-r--r--   0 linliding   (501) staff       (20)     4921 2023-05-19 14:45:33.000000 fabcohort-0.2.2/fab_cohort/cohort.py
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:55:00.783866 fabcohort-0.2.2/fabcohort.egg-info/
--rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:55:00.000000 fabcohort-0.2.2/fabcohort.egg-info/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      226 2023-05-19 14:55:00.000000 fabcohort-0.2.2/fabcohort.egg-info/SOURCES.txt
--rw-r--r--   0 linliding   (501) staff       (20)        1 2023-05-19 14:55:00.000000 fabcohort-0.2.2/fabcohort.egg-info/dependency_links.txt
--rw-r--r--   0 linliding   (501) staff       (20)       13 2023-05-19 14:55:00.000000 fabcohort-0.2.2/fabcohort.egg-info/requires.txt
--rw-r--r--   0 linliding   (501) staff       (20)       11 2023-05-19 14:55:00.000000 fabcohort-0.2.2/fabcohort.egg-info/top_level.txt
--rw-r--r--   0 linliding   (501) staff       (20)       38 2023-05-19 14:55:00.784276 fabcohort-0.2.2/setup.cfg
--rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-05-19 14:54:07.000000 fabcohort-0.2.2/setup.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-25 16:08:19.517923 fabcohort-0.2.3/
+-rw-r--r--   0 linliding   (501) staff       (20)     2527 2023-05-25 16:08:19.517710 fabcohort-0.2.3/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)     1836 2023-05-25 16:00:55.000000 fabcohort-0.2.3/README.md
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-25 16:08:19.516611 fabcohort-0.2.3/fab_cohort/
+-rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.2.3/fab_cohort/__init__.py
+-rw-r--r--   0 linliding   (501) staff       (20)     4921 2023-05-19 14:45:33.000000 fabcohort-0.2.3/fab_cohort/cohort.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-25 16:08:19.517464 fabcohort-0.2.3/fabcohort.egg-info/
+-rw-r--r--   0 linliding   (501) staff       (20)     2527 2023-05-25 16:08:19.000000 fabcohort-0.2.3/fabcohort.egg-info/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      226 2023-05-25 16:08:19.000000 fabcohort-0.2.3/fabcohort.egg-info/SOURCES.txt
+-rw-r--r--   0 linliding   (501) staff       (20)        1 2023-05-25 16:08:19.000000 fabcohort-0.2.3/fabcohort.egg-info/dependency_links.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       13 2023-05-25 16:08:19.000000 fabcohort-0.2.3/fabcohort.egg-info/requires.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       11 2023-05-25 16:08:19.000000 fabcohort-0.2.3/fabcohort.egg-info/top_level.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       38 2023-05-25 16:08:19.517983 fabcohort-0.2.3/setup.cfg
+-rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-05-25 16:08:05.000000 fabcohort-0.2.3/setup.py
```

### Comparing `fabcohort-0.2.2/fab_cohort/cohort.py` & `fabcohort-0.2.3/fab_cohort/cohort.py`

 * *Files identical despite different names*

### Comparing `fabcohort-0.2.2/setup.py` & `fabcohort-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="fabcohort",
-    version="0.2.2",
+    version="0.2.3",
     description="for cohort analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/linliD/fabcohort/",
     author="Linli Ding",
     author_email="linli@joinbonnet.com",
     license="MIT",
```

