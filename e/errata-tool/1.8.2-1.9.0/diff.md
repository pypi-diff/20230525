# Comparing `tmp/errata-tool-1.8.2.tar.gz` & `tmp/errata-tool-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/errata-tool-1.8.2.tar", last modified: Wed Aug 23 18:57:45 2017, max compression
+gzip compressed data, was "dist/errata-tool-1.9.0.tar", last modified: Tue Oct  3 16:14:51 2017, max compression
```

## Comparing `errata-tool-1.8.2.tar` & `errata-tool-1.9.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     7777 2017-08-23 18:57:45.000000 errata-tool-1.8.2/PKG-INFO
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     4363 2017-08-23 18:54:33.000000 errata-tool-1.8.2/setup.py
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    12945 2017-08-23 18:54:33.000000 errata-tool-1.8.2/errata_tool/products.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    32733 2017-08-23 18:54:33.000000 errata-tool-1.8.2/errata_tool/erratum.py
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      630 2017-04-06 17:25:03.000000 errata-tool-1.8.2/errata_tool/tests/test_change_docs_reviewer.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2567 2017-08-23 18:54:33.000000 errata-tool-1.8.2/errata_tool/tests/conftest.py
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1246 2017-04-04 19:08:27.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products.json
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/104/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      602 2017-04-04 19:08:27.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/104/product_versions.json
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/78/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1212 2017-04-04 19:08:27.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/78/product_versions.json
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     6986 2017-03-27 22:45:09.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175/builds.json
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1781 2017-03-27 22:45:09.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175.json
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/build/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    12180 2017-03-27 22:45:09.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/build/ceph-10.2.5-37.el7cp
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/erratum/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    49761 2017-03-27 22:45:09.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/erratum/26175
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1669 2017-04-04 19:08:27.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/releases?page[number]=1
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       12 2017-04-04 19:08:27.000000 errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/releases?page[number]=2
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2740 2017-04-20 21:14:56.000000 errata-tool-1.8.2/errata_tool/tests/test_products.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2582 2017-04-20 21:14:54.000000 errata-tool-1.8.2/errata_tool/tests/test_advisory.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      614 2017-05-30 20:32:50.000000 errata-tool-1.8.2/errata_tool/tests/test_add_cc.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      491 2016-08-31 15:43:53.000000 errata-tool-1.8.2/errata_tool/tests/test_init.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1040 2017-02-14 16:17:06.000000 errata-tool-1.8.2/errata_tool/security.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      191 2017-08-23 18:54:33.000000 errata-tool-1.8.2/errata_tool/__init__.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       43 2016-08-26 20:39:11.000000 errata-tool-1.8.2/errata_tool/exception.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     8673 2017-03-27 22:48:16.000000 errata-tool-1.8.2/errata_tool/connector.py
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1079 2016-08-31 17:15:18.000000 errata-tool-1.8.2/LICENSE
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      536 2017-02-14 16:17:06.000000 errata-tool-1.8.2/Makefile
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     5809 2017-08-23 18:54:33.000000 errata-tool-1.8.2/README.rst
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       38 2017-08-23 18:57:45.000000 errata-tool-1.8.2/setup.cfg
-drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool.egg-info/
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     7777 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool.egg-info/PKG-INFO
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       12 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool.egg-info/top_level.txt
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)        1 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)        1 2016-08-26 20:46:56.000000 errata-tool-1.8.2/errata_tool.egg-info/not-zip-safe
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       43 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool.egg-info/requires.txt
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1394 2017-08-23 18:57:45.000000 errata-tool-1.8.2/errata_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      241 2017-03-27 22:45:09.000000 errata-tool-1.8.2/.gitignore
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2154 2017-08-23 18:54:33.000000 errata-tool-1.8.2/python-errata-tool.spec
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       33 2016-08-26 20:56:33.000000 errata-tool-1.8.2/.coveragerc
--rwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)      611 2017-04-04 19:08:27.000000 errata-tool-1.8.2/new-fixture.sh
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1046 2017-03-27 22:48:16.000000 errata-tool-1.8.2/.travis.yml
--rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     4910 2017-08-23 18:54:33.000000 errata-tool-1.8.2/CHANGELOG.rst
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     8307 2017-10-03 16:14:51.000000 errata-tool-1.9.0/PKG-INFO
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     4363 2017-08-23 18:54:33.000000 errata-tool-1.9.0/setup.py
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    13014 2017-10-02 20:03:08.000000 errata-tool-1.9.0/errata_tool/products.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    33240 2017-10-03 16:06:54.000000 errata-tool-1.9.0/errata_tool/erratum.py
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      630 2017-04-06 17:25:03.000000 errata-tool-1.9.0/errata_tool/tests/test_change_docs_reviewer.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2567 2017-09-22 16:49:01.000000 errata-tool-1.9.0/errata_tool/tests/conftest.py
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1246 2017-04-04 19:08:27.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products.json
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/104/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      602 2017-04-04 19:08:27.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/104/product_versions.json
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/78/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1212 2017-04-04 19:08:27.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/78/product_versions.json
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     6986 2017-03-27 22:45:09.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175/builds.json
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1781 2017-03-27 22:45:09.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175.json
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/build/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    12180 2017-03-27 22:45:09.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/build/ceph-10.2.5-37.el7cp
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/erratum/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)    49761 2017-03-27 22:45:09.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/erratum/26175
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1669 2017-04-04 19:08:27.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/releases?page[number]=1
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       12 2017-04-04 19:08:27.000000 errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/releases?page[number]=2
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2740 2017-04-20 21:14:56.000000 errata-tool-1.9.0/errata_tool/tests/test_products.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2582 2017-04-20 21:14:54.000000 errata-tool-1.9.0/errata_tool/tests/test_advisory.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      614 2017-05-30 20:32:50.000000 errata-tool-1.9.0/errata_tool/tests/test_add_cc.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      491 2016-08-31 15:43:53.000000 errata-tool-1.9.0/errata_tool/tests/test_init.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1040 2017-02-14 16:17:06.000000 errata-tool-1.9.0/errata_tool/security.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      191 2017-10-03 16:14:01.000000 errata-tool-1.9.0/errata_tool/__init__.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       43 2016-08-26 20:39:11.000000 errata-tool-1.9.0/errata_tool/exception.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     8673 2017-09-22 16:39:49.000000 errata-tool-1.9.0/errata_tool/connector.py
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1079 2016-08-31 17:15:18.000000 errata-tool-1.9.0/LICENSE
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      536 2017-02-14 16:17:06.000000 errata-tool-1.9.0/Makefile
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     6243 2017-10-02 20:03:08.000000 errata-tool-1.9.0/README.rst
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       38 2017-10-03 16:14:51.000000 errata-tool-1.9.0/setup.cfg
+drwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)        0 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool.egg-info/
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     8307 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       12 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool.egg-info/top_level.txt
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)        1 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)        1 2016-08-26 20:46:56.000000 errata-tool-1.9.0/errata_tool.egg-info/not-zip-safe
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       43 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool.egg-info/requires.txt
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1394 2017-10-03 16:14:51.000000 errata-tool-1.9.0/errata_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)      241 2017-03-27 22:45:09.000000 errata-tool-1.9.0/.gitignore
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     2154 2017-10-03 16:14:01.000000 errata-tool-1.9.0/python-errata-tool.spec
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)       33 2016-08-26 20:56:33.000000 errata-tool-1.9.0/.coveragerc
+-rwxrwxr-x   0 kdreyer   (1000) kdreyer   (1000)      611 2017-04-04 19:08:27.000000 errata-tool-1.9.0/new-fixture.sh
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     1046 2017-03-27 22:48:16.000000 errata-tool-1.9.0/.travis.yml
+-rw-rw-r--   0 kdreyer   (1000) kdreyer   (1000)     5155 2017-10-03 16:13:35.000000 errata-tool-1.9.0/CHANGELOG.rst
```

### Comparing `errata-tool-1.8.2/PKG-INFO` & `errata-tool-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: errata-tool
-Version: 1.8.2
+Version: 1.9.0
 Summary: Python API for Red Hat Errata Tool
 Home-page: https://github.com/red-hat-storage/errata-tool
 Author: Ken Dreyer
 Author-email: kdreyer@redhat.com
 License: MIT
 Description: ``errata-tool``
         ===============
