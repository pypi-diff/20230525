# Comparing `tmp/enebootools-2.0.5.tar.gz` & `tmp/enebootools-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.0.5.tar", last modified: Wed May 24 18:52:18 2023, max compression
+gzip compressed data, was "enebootools-2.0.6.tar", last modified: Thu May 25 11:00:52 2023, max compression
```

## Comparing `enebootools-2.0.5.tar` & `enebootools-2.0.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.5/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.5/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 18:52:18.814128 enebootools-2.0.5/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.5/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.802128 enebootools-2.0.5/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-24 18:51:44.000000 enebootools-2.0.5/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.5/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.802128 enebootools-2.0.5/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.5/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.5/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.5/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25310 2023-05-24 09:01:44.000000 enebootools-2.0.5/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.5/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.5/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.5/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.5/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.810128 enebootools-2.0.5/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.5/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.5/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.810128 enebootools-2.0.5/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.5/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.810128 enebootools-2.0.5/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.5/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31916 2023-05-24 18:04:44.000000 enebootools-2.0.5/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 13:56:51.000000 enebootools-2.0.5/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.0.5/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-24 18:03:05.000000 enebootools-2.0.5/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-24 08:26:10.000000 enebootools-2.0.5/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.5/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.5/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.5/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.5/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.5/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.5/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.5/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.5/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.5/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.802128 enebootools-2.0.5/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-24 18:52:18.814128 enebootools-2.0.5/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.5/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.684831 enebootools-2.0.6/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.6/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.6/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-25 11:00:52.684831 enebootools-2.0.6/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.6/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.672831 enebootools-2.0.6/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-25 11:00:27.000000 enebootools-2.0.6/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.6/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.672831 enebootools-2.0.6/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.6/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.6/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.6/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26191 2023-05-25 10:49:49.000000 enebootools-2.0.6/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.6/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.672831 enebootools-2.0.6/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.6/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.6/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.6/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.6/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.6/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.6/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.6/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.676831 enebootools-2.0.6/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.6/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.6/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.6/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.680831 enebootools-2.0.6/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26271 2023-05-25 10:58:59.000000 enebootools-2.0.6/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.680831 enebootools-2.0.6/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.680831 enebootools-2.0.6/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.6/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.680831 enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.6/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    32041 2023-05-25 10:53:57.000000 enebootools-2.0.6/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 13:56:51.000000 enebootools-2.0.6/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.0.6/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-24 18:03:05.000000 enebootools-2.0.6/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-24 08:26:10.000000 enebootools-2.0.6/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.6/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.6/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.680831 enebootools-2.0.6/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.6/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.6/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.684831 enebootools-2.0.6/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.6/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.6/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.6/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.6/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.684831 enebootools-2.0.6/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.6/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.684831 enebootools-2.0.6/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.6/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 11:00:52.672831 enebootools-2.0.6/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-25 11:00:52.000000 enebootools-2.0.6/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-25 11:00:52.000000 enebootools-2.0.6/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-25 11:00:52.000000 enebootools-2.0.6/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-25 11:00:52.000000 enebootools-2.0.6/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-25 11:00:52.000000 enebootools-2.0.6/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-25 11:00:52.000000 enebootools-2.0.6/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-25 11:00:52.684831 enebootools-2.0.6/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.6/setup.py
```

### Comparing `enebootools-2.0.5/LICENSE.gplv3` & `enebootools-2.0.6/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/PKG-INFO` & `enebootools-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.5
+Version: 2.0.6
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.5/README.rst` & `enebootools-2.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/__init__.py` & `enebootools-2.0.6/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.0.5"
+__VERSION__ = "2.0.6"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.0.5/enebootools/__init__.pyc` & `enebootools-2.0.6/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/__init__.py` & `enebootools-2.0.6/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/config.py` & `enebootools-2.0.6/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/database.py` & `enebootools-2.0.6/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/databasemodels.py` & `enebootools-2.0.6/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/featureconfig.py` & `enebootools-2.0.6/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/kobjects.py` & `enebootools-2.0.6/enebootools/assembler/kobjects.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,27 +106,27 @@
             cname, name = k
             if cname != self.__name__:
                 continue
             obj.finish_setup()
 
     def _get_full_required_modules(self):
         if self.all_required_modules:
