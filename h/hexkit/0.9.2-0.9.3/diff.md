# Comparing `tmp/hexkit-0.9.2.tar.gz` & `tmp/hexkit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexkit-0.9.2.tar", last modified: Tue Mar 14 14:37:47 2023, max compression
+gzip compressed data, was "hexkit-0.9.3.tar", last modified: Wed May 24 14:01:10 2023, max compression
```

## Comparing `hexkit-0.9.2.tar` & `hexkit-0.9.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.966062 hexkit-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-03-14 14:37:30.000000 hexkit-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-14 14:37:47.966062 hexkit-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-14 14:37:30.000000 hexkit-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.958062 hexkit-0.9.2/hexkit/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/inject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.958062 hexkit-0.9.2/hexkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16350 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/protocols/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/protocols/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/protocols/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/protocols/objstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.958062 hexkit-0.9.2/hexkit/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.958062 hexkit-0.9.2/hexkit/providers/akafka/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/akafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/akafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/akafka/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.962062 hexkit-0.9.2/hexkit/providers/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/mongodb/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/mongodb/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.962062 hexkit-0.9.2/hexkit/providers/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32659 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.962062 hexkit-0.9.2/hexkit/providers/s3/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/s3/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.962062 hexkit-0.9.2/hexkit/providers/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/providers/testing/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-14 14:37:30.000000 hexkit-0.9.2/hexkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.958062 hexkit-0.9.2/hexkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-14 14:37:47.000000 hexkit-0.9.2/hexkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-14 14:37:47.000000 hexkit-0.9.2/hexkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:37:47.000000 hexkit-0.9.2/hexkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:37:47.000000 hexkit-0.9.2/hexkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 14:37:47.000000 hexkit-0.9.2/hexkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-14 14:37:47.000000 hexkit-0.9.2/hexkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-14 14:37:47.966062 hexkit-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-03-14 14:37:30.000000 hexkit-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.954062 hexkit-0.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.962062 hexkit-0.9.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/config_env_var_sets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/inject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.962062 hexkit-0.9.2/tests/fixtures/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.966062 hexkit-0.9.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/integration/test_akafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/integration/test_akafka_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/integration/test_inject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/integration/test_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:37:47.966062 hexkit-0.9.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_akafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_eventpub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_eventsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_testing_eventpub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-14 14:37:30.000000 hexkit-0.9.2/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.809886 hexkit-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-24 14:00:59.000000 hexkit-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-24 14:01:10.809886 hexkit-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-24 14:00:59.000000 hexkit-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.797886 hexkit-0.9.3/hexkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/inject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.797886 hexkit-0.9.3/hexkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16350 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/protocols/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/protocols/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/protocols/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/protocols/objstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.801886 hexkit-0.9.3/hexkit/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.801886 hexkit-0.9.3/hexkit/providers/akafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/akafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/akafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/akafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.801886 hexkit-0.9.3/hexkit/providers/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/mongodb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/mongodb/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.801886 hexkit-0.9.3/hexkit/providers/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32659 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.801886 hexkit-0.9.3/hexkit/providers/s3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/s3/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.801886 hexkit-0.9.3/hexkit/providers/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/providers/testing/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-24 14:00:59.000000 hexkit-0.9.3/hexkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.797886 hexkit-0.9.3/hexkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-24 14:01:10.000000 hexkit-0.9.3/hexkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-24 14:01:10.000000 hexkit-0.9.3/hexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:01:10.000000 hexkit-0.9.3/hexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:01:10.000000 hexkit-0.9.3/hexkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-24 14:01:10.000000 hexkit-0.9.3/hexkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 14:01:10.000000 hexkit-0.9.3/hexkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-24 14:01:10.809886 hexkit-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-24 14:00:59.000000 hexkit-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.793886 hexkit-0.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.805886 hexkit-0.9.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/config_env_var_sets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/inject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.805886 hexkit-0.9.3/tests/fixtures/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.805886 hexkit-0.9.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/integration/test_akafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/integration/test_akafka_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/integration/test_inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/integration/test_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:10.809886 hexkit-0.9.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_akafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_testing_eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-24 14:00:59.000000 hexkit-0.9.3/tests/unit/test_utils.py
```

### Comparing `hexkit-0.9.2/LICENSE` & `hexkit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/PKG-INFO` & `hexkit-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Home-page: https://github.com/ghga-de/hexkit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `hexkit-0.9.2/README.md` & `hexkit-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/__init__.py` & `hexkit-0.9.3/hexkit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A Toolkit for Building Microservices using the Hexagonal Architecture"""
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
```

### Comparing `hexkit-0.9.2/hexkit/__main__.py` & `hexkit-0.9.3/hexkit/__main__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/base.py` & `hexkit-0.9.3/hexkit/base.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/config.py` & `hexkit-0.9.3/hexkit/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/custom_types.py` & `hexkit-0.9.3/hexkit/custom_types.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/inject.py` & `hexkit-0.9.3/hexkit/inject.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,10 +216,10 @@
 
 def get_configurator(
     pydantic_cls: type[PydanticConfig],
 ) -> Configurator[PydanticConfig]:
     """Initializes a configuration provider.
 
     This helper function is necessary because the __init__ of Providers used by the
-    dependency_injector framework need to always use the same singnature."""
+    dependency_injector framework need to always use the same signature."""
 
     return Configurator[PydanticConfig](pydantic_cls)
```

### Comparing `hexkit-0.9.2/hexkit/protocols/__init__.py` & `hexkit-0.9.3/hexkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/protocols/dao.py` & `hexkit-0.9.3/hexkit/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/protocols/eventpub.py` & `hexkit-0.9.3/hexkit/protocols/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/protocols/eventsub.py` & `hexkit-0.9.3/hexkit/protocols/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/protocols/objstorage.py` & `hexkit-0.9.3/hexkit/protocols/objstorage.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/__init__.py` & `hexkit-0.9.3/hexkit/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/akafka/__init__.py` & `hexkit-0.9.3/hexkit/providers/akafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/akafka/provider.py` & `hexkit-0.9.3/hexkit/providers/akafka/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,29 @@
 
 Require dependencies of the `akafka` extra. See the `setup.cfg`.
 """
 
 import json
 import logging
 from contextlib import asynccontextmanager
