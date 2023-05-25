# Comparing `tmp/Gamerig-0.0.4.tar.gz` & `tmp/Gamerig-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gamerig-0.0.4.tar", last modified: Thu May 25 19:35:39 2023, max compression
+gzip compressed data, was "Gamerig-0.0.5.tar", last modified: Thu May 25 19:46:52 2023, max compression
```

## Comparing `Gamerig-0.0.4.tar` & `Gamerig-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 19:35:39.340216 Gamerig-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-25 19:35:39.321018 Gamerig-0.0.4/GamerIg/
--rw-rw-rw-   0        0        0     6526 2023-05-25 19:32:23.000000 Gamerig-0.0.4/GamerIg/__init__.py
--rw-rw-rw-   0        0        0     5643 2023-05-25 08:45:42.000000 Gamerig-0.0.4/GamerIg/cookies.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:35:39.340216 Gamerig-0.0.4/Gamerig.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-25 19:35:39.000000 Gamerig-0.0.4/Gamerig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-25 19:35:39.000000 Gamerig-0.0.4/Gamerig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 19:35:39.000000 Gamerig-0.0.4/Gamerig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-25 19:35:39.000000 Gamerig-0.0.4/Gamerig.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 19:35:39.000000 Gamerig-0.0.4/Gamerig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 Gamerig-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      584 2023-05-25 19:35:39.340216 Gamerig-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-25 19:35:39.342865 Gamerig-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-25 19:35:24.000000 Gamerig-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:46:52.776800 Gamerig-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-25 19:46:52.753505 Gamerig-0.0.5/GamerIg/
+-rw-rw-rw-   0        0        0     6533 2023-05-25 19:46:46.000000 Gamerig-0.0.5/GamerIg/__init__.py
+-rw-rw-rw-   0        0        0     5643 2023-05-25 08:45:42.000000 Gamerig-0.0.5/GamerIg/tokens.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:46:52.776800 Gamerig-0.0.5/Gamerig.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-25 19:46:52.000000 Gamerig-0.0.5/Gamerig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-25 19:46:52.000000 Gamerig-0.0.5/Gamerig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 19:46:52.000000 Gamerig-0.0.5/Gamerig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-25 19:46:52.000000 Gamerig-0.0.5/Gamerig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 19:46:52.000000 Gamerig-0.0.5/Gamerig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 Gamerig-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      584 2023-05-25 19:46:52.776800 Gamerig-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-25 19:46:52.776800 Gamerig-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-05-25 19:44:16.000000 Gamerig-0.0.5/setup.py
```

### Comparing `Gamerig-0.0.4/GamerIg/__init__.py` & `Gamerig-0.0.5/GamerIg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import httpx
 import random
 import uuid
 from time import *
 import string
 import secrets
 import binascii
-from cookies import Tokens
+from GamerIg.tokens import Tokens
 
 
 
 
 def generateRandomString(n):
     # Generate a random string of length n
     return ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(n))
```

### Comparing `Gamerig-0.0.4/GamerIg/cookies.py` & `Gamerig-0.0.5/GamerIg/tokens.py`

 * *Files identical despite different names*

### Comparing `Gamerig-0.0.4/Gamerig.egg-info/PKG-INFO` & `Gamerig-0.0.5/Gamerig.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Gamerig
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Gamerig-0.0.4/LICENSE` & `Gamerig-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Gamerig-0.0.4/PKG-INFO` & `Gamerig-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Gamerig
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Gamerig-0.0.4/setup.py` & `Gamerig-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Instagram Android Api For Login '
 LONG_DESCRIPTION = 'A package to perform login in instagram using beta api'
 
 # Setting up
 setup(
     name="Gamerig",
     version=VERSION,
```

