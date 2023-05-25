# Comparing `tmp/pygbif-0.6.2.tar.gz` & `tmp/pygbif-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygbif-0.6.2.tar", last modified: Tue Jan 24 15:31:27 2023, max compression
+gzip compressed data, was "pygbif-0.6.3.tar", last modified: Thu May 25 12:24:06 2023, max compression
```

## Comparing `pygbif-0.6.2.tar` & `pygbif-0.6.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.310058 pygbif-0.6.2/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     5017 2022-05-04 11:01:45.000000 pygbif-0.6.2/CONDUCT.md
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     5631 2023-01-24 15:30:21.000000 pygbif-0.6.2/Changelog.rst
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1061 2022-05-04 11:01:45.000000 pygbif-0.6.2/LICENSE
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       27 2022-05-04 11:01:45.000000 pygbif-0.6.2/MANIFEST.in
--rw-r--r--   0 mblissett  (1001) gbif      (1000)    10800 2023-01-24 15:31:27.310058 pygbif-0.6.2/PKG-INFO
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     4522 2022-06-23 10:53:54.000000 pygbif-0.6.2/README.rst
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1912 2022-06-23 12:59:33.000000 pygbif-0.6.2/RELEASING.md
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.302059 pygbif-0.6.2/pygbif/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1672 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     3574 2022-06-23 10:53:54.000000 pygbif-0.6.2/pygbif/caching.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     6922 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/gbifissues.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     4354 2023-01-24 15:02:26.000000 pygbif-0.6.2/pygbif/gbifutils.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.306059 pygbif-0.6.2/pygbif/maps/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       30 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/maps/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     9372 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/maps/map.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.306059 pygbif-0.6.2/pygbif/occurrences/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1518 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/occurrences/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     4766 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/occurrences/count.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)    17531 2023-01-24 15:30:21.000000 pygbif-0.6.2/pygbif/occurrences/download.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1562 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/occurrences/get.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)    20844 2023-01-24 15:30:21.000000 pygbif-0.6.2/pygbif/occurrences/search.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       96 2023-01-24 14:53:00.000000 pygbif-0.6.2/pygbif/package_metadata.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.306059 pygbif-0.6.2/pygbif/registry/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      637 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/registry/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)    13450 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/registry/datasets.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     3457 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/registry/installations.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     2486 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/registry/networks.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     3950 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/registry/nodes.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     3417 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/registry/organizations.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.306059 pygbif-0.6.2/pygbif/species/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      862 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/species/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     3717 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/species/name_backbone.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     7978 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/species/name_lookup.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      694 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/species/name_parser.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     2894 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/species/name_suggest.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     5390 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/species/name_usage.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.306059 pygbif-0.6.2/pygbif/utils/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       35 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/utils/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1305 2022-05-04 11:01:45.000000 pygbif-0.6.2/pygbif/utils/wkt_rewind.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.306059 pygbif-0.6.2/pygbif.egg-info/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)    10800 2023-01-24 15:31:27.000000 pygbif-0.6.2/pygbif.egg-info/PKG-INFO
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1560 2023-01-24 15:31:27.000000 pygbif-0.6.2/pygbif.egg-info/SOURCES.txt
--rw-r--r--   0 mblissett  (1001) gbif      (1000)        1 2023-01-24 15:31:27.000000 pygbif-0.6.2/pygbif.egg-info/dependency_links.txt
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       76 2023-01-24 15:31:27.000000 pygbif-0.6.2/pygbif.egg-info/requires.txt
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       12 2023-01-24 15:31:27.000000 pygbif-0.6.2/pygbif.egg-info/top_level.txt
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       81 2022-06-23 11:54:14.000000 pygbif-0.6.2/pyproject.toml
--rw-r--r--   0 mblissett  (1001) gbif      (1000)       80 2023-01-24 15:31:27.310058 pygbif-0.6.2/setup.cfg
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1653 2023-01-24 15:30:21.000000 pygbif-0.6.2/setup.py
-drwxr-xr-x   0 mblissett  (1001) gbif      (1000)        0 2023-01-24 15:31:27.310058 pygbif-0.6.2/test/
--rw-r--r--   0 mblissett  (1001) gbif      (1000)        0 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/__init__.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     2362 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-maps-map.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     2699 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-occurrences-count.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      491 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-occurrences-download_cancel.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      333 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-occurrences-download_get.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     7105 2023-01-24 15:30:21.000000 pygbif-0.6.2/test/test-occurrences-download_request.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      918 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-occurrences-get.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1763 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-occurrences-search.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      765 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-registry-dataset_metrics.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      952 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-registry-datasets.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1083 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-registry-installations.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      964 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-registry-networks.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      980 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-registry-nodes.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1169 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-registry-organizations.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      737 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-species-name_backbone.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1429 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-species-name_lookup.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      668 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-species-name_suggest.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)     1027 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-species-name_usage.py
--rw-r--r--   0 mblissett  (1001) gbif      (1000)      753 2022-05-04 11:01:45.000000 pygbif-0.6.2/test/test-wkt_rewind.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:06.633090 pygbif-0.6.3/
+-rw-rw-rw-   0        0        0     5017 2023-05-25 12:16:37.000000 pygbif-0.6.3/CONDUCT.md
+-rw-rw-rw-   0        0        0     6256 2023-05-25 12:16:37.000000 pygbif-0.6.3/Changelog.rst
+-rw-rw-rw-   0        0        0     1061 2023-05-25 12:16:37.000000 pygbif-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-25 12:16:37.000000 pygbif-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    11683 2023-05-25 12:24:06.634093 pygbif-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2023-05-25 12:16:37.000000 pygbif-0.6.3/README.rst
+-rw-rw-rw-   0        0        0     1972 2023-05-25 12:16:37.000000 pygbif-0.6.3/RELEASING.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:05.661805 pygbif-0.6.3/pygbif/
+-rw-rw-rw-   0        0        0     1672 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/__init__.py
+-rw-rw-rw-   0        0        0     3574 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/caching.py
+-rw-rw-rw-   0        0        0     6922 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/gbifissues.py
+-rw-rw-rw-   0        0        0     4354 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/gbifutils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:05.752797 pygbif-0.6.3/pygbif/maps/
+-rw-rw-rw-   0        0        0       30 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/maps/__init__.py
+-rw-rw-rw-   0        0        0     9372 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/maps/map.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:05.874794 pygbif-0.6.3/pygbif/occurrences/
+-rw-rw-rw-   0        0        0     1518 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/occurrences/__init__.py
+-rw-rw-rw-   0        0        0     4766 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/occurrences/count.py
+-rw-rw-rw-   0        0        0    26129 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/occurrences/download.py
+-rw-rw-rw-   0        0        0     1562 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/occurrences/get.py
+-rw-rw-rw-   0        0        0    20844 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/occurrences/search.py
+-rw-rw-rw-   0        0        0      101 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/package_metadata.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:06.045788 pygbif-0.6.3/pygbif/registry/
+-rw-rw-rw-   0        0        0      637 2023-05-25 12:16:39.000000 pygbif-0.6.3/pygbif/registry/__init__.py
+-rw-rw-rw-   0        0        0    13450 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/registry/datasets.py
+-rw-rw-rw-   0        0        0     3457 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/registry/installations.py
+-rw-rw-rw-   0        0        0     2486 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/registry/networks.py
+-rw-rw-rw-   0        0        0     3950 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/registry/nodes.py
+-rw-rw-rw-   0        0        0     3417 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/registry/organizations.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:06.186783 pygbif-0.6.3/pygbif/species/
+-rw-rw-rw-   0        0        0      862 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/species/__init__.py
+-rw-rw-rw-   0        0        0     3717 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/species/name_backbone.py
+-rw-rw-rw-   0        0        0     7978 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/species/name_lookup.py
+-rw-rw-rw-   0        0        0      694 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/species/name_parser.py
+-rw-rw-rw-   0        0        0     2894 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/species/name_suggest.py
+-rw-rw-rw-   0        0        0     5390 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/species/name_usage.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:06.234787 pygbif-0.6.3/pygbif/utils/
+-rw-rw-rw-   0        0        0       35 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/utils/__init__.py
+-rw-rw-rw-   0        0        0     1305 2023-05-25 12:16:40.000000 pygbif-0.6.3/pygbif/utils/wkt_rewind.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:05.706800 pygbif-0.6.3/pygbif.egg-info/
+-rw-rw-rw-   0        0        0    11683 2023-05-25 12:24:05.000000 pygbif-0.6.3/pygbif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2023-05-25 12:24:05.000000 pygbif-0.6.3/pygbif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:24:05.000000 pygbif-0.6.3/pygbif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-25 12:24:05.000000 pygbif-0.6.3/pygbif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 12:24:05.000000 pygbif-0.6.3/pygbif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2023-05-25 12:16:37.000000 pygbif-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       87 2023-05-25 12:24:06.637093 pygbif-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1653 2023-05-25 12:16:37.000000 pygbif-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:24:06.629094 pygbif-0.6.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/__init__.py
+-rw-rw-rw-   0        0        0     2362 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-maps-map.py
+-rw-rw-rw-   0        0        0     2699 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-occurrences-count.py
+-rw-rw-rw-   0        0        0      491 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-occurrences-download_cancel.py
+-rw-rw-rw-   0        0        0      333 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-occurrences-download_get.py
+-rw-rw-rw-   0        0        0     7183 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-occurrences-download_request.py
+-rw-rw-rw-   0        0        0      918 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-occurrences-get.py
+-rw-rw-rw-   0        0        0     1763 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-occurrences-search.py
+-rw-rw-rw-   0        0        0      765 2023-05-25 12:16:40.000000 pygbif-0.6.3/test/test-registry-dataset_metrics.py
+-rw-rw-rw-   0        0        0      952 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-registry-datasets.py
+-rw-rw-rw-   0        0        0     1083 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-registry-installations.py
+-rw-rw-rw-   0        0        0      964 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-registry-networks.py
+-rw-rw-rw-   0        0        0      980 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-registry-nodes.py
+-rw-rw-rw-   0        0        0     1169 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-registry-organizations.py
+-rw-rw-rw-   0        0        0      737 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-species-name_backbone.py
+-rw-rw-rw-   0        0        0     1429 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-species-name_lookup.py
+-rw-rw-rw-   0        0        0      668 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-species-name_suggest.py
+-rw-rw-rw-   0        0        0     1027 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-species-name_usage.py
+-rw-rw-rw-   0        0        0      753 2023-05-25 12:16:41.000000 pygbif-0.6.3/test/test-wkt_rewind.py
```

### Comparing `pygbif-0.6.2/CONDUCT.md` & `pygbif-0.6.3/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/Changelog.rst` & `pygbif-0.6.3/Changelog.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+0.6.3 (2023-05-25)
+------------------
+- added support for predicates: ``isNull``, ``isNotNull``, ``in`` and ``not`` :issue:`92`, :issue:`102` and :issue:`103` 
+- added support for nested queries/dictionaries :issue:`104`
+- deprecated the ``add_predicate`` function and added ``add_pred_dict`` to accomodate for newly supported predicates to ensure that the arguments that are sent are added in the payload function :issue:`108`
+- added support for multiple download formats :issue:`105`
+- updated operators and look-up tables :issue:`107`
+- included documentation on newly supported predicates and dictionaries :issue:`106`
+
 0.6.2 (2023-01-24)
 ------------------
 - update to fix requesting GBIF downloads
 - minor documentation updates :issue:`95` and :issue:`99`
 
 0.6.1 (2022-06-23)
 ------------------