-from typing import Any, Callable, Literal, Protocol, TypeVar
+from typing import Any, Callable, Protocol, TypeVar
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from pydantic import BaseSettings, Field
 
 from hexkit.base import InboundProviderBase
 from hexkit.custom_types import Ascii, JsonObject
 from hexkit.protocols.eventpub import EventPublisherProtocol
 from hexkit.protocols.eventsub import EventSubscriberProtocol
 
+try:  # workaround for https://github.com/pydantic/pydantic/issues/5821
+    from typing_extensions import Literal
+except ImportError:
+    from typing import Literal  # type: ignore
+
 __all__ = [
     "KafkaConfig",
     "KafkaEventPublisher",
     "ConsumerEvent",
     "KafkaEventSubscriber",
 ]
 
@@ -248,15 +253,15 @@
         ...
 
     async def stop(self) -> None:
         """Teardown the consumer."""
         ...
 
     def __aiter__(self: KCC) -> KCC:
-        """Returns an asnyc iterator for iterating through events."""  #
+        """Returns an async iterator for iterating through events."""  #
         ...
 
     async def __anext__(self) -> ConsumerEvent:
         """Used to get the next event."""
         ...
```

### Comparing `hexkit-0.9.2/hexkit/providers/akafka/testutils.py` & `hexkit-0.9.3/hexkit/providers/akafka/testutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,26 +353,26 @@
         self, *, payload: JsonObject, type_: Ascii, topic: Ascii, key: Ascii = "test"
     ) -> None:
         """A convenience method to publish a test event."""
 
         await self.publisher.publish(payload=payload, type_=type_, key=key, topic=topic)
 
     def record_events(self, *, in_topic: Ascii) -> EventRecorder:
