# Comparing `tmp/pygn-0.9.13.tar.gz` & `tmp/pygn-0.9.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygn-0.9.13.tar", last modified: Mon Jan  5 12:00:57 2015, max compression
+gzip compressed data, was "dist/pygn-0.9.14.tar", last modified: Mon Jan  5 12:08:14 2015, max compression
```

## Comparing `pygn-0.9.13.tar` & `pygn-0.9.14.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 matej     (1000) matej     (1000)        0 2015-01-05 12:00:57.000000 pygn-0.9.13/
-drwxrwxr-x   0 matej     (1000) matej     (1000)        0 2015-01-05 12:00:57.000000 pygn-0.9.13/pygn.egg-info/
--rw-rw-r--   0 matej     (1000) matej     (1000)     2240 2015-01-05 12:00:57.000000 pygn-0.9.13/pygn.egg-info/PKG-INFO
--rw-rw-r--   0 matej     (1000) matej     (1000)      214 2015-01-05 12:00:57.000000 pygn-0.9.13/pygn.egg-info/SOURCES.txt
--rw-rw-r--   0 matej     (1000) matej     (1000)        1 2015-01-05 12:00:57.000000 pygn-0.9.13/pygn.egg-info/dependency_links.txt
--rw-rw-r--   0 matej     (1000) matej     (1000)       36 2015-01-05 12:00:57.000000 pygn-0.9.13/pygn.egg-info/top_level.txt
-drwxrwxr-x   0 matej     (1000) matej     (1000)        0 2015-01-05 12:00:57.000000 pygn-0.9.13/test/
--rwxrwxr-x   0 matej     (1000) matej     (1000)     2757 2015-01-05 11:59:40.000000 pygn-0.9.13/test/test_pyg.py
--rwxrwxr-x   0 matej     (1000) matej     (1000)     3618 2015-01-05 11:59:40.000000 pygn-0.9.13/test/test_wlp.py
--rw-rw-r--   0 matej     (1000) matej     (1000)     1228 2015-01-03 09:35:14.000000 pygn-0.9.13/README
--rw-rw-r--   0 matej     (1000) matej     (1000)     6214 2015-01-05 12:00:34.000000 pygn-0.9.13/mail2news.py
--rw-rw-r--   0 matej     (1000) matej     (1000)     5437 2015-01-05 11:40:37.000000 pygn-0.9.13/news2mail.py
--rwxrwxr-x   0 matej     (1000) matej     (1000)     3103 2015-01-03 09:35:14.000000 pygn-0.9.13/pygm2n
--rwxrwxr-x   0 matej     (1000) matej     (1000)     3516 2015-01-03 09:35:14.000000 pygn-0.9.13/pygn2m
--rw-rw-r--   0 matej     (1000) matej     (1000)     1191 2015-01-05 11:59:40.000000 pygn-0.9.13/setup.py
--rw-rw-r--   0 matej     (1000) matej     (1000)     3521 2015-01-05 11:59:40.000000 pygn-0.9.13/whitelist.py
--rw-rw-r--   0 matej     (1000) matej     (1000)     2240 2015-01-05 12:00:57.000000 pygn-0.9.13/PKG-INFO
--rw-rw-r--   0 matej     (1000) matej     (1000)       59 2015-01-05 12:00:57.000000 pygn-0.9.13/setup.cfg
+drwxrwxr-x   0 matej     (1000) matej     (1000)        0 2015-01-05 12:08:14.000000 pygn-0.9.14/
+drwxrwxr-x   0 matej     (1000) matej     (1000)        0 2015-01-05 12:08:14.000000 pygn-0.9.14/pygn.egg-info/
+-rw-rw-r--   0 matej     (1000) matej     (1000)     2240 2015-01-05 12:08:14.000000 pygn-0.9.14/pygn.egg-info/PKG-INFO
+-rw-rw-r--   0 matej     (1000) matej     (1000)      235 2015-01-05 12:08:14.000000 pygn-0.9.14/pygn.egg-info/SOURCES.txt
+-rw-rw-r--   0 matej     (1000) matej     (1000)        1 2015-01-05 12:08:14.000000 pygn-0.9.14/pygn.egg-info/dependency_links.txt
+-rw-rw-r--   0 matej     (1000) matej     (1000)       51 2015-01-05 12:08:14.000000 pygn-0.9.14/pygn.egg-info/top_level.txt
+drwxrwxr-x   0 matej     (1000) matej     (1000)        0 2015-01-05 12:08:14.000000 pygn-0.9.14/test/
+-rwxrwxr-x   0 matej     (1000) matej     (1000)     2757 2015-01-05 11:59:40.000000 pygn-0.9.14/test/test_pyg.py
+-rwxrwxr-x   0 matej     (1000) matej     (1000)     3618 2015-01-05 11:59:40.000000 pygn-0.9.14/test/test_wlp.py
+-rw-rw-r--   0 matej     (1000) matej     (1000)     1228 2015-01-03 09:35:14.000000 pygn-0.9.14/README
+-rw-rw-r--   0 matej     (1000) matej     (1000)     6214 2015-01-05 12:07:37.000000 pygn-0.9.14/mail2news.py
+-rw-rw-r--   0 matej     (1000) matej     (1000)     5437 2015-01-05 11:40:37.000000 pygn-0.9.14/news2mail.py
+-rwxrwxr-x   0 matej     (1000) matej     (1000)     3103 2015-01-03 09:35:14.000000 pygn-0.9.14/pygm2n
+-rwxrwxr-x   0 matej     (1000) matej     (1000)     3516 2015-01-03 09:35:14.000000 pygn-0.9.14/pygn2m
+-rw-rw-r--   0 matej     (1000) matej     (1000)     1230 2015-01-05 12:07:42.000000 pygn-0.9.14/setup.py
+-rw-rw-r--   0 matej     (1000) matej     (1000)     3521 2015-01-05 11:59:40.000000 pygn-0.9.14/whitelist.py
+-rw-rw-r--   0 matej     (1000) matej     (1000)      768 2015-01-05 11:59:40.000000 pygn-0.9.14/wlp.py
+-rw-rw-r--   0 matej     (1000) matej     (1000)     1402 2015-01-05 11:59:40.000000 pygn-0.9.14/wlp_parser.py
+-rw-rw-r--   0 matej     (1000) matej     (1000)     2240 2015-01-05 12:08:14.000000 pygn-0.9.14/PKG-INFO
+-rw-rw-r--   0 matej     (1000) matej     (1000)       59 2015-01-05 12:08:14.000000 pygn-0.9.14/setup.cfg
```

### Comparing `pygn-0.9.13/pygn.egg-info/PKG-INFO` & `pygn-0.9.14/pygn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygn
-Version: 0.9.13
+Version: 0.9.14
 Summary: The Python Gateway Script: news2mail mail2news gateway
 Home-page: https://gitlab.com/mcepl/pyg
 Author: Cosimo Alfarano, Matej Cepl
 Author-email: kalfa@debian.org, mcepl@cepl.eu
 License: GPLv3
 Description: Python Gateway Script from news to mail and vice versa.
