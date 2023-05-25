# Comparing `tmp/enebootools-2.0.4.tar.gz` & `tmp/enebootools-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.0.4.tar", last modified: Wed May 24 09:22:19 2023, max compression
+gzip compressed data, was "enebootools-2.0.5.tar", last modified: Wed May 24 18:52:18 2023, max compression
```

## Comparing `enebootools-2.0.4.tar` & `enebootools-2.0.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.4/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.4/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 09:22:19.448222 enebootools-2.0.4/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.4/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.440222 enebootools-2.0.4/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-24 09:19:34.000000 enebootools-2.0.4/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.4/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.4/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.4/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.4/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25310 2023-05-24 09:01:44.000000 enebootools-2.0.4/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.4/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.4/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.4/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.4/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.4/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.4/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.4/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.4/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31644 2023-05-24 09:19:21.000000 enebootools-2.0.4/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 08:29:10.000000 enebootools-2.0.4/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.4/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.4/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-24 08:26:10.000000 enebootools-2.0.4/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.4/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.4/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.4/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.4/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.4/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.4/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.4/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.4/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.4/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-24 09:22:19.448222 enebootools-2.0.4/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.4/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.5/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.5/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 18:52:18.814128 enebootools-2.0.5/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.5/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.802128 enebootools-2.0.5/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-24 18:51:44.000000 enebootools-2.0.5/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.5/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.802128 enebootools-2.0.5/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.5/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.5/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.5/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25310 2023-05-24 09:01:44.000000 enebootools-2.0.5/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.5/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.5/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.5/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.5/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.806128 enebootools-2.0.5/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.810128 enebootools-2.0.5/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.5/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.5/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.5/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.810128 enebootools-2.0.5/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.5/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.810128 enebootools-2.0.5/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.5/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31916 2023-05-24 18:04:44.000000 enebootools-2.0.5/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 13:56:51.000000 enebootools-2.0.5/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.0.5/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-24 18:03:05.000000 enebootools-2.0.5/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-24 08:26:10.000000 enebootools-2.0.5/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.5/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.5/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.5/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.5/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.5/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.5/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.5/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.5/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.5/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.814128 enebootools-2.0.5/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.5/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 18:52:18.802128 enebootools-2.0.5/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-24 18:52:18.000000 enebootools-2.0.5/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-24 18:52:18.814128 enebootools-2.0.5/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.5/setup.py
```

### Comparing `enebootools-2.0.4/LICENSE.gplv3` & `enebootools-2.0.5/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/PKG-INFO` & `enebootools-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.4
+Version: 2.0.5
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.4/README.rst` & `enebootools-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/__init__.py` & `enebootools-2.0.5/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.0.4"
+__VERSION__ = "2.0.5"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.0.4/enebootools/__init__.pyc` & `enebootools-2.0.5/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/__init__.py` & `enebootools-2.0.5/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/config.py` & `enebootools-2.0.5/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/database.py` & `enebootools-2.0.5/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/databasemodels.py` & `enebootools-2.0.5/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/featureconfig.py` & `enebootools-2.0.5/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/kobjects.py` & `enebootools-2.0.5/enebootools/assembler/kobjects.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/mypeewee.py` & `enebootools-2.0.5/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/assembler/save_auto.py` & `enebootools-2.0.5/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/autoconfig/autoconfig.py` & `enebootools-2.0.5/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/autoconfig/parsers.py` & `enebootools-2.0.5/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/__init__.py` & `enebootools-2.0.5/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.0.5/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.0.5/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.0.5/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.0.5/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/certificates/README.txt` & `enebootools-2.0.5/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/crypto/main.py` & `enebootools-2.0.5/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.0.5/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/entry_points.py` & `enebootools-2.0.5/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/extracttool/__init__.py` & `enebootools-2.0.5/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/extracttool/extractfunctions.py` & `enebootools-2.0.5/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.0.5/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/lib/etree/ElementPath.py` & `enebootools-2.0.5/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/lib/etree/ElementTree.py` & `enebootools-2.0.5/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/lib/etree/__init__.py` & `enebootools-2.0.5/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/lib/peewee.py` & `enebootools-2.0.5/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/lib/utils.py` & `enebootools-2.0.5/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/__init__.py` & `enebootools-2.0.5/enebootools/mergetool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/index.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.0.5/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchapipy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchdir.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             ret = flpatchqs.patch_qs_dir(self.iface, dst, src)
         else:
             raise ValueError("Estilo de parche QS desconocido: %s" % style)
         self.iface.output = old_output
         self.iface.verbosity = old_verbosity
         self.iface.patch_qs_style_name = old_style
         if not ret:
