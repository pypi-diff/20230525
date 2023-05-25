# Comparing `tmp/pgml-0.5.1.tar.gz` & `tmp/pgml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgml-0.5.1.tar", last modified: Wed Apr 20 23:02:14 2022, max compression
+gzip compressed data, was "pgml-0.6.0.tar", max compression
```

## Comparing `pgml-0.5.1.tar` & `pgml-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 23:02:14.552221 pgml-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-20 23:02:14.552221 pgml-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-04-20 23:01:58.000000 pgml-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 23:02:14.552221 pgml-0.5.1/pgml/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-04-20 23:01:58.000000 pgml-0.5.1/pgml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-04-20 23:01:58.000000 pgml-0.5.1/pgml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-20 23:01:58.000000 pgml-0.5.1/pgml/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    23638 2022-04-20 23:01:58.000000 pgml-0.5.1/pgml/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-20 23:01:58.000000 pgml-0.5.1/pgml/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 23:02:14.552221 pgml-0.5.1/pgml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-20 23:02:14.000000 pgml-0.5.1/pgml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-04-20 23:02:14.000000 pgml-0.5.1/pgml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 23:02:14.000000 pgml-0.5.1/pgml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-20 23:02:14.000000 pgml-0.5.1/pgml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-20 23:02:14.000000 pgml-0.5.1/pgml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-20 23:02:14.552221 pgml-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-04-20 23:01:58.000000 pgml-0.5.1/setup.py
+-rw-r--r--   0        0        0    14964 2023-05-25 19:03:39.727488 pgml-0.6.0/README.md
+-rw-r--r--   0        0        0      187 2023-05-23 22:45:11.017123 pgml-0.6.0/pgml/__init__.py
+-rw-r--r--   0        0        0    34213 2023-05-24 23:22:00.246179 pgml-0.6.0/pgml/collection.py
+-rw-r--r--   0        0        0     4345 2023-05-23 22:45:11.017794 pgml-0.6.0/pgml/database.py
+-rw-r--r--   0        0        0     3627 2023-05-25 00:40:33.188921 pgml-0.6.0/pgml/dbutils.py
+-rw-r--r--   0        0        0      621 2023-05-25 19:56:23.864497 pgml-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    15758 1970-01-01 00:00:00.000000 pgml-0.6.0/PKG-INFO
```