@@ -195,14 +195,26 @@
         Where "RH-IT-Root-CA.crt" is the public cert that signed the ET server's
         HTTPS certificate.
         
         When using RHEL 7's python-requests RPM, requests simply checks
         ``/etc/pki/tls/certs/ca-bundle.crt``, so you'll need to add the IT CA cert to
         that big bundle file.
         
+        If you've already added the Red Hat IT CA to your system-wide bundle, you can
+        have your Python code always use this file:
+        
+        .. code-block:: python
+        
+            if 'REQUESTS_CA_BUNDLE' not in os.environ:
+                os.environ['REQUESTS_CA_BUNDLE'] = '/etc/pki/tls/certs/ca-bundle.crt'
+        
+        This will make requests behave the same inside or outside your virtualenv. In
+        other words, with this code, your program will always validate the Red Hat IT
+        CA.
+        
         Building RPMs
         -------------
         
         Install fedpkg, then use the Makefile::
         
             $ make srpm
```

### Comparing `errata-tool-1.8.2/setup.py` & `errata-tool-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/products.py` & `errata-tool-1.9.0/errata_tool/products.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,16 +138,17 @@
                 info['bz_flags'] = []
                 for f in attrs['blocker_flags']:
                     if f not in ('devel_ack', 'pm_ack', 'qa_ack'):
                         info['bz_flags'].append(f)
 
                 info['versions'] = {}
                 info['products'] = {}