```

### Comparing `pygbif-0.6.2/LICENSE` & `pygbif-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/README.rst` & `pygbif-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/RELEASING.md` & `pygbif-0.6.3/RELEASING.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
      password = <TestPyPI token>
      ```
 
 2. Prepare the release
 
 - Update `Changelog.rst` with a new section describing the changes in this release
 - Change the version number in `setup.py`.  It is in the version line and the download_url line.
+- Change the version number in `pygbif/package_metadata.py`
   - For a trial run, just use a version like "0.6.1.dev1".
   - Otherwise, commit and push the changes to both files.
 
 3. Build and verify the package
 
 - `rm -rf dist && python3 -m build`
 - `python3 -m twine check dist/*`
```

### Comparing `pygbif-0.6.2/pygbif/__init__.py` & `pygbif-0.6.3/pygbif/__init__.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/caching.py` & `pygbif-0.6.3/pygbif/caching.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/gbifissues.py` & `pygbif-0.6.3/pygbif/gbifissues.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/gbifutils.py` & `pygbif-0.6.3/pygbif/gbifutils.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/maps/map.py` & `pygbif-0.6.3/pygbif/maps/map.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/occurrences/__init__.py` & `pygbif-0.6.3/pygbif/occurrences/__init__.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/occurrences/count.py` & `pygbif-0.6.3/pygbif/occurrences/count.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/occurrences/download.py` & `pygbif-0.6.3/pygbif/occurrences/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,54 @@
+# import external libraries
 import os
 import csv
 import json
 import re
 import datetime
 import requests
+import logging
+from warnings import warn
 
+# import internal libraries
 from .. import package_metadata, occurrences
 from ..gbifutils import (
     is_not_none,
     is_none,
     stop,
     gbif_GET,
     gbif_GET_write,
     gbif_DELETE,
 )
-import logging
-
 
+# how to parse arguments/predicates 
 def _parse_args(x):
+    x = x.replace("'", '"')
+    tmp = re.split("\s", x) 
+    key = key_lkup.get(tmp[0])
+    # check special predicates
+    if re.search(r"Null|NULL|null", x):
+        pred_type = "isNull"
+        if re.search(r"not|\!", x):
+            pred_type = "isNotNull"
+        return {"type": pred_type,"parameter": key}
+    if re.search(r"\s+not|\!", x):
+        return {"type": "not","predicate": _parse_args(re.sub(r"not\s*|\!\s*", "", x))}
     if re.match("geometry", x):
         geometry = re.search("(POLY|MULTIPOLY).+", x, re.IGNORECASE).group()
         return {"type": "within", "geometry": geometry}
-    tmp = re.split("\s", x)
+    if re.search(r"\s+in", x):
+        value_list = re.search(r"\[.*\]", x)
+        if not value_list: 
+            raise Exception(
+                "error: in predicate has to be associated with a list in square brackets (for example [1, 2, 3])"
+            )
+        else:
+            return {"type": "in", "key": key, "values": json.loads(value_list.group(0))}
     pred_type = operator_lkup.get(tmp[1])
-    key = key_lkup.get(tmp[0])
-    return {"type": pred_type, "key": key, "value": tmp[2]}
-
+    return {"type": pred_type, "key": key, "value": tmp[2]} # does not work for in, within, geodistance, not, like, isnull and isnotnull predicate values
 
 def _check_environ(variable, value):
     """check if a variable is present in the environmental variables"""
     if is_not_none(value):
         return value
     else:
         value = os.environ.get(variable)
@@ -42,22 +61,23 @@
                            variables""",
                     ]
                 )
             )
         else:
             return value
 
-
-def download(queries, user=None, pwd=None, email=None, pred_type="and"):
+# download function 
+def download(queries, format = "SIMPLE_CSV", user=None, pwd=None, email=None, pred_type="and"):
     """
     Spin up a download request for GBIF occurrence data.
 
     :param queries: One or more of query arguments to kick of a download job.
         See Details.
-    :type queries: str or list
+    :type queries: str, list or dictionary  
+    :param format: (character) One of the GBIF accepted download formats https://www.gbif.org/faq?question=download-formats
     :param pred_type: (character) One of ``equals`` (``=``), ``and`` (``&``),
         `or`` (``|``), ``lessThan`` (``<``), ``lessThanOrEquals`` (``<=``),
         ``greaterThan`` (``>``), ``greaterThanOrEquals`` (``>=``),
         ``in``, ``within``, ``not`` (``!``), ``like``
     :param user: (character) User name within GBIF's website.
         Required. Set in your env vars with the option ``GBIF_USER``
     :param pwd: (character) User password within GBIF's website. Required.
@@ -66,28 +86,28 @@
         email. Required. Set in your env vars with the option ``GBIF_EMAIL``
 
     Argument passed have to be passed as character (e.g., ``country = US``),
     with a space between key (``country``), operator (``=``), and value (``US``).
     See the ``type`` parameter for possible options for the operator.
     This character string is parsed internally.
 
-    Acceptable arguments to ``...`` (args) are:
+    Acceptable arguments to ``...`` (args) are: 
 
      - taxonKey = ``TAXON_KEY``
      - scientificName = ``SCIENTIFIC_NAME``
      - country = ``COUNTRY``
      - publishingCountry = ``PUBLISHING_COUNTRY``
      - hasCoordinate = ``HAS_COORDINATE``
      - hasGeospatialIssue = ``HAS_GEOSPATIAL_ISSUE``
      - typeStatus = ``TYPE_STATUS``
      - recordNumber = ``RECORD_NUMBER``
      - lastInterpreted = ``LAST_INTERPRETED``
      - continent = ``CONTINENT``
      - geometry = ``GEOMETRY``
-     - basisOfRecord = ``BASIS_OF_RECORD``
+     - basisOfRecord = ``BASIS_OF_RECORD`` 
      - datasetKey = ``DATASET_KEY``
      - eventDate = ``EVENT_DATE``
      - catalogNumber = ``CATALOG_NUMBER``
      - year = ``YEAR``
      - month = ``MONTH``
      - decimalLatitude = ``DECIMAL_LATITUDE``
      - decimalLongitude = ``DECIMAL_LONGITUDE``
@@ -95,18 +115,67 @@
      - depth = ``DEPTH``
      - institutionCode = ``INSTITUTION_CODE``
      - collectionCode = ``COLLECTION_CODE``
      - issue = ``ISSUE``
      - mediatype = ``MEDIA_TYPE``
      - recordedBy = ``RECORDED_BY``
      - repatriated = ``REPATRIATED``
+     - classKey = ``CLASS_KEY``
+     - coordinateUncertaintyInMeters = ``COORDINATE_UNCERTAINTY_IN_METERS``
+     - crawlId = ``CRAWL_ID``
+     - datasetId = ``DATASET_ID``
+     - datasetName = ``DATASET_NAME``
+     - distanceFromCentroidInMeters = ``DISTANCE_FROM_CENTROID_IN_METERS``
+     - establishmentMeans = ``ESTABLISHMENT_MEANS``
+     - eventId = ``EVENT_ID``
+     - familyKey = ``FAMILY_KEY``
+     - format = ``FORMAT``
+     - fromDate = ``FROM_DATE``
+     - genusKey = ``GENUS_KEY``
+     - geoDistance = ``GEO_DISTANCE``
+     - identifiedBy = ``IDENTIFIED_BY``
+     - identifiedByID = ``IDENTIFIED_BY_ID``
+     - kingdomKey = ``KINGDON_KEY``
+     - license = ``LICENSE``
+     - locality = ``LOCALITY``
+     - modified = ``MODIFIED``
+     - networkKey = ``NETWORK_KEY``
+     - occurrenceId = ``OCCURRENCE_ID``
+     - occurrenceStatus = ``OCCURRENCE_STATUS``
+     - orderKey = ``ORDER_KEY``
+     - organismId = ``ORGANISM_ID``
+     - organismQuantity = ``ORGANISM_QUANTITY``
+     - organismQuantityType = ``ORGANISM_QUANTITY_TYPE``
+     - otherCatalogNumbers = ``OTHER_CATALOG_NUMBERS``
+     - phylumKey = ``PHYLUM_KEY``
+     - preparations = ``PREPARATIONS``
+     - programme = ``PROGRAMME``
+     - projectId = ``PROJECT_ID``
+     - protocol = ``PROTOCOL``
+     - publishingCountry = ``PUBLISHING_COUNTRY``
+     - publishingOrg = ``PUBLISHING_ORG``
+     - publishingOrgKey = ``PUBLISHING_ORG_KEY``
+     - recordedByID = ``RECORDED_BY_ID``
+     - recordNumber = ``RECORD_NUMBER``
+     - relativeOrganismQuantity = ``RELATIVE_ORGANISM_QUANTITY``
+     - sampleSizeUnit = ``SAMPLE_SIZE_UNIT``
+     - sampleSizeValue = ``SAMPLE_SIZE_VALUE``
+     - samplingProtocol = ``SAMPLING_PROTOCOL``
+     - speciesKey = ``SPECIES_KEY``
+     - stateProvince = ``STATE_PROVINCE``
+     - subgenusKey = ``SUBGENUS_KEY``
+     - taxonId = ``TAXON_ID``
+     - toDate = ``TO_DATE``
+     - userCountry = ``USER_COUNTRY``
+     - verbatimScientificName = ``VERBATIM_SCIENTIFIC_NAME``
+     - waterBody = ``WATER_BODY``
+
 
-    See the API docs http://www.gbif.org/developer/occurrence#download
-    for more info, and the predicates docs
-    http://www.gbif.org/developer/occurrence#predicates
+    See the API docs http://www.gbif.org/developer/occurrence#download and the predicates docs
+    http://www.gbif.org/developer/occurrence#predicates for more info.
 
     GBIF has a limit of 100,000 predicates and 10,000 points (in within
     predicates) for download queries – so if your download request is
     particularly complex, you may need to split it into multiple
     requests by one factor or another.
 
     :return: A dictionary, of results
@@ -125,68 +194,96 @@
         occ.download('catalogNumber = Bird.27847588')
 
         res = occ.download(['taxonKey = 7264332', 'hasCoordinate = TRUE'])
 
         # pass output to download_meta for more information
         occ.download_meta(occ.download('decimalLatitude > 75'))
 
-        # Multiple queries
+        # multiple queries
         gg = occ.download(['decimalLatitude >= 65',
-                          'decimalLatitude <= -65'], type='or')
+                          'decimalLatitude <= -65'], pred_type ='or')
         gg = occ.download(['depth = 80', 'taxonKey = 2343454'],
-                          type='or')
+                          pred_type ='or')
 
-        # Repratriated data for Costa Rica
+        # repratriated data for Costa Rica
         occ.download(['country = CR', 'repatriated = true'])
 
         # turn off logging
         import logging
         logger = logging.getLogger()
         logger.disabled = True
         z = occ.download('elevation >= 95000')
         logger.disabled = False
         w = occ.download('elevation >= 10000')
+        
+        # nested and complex queries with multiple predicates
+        ## For more complex queries, it may be advantagous to format the query in JSON format. It must follow the predicate format described in the API documentation (https://www.gbif.org/developer/occurrence#download):
+        query = { "type": "and",
+          "predicates": [
+            {  "type": "in",
+                "key": "TAXON_KEY",
+                "values": ["2387246","2399391","2364604"]},
+            {   "type": "isNotNull",
+                "parameter": "YEAR"},
+            {  "type": "not",
+               "predicate": {  "type": "in",
+                                        "key": "ISSUE",
+                                        "values": ["RECORDED_DATE_INVALID",
+                                                         "TAXON_MATCH_FUZZY",
+                                                         "TAXON_MATCH_HIGHERRANK"] }} ]}
+        occ.download(query)
+    
+        # The same query can also be applied in the occ.download function (including download format specified):
+        occ.download(['taxonKey in ["2387246", "2399391","2364604"]', 'year !Null', "issue !in ['RECORDED_DATE_INVALID', 'TAXON_MATCH_FUZZY', 'TAXON_MATCH_HIGHERRANK']"], "DWCA")
+    
     """
 
     user = _check_environ("GBIF_USER", user)
     pwd = _check_environ("GBIF_PWD", pwd)
     email = _check_environ("GBIF_EMAIL", email)
 
-    if isinstance(queries, str):
-        queries = [queries]
+# if it is a dictionary then use directly as a query, otherwise if it is a string turn it into a list
+    req = GbifDownload(user, email)
+    req.format = format
 
-    keyval = [_parse_args(z) for z in queries]
+    if isinstance(queries, dict):
+        req.predicate = queries
 
-    # USE GBIFDownload class to set up the predicates
-    req = GbifDownload(user, email)
-    req.main_pred_type = pred_type
-    for predicate in keyval:
-        if "geometry" in predicate.keys():
-            req.add_geometry(predicate["geometry"])
-        else:
-            req.add_predicate(predicate["key"], predicate["value"], predicate["type"])
+    else: # retro-compatible
+
+        if isinstance(queries, str):
+            queries = [queries]
+
+        keyval = [_parse_args(z) for z in queries]
+
+        # USE GBIFDownload class to set up the predicates
+        req.main_pred_type = pred_type
+        for predicate in keyval:
+            req.add_predicate_dict(predicate)
 
     out = req.post_download(user, pwd)
     return out, req.payload
 
 
 class GbifDownload(object):
     def __init__(self, creator, email, polygon=None):
         """class to setup a JSON doc with the query and POST a request
 
         All predicates (default key-value or iterative based on a list of
         values) are combined with an AND statement. Iterative predicates are
         creating a subset equal statements combined with OR
 
-        :param creator: User name.
+        :param creator: user name
         :param email: user email
         :param polygon: Polygon of points to extract data from
         """
-        self.predicates = []
+        self._format = "SIMPLE_CSV"
+        self.predicates = [] 
         self._main_pred_type = "and"
+        self._predicate = {"type": self._main_pred_type, "predicates": self.predicates} 
 
         self.url = "http://api.gbif.org/v1/occurrence/download/request"
         self.header = {
             "accept": "application/json",
             "content-type": "application/json",
             "user-agent": "".join(
                 [
@@ -198,15 +295,16 @@
             ),
         }
 
         self.payload = {
             "creator": creator,
             "notification_address": [email],
             "sendNotification": True,
-            "predicate": {"type": self._main_pred_type, "predicates": self.predicates},
+            "predicate": self._predicate,
+            "format": self._format
         }
         self.request_id = None
 
         # prepare the geometry polygon constructions
         if polygon:
             self.add_geometry(polygon)
 
@@ -227,29 +325,79 @@
             value = operator_lkup.get(value)
         if value:
             self._main_pred_type = value
             self.payload["predicate"]["type"] = self._main_pred_type
         else:
             raise Exception("main predicate combiner not a valid operator")
 
+    @property
+    def predicate(self):
+        """get main predicate combination type"""
+        return self._predicate
+
+    @predicate.setter
+    def predicate(self, value):
+        """set predicate
+
+        :param value: python dictionary formatted as API compatible JSON query (https://www.gbif.org/developer/occurrence#download)
+        """
+        if isinstance(value, dict):
+            self._predicate = value
+            self.payload["predicate"] = self._predicate
+        else:
+            raise Exception("predicate must be a dictionary")
+
+    @property
+    def format(self):
+        """get ¨download format"""
+        return self._format
+
+    @format.setter
+    def format(self, value):
+        """set format
+
+        :param value: the format must be one of the accepted download formats of GBIF https://www.gbif.org/faq?question=download-formats 
+        """
+        if value in formats:
+            self._format = value
+            self.payload["format"] = self._format
+        else:
+            raise Exception("format must be one of the accepted download formats of GBIF " + ", ".join(formats))   
+
     def add_predicate(self, key, value, predicate_type="equals"):
         """
+        this function is deprecated, please use add_predicate_dict instead
         add key, value, type combination of a predicate
 
         :param key: query KEY parameter
         :param value: the value used in the predicate
         :param predicate_type: the type of predicate (e.g. ``equals``)
         """
+        warn('This method is deprecated. Please use add_predicate_dict() instead', DeprecationWarning, stacklevel=2)
+
         if predicate_type not in operators:
             predicate_type = operator_lkup.get(predicate_type)
         if predicate_type:
             self.predicates.append({"type": predicate_type, "key": key, "value": value})
         else:
             raise Exception("predicate type not a valid operator")
 
+    def add_predicate_dict(self, predicate_dictionary):
+        """
+        allows for nested queries and will take a predicate and add it to a list of predicates
+
+        :param predicate_dictionary: has to be a predicate formatted as a dictionary, for example {"type": "in", "key": "TAXON_KEY", "values": ["2387246","2399391","2364604"]} or {"type": "isNotNull",
+        "parameter": "YEAR"} see the API documentation for more information: https://www.gbif.org/developer/occurrence#predicates 
+        """
+
+        if isinstance(predicate_dictionary, dict):
+            self.predicates.append(predicate_dictionary)
+        else:
+            raise Exception("argument must be a dictionary")
+
     @staticmethod
     def _extract_values(values_list):
         """extract values from either file or list
 
         :param values_list: list or file name (str) with list of values
         """
         values = []
@@ -469,28 +617,32 @@
     "lessThanOrEquals",
     "greaterThan",
     "greaterThanOrEquals",
     "in",
     "within",
     "not",
     "like",
+    "isNull",
+    "isNotNull"
 ]
 
 operator_lkup = {
     "=": "equals",
     "&": "and",
     "|": "or",
     "<": "lessThan",
     "<=": "lessThanOrEquals",
     ">": "greaterThan",
     ">=": "greaterThanOrEquals",
     "!": "not",
     "in": "in",
     "within": "within",
     "like": "like",
+    "is NULL" : "isNull",
+    "is not NULL" : "isNotNull"
 }
 
 key_lkup = {
     "taxonKey": "TAXON_KEY",
     "scientificName": "SCIENTIFIC_NAME",
     "country": "COUNTRY",
     "publishingCountry": "PUBLISHING_COUNTRY",
@@ -513,8 +665,59 @@
     "depth": "DEPTH",
     "institutionCode": "INSTITUTION_CODE",
     "collectionCode": "COLLECTION_CODE",
     "issue": "ISSUE",
     "mediatype": "MEDIA_TYPE",
     "recordedBy": "RECORDED_BY",
     "repatriated": "REPATRIATED",
+    "classKey": "CLASS_KEY",
+    "coordinateUncertaintyInMeters": "COORDINATE_UNCERTAINTY_IN_METERS",
+    "crawlId": "CRAWL_ID",
+    "datasetId": "DATASET_ID",
+    "datasetName": "DATASET_NAME",
+    "distanceFromCentroidInMeters": "DISTANCE_FROM_CENTROID_IN_METERS",
+    "establishmentMeans": "ESTABLISHMENT_MEANS",
+    "eventId": "EVENT_ID",
+    "familyKey": "FAMILY_KEY",
+    "format": "FORMAT",
+    "fromDate": "FROM_DATE",
+    "genusKey": "GENUS_KEY",
+    "geoDistance": "GEO_DISTANCE",
+    "identifiedBy": "IDENTIFIED_BY",
+    "identifiedByID": "IDENTIFIED_BY_ID",
+    "kingdomKey": "KINGDON_KEY",
+    "license": "LICENSE",
+    "locality": "LOCALITY",
+    "modified": "MODIFIED",
+    "networkKey": "NETWORK_KEY",
+    "occurrenceId": "OCCURRENCE_ID",
+    "occurrenceStatus": "OCCURRENCE_STATUS",
+    "orderKey": "ORDER_KEY",
+    "organismId": "ORGANISM_ID",
+    "organismQuantity": "ORGANISM_QUANTITY",
+    "organismQuantityType": "ORGANISM_QUANTITY_TYPE",
+    "otherCatalogNumbers": "OTHER_CATALOG_NUMBERS",
+    "phylumKey": "PHYLUM_KEY",
+    "preparations": "PREPARATIONS",
+    "programme": "PROGRAMME",
+    "projectId": "PROJECT_ID",
+    "protocol": "PROTOCOL",
+    "publishingCountry": "PUBLISHING_COUNTRY",
+    "publishingOrg": "PUBLISHING_ORG",
+    "publishingOrgKey": "PUBLISHING_ORG_KEY",
+    "recordedByID": "RECORDED_BY_ID",
+    "recordNumber": "RECORD_NUMBER",
+    "relativeOrganismQuantity": "RELATIVE_ORGANISM_QUANTITY",
+    "sampleSizeUnit": "SAMPLE_SIZE_UNIT",
+    "sampleSizeValue": "SAMPLE_SIZE_VALUE",
+    "samplingProtocol": "SAMPLING_PROTOCOL",
+    "speciesKey": "SPECIES_KEY",
+    "stateProvince": "STATE_PROVINCE",
+    "subgenusKey": "SUBGENUS_KEY",
+    "taxonId": "TAXON_ID",
+    "toDate": "TO_DATE",
+    "userCountry": "USER_COUNTRY",
+    "verbatimScientificName": "VERBATIM_SCIENTIFIC_NAME",
+    "waterBody": "WATER_BODY"
 }
+
+formats = ["SIMPLE_CSV", "DWCA", "SPECIES_LIST"]
```

### Comparing `pygbif-0.6.2/pygbif/occurrences/get.py` & `pygbif-0.6.3/pygbif/occurrences/get.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/occurrences/search.py` & `pygbif-0.6.3/pygbif/occurrences/search.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/registry/__init__.py` & `pygbif-0.6.3/pygbif/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/registry/datasets.py` & `pygbif-0.6.3/pygbif/registry/datasets.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/registry/installations.py` & `pygbif-0.6.3/pygbif/registry/installations.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/registry/networks.py` & `pygbif-0.6.3/pygbif/registry/networks.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/registry/nodes.py` & `pygbif-0.6.3/pygbif/registry/nodes.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/registry/organizations.py` & `pygbif-0.6.3/pygbif/registry/organizations.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/species/__init__.py` & `pygbif-0.6.3/pygbif/species/__init__.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/species/name_backbone.py` & `pygbif-0.6.3/pygbif/species/name_backbone.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/species/name_lookup.py` & `pygbif-0.6.3/pygbif/species/name_lookup.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/species/name_parser.py` & `pygbif-0.6.3/pygbif/species/name_parser.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/species/name_suggest.py` & `pygbif-0.6.3/pygbif/species/name_suggest.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/species/name_usage.py` & `pygbif-0.6.3/pygbif/species/name_usage.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif/utils/wkt_rewind.py` & `pygbif-0.6.3/pygbif/utils/wkt_rewind.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/pygbif.egg-info/SOURCES.txt` & `pygbif-0.6.3/pygbif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/setup.py` & `pygbif-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 with codecs.open("Changelog.rst", "r", "utf-8") as f:
     changes = f.read().replace("\r", '')
 changes = changes.replace(":issue:", "")
 long_description = readme + "\n\n" + changes
 
 setup(
     name="pygbif",
-    version="0.6.2",
+    version="0.6.3",
     description="Python client for GBIF",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Scott Chamberlain",
     author_email="myrmecocystus@gmail.com",
     url="http://github.com/gbif/pygbif",
-    download_url="https://github.com/gbif/pygbif/archive/refs/tags/v0.6.2.tar.gz",
+    download_url="https://github.com/gbif/pygbif/archive/refs/tags/v0.6.3.tar.gz",
     license="MIT",
     packages=find_packages(exclude=["test-*"]),
     install_requires=[
         "requests>2.7",
         "requests-cache",
         "geojson_rewind",
         "geomet",
```

### Comparing `pygbif-0.6.2/test/test-maps-map.py` & `pygbif-0.6.3/test/test-maps-map.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-occurrences-count.py` & `pygbif-0.6.3/test/test-occurrences-count.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-occurrences-download_request.py` & `pygbif-0.6.3/test/test-occurrences-download_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self.assertDictEqual(
             req.payload,
             {
                 "creator": "name",
                 "notification_address": ["email"],
                 "predicate": {"predicates": [], "type": "and"},
                 "sendNotification": True,
+                "format": "SIMPLE_CSV",
             },
         )
         self.assertIsNone(req.request_id)
 
     def test_alternative_main_type(self):
         """test the addition of another predicate combiner"""
         req = GbifDownload("name", "email")
@@ -43,15 +44,16 @@
         self.assertDictEqual(
             req.payload,
             {
                 "creator": "name",
                 "notification_address": ["email"],
                 "predicate": {"predicates": [], "type": "or"},
                 "sendNotification": True,
-            },
+                "format": "SIMPLE_CSV"
+            }
         )
 
     def test_add_predicate(self):
         """test the predicate addition"""
         req = GbifDownload("name", "email")
         req.add_predicate("COUNTRY", "BE", "equals")
         self.assertIsInstance(req.payload["predicate"]["predicates"], list)
```

### Comparing `pygbif-0.6.2/test/test-occurrences-get.py` & `pygbif-0.6.3/test/test-occurrences-get.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-occurrences-search.py` & `pygbif-0.6.3/test/test-occurrences-search.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-registry-dataset_metrics.py` & `pygbif-0.6.3/test/test-registry-dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-registry-datasets.py` & `pygbif-0.6.3/test/test-registry-datasets.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-registry-installations.py` & `pygbif-0.6.3/test/test-registry-installations.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-registry-networks.py` & `pygbif-0.6.3/test/test-registry-networks.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-registry-nodes.py` & `pygbif-0.6.3/test/test-registry-nodes.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-registry-organizations.py` & `pygbif-0.6.3/test/test-registry-organizations.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-species-name_backbone.py` & `pygbif-0.6.3/test/test-species-name_backbone.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-species-name_lookup.py` & `pygbif-0.6.3/test/test-species-name_lookup.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-species-name_suggest.py` & `pygbif-0.6.3/test/test-species-name_suggest.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-species-name_usage.py` & `pygbif-0.6.3/test/test-species-name_usage.py`

 * *Files identical despite different names*

### Comparing `pygbif-0.6.2/test/test-wkt_rewind.py` & `pygbif-0.6.3/test/test-wkt_rewind.py`

 * *Files identical despite different names*

