# Comparing `tmp/zar-2.0.1.tar.gz` & `tmp/zar-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zar-2.0.1.tar", last modified: Sun Apr 23 14:04:27 2023, max compression
+gzip compressed data, was "dist/zar-2.0.2.tar", last modified: Thu May 25 08:54:11 2023, max compression
```

## Comparing `zar-2.0.1.tar` & `zar-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:04:27.171901 zar-2.0.1/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1199 2023-04-23 14:04:27.171901 zar-2.0.1/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6678 2023-04-23 14:04:26.000000 zar-2.0.1/README.rst
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:04:27.171901 zar-2.0.1/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1359 2023-02-25 14:51:46.000000 zar-2.0.1/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:04:27.171901 zar-2.0.1/zar/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       46 2022-12-09 05:08:44.000000 zar-2.0.1/zar/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zar-2.0.1/zar/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:04:27.171901 zar-2.0.1/zar.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1199 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      185 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 09:05:11.000000 zar-2.0.1/zar.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        4 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/top_level.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:54:11.000000 zar-2.0.2/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:54:11.000000 zar-2.0.2/zar/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zar-2.0.2/zar/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       46 2022-12-09 05:08:44.000000 zar-2.0.2/zar/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        4 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 09:05:11.000000 zar-2.0.2/zar.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      185 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1250 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:54:11.000000 zar-2.0.2/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1359 2023-05-20 08:03:42.000000 zar-2.0.2/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1250 2023-05-25 08:54:11.000000 zar-2.0.2/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5707 2023-05-21 13:34:30.000000 zar-2.0.2/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `zar-2.0.1/PKG-INFO` & `zar-2.0.2/zar.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: zar
-Version: 2.0.1
+Version: 2.0.2
 Summary: Zeroincombenze Archive Replica
 Home-page: UNKNOWN
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        ZAR stand for Zeroincombenze® Archive Replica.
+        It is a tool kit to backup, restore, replicate files and/or database.
+        
+        ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
+        
 Keywords: backup,restore,replica
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
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
-ZAR stand for Zeroincombenze® Archive Replica.
-It is a tool kit to backup, restore, replicate files and/or database.
-
-ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
-
-
```

### Comparing `zar-2.0.1/README.rst` & `zar-2.0.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 =========
-zar 2.0.1
+zar 2.0.2
 =========
 
 
 
-|Maturity| |Build Status| |Coverage Status| |license gpl|
+|Maturity| |license gpl|
 
 
 
 
 Overview
 ========
 
@@ -68,19 +68,14 @@
 |
 |
 
 Getting started
 ===============
 
 
-|
-
-Installation
-------------
-
 For stable version:
 
 `pip install zar`
 
 For current version:
 
 `cd $HOME`
@@ -88,46 +83,41 @@
 `cd $HOME/tools`
 `./install_tools.sh`
 
 
 Upgrade
 -------
 
-Upgrade
--------
-
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+::
+
     pip install zar -U
 
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
 
+2.0.2 (2023-05-14)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] reassing_owner accept db_port
+
 2.0.1 (2023-02-25)
 ~~~~~~~~~~~~~~~~~~
 
 * [IMP] Remote bckdir different from local
 
 2.0.0 (2022-10-20)
 ~~~~~~~~~~~~~~~~~~
@@ -148,58 +138,44 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio M. Vigliotti <info@shs-av.com>
+* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
 Contributors
 ------------
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-04-23
+Last Update / Ultimo aggiornamento: 2023-05-21
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Alfa-black.png
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

### Comparing `zar-2.0.1/setup.py` & `zar-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='zar',
-    version='2.0.1',
+    version='2.0.2',
     description='Zeroincombenze Archive Replica',
     long_description="""
 ZAR stand for Zeroincombenze® Archive Replica.
 It is a tool kit to backup, restore, replicate files and/or database.
 
 ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
 """,
```

### Comparing `zar-2.0.1/zar.egg-info/PKG-INFO` & `zar-2.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: zar
-Version: 2.0.1
+Version: 2.0.2
 Summary: Zeroincombenze Archive Replica
 Home-page: UNKNOWN
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        ZAR stand for Zeroincombenze® Archive Replica.
+        It is a tool kit to backup, restore, replicate files and/or database.
+        
+        ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
+        
 Keywords: backup,restore,replica
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
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
-ZAR stand for Zeroincombenze® Archive Replica.
-It is a tool kit to backup, restore, replicate files and/or database.
-
-ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
-
-
```

