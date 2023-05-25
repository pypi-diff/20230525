# Comparing `tmp/django-ows-lib-0.2.0.tar.gz` & `tmp/django-ows-lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ows-lib-0.2.0.tar", last modified: Wed May 17 06:21:11 2023, max compression
+gzip compressed data, was "django-ows-lib-0.3.0.tar", last modified: Thu May 25 07:04:40 2023, max compression
```

## Comparing `django-ows-lib-0.2.0.tar` & `django-ows-lib-0.3.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/django_ows_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/csw/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/wms130.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/models/ogc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/csw/
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/gml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/gml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/gml/gml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/django_ows_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/csw/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/wms130.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/models/ogc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/xml_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/gml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/gml/gml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/setup.py
```

### Comparing `django-ows-lib-0.2.0/LICENSE` & `django-ows-lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/PKG-INFO` & `django-ows-lib-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.2.0/README.rst` & `django-ows-lib-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/django_ows_lib.egg-info/PKG-INFO` & `django-ows-lib-0.3.0/django_ows_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.2.0/django_ows_lib.egg-info/SOURCES.txt` & `django-ows-lib-0.3.0/django_ows_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/csw/mixins.py` & `django-ows-lib-0.3.0/ows_lib/client/csw/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/enums.py` & `django-ows-lib-0.3.0/ows_lib/client/enums.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/exceptions.py` & `django-ows-lib-0.3.0/ows_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/mixins.py` & `django-ows-lib-0.3.0/ows_lib/client/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/utils.py` & `django-ows-lib-0.3.0/ows_lib/client/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/wfs/mixins.py` & `django-ows-lib-0.3.0/ows_lib/client/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/client/wms/mixins.py` & `django-ows-lib-0.3.0/ows_lib/client/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/models/ogc_request.py` & `django-ows-lib-0.3.0/ows_lib/models/ogc_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 
 class OGCRequest(Request):
     """Extended Request class which provides some analyzing functionality for ogc requests."""
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self._params_lower: dict = {}
-        self._ogc_query_params: dict = {}
+        self._ogc_query_params: Dict = {}
         self._bbox: GEOSGeometry = None
         self._requested_entities: List[str] = []
         self._xml_request: XmlObject = None
 
         if self.method == "GET":
-            self.operation: str = self.params_lower.get("request", "")
-            self.service_version: str = self.params_lower.get("version", "")
-            self.service_type: str = self.params_lower.get("service", "")
+            self.operation: str = self.ogc_query_params.get("REQUEST", "")
+            self.service_version: str = self.ogc_query_params.get(
+                "VERSION", "")
+            self.service_type: str = self.ogc_query_params.get("SERVICE", "")
         elif self.method == "POST":
             post_request: PostRequest = load_xmlobject_from_string(
                 string=self.data, xmlclass=PostRequest)
 
             self.operation: str = post_request.operation
             self.service_version: str = post_request.version
             self.service_type: str = post_request.service_type