```

### Comparing `pygn-0.9.13/test/test_pyg.py` & `pygn-0.9.14/test/test_pyg.py`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/test/test_wlp.py` & `pygn-0.9.14/test/test_wlp.py`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/README` & `pygn-0.9.14/README`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/mail2news.py` & `pygn-0.9.14/mail2news.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import sys
 
 
 #logging.basicConfig(level=logging.DEBUG)
 # This is the single source of Truth
 # Yes, it is awkward to have it assymetrically here
 # and not in news2mail as well.
-VERSION = '0.9.13'
+VERSION = '0.9.14'
 DESC = "The Python Gateway Script: news2mail mail2news gateway"
 
 
 class mail2news(object):
     """news to mail gateway class"""
 
     def __init__(self, options):
```

### Comparing `pygn-0.9.13/news2mail.py` & `pygn-0.9.14/news2mail.py`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/pygm2n` & `pygn-0.9.14/pygm2n`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/pygn2m` & `pygn-0.9.14/pygn2m`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/setup.py` & `pygn-0.9.14/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 setup(name='pygn',
       version=VERSION,  # the current Debian version is 0.9.8
       author="Cosimo Alfarano, Matej Cepl",
       author_email="kalfa@debian.org, mcepl@cepl.eu",
       description=DESC,
       long_description=read('README'),
       url='https://gitlab.com/mcepl/pyg',
-      py_modules=['mail2news', 'news2mail', 'setup', 'whitelist'],
+      py_modules=['mail2news', 'news2mail', 'setup',
+                  'whitelist', 'wlp', 'wlp_parser'],
       test_suite="test",
       scripts=['pygm2n', 'pygn2m'],
       requires=['rply'],
       license="GPLv3",
       keywords=["nntp", "email", "gateway"],
       classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `pygn-0.9.13/whitelist.py` & `pygn-0.9.14/whitelist.py`

 * *Files identical despite different names*

### Comparing `pygn-0.9.13/PKG-INFO` & `pygn-0.9.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygn
-Version: 0.9.13
+Version: 0.9.14
 Summary: The Python Gateway Script: news2mail mail2news gateway
 Home-page: https://gitlab.com/mcepl/pyg
 Author: Cosimo Alfarano, Matej Cepl
 Author-email: kalfa@debian.org, mcepl@cepl.eu
 License: GPLv3
 Description: Python Gateway Script from news to mail and vice versa.
```