-        """Constructs an EventRecorder object that can be used in an asnyc with block to
+        """Constructs an EventRecorder object that can be used in an async with block to
         record events in the specified topic upon __aenter__ and stops the recording
         upon __aexit__.
         """
 
         return EventRecorder(kafka_servers=self.kafka_servers, topic=in_topic)
 
     @asynccontextmanager
     async def expect_events(
         self, events: Sequence[ExpectedEvent], *, in_topic: Ascii
     ) -> AsyncGenerator[EventRecorder, None]:
-        """Can be used in an asnyc with block to record events in the specified topic
+        """Can be used in an async with block to record events in the specified topic
         (on __aenter__) and check that they match the specified sequence of expected
         events (on __aexit__).
         """
 
         async with self.record_events(in_topic=in_topic) as event_recorder:
             yield event_recorder
```

### Comparing `hexkit-0.9.2/hexkit/providers/mongodb/__init__.py` & `hexkit-0.9.3/hexkit/providers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/mongodb/provider.py` & `hexkit-0.9.3/hexkit/providers/mongodb/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/mongodb/testutils.py` & `hexkit-0.9.3/hexkit/providers/mongodb/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/s3/__init__.py` & `hexkit-0.9.3/hexkit/providers/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/s3/provider.py` & `hexkit-0.9.3/hexkit/providers/s3/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/s3/test_files/__init__.py` & `hexkit-0.9.3/hexkit/providers/s3/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/s3/testutils.py` & `hexkit-0.9.3/hexkit/providers/s3/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/testing/__init__.py` & `hexkit-0.9.3/hexkit/providers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/providers/testing/eventpub.py` & `hexkit-0.9.3/hexkit/providers/testing/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit/utils.py` & `hexkit-0.9.3/hexkit/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit.egg-info/PKG-INFO` & `hexkit-0.9.3/hexkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Home-page: https://github.com/ghga-de/hexkit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `hexkit-0.9.2/hexkit.egg-info/SOURCES.txt` & `hexkit-0.9.3/hexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/hexkit.egg-info/requires.txt` & `hexkit-0.9.3/hexkit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/setup.cfg` & `hexkit-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/setup.py` & `hexkit-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/fixtures/__init__.py` & `hexkit-0.9.3/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/fixtures/config.py` & `hexkit-0.9.3/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/fixtures/inject.py` & `hexkit-0.9.3/tests/fixtures/inject.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/fixtures/test_files/__init__.py` & `hexkit-0.9.3/tests/fixtures/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/fixtures/utils.py` & `hexkit-0.9.3/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/integration/__init__.py` & `hexkit-0.9.3/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/integration/test_akafka.py` & `hexkit-0.9.3/tests/integration/test_akafka.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/integration/test_akafka_testutils.py` & `hexkit-0.9.3/tests/integration/test_akafka_testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/integration/test_inject.py` & `hexkit-0.9.3/tests/integration/test_inject.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/integration/test_mongodb.py` & `hexkit-0.9.3/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/integration/test_s3.py` & `hexkit-0.9.3/tests/integration/test_s3.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/__init__.py` & `hexkit-0.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_akafka.py` & `hexkit-0.9.3/tests/unit/test_akafka.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_config.py` & `hexkit-0.9.3/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_dao.py` & `hexkit-0.9.3/tests/unit/test_dao.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_eventpub.py` & `hexkit-0.9.3/tests/unit/test_eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_eventsub.py` & `hexkit-0.9.3/tests/unit/test_eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_inject.py` & `hexkit-0.9.3/tests/unit/test_inject.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_testing_eventpub.py` & `hexkit-0.9.3/tests/unit/test_testing_eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-0.9.2/tests/unit/test_utils.py` & `hexkit-0.9.3/tests/unit/test_utils.py`

 * *Files identical despite different names*

