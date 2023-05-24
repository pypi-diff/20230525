# Comparing `tmp/datawrapper-0.5.tar.gz` & `tmp/datawrapper-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawrapper-0.5.tar", last modified: Mon May 22 17:33:01 2023, max compression
+gzip compressed data, was "datawrapper-0.5.1.tar", last modified: Wed May 24 23:35:15 2023, max compression
```

## Comparing `datawrapper-0.5.tar` & `datawrapper-0.5.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-22 17:32:44.000000 datawrapper-0.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/.stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-22 17:32:44.000000 datawrapper-0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 17:32:44.000000 datawrapper-0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-22 17:32:44.000000 datawrapper-0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-22 17:32:44.000000 datawrapper-0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-22 17:32:44.000000 datawrapper-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-22 17:33:01.102587 datawrapper-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 17:32:44.000000 datawrapper-0.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    66724 2023-05-22 17:32:44.000000 datawrapper-0.5/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-22 17:32:44.000000 datawrapper-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-22 17:32:44.000000 datawrapper-0.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/datawrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-22 17:32:44.000000 datawrapper-0.5/datawrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23015 2023-05-22 17:32:44.000000 datawrapper-0.5/datawrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 17:32:44.000000 datawrapper-0.5/datawrapper/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/datawrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/_templates/class.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/static/datawrapper_logo_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/static/datawrapper_logo_light_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/user-guide/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/user-guide/usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:33:01.102587 datawrapper-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-22 17:32:44.000000 datawrapper-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.094586 datawrapper-0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/tests/test_example/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-22 17:32:44.000000 datawrapper-0.5/tests/test_example/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.236102 datawrapper-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.228102 datawrapper-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/.stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.228102 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.228102 datawrapper-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-24 23:34:57.000000 datawrapper-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 23:34:57.000000 datawrapper-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-24 23:34:57.000000 datawrapper-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-24 23:35:15.236102 datawrapper-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 23:34:57.000000 datawrapper-0.5.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    66724 2023-05-24 23:34:57.000000 datawrapper-0.5.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-24 23:34:57.000000 datawrapper-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-24 23:34:57.000000 datawrapper-0.5.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/datawrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 23:34:57.000000 datawrapper-0.5.1/datawrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23015 2023-05-24 23:34:57.000000 datawrapper-0.5.1/datawrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 23:34:57.000000 datawrapper-0.5.1/datawrapper/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/datawrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/_templates/class.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/static/datawrapper_logo_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/static/datawrapper_logo_light_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/user-guide/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/user-guide/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 23:35:15.236102 datawrapper-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-24 23:34:57.000000 datawrapper-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.224102 datawrapper-0.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.236102 datawrapper-0.5.1/tests/test_example/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-24 23:34:57.000000 datawrapper-0.5.1/tests/test_example/test_hello.py
```

### Comparing `datawrapper-0.5/.github/.stale.yml` & `datawrapper-0.5.1/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `datawrapper-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `datawrapper-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.github/PULL_REQUEST_TEMPLATE.md` & `datawrapper-0.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.github/dependabot.yml` & `datawrapper-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.github/workflows/continuous-deployment.yml` & `datawrapper-0.5.1/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.gitignore` & `datawrapper-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/.pre-commit-config.yaml` & `datawrapper-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/CODE_OF_CONDUCT.md` & `datawrapper-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/CONTRIBUTING.md` & `datawrapper-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/LICENSE` & `datawrapper-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/PKG-INFO` & `datawrapper-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawrapper
-Version: 0.5
+Version: 0.5.1
 Summary: A light-weight python wrapper for the Datawrapper API
 Home-page: https://github.com/chekos/datawrapper
 Author: chekos
 Author-email: chekos@tacosdedatos.com
 License: MIT
 Project-URL: Maintainer, https://github.com/chekos/
 Project-URL: Source, https://github.com/chekos/datawrapper
```

### Comparing `datawrapper-0.5/Pipfile.lock` & `datawrapper-0.5.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/README.md` & `datawrapper-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/SECURITY.md` & `datawrapper-0.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/datawrapper/__init__.py` & `datawrapper-0.5.1/datawrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/datawrapper/__main__.py` & `datawrapper-0.5.1/datawrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/datawrapper.egg-info/PKG-INFO` & `datawrapper-0.5.1/datawrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawrapper
-Version: 0.5
+Version: 0.5.1
 Summary: A light-weight python wrapper for the Datawrapper API
 Home-page: https://github.com/chekos/datawrapper
 Author: chekos
 Author-email: chekos@tacosdedatos.com
 License: MIT
 Project-URL: Maintainer, https://github.com/chekos/
 Project-URL: Source, https://github.com/chekos/datawrapper
```

### Comparing `datawrapper-0.5/datawrapper.egg-info/SOURCES.txt` & `datawrapper-0.5.1/datawrapper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 .github/workflows/continuous-deployment.yml
 datawrapper/__init__.py
 datawrapper/__main__.py
 datawrapper/example.py
 datawrapper.egg-info/PKG-INFO
 datawrapper.egg-info/SOURCES.txt
 datawrapper.egg-info/dependency_links.txt
+datawrapper.egg-info/requires.txt
 datawrapper.egg-info/top_level.txt
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/requirements.txt
 docs/_templates/class.md
```

### Comparing `datawrapper-0.5/docs/Makefile` & `datawrapper-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/docs/conf.py` & `datawrapper-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/docs/make.bat` & `datawrapper-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/docs/static/datawrapper_logo_light.png` & `datawrapper-0.5.1/docs/static/datawrapper_logo_light.png`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/docs/static/datawrapper_logo_light_small.png` & `datawrapper-0.5.1/docs/static/datawrapper_logo_light_small.png`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/docs/user-guide/installation.md` & `datawrapper-0.5.1/docs/user-guide/installation.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/docs/user-guide/usage.ipynb` & `datawrapper-0.5.1/docs/user-guide/usage.ipynb`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5/setup.py` & `datawrapper-0.5.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,14 +54,21 @@
     url="https://github.com/chekos/datawrapper",
     project_urls={
         "Maintainer": "https://github.com/chekos/",
         "Source": "https://github.com/chekos/datawrapper",
         "Tracker": "https://github.com/chekos/datawrapper/issues",
     },
     packages=("datawrapper",),
+    install_requires=[
+        "importlib_metadata",
+        "rich",
+        "requests",
+        "pandas",
+        "ipython",
+    ],
     setup_requires=["setuptools_scm"],
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `datawrapper-0.5/tests/test_example/test_hello.py` & `datawrapper-0.5.1/tests/test_example/test_hello.py`

 * *Files identical despite different names*