-            # print("***", self, self.all_required_modules)
             return self.all_required_modules
         req = []
         myreq = []
+
         for modname in self.required_modules:
             obj = ModuleObject.find(modname)
             if obj is None:
                 self.iface.info(
                     "Modulo con nombre %s no encontrado (requerido por %s )"
                     % (modname, self.formal_name())
                 )
                 continue
-            # print("*", self, modname)
+
             new_reqs = [
                 modulename
                 for modulename in obj._get_full_required_modules()
                 if modulename not in req
             ]
             if self.type == "prj":
                 for n in new_reqs:
@@ -165,51 +165,60 @@
                         % (self.formal_name(), n, featname)
                     )
 
             req += new_reqs
 
         req += [modulename for modulename in myreq if modulename not in req]
         new_list = []
+
         for module_name in req:
-            if "/" not in module_name:
+            if (
+                "/" not in module_name
+            ):  # esto filtra dependencias que son añadidas por código de módulo, para evitar que introduzca módulos con versiones incorrectas
                 module_obj = ModuleObject.find(module_name)
                 formal_name = module_obj.formal_name()
-                if formal_name in req:
-                    self.iface.debug(
-                        "Omitiendo módulo %s (ya existe %s)" % (module_name, formal_name)
-                    )
+                if formal_name in [
+                    formal_name for req_item in req if str(req_item).endswith(formal_name)
+                ]:
+                    if str(self.fullpath).endswith("fun_euromoda"):
+                        self.iface.debug(
+                            "Omitiendo módulo %s (ya existe %s : %s)"
+                            % (module_name, formal_name, module_obj.fullpath)
+                        )
                     continue
 
             new_list.append(module_name)
 
         self.all_required_modules = new_list
         return req
 
     def _get_full_required_features(self):
         if self.all_required_features:
             return self.all_required_features
         req = []
         myreq = []
+
         for featname in self.required_features:
             obj = FeatureObject.find(featname)
             if obj is None:
                 self.iface.info(
                     "Funcionalidad con nombre %s no encontrada (requerida por %s )"
                     % (featname, self.formal_name())
                 )
+                if self.formal_name() == "fun_euromoda":
+                    print("No existe", featname)
+
                 continue
-            new_reqs = [
-                featurename
-                for featurename in obj._get_full_required_features()
-                if featurename not in req
-            ]
+
+            new_reqs = []
+            for featurename in obj._get_full_required_features():
+                if featurename not in req and "24_%s" % featurename not in req:
+                    new_reqs.append(featurename)
             if self.type == "prj":
                 for n in new_reqs:
-                    if n in self.required_features:
-                        continue
                     self.iface.debug(
                         "Proyecto %s, se agrega funcionalidad %s solicitada por %s"
                         % (self.formal_name(), n, featname)
                     )
             req += new_reqs
             # req += new_reqs
             if obj.formal_name() not in req:
@@ -323,22 +332,32 @@
         binstr.set("feature", self.formal_name())
         binstr.set("target", "base")
         binstr.set("path", self.fullpath)
         binstr.set("dstfolder", "build/base")
         if self.dstfolder:
             binstr.set("dstfolder", self.dstfolder)
         etree.SubElement(binstr, "Message", text="Copiando módulos . . .")
-        # print("------->", self._get_full_required_modules())
-        for modulename in self._get_full_required_modules():
+
+        self.iface.debug("-- MODULES -----> %s" % self._get_full_required_modules())
+
+        for modulename in (
+            self.required_modules
+            if self.qs_extend_mode == "yeboyebo"
+            else self._get_full_required_modules()
+        ):
             module = ModuleObject.find(modulename)