-            self.iface.warn("Hubo algún problema aplicando el parche QS para %s" % filename)
+            self.iface.debug("Hubo algún problema aplicando el parche QS para %s" % filename)
             try:
                 os.unlink(dst + ".patched")
             except IOError:
                 pass
         else:
             os.unlink(dst)
             os.rename(dst + ".patched", dst)
@@ -282,15 +282,15 @@
         if self.iface.verbosity < 0:
             self.iface.verbosity = min([0, self.iface.verbosity])
         self.iface.set_output_file(dst + ".patched")
         ret = flpatchlxml.patch_lxml(self.iface, src, dst)
         self.iface.output = old_output
         self.iface.verbosity = old_verbosity
         if not ret:
-            self.iface.warn("Hubo algún problema aplicando el parche XML para %s" % filename)
+            self.iface.debug("Hubo algún problema aplicando el parche XML para %s" % filename)
             try:
                 os.unlink(dst + ".patched")
             except IOError:
                 pass
         else:
             os.unlink(dst)
             os.rename(dst + ".patched", dst)
@@ -324,15 +324,15 @@
             ret = flpatchpy.patch_py_dir(self.iface, dst, src)
         else:
             raise ValueError("Estilo de parche PY desconocido: %s" % style)
         self.iface.output = old_output
         self.iface.verbosity = old_verbosity
         self.iface.patch_qs_style_name = old_style
         if not ret:
-            self.iface.warn("Hubo algún problema aplicando el parche PY para %s" % filename)
+            self.iface.debug("Hubo algún problema aplicando el parche PY para %s" % filename)
             try:
                 os.unlink(dst + ".patched")
             except IOError:
                 pass
         else:
             os.unlink(dst)
             os.rename(dst + ".patched", dst)
@@ -457,24 +457,27 @@
             return
         if final_hexdigest == none_hexdigest:
             return
 
         script_exts = ".qs".split(" ")
         xml_exts = ".xml .ui .mtd".split(" ")
         php_exts = ".php".split(" ")
+        py_exts = ".py".split(" ")
 
         path, name = os.path.split(filename)
         froot, ext = os.path.splitext(name)
 
         if ext in script_exts:
             # flpatch:patchScript
             self.create_action("patchScript", filename)
         elif ext in xml_exts:
             # flpatch:patchXml
             self.create_action("patchXml", filename)
+        elif ext in py_exts:
+            self.create_action("patchPy", filename)
         # elif ext in php_exts:
         # TODO: flpatch:patchPhp
         else:
             # flpatch:replaceFile
             self.create_action("replaceFile", filename)
 
     def remove_file(self, filename):
@@ -824,17 +827,21 @@
         iface.info("No hay cambios!")
         return
     iface.info("Cambios detectados!")
     iface.info("Guardando cambios en %s" % patch_xml_file)
 
     file_ = open(patch_xml_file, "w", encoding="UTF-8")
     result = _xf(current_et)
-    result = result.replace("/></flpatch", "/>\n</flpatch")
-    result = result.replace("\n<flpatch", "\n  <flpatch")
-    result = result.replace("/><flpatch", "/>\n  <flpatch")
+    result = result.replace(
+        'xmlns:flpatch="http://www.abanqg2.com/es/directori/abanq-ensambla/?flpatch"', ""
+    )
+    result = result.replace("><flpatch", ">\n    <flpatch")
+    result = result.replace("\n  <flpatch", "\n    <flpatch")
+    result = result.replace('">', '" >')
+    result = result.replace('"/>', '" />')
     file_.write(result)
     file_.close()
 
 
 def patch_folder_inplace(iface, patchdir, finaldir):
     fpatch = FolderApplyPatch(iface, patchdir)
     fpatch.patch_folder(finaldir)
