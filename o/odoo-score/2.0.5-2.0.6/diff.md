# Comparing `tmp/odoo_score-2.0.5.tar.gz` & `tmp/odoo_score-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_score-2.0.5.tar", last modified: Sun Apr 23 13:59:27 2023, max compression
+gzip compressed data, was "dist/odoo_score-2.0.6.tar", last modified: Thu May 25 08:59:59 2023, max compression
```

## Comparing `odoo_score-2.0.5.tar` & `odoo_score-2.0.6.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1117 2023-04-23 13:59:27.229416 odoo_score-2.0.5/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8940 2023-04-23 13:59:26.000000 odoo_score-2.0.5/README.rst
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/odoo_score/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      758 2023-04-20 06:09:47.000000 odoo_score-2.0.5/odoo_score/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/__main__.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      299 2022-12-13 18:54:38.000000 odoo_score-2.0.5/odoo_score/api.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      413 2022-12-13 18:54:38.000000 odoo_score-2.0.5/odoo_score/fields.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6144 2023-04-15 07:42:48.000000 odoo_score-2.0.5/odoo_score/migrate.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      455 2023-04-20 06:11:16.000000 odoo_score-2.0.5/odoo_score/models_2.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      431 2023-04-20 06:11:16.000000 odoo_score-2.0.5/odoo_score/models_3.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    11822 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/odoo_score.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_10.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_11.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_12.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_13.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_14.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_6.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_7.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_9.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)   163851 2023-04-15 07:43:03.000000 odoo_score-2.0.5/odoo_score/odoo_shell.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/odoo_score/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      144 2023-04-23 10:07:05.000000 odoo_score-2.0.5/odoo_score/scripts/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5916 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5807 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/scripts/map_module_dependecies.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     4769 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/scripts/rename_odoo_module.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/scripts/run_odoo_debug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29084 2023-04-20 10:41:38.000000 odoo_score-2.0.5/odoo_score/scripts/run_odoo_debug.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1821 2023-04-23 13:49:43.000000 odoo_score-2.0.5/odoo_score/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3075 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/secure_db.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    15765 2023-04-15 08:02:21.000000 odoo_score-2.0.5/odoo_score/set_workers
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/odoo_score.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1117 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1004 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      130 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:00.000000 odoo_score-2.0.5/odoo_score.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 13:59:27.229416 odoo_score-2.0.5/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1821 2023-04-23 10:07:05.000000 odoo_score-2.0.5/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:59:59.000000 odoo_score-2.0.6/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:00.000000 odoo_score-2.0.6/odoo_score.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      130 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      953 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1168 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:59:59.000000 odoo_score-2.0.6/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1757 2023-05-20 06:23:34.000000 odoo_score-2.0.6/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_8.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      476 2023-04-23 14:59:55.000000 odoo_score-2.0.6/odoo_score/models_3.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_14.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3075 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/secure_db.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_11.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    15765 2023-05-20 06:23:34.000000 odoo_score-2.0.6/odoo_score/set_workers
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)   173356 2023-05-24 18:25:08.000000 odoo_score-2.0.6/odoo_score/odoo_shell.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_9.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:59:59.000000 odoo_score-2.0.6/odoo_score/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1757 2023-05-21 06:28:06.000000 odoo_score-2.0.6/odoo_score/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6324 2023-05-20 06:23:34.000000 odoo_score-2.0.6/odoo_score/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5807 2023-05-20 06:23:34.000000 odoo_score-2.0.6/odoo_score/scripts/map_module_dependecies.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     4769 2023-05-20 06:23:34.000000 odoo_score-2.0.6/odoo_score/scripts/rename_odoo_module.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      113 2023-05-01 07:22:39.000000 odoo_score-2.0.6/odoo_score/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_7.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      299 2022-12-13 18:54:38.000000 odoo_score-2.0.6/odoo_score/api.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_12.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    11822 2023-05-20 06:23:34.000000 odoo_score-2.0.6/odoo_score/odoo_score.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      501 2023-04-23 14:59:55.000000 odoo_score-2.0.6/odoo_score/models_2.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_6.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_13.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      413 2022-12-13 18:54:38.000000 odoo_score-2.0.6/odoo_score/fields.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      463 2023-05-01 07:50:35.000000 odoo_score-2.0.6/odoo_score/models_7.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      795 2023-04-23 15:09:55.000000 odoo_score-2.0.6/odoo_score/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6144 2023-04-15 07:42:48.000000 odoo_score-2.0.6/odoo_score/migrate.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.6/odoo_score/odoo_score_10.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1168 2023-05-25 08:59:59.000000 odoo_score-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7834 2023-05-21 13:33:33.000000 odoo_score-2.0.6/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `odoo_score-2.0.5/PKG-INFO` & `odoo_score-2.0.6/odoo_score.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1
-Name: odoo_score
-Version: 2.0.5
+Metadata-Version: 1.2
+Name: odoo-score
+Version: 2.0.6
 Summary: Odoo super core
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        Odoo supercore
+        
+        odoo_score is a library that extends the odoo orm functionality
+        and makes available a simple odoo shell.
+        
 Keywords: odoo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
-
-
-Odoo supercore
-
-odoo_score is a library that extends the odoo orm functionality
-and makes available a simple odoo shell.
-
-
```