+            if not module:
+                self.iface.warn("No encontramos el módulo %s" % modulename)
+
             cpfolder = etree.SubElement(binstr, "CopyFolderAction")
             cpfolder.set("src", module.fullpath)
             cpfolder.set("dst", module.obj.relpath)
             cpfolder.set("create_dst", "yes")
 
+        self.iface.debug("-- FEATURES -----> %s" % self._get_full_required_features())
         for featurename in self._get_full_required_features():
             feature = FeatureObject.find(featurename)
             patch_list = feature.get_patch_list()
             if len(patch_list) == 0:
                 self.iface.warn("No encontramos parches para aplicar en %s" % featurename)
             etree.SubElement(binstr, "Message", text="Aplicando extensión %s . . ." % featurename)
             for patchdir in patch_list:
@@ -361,15 +380,19 @@
         binstr.set("target", "final")
         binstr.set("depends", "base")
         binstr.set("path", self.fullpath)
         binstr.set("dstfolder", "build/final")
         if self.dstfolder:
             binstr.set("dstfolder", self.dstfolder)
 
-        for modulename in self._get_full_required_modules():
+        for modulename in (
+            self.required_modules
+            if self.qs_extend_mode == "yeboyebo"
+            else self._get_full_required_modules()
+        ):
             module = ModuleObject.find(modulename)
             cpfolder = etree.SubElement(binstr, "CopyFolderAction")
             cpfolder.set("src", os.path.join(dep_folder, module.obj.relpath))
             cpfolder.set("dst", module.obj.relpath)
             cpfolder.set("create_dst", "yes")
 
         featurename = self.formal_name()
@@ -397,15 +420,19 @@
         binstr.set("target", "src")
         binstr.set("depends", "final")
         binstr.set("path", self.fullpath)
         binstr.set("dstfolder", "build/src")
         if self.dstfolder:
             binstr.set("dstfolder", self.dstfolder)
 
-        for modulename in self.all_required_modules:
+        for modulename in (
+            self.required_modules
+            if self.qs_extend_mode == "yeboyebo"
+            else self._get_full_required_modules()
+        ):
             module = ModuleObject.find(modulename)
             cpfolder = etree.SubElement(binstr, "CopyFolderAction")
             cpfolder.set("src", os.path.join(dep_folder, module.obj.relpath))
             cpfolder.set("dst", module.obj.relpath)
             cpfolder.set("create_dst", "yes")
 
         return binstr
@@ -641,15 +668,14 @@
         if not feature:
             self.iface.error("Funcionalidad %s desconocida." % func)
             return None
         feature.set_patch_list([newname])
 
     def get_build_actions(self, target, func, dstfolder=None):
         feature = FeatureObject.find(func)
-        # print("*******************", func, feature)
         if not feature:
             self.iface.error("Funcionalidad %s desconocida." % func)
             return None
 
         feature.set_dstfolder(dstfolder)
 
         if target == "base":
```

### Comparing `enebootools-2.0.5/enebootools/assembler/mypeewee.py` & `enebootools-2.0.6/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/assembler/save_auto.py` & `enebootools-2.0.6/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/autoconfig/autoconfig.py` & `enebootools-2.0.6/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/autoconfig/parsers.py` & `enebootools-2.0.6/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/__init__.py` & `enebootools-2.0.6/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.0.6/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.0.6/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.0.6/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.0.6/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.0.6/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/certificates/README.txt` & `enebootools-2.0.6/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/crypto/main.py` & `enebootools-2.0.6/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.0.6/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/entry_points.py` & `enebootools-2.0.6/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/extracttool/__init__.py` & `enebootools-2.0.6/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/extracttool/extractfunctions.py` & `enebootools-2.0.6/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.0.6/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/lib/etree/ElementPath.py` & `enebootools-2.0.6/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/lib/etree/ElementTree.py` & `enebootools-2.0.6/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/lib/etree/__init__.py` & `enebootools-2.0.6/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/lib/peewee.py` & `enebootools-2.0.6/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/lib/utils.py` & `enebootools-2.0.6/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/__init__.py` & `enebootools-2.0.6/enebootools/mergetool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,15 +512,19 @@
                 return flpatchqs.diff_qs_dir(self, base, final)
             if ext == "PY":
                 aBase = base.split("/")
                 nom = aBase[-1:][0]
                 if nom.startswith("test_"):
                     return flpatchtest.diff_test(self, base, final)
 