-                for t in r['relationships']['product_versions']:
-                    info['versions'][int(t['id'])] = t['name']
+                if 'product_versions' in r['relationships']:
+                    for t in r['relationships']['product_versions']:
+                        info['versions'][int(t['id'])] = t['name']
 
                 releases[int(r['id'])] = info
 
             page = page + 1
         self.releases = releases
 
     #
```

### Comparing `errata-tool-1.8.2/errata_tool/erratum.py` & `errata-tool-1.9.0/errata_tool/erratum.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.current_flags = []
 
     def update(self, **kwargs):
         if 'errata_type' in kwargs:
             self.errata_type = kwargs['errata_type']
             self._update = True
         if 'text_only' in kwargs:
-            self.errata_type = kwargs['text_only']
+            self.text_only = kwargs['text_only']
             self._update = True
         if 'date' in kwargs:
             try:
                 datetime.datetime.strptime(kwargs['date'], '%Y-%b-%d')
             except ValueError:
                 raise ValueError(
                     'Date must be of the form: YYYY-MON-DD; 2015-Mar-11')
@@ -176,14 +176,21 @@
                 print('do not have requested data bailing')
                 return None
 
             # Short circuit to get the advisory
             for key in advisory['errata']:
                 erratum = advisory['errata'][key]
                 self.errata_type = key.upper()
+                # We cannot PUT a "PDC_"-prefixed value back to the server.
+                # The server expects "RHBA", not "PDC_RHBA". We will just
+                # remove the type internally here.
+                # (See bz 1493773 for background on why the key has the pdc_
+                # prefix here.)
+                if self.errata_type.startswith('PDC_'):
+                    self.errata_type = self.errata_type[4:]
                 break
 
             self.errata_id = erratum['id']
             # NEW_FILES QE etc.
             self.errata_state = erratum['status']
             self._original_state = self.errata_state
 
@@ -313,16 +320,15 @@
     def _cache_bug_info(self, bug_id_list):
         # Omitted: RHOS shale's use of bz_cache here.
         pass
 
     def _check_rpmdiff(self):
         # Check for rpmdiff failures (NEW_FILES state only)
         # rpmdiff_runs.json
-        url = "/advisory/" + str(self.errata_id)
-        url += '/rpmdiff_runs.json'
+        url = "/advisory/%i/rpmdiff_runs.json" % self.errata_id
         r = self._get(url)
         if r is not None:
             for rpmdiff in r:
                 rpmdiff_run = rpmdiff['rpmdiff_run']
                 if rpmdiff_run['obsolete'] == 1:
                     continue
                 if rpmdiff_run['overall_score'] == 3 or \
@@ -331,16 +337,15 @@
                     break
                 if rpmdiff_run['overall_score'] == 499 or \
                    rpmdiff_run['overall_score'] == 500:
                     self.addFlags('rpmdiff_wait')
 
     def _check_tps(self):
         # Check for TPS failure (QE state only)
-        url = '/advisory/'
-        url += str(self.errata_id) + '/tps_jobs.json'
+        url = '/advisory/%i/tps_jobs.json' % self.errata_id
         r = self._get(url)
         distqa_tps = 0
         distqa_passing = 0
         for tps in r:
             if tps['rhnqa'] is True:
                 distqa_tps = distqa_tps + 1
             if tps['state'] == 'BAD' or \