### Comparing `odoo_score-2.0.5/README.rst` & `odoo_score-2.0.6/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 ================
-odoo_score 2.0.5
+odoo_score 2.0.6
 ================
 
 
 
-|Maturity| |Build Status| |Coverage Status| |license gpl|
+|Maturity| |license gpl|
 
 
 
 
 Overview
 ========
 
@@ -82,77 +82,64 @@
 |
 |
 
 Getting started
 ===============
 
 
-|
-
-Installation
-------------
-
 Installation
 ------------
 
 Zeroincombenze tools require:
 
-* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20
-* python 2.7, some tools require python 3.6+
+* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
+* python 2.7+, some tools require python 3.6+
 * bash 5.0+
 
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+::
+
     pip install odoo_score
 
 |
 
 Current version via Git
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     git clone https://github.com/zeroincombenze/tools.git
     cd ./tools
     ./install_tools.sh -p
-    source /opt/odoo/devel/activate_tools
-
+    source $HOME/devel/activate_tools
 
-Upgrade
--------
 
 Upgrade
 -------
 
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+::
+
     pip install odoo_score -U
 
 |
 
-Current stable version
-~~~~~~~~~~~~~~~~~~~~~~
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     ./install_tools.sh -U
-    source /opt/odoo/devel/activate_tools
-
-Current development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    ./install_tools.sh -Ud
-    source /opt/odoo/devel/activate_tools
+    source $HOME/devel/activate_tools
 
 
 History
 -------
 
 2.0.6 (2023-04-16)
 ~~~~~~~~~~~~~~~~~~
@@ -237,49 +224,34 @@
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-04-23
+Last Update / Ultimo aggiornamento: 2023-05-21
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
-.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
-    :target: https://travis-ci.com/zeroincombenze/tools
-    :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
-.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
-    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
-    :alt: Coverage
-.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
-    :alt: Codecov
 .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
     :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
     :alt: Technical Documentation
 .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
     :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
     :alt: Technical Documentation
 .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
     :target: https://erp2.zeroincombenze.it
     :alt: Try Me
-.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/OCA/tools/branch/2.0
-    :alt: Codecov
-.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
-   :target: https://odoo-italia.org
-   :alt: Odoo Italia Associazione
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
 .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
 .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
```

### Comparing `odoo_score-2.0.5/odoo_score/__init__.py` & `odoo_score-2.0.6/odoo_score/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 except ImportError:
     try:
         _o = "openerp."
         _release = __import__(_o + "release", fromlist=[None])
     except ImportError:
         _o = _release = ""
         _suffix = str(sys.version_info[0])
-else:
+if _release:
     _suffix = _release.major_version.split(".")[0]
