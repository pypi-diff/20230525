# Comparing `tmp/copr-cli-1.98.tar.gz` & `tmp/copr-cli-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copr-cli-1.98.tar", last modified: Thu Feb  3 12:18:26 2022, max compression
+gzip compressed data, was "copr-cli-1.99.tar", last modified: Mon Mar 21 08:44:04 2022, max compression
```

## Comparing `copr-cli-1.98.tar` & `copr-cli-1.99.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-02-03 12:18:26.161997 copr-cli-1.98/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    18092 2021-12-12 15:37:48.000000 copr-cli-1.98/LICENSE
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      208 2021-12-12 15:37:48.000000 copr-cli-1.98/MANIFEST.in
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      856 2022-02-03 12:18:26.160997 copr-cli-1.98/PKG-INFO
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    37213 2022-02-02 21:55:33.000000 copr-cli-1.98/copr-cli.spec
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-02-03 12:18:26.158997 copr-cli-1.98/copr_cli/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1650 2021-12-12 15:37:48.000000 copr-cli-1.98/copr_cli/README.rst
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       24 2021-12-12 15:37:48.000000 copr-cli-1.98/copr_cli/__init__.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1847 2021-12-12 15:37:48.000000 copr-cli-1.98/copr_cli/build_config.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      623 2022-01-04 00:09:47.000000 copr-cli-1.98/copr_cli/helpers.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    82424 2022-01-31 23:11:50.000000 copr-cli-1.98/copr_cli/main.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3181 2022-02-03 12:15:39.000000 copr-cli-1.98/copr_cli/monitor.py
--rwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)     4836 2021-12-12 15:37:48.000000 copr-cli-1.98/copr_cli/package_build_order.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     4001 2022-02-02 21:55:33.000000 copr-cli-1.98/copr_cli/printers.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1169 2021-12-12 15:37:48.000000 copr-cli-1.98/copr_cli/util.py
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-02-03 12:18:26.158997 copr-cli-1.98/copr_cli.egg-info/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      856 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/PKG-INFO
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1043 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       49 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/entry_points.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/not-zip-safe
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       43 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/requires.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        9 2022-02-03 12:18:26.000000 copr-cli-1.98/copr_cli.egg-info/top_level.txt
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-02-03 12:18:26.159997 copr-cli-1.98/man/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    24537 2022-01-31 23:11:50.000000 copr-cli-1.98/man/copr-cli.1.asciidoc
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      918 2022-01-04 00:09:47.000000 copr-cli-1.98/man/copr-cli.cheat
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       20 2021-12-12 15:37:48.000000 copr-cli-1.98/man/copr.1
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      170 2021-12-12 15:37:48.000000 copr-cli-1.98/requirements.txt
--rwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)      124 2021-12-12 15:37:48.000000 copr-cli-1.98/run_tests.sh
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       38 2022-02-03 12:18:26.161997 copr-cli-1.98/setup.cfg
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1475 2022-02-02 21:55:33.000000 copr-cli-1.98/setup.py
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-02-03 12:18:26.159997 copr-cli-1.98/tests/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      445 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/cli_tests_lib.py
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-02-03 12:18:26.160997 copr-cli-1.98/tests/resources/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3742 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/get_package_expected.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1282 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/get_package_response.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     2672 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/get_package_response_builds.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      126 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/list_builds_expected.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3560 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/list_builds_response.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3303 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/list_packages_expected.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3260 2022-01-31 23:11:50.000000 copr-cli-1.98/tests/resources/list_packages_response.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1376 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/list_projects_expected.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1602 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/resources/list_projects_response.json
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    31475 2022-01-31 23:11:50.000000 copr-cli-1.98/tests/test_cli.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     5810 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/test_distgit.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     6166 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/test_mock_config.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      536 2021-12-12 15:37:48.000000 copr-cli-1.98/tests/test_util.py
+drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-03-21 08:44:04.307840 copr-cli-1.99/
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    18092 2021-12-12 15:37:48.000000 copr-cli-1.99/LICENSE
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      208 2021-12-12 15:37:48.000000 copr-cli-1.99/MANIFEST.in
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      856 2022-03-21 08:44:04.307840 copr-cli-1.99/PKG-INFO
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    37389 2022-03-18 16:26:14.000000 copr-cli-1.99/copr-cli.spec
+drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-03-21 08:44:04.305840 copr-cli-1.99/copr_cli/
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1632 2022-02-17 09:42:30.000000 copr-cli-1.99/copr_cli/README.rst
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       24 2021-12-12 15:37:48.000000 copr-cli-1.99/copr_cli/__init__.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1847 2021-12-12 15:37:48.000000 copr-cli-1.99/copr_cli/build_config.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      623 2022-01-04 00:09:47.000000 copr-cli-1.99/copr_cli/helpers.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    83721 2022-03-18 16:26:14.000000 copr-cli-1.99/copr_cli/main.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3181 2022-02-06 20:01:02.000000 copr-cli-1.99/copr_cli/monitor.py
+-rwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)     4836 2021-12-12 15:37:48.000000 copr-cli-1.99/copr_cli/package_build_order.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     4001 2022-02-09 12:03:09.000000 copr-cli-1.99/copr_cli/printers.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1169 2021-12-12 15:37:48.000000 copr-cli-1.99/copr_cli/util.py
+drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-03-21 08:44:04.306840 copr-cli-1.99/copr_cli.egg-info/
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      856 2022-03-21 08:44:04.000000 copr-cli-1.99/copr_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1043 2022-03-21 08:44:04.000000 copr-cli-1.99/copr_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-03-21 08:44:04.000000 copr-cli-1.99/copr_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       49 2022-03-21 08:44:04.000000 copr-cli-1.99/copr_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-02-03 12:18:26.000000 copr-cli-1.99/copr_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       43 2022-03-21 08:44:04.000000 copr-cli-1.99/copr_cli.egg-info/requires.txt
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        9 2022-03-21 08:44:04.000000 copr-cli-1.99/copr_cli.egg-info/top_level.txt
+drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-03-21 08:44:04.306840 copr-cli-1.99/man/
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    24537 2022-02-09 12:03:09.000000 copr-cli-1.99/man/copr-cli.1.asciidoc
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      918 2022-01-04 00:09:47.000000 copr-cli-1.99/man/copr-cli.cheat
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       20 2021-12-12 15:37:48.000000 copr-cli-1.99/man/copr.1
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      170 2021-12-12 15:37:48.000000 copr-cli-1.99/requirements.txt
+-rwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)      124 2021-12-12 15:37:48.000000 copr-cli-1.99/run_tests.sh
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       38 2022-03-21 08:44:04.307840 copr-cli-1.99/setup.cfg
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1475 2022-03-18 16:26:14.000000 copr-cli-1.99/setup.py
+drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-03-21 08:44:04.306840 copr-cli-1.99/tests/
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      445 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/cli_tests_lib.py
+drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-03-21 08:44:04.307840 copr-cli-1.99/tests/resources/
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3742 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/get_package_expected.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1282 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/get_package_response.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     2672 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/get_package_response_builds.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      126 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/list_builds_expected.txt
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3560 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/list_builds_response.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3303 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/list_packages_expected.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3260 2022-02-09 12:03:09.000000 copr-cli-1.99/tests/resources/list_packages_response.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1376 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/list_projects_expected.txt
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1602 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/resources/list_projects_response.json
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    31475 2022-02-09 12:03:09.000000 copr-cli-1.99/tests/test_cli.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     5810 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/test_distgit.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     6166 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/test_mock_config.py
+-rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      536 2021-12-12 15:37:48.000000 copr-cli-1.99/tests/test_util.py
```

### Comparing `copr-cli-1.98/LICENSE` & `copr-cli-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/PKG-INFO` & `copr-cli-1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copr-cli
-Version: 1.98
+Version: 1.99
 Summary: CLI tool to run copr
 Home-page: https://pagure.io/copr/copr
 Author: Pierre-Yves Chibon
 Author-email: pingou@pingoured.fr
 License: GPLv2+
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `copr-cli-1.98/copr-cli.spec` & `copr-cli-1.99/copr-cli.spec`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 %global __python %_bindir/python2
 %global with_python2 1
 %endif
 
 %global min_python_copr_version 1.105.2.dev
 
 Name:       copr-cli