@@ -370,16 +375,15 @@
     def _get_build_list(self, check_signatures=False):
         # Grab build list; store on a per-key basis
         # REFERENCE
 
         # Item 5.2.10.3. GET /advisory/{id}/builds.json
         # Then try to check to see if they are signed or not
         # Item 5.2.2.1. GET /api/v1/build/{id_or_nvr}
-        url = "/advisory/" + str(self.errata_id)
-        url += "/builds.json"
+        url = "/advisory/%i/builds.json" % self.errata_id
         rj = self._get(url)
         have_all_sigs = True
         for k in rj:
             builds = []
             for i in rj[k]:
                 for b in i:
                     builds.append(b)
@@ -392,15 +396,15 @@
             self.errata_builds[k] = builds
         if have_all_sigs:
             self.removeFlags(['request_sigs', 'needs_sigs'])
 
     def _fetch_by_bug(self, bug_id):
         # print("fetch_by_bug")
         try:
-            url = "/bugs/" + str(bug_id) + "/advisories.json"
+            url = "/bugs/%i/advisories.json" % bug_id
             rj = self._get(url)
 
             stored = False
             for e in rj:
                 if not stored:
                     stored = True
                     self._fetch(e['id'])
@@ -556,16 +560,15 @@
                     continue
             val = {}
             if file_types is not None and b in file_types:
                 val['file_types'] = file_types[b]
             val['build'] = b
             val['product_version'] = release
             pdata.append(val)
-        url = "/api/v1/erratum/" + str(self.errata_id)
-        url += "/add_builds"
+        url = "/api/v1/erratum/%i/add_builds" % self.errata_id
         r = self._post(url, json=pdata)
         self._processResponse(r)
         self._buildschanged = True
         return
 
     def addBuilds(self, buildlist, **kwargs):
         if self._new:
@@ -587,16 +590,15 @@
         if type(file_info) is not dict:
             raise ValueError('file_info is not a dict')
         if len(file_info) < 1:
             return
 
         # Get:
 
-        url = '/api/v1/erratum/' + str(self.errata_id)
-        url += '/filemeta'
+        url = '/api/v1/erratum/%i/filemeta' % self.errata_id
         r = self._get(url)
 
         info = []
         files = [k for k in file_info]
         for f in r:
             # print(f['file']['path'] + f['file']['id'])
             fn = os.path.basename(f['file']['path'])
@@ -622,16 +624,15 @@
             builds = []
             builds.append(buildlist)
         else:
             builds = buildlist
         for b in builds:
             val = {}
             val['nvr'] = b
-            url = "/api/v1/erratum/" + str(self.errata_id)
-            url += "/remove_build"
+            url = "/api/v1/erratum/%i/remove_build" % self.errata_id
             r = self._post(url, data=val)
             self._processResponse(r)
         self._buildschanged = True
 
     def _write(self):
         pdata = {}
 
@@ -731,42 +732,45 @@
             # REFERENCE
 
             # New is 'POST'
             url = "/api/v1/erratum"
             r = self._post(url, data=pdata)
             self._processResponse(r)
             rj = r.json()
-            self.errata_id = \
-                rj['errata'][self.errata_type.lower()]['errata_id']
+            # This might need a "pdc_" prefix, rhbz 1493773 for background
+            json_errata_type = self.errata_type.lower()
+            try:
+                rj['errata'][json_errata_type]
+            except KeyError:
+                json_errata_type = 'pdc_%s' % json_errata_type
+                rj['errata'][json_errata_type]
+            self.errata_id = rj['errata'][json_errata_type]['errata_id']
             # XXX return JSON returns full advisory name but not
             # typical advisory name - e.g. RHSA-2015:19999-01, but not
             # RHSA-2015:19999, but it's close enough
-            self.errata_name = \
-                rj['errata'][self.errata_type.lower()]['fulladvisory']
+            self.errata_name = rj['errata'][json_errata_type]['fulladvisory']
         else:
             # REFERENCE
 
             # Update is 'PUT'
