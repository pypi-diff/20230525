# Comparing `tmp/agraph-python-6.2.2.0.3.tar.gz` & `tmp/agraph-python-6.2.2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agraph-python-6.2.2.0.3.tar", last modified: Fri Jun  9 18:57:38 2017, max compression, from Unix
+gzip compressed data, was "agraph-python-6.2.2.0.4.tar", last modified: Tue Jun 20 15:44:41 2017, max compression, from Unix
```

## Comparing `agraph-python-6.2.2.0.3.tar` & `agraph-python-6.2.2.0.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/
--rw-r--r--   0 dancy      (443) ftp         (50)     1058 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/LICENSE
--rw-r--r--   0 dancy      (443) ftp         (50)    12019 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/PKG-INFO
--rw-r--r--   0 dancy      (443) ftp         (50)      223 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/MANIFEST.in
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/
--rw-r--r--   0 dancy      (443) ftp         (50)      487 2017-06-09 18:02:54.000000 agraph-python-6.2.2.0.3/src/franz/__init__.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/
--rw-r--r--   0 dancy      (443) ftp         (50)      922 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/exceptions.py
--rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/__init__.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/model/
--rw-r--r--   0 dancy      (443) ftp         (50)     4784 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/model/value.py
--rw-r--r--   0 dancy      (443) ftp         (50)      749 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/model/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)    16646 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/model/literal.py
--rw-r--r--   0 dancy      (443) ftp         (50)     4928 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/model/statement.py
--rw-r--r--   0 dancy      (443) ftp         (50)     4667 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/model/valuefactory.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/sail/
--rw-r--r--   0 dancy      (443) ftp         (50)      549 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/sail/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)     4910 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/sail/sail.py
--rw-r--r--   0 dancy      (443) ftp         (50)     1322 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/sail/spec.py
--rw-r--r--   0 dancy      (443) ftp         (50)    19418 2017-03-14 18:14:51.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/sail/allegrographserver.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/repository/
--rw-r--r--   0 dancy      (443) ftp         (50)      533 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/repository/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)    55838 2017-03-15 15:04:48.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/repository/repositoryconnection.py
--rw-r--r--   0 dancy      (443) ftp         (50)     6455 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/repository/repository.py
--rw-r--r--   0 dancy      (443) ftp         (50)     5675 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/repository/repositoryresult.py
--rw-r--r--   0 dancy      (443) ftp         (50)     5814 2017-03-14 18:14:51.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/connect.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/rio/
--rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/rio/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)     1080 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/rio/rdfxmlwriter.py
--rw-r--r--   0 dancy      (443) ftp         (50)     5466 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/rio/rdfformat.py
--rw-r--r--   0 dancy      (443) ftp         (50)     1391 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/rio/rdfwriter.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/query/
--rw-r--r--   0 dancy      (443) ftp         (50)     2889 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/query/dataset.py
--rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/query/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)     7854 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/query/queryresult.py
--rw-r--r--   0 dancy      (443) ftp         (50)    10173 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/query/query.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/util/
--rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/util/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)     2339 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/util/uris.py
--rw-r--r--   0 dancy      (443) ftp         (50)     6897 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/util/namedtuple.py
--rw-r--r--   0 dancy      (443) ftp         (50)      798 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/util/contexts.py
--rw-r--r--   0 dancy      (443) ftp         (50)     4627 2017-05-22 14:18:31.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/util/strings.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/
--rw-r--r--   0 dancy      (443) ftp         (50)      364 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)     5533 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy.ttl.gz
--rw-r--r--   0 dancy      (443) ftp         (50)     2770 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/test.cert
--rw-r--r--   0 dancy      (443) ftp         (50)     2083 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/tz.py
--rwxr-xr-x   0 dancy      (443) ftp         (50)      416 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/ssl-dir.sh
--rw-r--r--   0 dancy      (443) ftp         (50)   127981 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy.ntriples
--rw-r--r--   0 dancy      (443) ftp         (50)     8465 2017-05-22 14:18:31.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/newtests.py
--rw-r--r--   0 dancy      (443) ftp         (50)     2209 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy-error.nt
--rw-r--r--   0 dancy      (443) ftp         (50)     2586 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/relative_rules.txt
--rw-r--r--   0 dancy      (443) ftp         (50)   104097 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/tests.py
--rw-r--r--   0 dancy      (443) ftp         (50)     2308 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/conftest.py
--rw-r--r--   0 dancy      (443) ftp         (50)     1155 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/vc-db-1.rdf
--rw-r--r--   0 dancy      (443) ftp         (50)    79052 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy.ttl
--rw-r--r--   0 dancy      (443) ftp         (50)     2472 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/ca.cert
--rw-r--r--   0 dancy      (443) ftp         (50)    61212 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/tests/lesmis.rdf
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/
--rw-r--r--   0 dancy      (443) ftp         (50)      675 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)     1934 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/rdfs.py
--rw-r--r--   0 dancy      (443) ftp         (50)     3579 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/xmlschema.py
--rw-r--r--   0 dancy      (443) ftp         (50)     1866 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/rdf.py
--rw-r--r--   0 dancy      (443) ftp         (50)     3573 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/owl.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/
--rw-r--r--   0 dancy      (443) ftp         (50)     6005 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/test.py
--rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)    13707 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/request.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/backends/
--rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/backends/__init__.py
--rw-r--r--   0 dancy      (443) ftp         (50)    11232 2017-03-27 17:45:54.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/backends/curl.py
--rw-r--r--   0 dancy      (443) ftp         (50)     9225 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/backends/requests.py
--rw-r--r--   0 dancy      (443) ftp         (50)    38365 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/repository.py
--rw-r--r--   0 dancy      (443) ftp         (50)      953 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/src/franz/miniclient/agjson.py
-drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/agraph_python.egg-info/
--rw-r--r--   0 dancy      (443) ftp         (50)        1 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/agraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 dancy      (443) ftp         (50)    12019 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/agraph_python.egg-info/PKG-INFO
--rw-r--r--   0 dancy      (443) ftp         (50)     2384 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/agraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 dancy      (443) ftp         (50)        6 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/agraph_python.egg-info/top_level.txt
--rw-r--r--   0 dancy      (443) ftp         (50)      102 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/src/agraph_python.egg-info/requires.txt
--rw-r--r--   0 dancy      (443) ftp         (50)      142 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/requirements.txt
--rw-r--r--   0 dancy      (443) ftp         (50)       19 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/requirements2.txt
--rw-r--r--   0 dancy      (443) ftp         (50)     8898 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/README.rst
--rw-r--r--   0 dancy      (443) ftp         (50)     2310 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.3/setup.py
--rw-r--r--   0 dancy      (443) ftp         (50)      101 2017-06-09 18:57:38.000000 agraph-python-6.2.2.0.3/setup.cfg
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/
+-rw-r--r--   0 dancy      (443) ftp         (50)     1058 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/LICENSE
+-rw-r--r--   0 dancy      (443) ftp         (50)    12019 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/PKG-INFO
+-rw-r--r--   0 dancy      (443) ftp         (50)      223 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/MANIFEST.in
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:40.000000 agraph-python-6.2.2.0.4/src/
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/
+-rw-r--r--   0 dancy      (443) ftp         (50)      487 2017-06-19 21:27:05.000000 agraph-python-6.2.2.0.4/src/franz/__init__.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/
+-rw-r--r--   0 dancy      (443) ftp         (50)      922 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/exceptions.py
+-rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/__init__.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/model/
+-rw-r--r--   0 dancy      (443) ftp         (50)     4784 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/model/value.py
+-rw-r--r--   0 dancy      (443) ftp         (50)      749 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/model/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    16646 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/model/literal.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     4928 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/model/statement.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     4667 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/model/valuefactory.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/sail/
+-rw-r--r--   0 dancy      (443) ftp         (50)      549 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/sail/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     4910 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/sail/sail.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     1322 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/sail/spec.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    19418 2017-03-14 18:14:51.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/sail/allegrographserver.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/repository/
+-rw-r--r--   0 dancy      (443) ftp         (50)      533 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/repository/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    55838 2017-03-15 15:04:48.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/repository/repositoryconnection.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     6455 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/repository/repository.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     5675 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/repository/repositoryresult.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     5814 2017-03-14 18:14:51.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/connect.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/rio/
+-rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/rio/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     1080 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/rio/rdfxmlwriter.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     5466 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/rio/rdfformat.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     1391 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/rio/rdfwriter.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/query/
+-rw-r--r--   0 dancy      (443) ftp         (50)     2889 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/query/dataset.py
+-rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/query/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     7854 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/query/queryresult.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    10173 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/query/query.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/util/
+-rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/util/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     2339 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/util/uris.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     6897 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/util/namedtuple.py
+-rw-r--r--   0 dancy      (443) ftp         (50)      798 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/util/contexts.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     4627 2017-05-22 14:18:31.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/util/strings.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/
+-rw-r--r--   0 dancy      (443) ftp         (50)      364 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     5533 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy.ttl.gz
+-rw-r--r--   0 dancy      (443) ftp         (50)     2770 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/test.cert
+-rw-r--r--   0 dancy      (443) ftp         (50)     2083 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/tz.py
+-rwxr-xr-x   0 dancy      (443) ftp         (50)      416 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/ssl-dir.sh
+-rw-r--r--   0 dancy      (443) ftp         (50)   127981 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy.ntriples
+-rw-r--r--   0 dancy      (443) ftp         (50)     8465 2017-05-22 14:18:31.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/newtests.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     2209 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy-error.nt
+-rw-r--r--   0 dancy      (443) ftp         (50)     2586 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/relative_rules.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)   104097 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/tests.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     2308 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/conftest.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     1155 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/vc-db-1.rdf
+-rw-r--r--   0 dancy      (443) ftp         (50)    79052 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy.ttl
+-rw-r--r--   0 dancy      (443) ftp         (50)     2472 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/ca.cert
+-rw-r--r--   0 dancy      (443) ftp         (50)    61212 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/tests/lesmis.rdf
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/
+-rw-r--r--   0 dancy      (443) ftp         (50)      675 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     1934 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/rdfs.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     3579 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/xmlschema.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     1866 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/rdf.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     3573 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/owl.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/
+-rw-r--r--   0 dancy      (443) ftp         (50)     6005 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/test.py
+-rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    13707 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/request.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/backends/
+-rw-r--r--   0 dancy      (443) ftp         (50)        0 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/backends/__init__.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    11232 2017-03-27 17:45:54.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/backends/curl.py
+-rw-r--r--   0 dancy      (443) ftp         (50)     9225 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/backends/requests.py
+-rw-r--r--   0 dancy      (443) ftp         (50)    38365 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/repository.py
+-rw-r--r--   0 dancy      (443) ftp         (50)      953 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/src/franz/miniclient/agjson.py
+drwxr-xr-x   0 dancy      (443) ftp         (50)        0 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/src/agraph_python.egg-info/
+-rw-r--r--   0 dancy      (443) ftp         (50)        1 2017-06-20 15:44:40.000000 agraph-python-6.2.2.0.4/src/agraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)    12019 2017-06-20 15:44:40.000000 agraph-python-6.2.2.0.4/src/agraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 dancy      (443) ftp         (50)     2384 2017-06-20 15:44:40.000000 agraph-python-6.2.2.0.4/src/agraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)        6 2017-06-20 15:44:40.000000 agraph-python-6.2.2.0.4/src/agraph_python.egg-info/top_level.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)      102 2017-06-20 15:44:40.000000 agraph-python-6.2.2.0.4/src/agraph_python.egg-info/requires.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)      142 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/requirements.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)       19 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/requirements2.txt
+-rw-r--r--   0 dancy      (443) ftp         (50)     8898 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/README.rst
+-rw-r--r--   0 dancy      (443) ftp         (50)     2310 2017-03-08 22:14:43.000000 agraph-python-6.2.2.0.4/setup.py
+-rw-r--r--   0 dancy      (443) ftp         (50)      101 2017-06-20 15:44:41.000000 agraph-python-6.2.2.0.4/setup.cfg
```

### Comparing `agraph-python-6.2.2.0.3/LICENSE` & `agraph-python-6.2.2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/PKG-INFO` & `agraph-python-6.2.2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: agraph-python
-Version: 6.2.2.0.3
+Version: 6.2.2.0.4
 Summary: AllegroGraph Python client
 Home-page: http://franz.com/agraph/support/documentation/current/python-tutorial/python-API.html
 Author: Franz Inc.
 Author-email: UNKNOWN
 License: EPL
 Description: AllegroGraph Python API
         =======================
