# Comparing `tmp/logfrog-0.10.tar.gz` & `tmp/logfrog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfrog-0.10.tar", last modified: Thu May 25 20:49:57 2023, max compression
+gzip compressed data, was "logfrog-1.0.0.tar", last modified: Thu May 25 20:54:46 2023, max compression
```

## Comparing `logfrog-0.10.tar` & `logfrog-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lakshya.gupta   (501) staff       (20)        0 2023-05-25 20:49:57.155183 logfrog-0.10/
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)     1070 2023-05-25 20:25:08.000000 logfrog-0.10/LICENSE.txt
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)      412 2023-05-25 20:49:57.154681 logfrog-0.10/PKG-INFO
-drwxr-xr-x   0 lakshya.gupta   (501) staff       (20)        0 2023-05-25 20:49:57.151516 logfrog-0.10/logfrog/
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)       28 2023-05-25 20:26:51.000000 logfrog-0.10/logfrog/__init__.py
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)     1920 2023-05-25 20:26:58.000000 logfrog-0.10/logfrog/logfrog.py
-drwxr-xr-x   0 lakshya.gupta   (501) staff       (20)        0 2023-05-25 20:49:57.153999 logfrog-0.10/logfrog.egg-info/
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)      412 2023-05-25 20:49:57.000000 logfrog-0.10/logfrog.egg-info/PKG-INFO
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)      183 2023-05-25 20:49:57.000000 logfrog-0.10/logfrog.egg-info/SOURCES.txt
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)        1 2023-05-25 20:49:57.000000 logfrog-0.10/logfrog.egg-info/dependency_links.txt
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)        8 2023-05-25 20:49:57.000000 logfrog-0.10/logfrog.egg-info/top_level.txt
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)       38 2023-05-25 20:49:57.155307 logfrog-0.10/setup.cfg
--rw-r--r--   0 lakshya.gupta   (501) staff       (20)      510 2023-05-25 20:49:11.000000 logfrog-0.10/setup.py
+drwxr-xr-x   0 lakshya.gupta   (501) staff       (20)        0 2023-05-25 20:54:46.577035 logfrog-1.0.0/
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)     1070 2023-05-25 20:25:08.000000 logfrog-1.0.0/LICENSE.txt
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)     2505 2023-05-25 20:54:46.576543 logfrog-1.0.0/PKG-INFO
+drwxr-xr-x   0 lakshya.gupta   (501) staff       (20)        0 2023-05-25 20:54:46.573872 logfrog-1.0.0/logfrog/
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)       28 2023-05-25 20:26:51.000000 logfrog-1.0.0/logfrog/__init__.py
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)     1920 2023-05-25 20:26:58.000000 logfrog-1.0.0/logfrog/logfrog.py
+drwxr-xr-x   0 lakshya.gupta   (501) staff       (20)        0 2023-05-25 20:54:46.575772 logfrog-1.0.0/logfrog.egg-info/
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)     2505 2023-05-25 20:54:46.000000 logfrog-1.0.0/logfrog.egg-info/PKG-INFO
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)      183 2023-05-25 20:54:46.000000 logfrog-1.0.0/logfrog.egg-info/SOURCES.txt
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)        1 2023-05-25 20:54:46.000000 logfrog-1.0.0/logfrog.egg-info/dependency_links.txt
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)        8 2023-05-25 20:54:46.000000 logfrog-1.0.0/logfrog.egg-info/top_level.txt
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)       38 2023-05-25 20:54:46.577199 logfrog-1.0.0/setup.cfg
+-rw-r--r--   0 lakshya.gupta   (501) staff       (20)      613 2023-05-25 20:54:05.000000 logfrog-1.0.0/setup.py
```

### Comparing `logfrog-0.10/LICENSE.txt` & `logfrog-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logfrog-0.10/logfrog/logfrog.py` & `logfrog-1.0.0/logfrog/logfrog.py`

 * *Files identical despite different names*

