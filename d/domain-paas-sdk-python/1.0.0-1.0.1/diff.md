# Comparing `tmp/domain-paas-sdk-python-1.0.0.tar.gz` & `tmp/domain-paas-sdk-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-paas-sdk-python-1.0.0.tar", last modified: Wed May 24 11:48:10 2023, max compression
+gzip compressed data, was "domain-paas-sdk-python-1.0.1.tar", last modified: Wed May 24 12:07:06 2023, max compression
```

## Comparing `domain-paas-sdk-python-1.0.0.tar` & `domain-paas-sdk-python-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:48:10.811058 domain-paas-sdk-python-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 11:48:10.811058 domain-paas-sdk-python-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:48:10.811058 domain-paas-sdk-python-1.0.0/domain_paas_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 11:48:10.000000 domain-paas-sdk-python-1.0.0/domain_paas_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 11:48:10.000000 domain-paas-sdk-python-1.0.0/domain_paas_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:48:10.000000 domain-paas-sdk-python-1.0.0/domain_paas_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 11:48:10.000000 domain-paas-sdk-python-1.0.0/domain_paas_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:48:10.000000 domain-paas-sdk-python-1.0.0/domain_paas_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:48:10.811058 domain-paas-sdk-python-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-24 11:47:58.000000 domain-paas-sdk-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:07:06.464164 domain-paas-sdk-python-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 12:07:06.464164 domain-paas-sdk-python-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:07:06.464164 domain-paas-sdk-python-1.0.1/domain_paas_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 12:07:06.000000 domain-paas-sdk-python-1.0.1/domain_paas_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 12:07:06.000000 domain-paas-sdk-python-1.0.1/domain_paas_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:07:06.000000 domain-paas-sdk-python-1.0.1/domain_paas_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 12:07:06.000000 domain-paas-sdk-python-1.0.1/domain_paas_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:07:06.000000 domain-paas-sdk-python-1.0.1/domain_paas_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:07:06.464164 domain-paas-sdk-python-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-24 12:06:51.000000 domain-paas-sdk-python-1.0.1/setup.py
```