```

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/exceptions.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/model/value.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/model/value.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/model/__init__.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/model/literal.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/model/literal.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/model/statement.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/model/statement.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/model/valuefactory.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/model/valuefactory.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/sail/__init__.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/sail/__init__.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/sail/sail.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/sail/sail.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/sail/spec.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/sail/spec.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/sail/allegrographserver.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/sail/allegrographserver.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/repository/__init__.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/repository/repositoryconnection.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/repository/repositoryconnection.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/repository/repository.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/repository/repository.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/repository/repositoryresult.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/repository/repositoryresult.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/connect.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/connect.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/rio/rdfxmlwriter.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/rio/rdfxmlwriter.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/rio/rdfformat.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/rio/rdfformat.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/rio/rdfwriter.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/rio/rdfwriter.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/query/dataset.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/query/dataset.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/query/queryresult.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/query/queryresult.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/query/query.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/query/query.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/util/uris.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/util/uris.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/util/namedtuple.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/util/namedtuple.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/util/contexts.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/util/contexts.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/util/strings.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/util/strings.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy.ttl.gz` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy.ttl.gz`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/test.cert` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/test.cert`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/tz.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/tz.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy.ntriples` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy.ntriples`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/newtests.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/newtests.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy-error.nt` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy-error.nt`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/relative_rules.txt` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/relative_rules.txt`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/tests.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/tests.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/conftest.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/vc-db-1.rdf` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/vc-db-1.rdf`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/kennedy.ttl` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/kennedy.ttl`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/ca.cert` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/ca.cert`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/tests/lesmis.rdf` & `agraph-python-6.2.2.0.4/src/franz/openrdf/tests/lesmis.rdf`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/__init__.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/__init__.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/rdfs.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/rdfs.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/xmlschema.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/xmlschema.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/rdf.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/rdf.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/openrdf/vocabulary/owl.py` & `agraph-python-6.2.2.0.4/src/franz/openrdf/vocabulary/owl.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/miniclient/test.py` & `agraph-python-6.2.2.0.4/src/franz/miniclient/test.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/miniclient/request.py` & `agraph-python-6.2.2.0.4/src/franz/miniclient/request.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/miniclient/backends/curl.py` & `agraph-python-6.2.2.0.4/src/franz/miniclient/backends/curl.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/miniclient/backends/requests.py` & `agraph-python-6.2.2.0.4/src/franz/miniclient/backends/requests.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/miniclient/repository.py` & `agraph-python-6.2.2.0.4/src/franz/miniclient/repository.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/franz/miniclient/agjson.py` & `agraph-python-6.2.2.0.4/src/franz/miniclient/agjson.py`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/src/agraph_python.egg-info/PKG-INFO` & `agraph-python-6.2.2.0.4/src/agraph_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: agraph-python
-Version: 6.2.2.0.3
+Version: 6.2.2.0.4
 Summary: AllegroGraph Python client
 Home-page: http://franz.com/agraph/support/documentation/current/python-tutorial/python-API.html
 Author: Franz Inc.
 Author-email: UNKNOWN
 License: EPL
 Description: AllegroGraph Python API
         =======================
```

### Comparing `agraph-python-6.2.2.0.3/src/agraph_python.egg-info/SOURCES.txt` & `agraph-python-6.2.2.0.4/src/agraph_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/README.rst` & `agraph-python-6.2.2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `agraph-python-6.2.2.0.3/setup.py` & `agraph-python-6.2.2.0.4/setup.py`

 * *Files identical despite different names*