-#
-try:
-    models = __import__("odoo_score.models_" + _suffix, fromlist=[None]).odoo_models
-except ImportError:
-    _suffix = str(sys.version_info[0])
-    models = __import__("odoo_score.models_" + _suffix, fromlist=[None]).odoo_models
-for name in models.__dict__:
-    if callable(getattr(models, name)):
-        globals()[name] = getattr(models, name)
+    try:
+        models = __import__("odoo_score.models_" + _suffix, fromlist=[None]).odoo_models
+    except ImportError:
+        _suffix = str(sys.version_info[0])
+        models = __import__("odoo_score.models_" + _suffix, fromlist=[None]).odoo_models
+    for name in models.__dict__:
+        if callable(getattr(models, name)):
+            globals()[name] = getattr(models, name)
```

### Comparing `odoo_score-2.0.5/odoo_score/migrate.py` & `odoo_score-2.0.6/odoo_score/migrate.py`

 * *Files identical despite different names*

### Comparing `odoo_score-2.0.5/odoo_score/odoo_score.py` & `odoo_score-2.0.6/odoo_score/odoo_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     try:
         import oerplib  # noqa: F401
         __db_protocol__ = 'xml' if not __db_protocol__ else 'json+xml'
     except ImportError:
         pass
 
 
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 
 MODULE_ID = 'odoo_score'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 class SingletonCache(object):
```

### Comparing `odoo_score-2.0.5/odoo_score/odoo_shell.py` & `odoo_score-2.0.6/odoo_score/odoo_shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
+
+import random
+
 from past.builtins import long
 
 import csv
 import getpass
 import re
 import os
 import sys