-                elif nom.endswith("_api.py"):
+                elif (
+                    nom.endswith(("_api.py", "_schema.py", "_model.py"))
+                    or nom.startswith("test_")
+                    and nom.endswith(".py")
+                ):
                     return flpatchapipy.diff_py(self, base, final)
                 elif "models" in base or "pruebasqs" in base:
                     return flpatchmodel.diff_model(self, base, final)
                 else:
                     return flpatchpy.diff_py(self, base, final)
             # if ext == 'XML': return flpatchxml.diff_xml(self,base,final)
             if ext == "XML":
@@ -541,15 +545,19 @@
                 nom = aBase[-1:][0]
                 if nom.startswith("test_"):
                     return flpatchtest.patch_test(self, base, patch)
                 elif nom.endswith("_ut.py"):
                     return flpatchpy.patch_py(self, base, patch)
                 elif nom.endswith("_def.py"):
                     return flpatchpy.patch_py(self, base, patch)
-                elif nom.endswith(("_api.py", "_schema.py", "_model.py")):
+                elif (
+                    nom.endswith(("_api.py", "_schema.py", "_model.py"))
+                    or nom.startswith("test_")
+                    and nom.endswith(".py")
+                ):
                     return flpatchapipy.patch_py(self, base, patch)
                 elif "models" in base or "pruebasqs" in base:
                     return flpatchmodel.patch_model(self, base, patch)
                 else:
                     return flpatchpy.patch_py(self, base, patch)
             if ext == "XML":
                 return flpatchlxml.patch_lxml(self, patch, base)
```

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/index.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.0.6/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchapipy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchdir.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,19 @@
         old_verbosity = self.iface.verbosity
         self.iface.verbosity -= 2
         if self.iface.verbosity < 0:
             self.iface.verbosity = 0
         old_style, self.iface.patch_py_style_name = self.iface.patch_py_style_name, style
         self.iface.set_output_file(dst + ".patched")
         if style in ["legacy"]:
-            if filename.endswith(("_api.py", "_schema.py", "_model.py")):
+            if (
+                filename.endswith(("_api.py", "_schema.py", "_model.py"))
+                or filename.startswith("test_")
+                and filename.endswith(".py")
+            ):
                 ret = flpatchapipy.patch_py(self.iface, dst, src)
             else:
                 ret = flpatchpy.patch_py(self.iface, dst, src)
         elif style in ["qsdir"]:
             ret = flpatchpy.patch_py_dir(self.iface, dst, src)
         else:
             raise ValueError("Estilo de parche PY desconocido: %s" % style)
```

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchpy.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchqs.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchtest.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/flpatchxml.py` & `enebootools-2.0.6/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/projectbuilder.py` & `enebootools-2.0.6/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/test/__init__.py` & `enebootools-2.0.6/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.0.6/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/packager/__init__.py` & `enebootools-2.0.6/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/packager/pkgjoiner.py` & `enebootools-2.0.6/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/packager/pkgsplitter.py` & `enebootools-2.0.6/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/parseargs.py` & `enebootools-2.0.6/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools/parseargs.pyc` & `enebootools-2.0.6/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/enebootools.egg-info/PKG-INFO` & `enebootools-2.0.6/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.5
+Version: 2.0.6
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.5/enebootools.egg-info/SOURCES.txt` & `enebootools-2.0.6/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.5/setup.py` & `enebootools-2.0.6/setup.py`

 * *Files identical despite different names*