@@ -45,20 +45,20 @@
 
         :return: list of requested layers | list of request featuretypes
         :rtype: List[str]
         """
         if not self._requested_entities:
             if self.is_wms:
                 self._requested_entities.extend(
-                    get_requested_layers(params=self.params_lower))
+                    get_requested_layers(params=self.ogc_query_params))
             else:
                 if self.is_get_feature_request:
                     if self.is_get:
                         self._requested_entities.extend(
-                            get_requested_feature_types(params=self.params_lower))
+                            get_requested_feature_types(params=self.ogc_query_params))
                     elif self.is_post:
                         self._requested_entities.extend(
                             self.xml_request.requested_feature_types)
         return self._requested_entities
 
     @property
     def is_wms(self) -> bool:
@@ -99,51 +99,51 @@
     @property
     def is_get_capabilities_request(self) -> bool:
         """Check for ogc get capabilites request
 
         :return: true if this is a get capabilities request
         :rtype: bool
         """
-        return self.operation.lower() == OGCOperationEnum.GET_CAPABILITIES.value.lower()
+        return self.operation == OGCOperationEnum.GET_CAPABILITIES.value
 
     @property
     def is_get_map_request(self) -> bool:
         """Check for wms get map request
 
         :return: true if this is a wms get map request
         :rtype: bool
         """
-        return self.operation.lower() == OGCOperationEnum.GET_MAP.value.lower()
+        return self.operation == OGCOperationEnum.GET_MAP.value
 
     @property
     def is_get_feature_info_request(self) -> bool:
         """Check for wms transaction request
 
         :return: true if this is a wfs tranasction request
         :rtype: bool
         """
-        return self.operation.lower() == OGCOperationEnum.GET_FEATURE_INFO.value.lower()
+        return self.operation == OGCOperationEnum.GET_FEATURE_INFO.value
 
     @property
     def is_get_feature_request(self) -> bool:
         """Check for wfs get feature request
 
         :return: true if this is a wfs get feature request
         :rtype: bool
         """
-        return self.operation.lower() == OGCOperationEnum.GET_FEATURE.value.lower()
+        return self.operation == OGCOperationEnum.GET_FEATURE.value
 
     @property
     def is_transaction_request(self) -> bool:
         """Check for wfs transaction request
 
         :return: true if this is a wfs tranasction request
         :rtype: bool
         """
-        return self.operation.lower() == OGCOperationEnum.TRANSACTION.value.lower()
+        return self.operation == OGCOperationEnum.TRANSACTION.value
 
     @property
     def bbox(self) -> GEOSGeometry:
         """Analyzes the given request and tries to construct a Polygon from the query parameters.
 
         The axis order for different wms/wfs versions will be well transformed to the correct needed mathematical interpretation.
 
@@ -152,42 +152,44 @@
 
         :return: the given bbox as polygon object
         :rtype: GEOSGeometry
         """
         if not self._bbox:
             try:
                 self._bbox = construct_polygon_from_bbox_query_param(
-                    get_dict=self.params_lower)
+                    get_dict=self.ogc_query_params)
             except (MissingBboxParam, MissingServiceParam):
                 # only to avoid error while handling sql in service property
                 self._bbox = GEOSGeometry("POLYGON EMPTY")
         return self._bbox
 
     @property
-    def params_lower(self) -> Dict:
-        """Lower case key mapper for paramas
-
-        :return: all parameters of the request in lower case key
-        :rtype: Dict
-        """
-        return {k.lower(): v for k, v in self.params.items()} if not self._params_lower else self._params_lower
-
-    @property
     def ogc_query_params(self) -> Dict:
         """ Parses the GET parameters into all member variables, which can be found in a ogc request.
+
         :return: all ogc query parameters
         :rtype: Dict
         """
         if not self._ogc_query_params:
             query_keys = ["SERVICE", "REQUEST", "LAYERS", "BBOX", "VERSION", "FORMAT",
                           "OUTPUTFORMAT", "SRS", "CRS", "SRSNAME", "WIDTH", "HEIGHT",
                           "TRANSPARENT", "EXCEPTIONS", "BGCOLOR", "TIME", "ELEVATION",
                           "QUERY_LAYERS", "INFO_FORMAT", "FEATURE_COUNT", "I", "J"]
-            self._ogc_query_params = {key: self.params_lower.get(
-                key, self.params_lower.get(key.lower())) for key in query_keys}
+
+            for key in query_keys:
+                value = self.params.get(key, self.params.get(key.lower(), ""))
+
+                if value:
+                    if isinstance(value, list):
+                        # if multiple values are passed in multiple queryparams, we pick the first item
+                        value = value[0]
+
+                    self._ogc_query_params.update({
+                        key: value
+                    })
 
         return self._ogc_query_params
 
     @property
     def xml_request(self) -> XmlObject:
         """Constructs a xml request object based on the given request.
```

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/csw/csw202.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/csw/csw202.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/mixins.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/mixins.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms111.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms111.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms130.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms130.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/mixins.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/namespaces.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/namespaces.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/utils.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py` & `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.2.0/setup.py` & `django-ows-lib-0.3.0/setup.py`

 * *Files identical despite different names*