-            url = "/api/v1/erratum/" + str(self.errata_id)
+            url = "/api/v1/erratum/%i" % self.errata_id
             r = self._put(url, data=pdata)
         self._processResponse(r)
 
         # XXX WOW VERY HACK
         # If deleting last bug...
         if last_bug is not None:
             # This doesn't work to remove the last bug, nor does setting
             # idsfixed to empty-string
-            # url = ("/api/v1/erratum/" +
-            #        str(self.errata_id) + "/remove_bug")
+            # url = "/api/v1/erratum/%i/remove_bug" % self.errata_id
             # pdata = {'bug': str(last_bug)}
 
             # Solution: Use hacks to pretend we're using the remove-bugs
             # web UI :(
-            url = ('/bugs/remove_bugs_from_errata/' +
-                   str(self.errata_id))
+            url = '/bugs/remove_bugs_from_errata/%i' % self.errata_id
             pdata = {}
             pdata['bug[' + str(last_bug) + ']'] = 1
 
             # Handle weird interaction we get in this particular case
             try:
                 r = self._post(url, data=pdata)
             except requests_kerberos.exceptions.MutualAuthenticationError:
@@ -775,15 +779,15 @@
 
     def _putStatus(self):
         # REFERENCE
 
         # State change is 'POST'
         pdata = {}
         pdata['new_state'] = self.errata_state
-        url = "/api/v1/erratum/" + str(self.errata_id)
+        url = "/api/v1/erratum/%i" % self.errata_id
         url += "/change_state"
         r = self._post(url, data=pdata)
         self._processResponse(r)
 
     def commit(self):
         ret = False
         # Commit changes
```

### Comparing `errata-tool-1.8.2/errata_tool/tests/test_change_docs_reviewer.py` & `errata-tool-1.9.0/errata_tool/tests/test_change_docs_reviewer.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/conftest.py` & `errata-tool-1.9.0/errata_tool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products.json` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products.json`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/104/product_versions.json` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/104/product_versions.json`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/products/78/product_versions.json` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/products/78/product_versions.json`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175/builds.json` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175/builds.json`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175.json` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/advisory/26175.json`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/build/ceph-10.2.5-37.el7cp` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/build/ceph-10.2.5-37.el7cp`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/erratum/26175` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/erratum/26175`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/releases?page[number]=1` & `errata-tool-1.9.0/errata_tool/tests/fixtures/errata.devel.redhat.com/api/v1/releases?page[number]=1`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/test_products.py` & `errata-tool-1.9.0/errata_tool/tests/test_products.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/test_advisory.py` & `errata-tool-1.9.0/errata_tool/tests/test_advisory.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/tests/test_add_cc.py` & `errata-tool-1.9.0/errata_tool/tests/test_add_cc.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/security.py` & `errata-tool-1.9.0/errata_tool/security.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/errata_tool/connector.py` & `errata-tool-1.9.0/errata_tool/connector.py`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/LICENSE` & `errata-tool-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/Makefile` & `errata-tool-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/README.rst` & `errata-tool-1.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -339,26 +339,53 @@
 00001520: 2072 6571 7565 7374 7320 7369 6d70 6c79   requests simply
 00001530: 2063 6865 636b 730a 6060 2f65 7463 2f70   checks.``/etc/p
 00001540: 6b69 2f74 6c73 2f63 6572 7473 2f63 612d  ki/tls/certs/ca-
 00001550: 6275 6e64 6c65 2e63 7274 6060 2c20 736f  bundle.crt``, so
 00001560: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
 00001570: 6164 6420 7468 6520 4954 2043 4120 6365  add the IT CA ce
 00001580: 7274 2074 6f0a 7468 6174 2062 6967 2062  rt to.that big b