-Version:    1.98
+Version:    1.99
 Release:    1%{?dist}
 Summary:    Command line interface for COPR
 
 License:    GPLv2+
 URL:        https://pagure.io/copr/copr
 
 # Source is created by:
@@ -124,14 +124,19 @@
 %{_datadir}/cheat/copr-cli
 %{_datadir}/cheat/copr
 %{python_sitelib}/*
 %{_bindir}/package-build-order
 
 
 %changelog
+* Fri Mar 18 2022 Pavel Raiskup <praiskup@redhat.com> 1.99-1
+- add 'edit-chroot --reset' option
+- add 'edit-chroot --rpmbuild-with{,out}'
+- add 'edit-chroot --modules' option
+
 * Wed Feb 02 2022 Silvie Chlupova <schlupov@redhat.com> 1.98-1
 - don't traceback for missing field in frontend's output
 - paginate packages list in APIv3
 - fix exit code when a build is canceled
 - api monitor page to contain pkg_version
 
 * Wed Nov 10 2021 Silvie Chlupova <schlupov@redhat.com> 1.97-1
```

### Comparing `copr-cli-1.98/copr_cli/README.rst` & `copr-cli-1.99/copr_cli/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 About this project:
 -------------------
 - Website: https://pagure.io/copr/copr
 - Git: http://git.fedorahosted.org/cgit/copr.git
 - Production Fedora instance: https://copr.fedorainfracloud.org/
-- Development Fedora instance: http://copr-fe-dev.cloud.fedoraproject.org/
+- Development Fedora instance: http://copr.stg.fedoraproject.org/
 
 
 Dependencies:
 -------------
 .. _python-requests: http://docs.python-requests.org/en/latest/
 .. _python-argparse: https://pypi.python.org/pypi/argparse
 
@@ -27,15 +27,15 @@
 - python (should work on 2.5, not tested)
 - `python-argparse`_ (for python < 2.7)
 - `python-requests`_
 
 Usage:
 ------
 
-.. _test instance: http://copr-fe-dev.cloud.fedoraproject.org/
+.. _test instance: http://copr.stg.fedoraproject.org/
 
 - Create an account on copr `test instance`_
 - Go to the API page: http://copr.fedoraproject.org/api
 - Retrieve your API token
 - Create the file ``~/.config/copr``
 - In this file add the following content
 (simpler way is just to copy it from /api)
```

### Comparing `copr-cli-1.98/copr_cli/build_config.py` & `copr-cli-1.99/copr_cli/build_config.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/copr_cli/helpers.py` & `copr-cli-1.99/copr_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/copr_cli/main.py` & `copr-cli-1.99/copr_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,40 +647,51 @@
     @requires_api_auth
     def action_edit_chroot(self, args):
         """ Method called when the 'edit-chroot' action has been selected by the
         user.
 
         :param args: argparse arguments provided by the user
         """
-
         if args.bootstrap_image:
             args.bootstrap = 'image'
         owner, copr, chroot = self.parse_chroot_path(args.coprchroot)
+
+        with_opts = None
+        if args.rpmbuild_with:
+            with_opts = ' '.join(args.rpmbuild_with)
+
+        without_opts = None
+        if args.rpmbuild_without:
+            without_opts = ' '.join(args.rpmbuild_without)
+
         self.client.project_chroot_proxy.edit(
             ownername=owner, projectname=copr, chrootname=chroot,
             comps=args.upload_comps, delete_comps=args.delete_comps,
             additional_packages=args.packages, additional_repos=args.repos,
-            bootstrap=args.bootstrap, bootstrap_image=args.bootstrap_image,
+            additional_modules=args.modules, with_opts=with_opts,
+            without_opts=without_opts, bootstrap=args.bootstrap,
+            bootstrap_image=args.bootstrap_image,
             isolation=args.isolation,
+            reset_fields=args.reset,
         )
         print("Edit chroot operation was successful.")
 
     def action_get_chroot(self, args):
         """ Method called when the 'get-chroot' action has been selected by the
         user.
 
         :param args: argparse arguments provided by the user
         """
         owner, copr, chroot = self.parse_chroot_path(args.coprchroot)
         project_chroot = self.client.project_chroot_proxy.get(
             ownername=owner, projectname=copr, chrootname=chroot
         )
-        fields = ["additional_packages", "additional_repos", "comps_name", "delete_after_days",
-                  "isolation", "mock_chroot", "ownername", "projectname", "with_opts",
-                  "without_opts"]
+        fields = ["additional_packages", "additional_repos", "additional_modules",
+                  "comps_name", "delete_after_days", "isolation", "mock_chroot",
+                  "ownername", "projectname", "with_opts", "without_opts"]
         printer = get_printer(args.output_format, fields)
         printer.add_data(project_chroot)
         printer.finish()
 
     def action_list_chroots(self, args):
         """List all currently available chroots.
         """
@@ -1400,15 +1411,21 @@
     parser_edit_chroot_comps_group.add_argument("--delete-comps", action="store_true",
                                                   help="deletes already existing comps.xml for the chroot")
 
     parser_edit_chroot.add_argument("--packages",
                                       help="space separated string of package names to be added to buildroot")
     parser_edit_chroot.add_argument("--repos",
                                       help="space separated string of additional repo urls for chroot")
-    parser_edit_chroot.add_argument("--isolation", choices=["simple", "nspawn", "default"], default="unchanged",
+    parser_edit_chroot.add_argument("--modules",
+                                      help="comma separated list of modules that will be enabled or disabled in the given chroot, e.g. 'module1:stream,!module2:stream'")
+    parser_edit_chroot.add_argument("--rpmbuild-with", action='append',
+                                      help="rpmbuild --with option, can be set multiple times")
+    parser_edit_chroot.add_argument("--rpmbuild-without", action='append',
+                                      help="rpmbuild --without options, can be set multiple times")
+    parser_edit_chroot.add_argument("--isolation", choices=["simple", "nspawn", "default"],
                                     help="Choose the isolation method for running commands in buildroot.")
 
     parser_edit_chroot.add_argument(
         "--bootstrap",
         choices=["unchanged", "default", "on", "off", "image"],
         help=("Configure Mock's bootstrap feature, "
               "default is 'unchanged' so the configuration from Copr project "
@@ -1418,14 +1435,23 @@
               "See 'create --help' for more info."))
 
     parser_edit_chroot.add_argument(
         "--bootstrap-image",
         help=("Use a custom container image for initializing Mock's "
               "bootstrap (Implies --bootstrap=image)"))
 
+    parser_edit_chroot.add_argument(
+        "--reset",
+        action="append",
+        help=("Reset this parameters to their respective defaults. "
+              "Possible values are additional_packages, additional_modules, "
+              "isolation, etc. See the output of `copr-cli get-chroot' for all "
+              "the possible field names."),
+    )
+
     parser_edit_chroot.set_defaults(func="action_edit_chroot")
 
     parser_get_chroot = subparsers.add_parser("get-chroot", help="Get chroot of a project")
     parser_get_chroot.add_argument("coprchroot", help="Path to a project chroot as owner/project/chroot or project/chroot")
     cli_use_output_format(parser_get_chroot)
     parser_get_chroot.set_defaults(func="action_get_chroot")
```

### Comparing `copr-cli-1.98/copr_cli/monitor.py` & `copr-cli-1.99/copr_cli/monitor.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/copr_cli/package_build_order.py` & `copr-cli-1.99/copr_cli/package_build_order.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/copr_cli/printers.py` & `copr-cli-1.99/copr_cli/printers.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/copr_cli/util.py` & `copr-cli-1.99/copr_cli/util.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/copr_cli.egg-info/PKG-INFO` & `copr-cli-1.99/copr_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copr-cli
-Version: 1.98
+Version: 1.99
 Summary: CLI tool to run copr
 Home-page: https://pagure.io/copr/copr
 Author: Pierre-Yves Chibon
 Author-email: pingou@pingoured.fr
 License: GPLv2+
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `copr-cli-1.98/copr_cli.egg-info/SOURCES.txt` & `copr-cli-1.99/copr_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/man/copr-cli.1.asciidoc` & `copr-cli-1.99/man/copr-cli.1.asciidoc`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/man/copr-cli.cheat` & `copr-cli-1.99/man/copr-cli.cheat`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/setup.py` & `copr-cli-1.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 __author__ = "Pierre-Yves Chibon"
 __author_email__ = "pingou@pingoured.fr"
 __url__ = "https://pagure.io/copr/copr"
 
 
 setup(
     name=__name__,
-    version="1.98",
+    version="1.99",
     description=__description__,
     long_description=long_description,
     author=__author__,
     author_email=__author_email__,
     url=__url__,
     license='GPLv2+',
     classifiers=[
```

### Comparing `copr-cli-1.98/tests/resources/get_package_expected.json` & `copr-cli-1.99/tests/resources/get_package_expected.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/get_package_response.json` & `copr-cli-1.99/tests/resources/get_package_response.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/get_package_response_builds.json` & `copr-cli-1.99/tests/resources/get_package_response_builds.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/list_builds_response.json` & `copr-cli-1.99/tests/resources/list_builds_response.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/list_packages_expected.json` & `copr-cli-1.99/tests/resources/list_packages_expected.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/list_packages_response.json` & `copr-cli-1.99/tests/resources/list_packages_response.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/list_projects_expected.txt` & `copr-cli-1.99/tests/resources/list_projects_expected.txt`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/resources/list_projects_response.json` & `copr-cli-1.99/tests/resources/list_projects_response.json`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/test_cli.py` & `copr-cli-1.99/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/test_distgit.py` & `copr-cli-1.99/tests/test_distgit.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/test_mock_config.py` & `copr-cli-1.99/tests/test_mock_config.py`

 * *Files identical despite different names*

### Comparing `copr-cli-1.98/tests/test_util.py` & `copr-cli-1.99/tests/test_util.py`

 * *Files identical despite different names*

