# Comparing `tmp/analysisbykwok-0.0.28.tar.gz` & `tmp/analysisbykwok-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.28.tar", last modified: Thu May 25 10:34:37 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.29.tar", last modified: Thu May 25 10:37:47 2023, max compression
```

## Comparing `analysisbykwok-0.0.28.tar` & `analysisbykwok-0.0.29.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:34:37.061844 analysisbykwok-0.0.28/
--rw-rw-rw-   0        0        0       62 2023-05-25 10:34:37.061844 analysisbykwok-0.0.28/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 10:34:37.053865 analysisbykwok-0.0.28/analysisbykwok/
--rw-rw-rw-   0        0        0    19098 2023-05-25 10:33:11.000000 analysisbykwok-0.0.28/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-25 10:33:30.000000 analysisbykwok-0.0.28/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:34:37.060847 analysisbykwok-0.0.28/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-05-25 10:34:37.000000 analysisbykwok-0.0.28/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-25 10:34:37.000000 analysisbykwok-0.0.28/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:34:37.000000 analysisbykwok-0.0.28/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 10:34:37.000000 analysisbykwok-0.0.28/analysisbykwok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 10:34:37.000000 analysisbykwok-0.0.28/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-05-25 10:33:37.000000 analysisbykwok-0.0.28/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 10:34:37.061844 analysisbykwok-0.0.28/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 10:37:47.219898 analysisbykwok-0.0.29/
+-rw-rw-rw-   0        0        0       62 2023-05-25 10:37:47.218902 analysisbykwok-0.0.29/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 10:37:47.212916 analysisbykwok-0.0.29/analysisbykwok/
+-rw-rw-rw-   0        0        0    19183 2023-05-25 10:37:07.000000 analysisbykwok-0.0.29/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-25 10:37:20.000000 analysisbykwok-0.0.29/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:37:47.218902 analysisbykwok-0.0.29/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-05-25 10:37:47.000000 analysisbykwok-0.0.29/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-25 10:37:47.000000 analysisbykwok-0.0.29/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 10:37:47.000000 analysisbykwok-0.0.29/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 10:37:47.000000 analysisbykwok-0.0.29/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 10:37:47.000000 analysisbykwok-0.0.29/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-05-25 10:37:15.000000 analysisbykwok-0.0.29/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 10:37:47.219898 analysisbykwok-0.0.29/setup.cfg
```

### Comparing `analysisbykwok-0.0.28/analysisbykwok/__init__.py` & `analysisbykwok-0.0.29/analysisbykwok/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pandas as pd
 import requests
 import random
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
 import email
 import imaplib
 import numpy as np
 import re
 from email.header import decode_header
 import execjs
 import json
```