@@ -31,15 +34,15 @@
     from z0lib import z0lib
 
 import pdb  # pylint: disable=deprecated-module
 
 standard_library.install_aliases()  # noqa: E402
 
 
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 
 
 MAX_DEEP = 20
 PAY_MOVE_STS_2_DRAFT = ['posted']
 INVOICES_STS_2_DRAFT = ['open', 'paid']
 STATES_2_DRAFT = ['open', 'paid', 'posted']
 TECH_FIELDS = [
@@ -291,14 +294,55 @@
         if param.startswith('P'):
             product_id = eval(param[1:])
         elif param.startswith('A'):
             agent_id = eval(param[1:])
     return product_id, agent_id
 
 
+def show_module_group(ctx):
+    print('Show group infos and external names')
+    model_grp = 'res.groups'
+    model_ctg = 'ir.module.category'
+    model_ir_md = 'ir.model.data'
+    gid = True
+    while gid:
+        gid = input('Res.groups id: ')
+        if gid:
+            gid = eval(gid)
+        if gid:
+            group = clodoo.browseL8(ctx, model_grp, gid, context={'lang': 'en_US'})
+            cid = group.category_id.id
+            categ = clodoo.browseL8(ctx, model_ctg, cid, context={'lang': 'en_US'})
+            print('%6d) Category %s' % (cid, categ.name))
+            uniq_field = []
+            grp_ids = clodoo.searchL8(ctx, model_grp,
+                                      [('category_id', '=', cid)])
+            for group in clodoo.browseL8(ctx, model_grp, grp_ids):
+                if group.implied_ids:
+                    uniq_field.append(group.id)
+                    uniq_field += [x.id for x in group.implied_ids]
+            for group in clodoo.browseL8(ctx, model_grp, grp_ids,
+                                         context={'lang': 'en_US'}):
+                ir_md = clodoo.browseL8(ctx, model_ir_md,
+                    clodoo.searchL8(ctx, model_ir_md,
+                                    [('model', '=', model_grp),
+                                     ('res_id', '=', group.id)]))
+                if group.id in uniq_field:
+                    tag = '*'
+                else:
+                    tag = ''
+                print('%6d) -- Value [%-16.16s] > [%-32.32s] as "%s.%s" {%s}' % (
+                    group.id,
+                    group.name,
+                    group.full_name,
+                    ir_md.module,
+                    ir_md.name,
+                    tag))
+
+
 def all_addr_same_customer(ctx):
     print('Set delivery address to the same of customer on sale order')
     if ctx['param_1'] == 'help':
         print(
             'delivery_addr_same_customer '
             '[FROM_DATE|+DAYS|IDS] [Inv|Delivery|Both] [partner_id]'
         )
@@ -4222,14 +4266,161 @@
     store_inv_att_file(ctx, attachments, fn_attach_list)
 
     ctr += validate_moves(ctx)
 
     print("%d records update!" % ctr)
 
 
+RND_NAME_IT = [
+    "Giuseppe", "Giovanni", "Antonio", "Mario", "Luigi",
+    "Maria", "Anna", "Rosa", "Angela", "Teresa", "Lucia",
+    "Andrea", "Leonardo", "Alessandro", "Aurora", "Giulia",
+    "Gaia", "Alice", "Marco", "Lorenzo", "Luca", "Nicholas",
+    "Azzurra", "Bianca", "Celeste", "Viola", "Michele",
+    "Raffaele", "Daniele", "Pietro", "Vincenzo", "Bruno",
+    "Natale", "Rita", "Margherita", "Aldo", "Paolo",
+    "Luciano", "Sergio", "Alessio", "Tommaso", "Riccardo",
+    "Edoardo", "Federico", "Beatrice", "Francesco", "Vittorio",
+    "Ludovica", "Enea", "Virgilio", "Cesare", "Augusto",
+    "Leone", "Felice", "Umberto", "Filippo", "Ciro",
+    "Cinzia", "Antonello",
+]
+RND_NAME_XX = [
+    "Noah", "John", "Francis", "Jackob", "William", "Geroge",
+    "Emma", "Olivia", "Sophia", "Abigail", "Emily", "Elizabeth",
+    "Jack", "Harry", "Gil", "Rosemary", "Lilith", "Amelia",
+    "Sienna", "Ethan", "Charlie", "Thomas", "Edward", "Dylan",
+    "Bert", "Billy", "Giles", "Harold", "Quincy",
+    "Simon", "Teddy", "Tony", "Walter",
+]
+RND_LASTNAME_IT = [
+    "ROSSI", "FERRARI", "BIANCHI", "ROMANO", "VERDI",
+    "GENOVESE", "TOSCANO", "ANCONETANO", "NAPOLITANO", "PUGLISI",
+    "MARINO", "GRECO", "LOMBARDI", "COLOMBO", "GALLI", "GENTILE",
+    "FONTANA", "PADOVANO", "PERUGINO", "SICILIANO", "FERRERO",
+    "MORETTI", "GIORDANO", "TESTA", "NERI", "MAZZA", "MARTINELLI",
+    "DI LORENZO", "FAGIANI", "SANTORO", "BARBIERI", "CASANOVA",
+    "COSTA", "LONGO", "DE LUCA", "ESPOSITO", "SAVASTA",
+    "RIZZO", "SERRA", "PELLEGRINI", "POLLI", "PORTOGHESE",
+    "SPAGNOLO", "FRANCO", "TURCO", "PACIFICO",
+]
+RND_LASTNAME_XX = [
+    "BROOKS", "CHAPMAN", "COOPER", "FISHER", "FOX",
+    "HAMILTON", "JACKSON", "LEE", "PALMER", "TAYLOR",
+    "SMITH", "WELLS", "MARTIN", "GARCIA", "ROUX",
+    "JONES", "BROWN", "WILSON", "WRIGHT", "WALKER", "WHITE",
+    "LEROY", "MERCIERS", "DUMONT", "FISCHER",
+]
+RND_CITY_IT = [
+    "Torino", "Milano", "Roma", "Napoli", "Pistoia", "Genova",
+    "Firenze", "Bologna", "Venezia", "Bari", "Palermo",
+    "Cagliari", "Pescara", "Domodossola", "Empoli", "Jesolo",
+    "Lucca", "Montecatini", "Sassari", "Catania", "Lecce",
+    "Salerno", "Perugia", "Sanremo", "Brescia", "Bergamo",
+    "Verona", "Trieste", "Ravenna", "Matera", "Crotone",
+    "Siracusa", "Agrigento", "Marsala", "La Spezia",
+]
+RND_CITY_PREFIX_IT = [
+    "Quarto", "Quinto", "Sesto", "Settimo", "Finale", "Marina"
+]
+RND_CITY_XX = [
+    "Wien", "Antwerpen", "Sofija", "Zagreb", "Copenaghen",
+    "Helsinki", "Paris", "Berlin", "Athina", "Dublin",
+    "Amsterdam", "Warszawa", "Lisboa", "London", "Praha",
+    "Madrid", "Budapest", "Tel Aviv", "Casablanca", "New York",
+    "Los Angeles", "Atalanta", "Motevideo",
+]
+RND_TLD = [
+    "gmail.com", "outlook.com", "libero.it", "example.com",
+    "hotmail.com",
+]
+
+def anonimize_database(ctx):
+    def rnd_item(ctx, rndlist):
+        return rndlist[random.randint(0, len(rndlist) - 1)]
+
+    def read_partner(id):
+        try:
+            partner = clodoo.browseL8(ctx, _partner, id)
+            vals = {}
+        except BaseException:
+            vals = {
+                "name": "Unknown %d" % id,
+                "vat": False,
+                "codicefiscale": False,
+            }
+        if vals:
+            clodoo.writeL8(ctx, _partner, id, vals)
+            partner = clodoo.browseL8(ctx, _partner, id)
+        return partner
+
+    def build_random_data(ctx, id):
+        partner = read_partner(id)
+        if partner.country_id and partner.country_id.id != country_it_id:
+            name = rnd_item(ctx, RND_NAME_XX) + " " + rnd_item(ctx, RND_LASTNAME_XX)
+            city = rnd_item(ctx, RND_CITY_XX)
+            zip = ""
+            if partner.vat:
+                name += " Ltd"
+        else:
+            name = rnd_item(ctx, RND_NAME_IT) + " " + rnd_item(ctx, RND_LASTNAME_IT)
+            if id % 3:
+                city = rnd_item(ctx, RND_CITY_IT)
+            else:
+                city = rnd_item(ctx, RND_CITY_PREFIX_IT) + " di " + rnd_item(
+                    ctx, RND_CITY_IT)
+            zip = "%03d00" % random.randint(1, 999)
+            if partner.vat:
+                name += " s.r.l."
+        email = name.lower().replace(" ", ".") + "@" + rnd_item(ctx, RND_TLD)
+        phone = "0%d" % random.randint(200000000, 999999999)
+        mobile = "3%d" % random.randint(200000000, 999999999)
+        return {
+            "name": name,
+            "city": city,
+            "email": email,
+            "zip": zip,
+            "phone": phone,
+            "mobile": mobile,
+            "comment": "",
+            "text_GECS": "",
+        }
+
+    print('🎺🎺🎺 Anonimize database')
+    if ctx['param_1'] == 'help':
+        print('anonimize_database')
+        return
+
+    _partner = "res.partner"
+    _user = "res.users"
+    _company = "res.company"
+    _country = "res.country"
+    country_it_id = clodoo.searchL8(ctx, _country, [("code", "in", ["it", "IT"])])[0]
+    protected_partner_ids = []
+    for id in clodoo.searchL8(ctx, _user, []):
+        try:
+            user = clodoo.browseL8(ctx, _user, id)
+            msg_burst('%d) %s ...' % (id, user.login))
+            protected_partner_ids.append(user.partner_id.id)
+        except BaseException:
+            pass
+    for id in clodoo.searchL8(ctx, _company, []):
+        clodoo.writeL8(ctx, _company, id, {"name": "Test Company %d" % id})
+    for id in clodoo.searchL8(ctx,
+                              _partner,
+                              [("id", "not in", protected_partner_ids)],
+                              order="id"):
+        vals = build_random_data(ctx, id)
+        msg_burst('%d) %s ...' % (id, vals["name"]))
+        try:
+            clodoo.writeL8(ctx, _partner, id, vals)
+        except BaseException:
+            pass
+
+
 def move_database_by_postgres(ctx):
     print('🎺🎺🎺 Move database from postgres version to another')
     if ctx['param_1'] == 'help':
         print('move_database_by_postgres pg_port_orig pg_port_dest role')
         return
     if not ctx.get('param_1'):
         print("Missed postgres port of orig")
@@ -4300,14 +4491,69 @@
             print(stderr)
             return
         os.unlink(sqlfn)
         ctr += 1
     print("%d databases moved")
 
 
+def display_stock(ctx):
+    _picking = "stock.picking"
+    # _operation = "stock.pack.operation"
+    # _product = "product.product"
+    picking_id = 0
+    while picking_id >= 0:
+        picking_id = input("\nPicking ID (-1 to end): ")
+        picking_id = eval(picking_id) if picking_id else 0
+        if picking_id == 0:
+            continue
+        elif picking_id < 0:
+            break
+        try:
+            picking = clodoo.browseL8(ctx, _picking, picking_id)
+        except BaseException:
+            print("Picking %d not found!" % picking_id)
+            continue
+        print("Picking name: %s" % picking.name)
+        print("Picking state: %s" % picking.state)
+        fmt = (
+            "prod.%(product_id)5s %(product_name)-30.30s %(ordered_qty)7s"
+            " %(product_qty)7s  %(qty_done)7s %(ln_move_ids)8s"
+        )
+        fmt_m = (
+            "move.%(move_id)5s %(name)-30.30s %(ordered_qty)7s"
+            " %(product_qty)7s"
+        )
+        print(fmt % {
+            "product_id": "id",
+            "product_name": "product_name",
+            "product_qty": "p.qty",
+            "ordered_qty": "o.qty",
+            "qty_done": "done",
+            "ln_move_ids": "ln",
+        })
+        for operation in picking.pack_operation_product_ids:
+            params = {
+                "product_id": operation.id,
+                "product_name": operation.product_id.name,
+                "product_qty": operation.product_qty,
+                "ordered_qty": operation.ordered_qty,
+                "qty_done": operation.qty_done,
+                "ln_move_ids": operation.linked_move_operation_ids.ids,
+            }
+            print(fmt % params)
+            for ln in operation.linked_move_operation_ids:
+                params_m = {
+                    "move_id": ln.move_id.id,
+                    "name": ln.move_id.name,
+                    "product_qty": ln.move_id.product_qty,
+                    "ordered_qty": ln.move_id.ordered_qty,
+                }
+                print(fmt_m % params_m)
+
+
 if ctx['function']:
     function = ctx['function']
     globals()[function](ctx)
     exit()
 
 print('Avaiable functions:')
 print(' SALE ORDER                      ACCOUNT INVOICE')
```

### Comparing `odoo_score-2.0.5/odoo_score/scripts/main.py` & `odoo_score-2.0.6/odoo_score/scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 Odoo super core by Zeroincombenze(R)
 """
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -91,20 +91,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `odoo_score-2.0.5/odoo_score/scripts/map_module_dependecies.py` & `odoo_score-2.0.6/odoo_score/scripts/map_module_dependecies.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # import os
 from datetime import datetime
 import argparse
 import ast
 from python_plus import unicodes
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 class OdooMap(object):
     """ """
 
     def __init__(self, opt_args):
         self.opt_args = opt_args
```

### Comparing `odoo_score-2.0.5/odoo_score/scripts/rename_odoo_module.py` & `odoo_score-2.0.6/odoo_score/scripts/rename_odoo_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import argparse
 
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 
 
 def update_module_names(ctx, namespec, merge_modules=False):
     """Deal with changed module names, making all the needed changes on the
     related tables, like XML-IDs, translations, and so on.
 
     :param namespec: list of tuples of (old name, new name)
```

### Comparing `odoo_score-2.0.5/odoo_score/scripts/setup.info` & `odoo_score-2.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='odoo_score',
-    version='2.0.5',
+    version='2.0.6',
     description='Odoo super core',
     long_description="""
 Odoo supercore
 
 odoo_score is a library that extends the odoo orm functionality
 and makes available a simple odoo shell.
 """,
@@ -33,17 +33,15 @@
     author='Antonio Maria Vigliotti',
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
     install_requires=['z0lib', 'future'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={'': [
         'scripts/setup.info',
-        'scripts/run_odoo_debug.sh',
         './set_workers',
-        './models_barely',
     ]},
     entry_points={
         'console_scripts': [
             'odoo_score-info = odoo_score.scripts.main:main',
             'rename_odoo_module = odoo_score.scripts.rename_odoo_module:main',
             # 'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
         ]
```

### Comparing `odoo_score-2.0.5/odoo_score/secure_db.py` & `odoo_score-2.0.6/odoo_score/secure_db.py`

 * *Files identical despite different names*

### Comparing `odoo_score-2.0.5/odoo_score/set_workers` & `odoo_score-2.0.6/odoo_score/set_workers`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 evaluate_params() {
     local val prc minconn
     [[ $opt_branch =~ ^1[123456789] ]] && minconn=64 || minconn=32
     if [[ $opt_nopsql -ne 0 ]]; then
         ((AVAI_MEM=(CUR_MEM*3)/4))
```

### Comparing `odoo_score-2.0.5/odoo_score.egg-info/PKG-INFO` & `odoo_score-2.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1
-Name: odoo-score
-Version: 2.0.5
+Metadata-Version: 1.2
+Name: odoo_score
+Version: 2.0.6
 Summary: Odoo super core
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        Odoo supercore
+        
+        odoo_score is a library that extends the odoo orm functionality
+        and makes available a simple odoo shell.
+        
 Keywords: odoo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
-
-
-Odoo supercore
-
-odoo_score is a library that extends the odoo orm functionality
-and makes available a simple odoo shell.
-
-
```

### Comparing `odoo_score-2.0.5/odoo_score.egg-info/SOURCES.txt` & `odoo_score-2.0.6/odoo_score.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 odoo_score/__init__.py
 odoo_score/__main__.py
 odoo_score/api.py
 odoo_score/fields.py
 odoo_score/migrate.py
 odoo_score/models_2.py
 odoo_score/models_3.py
+odoo_score/models_7.py
 odoo_score/odoo_score.py
 odoo_score/odoo_score_10.py
 odoo_score/odoo_score_11.py
 odoo_score/odoo_score_12.py
 odoo_score/odoo_score_13.py
 odoo_score/odoo_score_14.py
 odoo_score/odoo_score_6.py
@@ -27,10 +28,8 @@
 odoo_score.egg-info/not-zip-safe
 odoo_score.egg-info/requires.txt
 odoo_score.egg-info/top_level.txt
 odoo_score/scripts/__init__.py
 odoo_score/scripts/main.py
 odoo_score/scripts/map_module_dependecies.py
 odoo_score/scripts/rename_odoo_module.py
-odoo_score/scripts/run_odoo_debug.py
-odoo_score/scripts/run_odoo_debug.sh
 odoo_score/scripts/setup.info
```

### Comparing `odoo_score-2.0.5/setup.py` & `odoo_score-2.0.6/odoo_score/scripts/setup.info`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='odoo_score',
-    version='2.0.5',
+    version='2.0.6',
     description='Odoo super core',
     long_description="""
 Odoo supercore
 
 odoo_score is a library that extends the odoo orm functionality
 and makes available a simple odoo shell.
 """,
@@ -33,17 +33,15 @@
     author='Antonio Maria Vigliotti',
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
     install_requires=['z0lib', 'future'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={'': [
         'scripts/setup.info',
-        'scripts/run_odoo_debug.sh',
         './set_workers',
-        './models_barely',
     ]},
     entry_points={
         'console_scripts': [
             'odoo_score-info = odoo_score.scripts.main:main',
             'rename_odoo_module = odoo_score.scripts.rename_odoo_module:main',
             # 'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
         ]
```