```

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchlxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -938,15 +938,15 @@
             close_matches = difflib.get_close_matches(searching, alternatives, 4, 0.4)
             if actionname == "delete":
                 self.iface.info(
                     "No se encontró elemento %s para %s entre %s"
                     % (repr(searching), repr(actionname), close_matches)
                 )
             else:
-                self.iface.warn(
+                self.iface.info(
                     "No se encontró elemento %s para %s entre %s"
                     % (repr(searching), repr(actionname), close_matches)
                 )
             return
 
         if actionname == "update" and select == "text()":
             element.text = action.text
@@ -984,15 +984,15 @@
             self.xfinal.load_entities(parent, added.tag)
 
         elif actionname == "insert-after" and select != ".":
             searching = select.split("/")[0]
             alternatives = element.xpath("*/@ctx-id")
             close_matches = difflib.get_close_matches(searching, alternatives, 4, 0.4)
 
-            self.iface.warn(
+            self.iface.info(
                 "No se encontró el elemento %s entre %s y se agregó el nodo al final"
                 % (searching, close_matches)
             )
             added = deepcopy(action[0])
             tail = element.text
             try:
                 previous = element.getchildren()[-1]
```

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,24 +148,24 @@
     delclasses = []
     declidx = {}
     defidx = {}
     iface_n = None
     classpatch = []
     for n, line in enumerate(file_lines):
         line2 = latin1_to_ascii(line)
-        m = re.search(r"#\s*@\s*([\w\.,;-]+)\s+([^ #]+)?\s*#", line2)
+        m = re.search(r"#\s*@\s*([\w\.,;-]+)\s+([^ #]+)", line2)
         if m:
-            m2 = re.search("^\s*# @(\w+)( \w+)?\s#\s*$", line)
+            m2 = re.search("^\s*# @(\w+)( \w+)", line)
             if not m2:
                 iface.warn("Formato incorrecto de la linea %s" % repr(line))
             dtype = m.group(1)
             cname = m.group(2)
             for n2, sline in enumerate(file_lines[n + 1 :]):
                 sline2 = latin1_to_ascii(sline)
-                sm = re.search(r"#\s*@\s*([\w\.,;-]+)\s+([^ #]+)?\s*#", sline2)
+                sm = re.search(r"#\s*@\s*([\w\.,;-]+)\s+([^ #]+)", sline2)
                 if sm:
                     break
             n2 += n + 1
             class_lines = file_lines[n:n2]
             heu_dtype = None
             heu_cname = None
             heu_extends = None
@@ -1125,15 +1125,14 @@
 
         new_block = []
         add_buffer_a = []
         add_buffer_b = []
         last_a_diff = 0
         last_b_diff = 0
         while True:
-
             if a_diffs and a_diffs[0][0] == base_pos:
                 f_a_diff = a_diffs.pop(0)
                 if f_a_diff[1] == "+ ":
                     a_offset += 1
                     add_buffer_a.append(f_a_diff[3])
                     last_a_diff = 0
                 if f_a_diff[1] == "- ":
```

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchpy.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchqs.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchtest.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/flpatchxml.py` & `enebootools-2.0.5/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/projectbuilder.py` & `enebootools-2.0.5/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/test/__init__.py` & `enebootools-2.0.5/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.0.5/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/packager/__init__.py` & `enebootools-2.0.5/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/packager/pkgjoiner.py` & `enebootools-2.0.5/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/packager/pkgsplitter.py` & `enebootools-2.0.5/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/parseargs.py` & `enebootools-2.0.5/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools/parseargs.pyc` & `enebootools-2.0.5/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/enebootools.egg-info/PKG-INFO` & `enebootools-2.0.5/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.4
+Version: 2.0.5
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.4/enebootools.egg-info/SOURCES.txt` & `enebootools-2.0.5/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.4/setup.py` & `enebootools-2.0.5/setup.py`

 * *Files identical despite different names*

