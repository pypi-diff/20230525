# Comparing `tmp/otc_sphinx_directives-0.2.4.tar.gz` & `tmp/otc_sphinx_directives-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otc_sphinx_directives-0.2.4.tar", last modified: Wed May 24 10:04:53 2023, max compression
+gzip compressed data, was "otc_sphinx_directives-0.2.5.tar", last modified: Thu May 25 12:42:50 2023, max compression
```

## Comparing `otc_sphinx_directives-0.2.4.tar` & `otc_sphinx_directives-0.2.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.533503 otc_sphinx_directives-0.2.4/
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/.stestr.conf
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1816 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-24 10:04:53.533503 otc_sphinx_directives-0.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.529503 otc_sphinx_directives-0.2.4/doc/
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.530503 otc_sphinx_directives-0.2.4/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.530503 otc_sphinx_directives-0.2.4/doc/source/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/_static/.placeholder
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.530503 otc_sphinx_directives-0.2.4/doc/source/examples/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/examples/directives_docsportal.rst
--rw-r--r--   0 root         (0) root         (0)      966 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/examples/directives_ecs.rst
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/examples/directives_obs.rst
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/examples/directives_obs_clean.rst
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/examples/index.rst
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.531503 otc_sphinx_directives-0.2.4/otc_sphinx_directives/
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/container_item.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/document_navigator.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/navigator.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/otc_sphinx_directives_setup.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/service_card.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/service_group.py
--rw-r--r--   0 root         (0) root         (0)     2935 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/service_navigator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.533503 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.528503 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.533503 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/directive_wrapper/
--rw-r--r--   0 root         (0) root         (0)      791 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.533503 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/service_card/
--rw-r--r--   0 root         (0) root         (0)      791 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/service_card/conf.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/service_card/index.rst
--rw-r--r--   0 root         (0) root         (0)     2330 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/test_directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/test_service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:04:53.532503 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1523 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 10:04:53.000000 otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-05-24 10:04:53.534503 otc_sphinx_directives-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/setup.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/tox.ini
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-24 10:03:32.000000 otc_sphinx_directives-0.2.4/zuul.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.649372 otc_sphinx_directives-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/.stestr.conf
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-25 12:42:50.698372 otc_sphinx_directives-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.646372 otc_sphinx_directives-0.2.5/doc/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.646372 otc_sphinx_directives-0.2.5/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.646372 otc_sphinx_directives-0.2.5/doc/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/_static/.placeholder
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.647372 otc_sphinx_directives-0.2.5/doc/source/examples/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/examples/directives_docsportal.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/examples/directives_ecs.rst
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/examples/directives_obs.rst
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/examples/directives_obs_clean.rst
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/examples/index.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.648372 otc_sphinx_directives-0.2.5/otc_sphinx_directives/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/container_item.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/document_navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/otc_sphinx_directives_setup.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/service_card.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/service_group.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/service_navigator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.649372 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.644372 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.649372 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/directive_wrapper/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.649372 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/service_card/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/service_card/conf.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/service_card/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/test_directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/test_service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:42:50.648372 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 12:42:50.000000 otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-05-25 12:42:50.698372 otc_sphinx_directives-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/setup.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-25 12:41:28.000000 otc_sphinx_directives-0.2.5/zuul.yaml
```

### Comparing `otc_sphinx_directives-0.2.4/ChangeLog` & `otc_sphinx_directives-0.2.5/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.2.5
+-----
+
+* fix links (#19)
+
 0.2.4
 -----
 
 * Switched to relative links (#18)
 
 0.2.3
 -----
```

### Comparing `otc_sphinx_directives-0.2.4/LICENSE` & `otc_sphinx_directives-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/PKG-INFO` & `otc_sphinx_directives-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc_sphinx_directives
-Version: 0.2.4
+Version: 0.2.5
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.4/doc/source/examples/directives_ecs.rst` & `otc_sphinx_directives-0.2.5/doc/source/examples/directives_ecs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/doc/source/examples/directives_obs.rst` & `otc_sphinx_directives-0.2.5/doc/source/examples/directives_obs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/container_item.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/container_item.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/directive_wrapper.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/document_navigator.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/document_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/navigator.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/otc_sphinx_directives_setup.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/otc_sphinx_directives_setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/service_card.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/service_card.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/service_group.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/service_group.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/service_navigator.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/service_navigator.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             f'<ul class="list-group list-group-flush">'
         )
 
         for service in METADATA.services_by_category(category=category):
             title = service['service_title']
             link = service['service_uri']
             if link:
-                if (link[:-1] != '/'):
+                if (link[-1] != '/'):
                     link = link + '/index.html'
                 else:
                     link = link + 'index.html'
             img = service['service_type']
             environment = service['environment']
             if environment == "hidden":
                 continue
```

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/base.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/base.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/templates/service_card/conf.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/templates/service_card/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/test_directive_wrapper.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/test_directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives/tests/test_service_card.py` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives/tests/test_service_card.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/PKG-INFO` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc-sphinx-directives
-Version: 0.2.4
+Version: 0.2.5
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.4/otc_sphinx_directives.egg-info/SOURCES.txt` & `otc_sphinx_directives-0.2.5/otc_sphinx_directives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/setup.cfg` & `otc_sphinx_directives-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/setup.py` & `otc_sphinx_directives-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.4/tox.ini` & `otc_sphinx_directives-0.2.5/tox.ini`

 * *Files identical despite different names*