-00001590: 756e 646c 6520 6669 6c65 2e0a 0a42 7569  undle file...Bui
-000015a0: 6c64 696e 6720 5250 4d73 0a2d 2d2d 2d2d  lding RPMs.-----
-000015b0: 2d2d 2d2d 2d2d 2d2d 0a0a 496e 7374 616c  --------..Instal
-000015c0: 6c20 6665 6470 6b67 2c20 7468 656e 2075  l fedpkg, then u
-000015d0: 7365 2074 6865 204d 616b 6566 696c 653a  se the Makefile:
-000015e0: 3a0a 0a20 2020 2024 206d 616b 6520 7372  :..    $ make sr
-000015f0: 706d 0a0a 596f 7520 6361 6e20 7468 656e  pm..You can then
-00001600: 2075 706c 6f61 6420 7468 6520 5352 504d   upload the SRPM
-00001610: 2074 6f20 436f 7072 2e20 4f72 2c20 746f   to Copr. Or, to
-00001620: 2062 7569 6c64 2052 504d 7320 6f6e 2079   build RPMs on y
-00001630: 6f75 7220 6c6f 6361 6c0a 636f 6d70 7574  our local.comput
-00001640: 6572 2c20 7573 696e 6720 6d6f 636b 3a3a  er, using mock::
-00001650: 0a0a 2020 2020 2420 6d61 6b65 2072 706d  ..    $ make rpm
-00001660: 0a0a 0a43 6861 6e67 656c 6f67 0a2d 2d2d  ...Changelog.---
-00001670: 2d2d 2d2d 2d2d 0a43 6865 636b 206f 7574  ------.Check out
-00001680: 2074 6865 2060 4348 414e 4745 4c4f 4760   the `CHANGELOG`
-00001690: 5f2e 0a0a 2e2e 205f 4348 414e 4745 4c4f  _..... _CHANGELO
-000016a0: 473a 2043 4841 4e47 454c 4f47 2e72 7374  G: CHANGELOG.rst
-000016b0: 0a                                       .
+00001590: 756e 646c 6520 6669 6c65 2e0a 0a49 6620  undle file...If 
+000015a0: 796f 7527 7665 2061 6c72 6561 6479 2061  you've already a
+000015b0: 6464 6564 2074 6865 2052 6564 2048 6174  dded the Red Hat
+000015c0: 2049 5420 4341 2074 6f20 796f 7572 2073   IT CA to your s
+000015d0: 7973 7465 6d2d 7769 6465 2062 756e 646c  ystem-wide bundl
+000015e0: 652c 2079 6f75 2063 616e 0a68 6176 6520  e, you can.have 
+000015f0: 796f 7572 2050 7974 686f 6e20 636f 6465  your Python code
+00001600: 2061 6c77 6179 7320 7573 6520 7468 6973   always use this
+00001610: 2066 696c 653a 0a0a 2e2e 2063 6f64 652d   file:.... code-
+00001620: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+00001630: 2020 2020 6966 2027 5245 5155 4553 5453      if 'REQUESTS
+00001640: 5f43 415f 4255 4e44 4c45 2720 6e6f 7420  _CA_BUNDLE' not 
+00001650: 696e 206f 732e 656e 7669 726f 6e3a 0a20  in os.environ:. 
+00001660: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
+00001670: 6e5b 2752 4551 5545 5354 535f 4341 5f42  n['REQUESTS_CA_B
+00001680: 554e 444c 4527 5d20 3d20 272f 6574 632f  UNDLE'] = '/etc/
+00001690: 706b 692f 746c 732f 6365 7274 732f 6361  pki/tls/certs/ca
+000016a0: 2d62 756e 646c 652e 6372 7427 0a0a 5468  -bundle.crt'..Th
+000016b0: 6973 2077 696c 6c20 6d61 6b65 2072 6571  is will make req
+000016c0: 7565 7374 7320 6265 6861 7665 2074 6865  uests behave the
+000016d0: 2073 616d 6520 696e 7369 6465 206f 7220   same inside or 
+000016e0: 6f75 7473 6964 6520 796f 7572 2076 6972  outside your vir
+000016f0: 7475 616c 656e 762e 2049 6e0a 6f74 6865  tualenv. In.othe
+00001700: 7220 776f 7264 732c 2077 6974 6820 7468  r words, with th
+00001710: 6973 2063 6f64 652c 2079 6f75 7220 7072  is code, your pr
+00001720: 6f67 7261 6d20 7769 6c6c 2061 6c77 6179  ogram will alway
+00001730: 7320 7661 6c69 6461 7465 2074 6865 2052  s validate the R
+00001740: 6564 2048 6174 2049 540a 4341 2e0a 0a42  ed Hat IT.CA...B
+00001750: 7569 6c64 696e 6720 5250 4d73 0a2d 2d2d  uilding RPMs.---
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e 7374  ----------..Inst
+00001770: 616c 6c20 6665 6470 6b67 2c20 7468 656e  all fedpkg, then
+00001780: 2075 7365 2074 6865 204d 616b 6566 696c   use the Makefil
+00001790: 653a 3a0a 0a20 2020 2024 206d 616b 6520  e::..    $ make 
+000017a0: 7372 706d 0a0a 596f 7520 6361 6e20 7468  srpm..You can th
+000017b0: 656e 2075 706c 6f61 6420 7468 6520 5352  en upload the SR
+000017c0: 504d 2074 6f20 436f 7072 2e20 4f72 2c20  PM to Copr. Or, 
+000017d0: 746f 2062 7569 6c64 2052 504d 7320 6f6e  to build RPMs on
+000017e0: 2079 6f75 7220 6c6f 6361 6c0a 636f 6d70   your local.comp
+000017f0: 7574 6572 2c20 7573 696e 6720 6d6f 636b  uter, using mock
+00001800: 3a3a 0a0a 2020 2020 2420 6d61 6b65 2072  ::..    $ make r
+00001810: 706d 0a0a 0a43 6861 6e67 656c 6f67 0a2d  pm...Changelog.-
+00001820: 2d2d 2d2d 2d2d 2d2d 0a43 6865 636b 206f  --------.Check o
+00001830: 7574 2074 6865 2060 4348 414e 4745 4c4f  ut the `CHANGELO
+00001840: 4760 5f2e 0a0a 2e2e 205f 4348 414e 4745  G`_..... _CHANGE
+00001850: 4c4f 473a 2043 4841 4e47 454c 4f47 2e72  LOG: CHANGELOG.r
+00001860: 7374 0a                                  st.
```

### Comparing `errata-tool-1.8.2/errata_tool.egg-info/PKG-INFO` & `errata-tool-1.9.0/errata_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: errata-tool
-Version: 1.8.2
+Version: 1.9.0
 Summary: Python API for Red Hat Errata Tool
 Home-page: https://github.com/red-hat-storage/errata-tool
 Author: Ken Dreyer
 Author-email: kdreyer@redhat.com
 License: MIT
 Description: ``errata-tool``
         ===============
@@ -195,14 +195,26 @@
         Where "RH-IT-Root-CA.crt" is the public cert that signed the ET server's
         HTTPS certificate.
         
         When using RHEL 7's python-requests RPM, requests simply checks
         ``/etc/pki/tls/certs/ca-bundle.crt``, so you'll need to add the IT CA cert to
         that big bundle file.
         
+        If you've already added the Red Hat IT CA to your system-wide bundle, you can
+        have your Python code always use this file:
+        
+        .. code-block:: python
+        
+            if 'REQUESTS_CA_BUNDLE' not in os.environ:
+                os.environ['REQUESTS_CA_BUNDLE'] = '/etc/pki/tls/certs/ca-bundle.crt'
+        
+        This will make requests behave the same inside or outside your virtualenv. In
+        other words, with this code, your program will always validate the Red Hat IT
+        CA.
+        
         Building RPMs
         -------------
         
         Install fedpkg, then use the Makefile::
         
             $ make srpm
```

### Comparing `errata-tool-1.8.2/errata_tool.egg-info/SOURCES.txt` & `errata-tool-1.9.0/errata_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/python-errata-tool.spec` & `errata-tool-1.9.0/python-errata-tool.spec`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 %global with_python3 1
 %global _docdir_fmt %{name}
 %endif
 
 %global pkgname errata-tool
 
 Name:           python-%{pkgname}
-Version:        1.8.2
+Version:        1.9.0
 Release:        1%{?dist}
 Summary:        Modern Python API to Red Hat's Errata Tool
 Group:          Development/Languages
 
 License:        MIT
 URL:            https://github.com/red-hat-storage/errata-tool
```

### Comparing `errata-tool-1.8.2/new-fixture.sh` & `errata-tool-1.9.0/new-fixture.sh`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/.travis.yml` & `errata-tool-1.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `errata-tool-1.8.2/CHANGELOG.rst` & `errata-tool-1.9.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v1.9.0
+======
+
+* Fix traceback in ``ProductList`` if a release has no versions associated.
+
+* Fix ability to change an existing advisory to be text-only or non-text-only.
+
+* Basic PDC support: Gracefully handle PDC prefixes for advisory types.
+
 v1.8.2
 ======
 
 * New project URL: https://github.com/red-hat-storage/errata-tool
 
 * Avoid re-adding the RHSA severity prefix to an advisory's synopsis when
   making unrelated updates.
```

