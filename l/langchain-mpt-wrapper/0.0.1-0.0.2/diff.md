# Comparing `tmp/langchain_mpt_wrapper-0.0.1.tar.gz` & `tmp/langchain_mpt_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/langchain_mpt_wrapper-0.0.1.tar", last modified: Thu May 25 07:48:20 2023, max compression
+gzip compressed data, was "dist/langchain_mpt_wrapper-0.0.2.tar", last modified: Thu May 25 07:54:41 2023, max compression
```

## Comparing `langchain_mpt_wrapper-0.0.1.tar` & `langchain_mpt_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/
--rw-r--r--   0 pawel      (501) staff       (20)      195 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/PKG-INFO
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper.egg-info/
--rw-r--r--   0 pawel      (501) staff       (20)      195 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      309 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 pawel      (501) staff       (20)       53 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper.egg-info/requires.txt
--rw-r--r--   0 pawel      (501) staff       (20)       22 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper.egg-info/top_level.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 pawel      (501) staff       (20)       24 2023-05-24 14:01:23.000000 langchain_mpt_wrapper-0.0.1/README.md
--rw-r--r--   0 pawel      (501) staff       (20)      307 2023-05-25 07:48:19.000000 langchain_mpt_wrapper-0.0.1/setup.py
--rw-r--r--   0 pawel      (501) staff       (20)       38 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/setup.cfg
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-05-25 07:48:20.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper/
--rw-r--r--   0 pawel      (501) staff       (20)     2568 2023-05-25 07:48:19.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper/wrapper.py
--rw-r--r--   0 pawel      (501) staff       (20)       37 2023-05-24 14:11:53.000000 langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper/__init__.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/
+-rw-r--r--   0 pawel      (501) staff       (20)      195 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/PKG-INFO
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper.egg-info/
+-rw-r--r--   0 pawel      (501) staff       (20)      195 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      309 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       53 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper.egg-info/requires.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       22 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       24 2023-05-24 14:01:23.000000 langchain_mpt_wrapper-0.0.2/README.md
+-rw-r--r--   0 pawel      (501) staff       (20)      307 2023-05-25 07:54:38.000000 langchain_mpt_wrapper-0.0.2/setup.py
+-rw-r--r--   0 pawel      (501) staff       (20)       38 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/setup.cfg
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-05-25 07:54:41.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper/
+-rw-r--r--   0 pawel      (501) staff       (20)     2568 2023-05-25 07:48:19.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper/wrapper.py
+-rw-r--r--   0 pawel      (501) staff       (20)       40 2023-05-25 07:54:38.000000 langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper/__init__.py
```

### Comparing `langchain_mpt_wrapper-0.0.1/langchain_mpt_wrapper/wrapper.py` & `langchain_mpt_wrapper-0.0.2/langchain_mpt_wrapper/wrapper.py`

 * *Files identical despite different names*

