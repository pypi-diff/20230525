# Comparing `tmp/datalad_container-1.1.9.tar.gz` & `tmp/datalad_container-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_container-1.1.9.tar", last modified: Mon Feb  6 01:23:06 2023, max compression
+gzip compressed data, was "datalad_container-1.2.0.tar", last modified: Thu May 25 19:30:05 2023, max compression
```

## Comparing `datalad_container-1.1.9.tar` & `datalad_container-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.225145 datalad_container-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-06 01:22:30.000000 datalad_container-1.1.9/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-06 01:22:30.000000 datalad_container-1.1.9/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-06 01:22:30.000000 datalad_container-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-06 01:23:06.225145 datalad_container-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-02-06 01:22:30.000000 datalad_container-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/_datalad_buildsupport/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-06 01:22:30.000000 datalad_container-1.1.9/_datalad_buildsupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-02-06 01:22:30.000000 datalad_container-1.1.9/_datalad_buildsupport/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-02-06 01:22:30.000000 datalad_container-1.1.9/_datalad_buildsupport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.225145 datalad_container-1.1.9/datalad_container/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-06 01:23:06.225145 datalad_container-1.1.9/datalad_container/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/datalad_container/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/adapters/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/datalad_container/adapters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/adapters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/adapters/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/containers_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/containers_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/containers_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/containers_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/find_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/datalad_container/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/test_find.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/test_schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-02-06 01:22:30.000000 datalad_container-1.1.9/datalad_container/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-06 01:22:57.000000 datalad_container-1.1.9/datalad_container/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/datalad_container.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-06 01:23:06.000000 datalad_container-1.1.9/datalad_container.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-06 01:23:06.000000 datalad_container-1.1.9/datalad_container.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 01:23:06.000000 datalad_container-1.1.9/datalad_container.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-06 01:23:06.000000 datalad_container-1.1.9/datalad_container.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-06 01:23:06.000000 datalad_container-1.1.9/datalad_container.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-06 01:23:06.000000 datalad_container-1.1.9/datalad_container.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/examples/basic_demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.221145 datalad_container-1.1.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.225145 datalad_container-1.1.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/source/_static/datalad_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.217145 datalad_container-1.1.9/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.225145 datalad_container-1.1.9/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/source/acknowledgements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 01:23:06.225145 datalad_container-1.1.9/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-02-06 01:22:30.000000 datalad_container-1.1.9/docs/utils/pygments_ansi_color.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-06 01:22:30.000000 datalad_container-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-06 01:23:06.225145 datalad_container-1.1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-02-06 01:22:30.000000 datalad_container-1.1.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68607 2023-02-06 01:22:30.000000 datalad_container-1.1.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 19:29:30.000000 datalad_container-1.2.0/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-25 19:29:30.000000 datalad_container-1.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 19:29:30.000000 datalad_container-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-25 19:30:05.447893 datalad_container-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-25 19:29:30.000000 datalad_container-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/_datalad_buildsupport/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-25 19:29:30.000000 datalad_container-1.2.0/_datalad_buildsupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-25 19:29:30.000000 datalad_container-1.2.0/_datalad_buildsupport/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-25 19:29:30.000000 datalad_container-1.2.0/_datalad_buildsupport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container/adapters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/extractors/_load_singularity_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/extractors/metalad_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/find_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/fixtures/singularity_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 19:29:56.000000 datalad_container-1.2.0/datalad_container/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/examples/basic_demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/_static/datalad_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.439893 datalad_container-1.2.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/acknowledgements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/metadata-extraction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/utils/pygments_ansi_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 19:29:30.000000 datalad_container-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-25 19:30:05.447893 datalad_container-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-25 19:29:30.000000 datalad_container-1.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68607 2023-05-25 19:29:30.000000 datalad_container-1.2.0/versioneer.py
```

### Comparing `datalad_container-1.1.9/COPYING` & `datalad_container-1.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/PKG-INFO` & `datalad_container-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_container
-Version: 1.1.9
+Version: 1.2.0
 Summary: DataLad extension package for working with containerized environments
 Home-page: https://github.com/datalad/datalad-container
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `datalad_container-1.1.9/README.md` & `datalad_container-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/_datalad_buildsupport/__init__.py` & `datalad_container-1.2.0/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/_datalad_buildsupport/formatters.py` & `datalad_container-1.2.0/_datalad_buildsupport/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def _mk_title(self, prog):
         name_version = "{0} {1}".format(prog, self._version)
         return '.TH "{0}" "{1}" "{2}" "{3}"\n'.format(
             prog, self._section, self._today, name_version)
 
     def _mk_name(self, prog, desc):
         """
-        this method is in consitent with others ... it relies on
+        this method is in consistent with others ... it relies on
         distribution
         """
         desc = desc.splitlines()[0] if desc else 'it is in the name'
         # ensure starting lower case
         desc = desc[0].lower() + desc[1:]
         return '.SH NAME\n%s \\- %s\n' % (self._bold(prog), desc)
```

### Comparing `datalad_container-1.1.9/_datalad_buildsupport/setup.py` & `datalad_container-1.2.0/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/__init__.py` & `datalad_container-1.2.0/datalad_container/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """DataLad container extension"""
 
 __docformat__ = 'restructuredtext'
 
 from .version import __version__
 
+# Imported to set singularity/apptainer version commands at init
+import datalad_container.extractors._load_singularity_versions # noqa
+
 # defines a datalad command suite
 # this symbold must be identified as a setuptools entrypoint
 # to be found by datalad
 command_suite = (
     # description of the command suite, displayed in cmdline help
     "Containerized environments",
     [
```

### Comparing `datalad_container-1.1.9/datalad_container/adapters/docker.py` & `datalad_container-1.2.0/datalad_container/adapters/docker.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 this is that it allows the components of an image to be tracked as objects in a
 DataLad dataset.
 
 Run `python -m datalad_container.adapters.docker --help` for details about the
 command-line interface.
 """
 
-from glob import glob
 import hashlib
+import json
 import os
 import os.path as op
 import subprocess as sp
 import sys
 import tarfile
 import tempfile
 
@@ -43,14 +43,16 @@
     image : str
         A unique identifier for a docker image.
     path : str
         A directory to extract the image to.
     """
     # Use a temporary file because docker save (or actually tar underneath)
     # complains that stdout needs to be redirected if we use Popen and PIPE.
+    if ":" not in image:
+        image = f"{image}:latest"
     with tempfile.NamedTemporaryFile() as stream:
         # Windows can't write to an already opened file
         stream.close()
         sp.check_call(["docker", "save", "-o", stream.name, image])
         with tarfile.open(stream.name, mode="r:") as tar:
             if not op.exists(path):
                 lgr.debug("Creating new directory at %s", path)
@@ -82,46 +84,59 @@
 
 def _list_images():
     out = sp.check_output(
         ["docker", "images", "--all", "--quiet", "--no-trunc"])
     return out.decode().splitlines()
 
 
-def get_image(path):
+def get_image(path, repo_tag=None, config=None):
     """Return the image ID of the image extracted at `path`.
     """
-    jsons = [j for j in glob(op.join(path, "*.json"))
-             if not j.endswith(op.sep + "manifest.json")]
-    if len(jsons) != 1:
-        raise ValueError("Could not find a unique JSON configuration object "
-                         "in {}".format(path))
+    manifest_path = op.join(path, "manifest.json")
+    with open(manifest_path) as fp:
+        manifest = json.load(fp)
+    if repo_tag is not None:
+        manifest = [img for img in manifest if repo_tag in img.get("RepoTags", [])]
+    if config is not None:
+        manifest = [img for img in manifest if img["Config"].startswith(config)]
+    if len(manifest) == 0:
+        raise ValueError(f"No matching images found in {manifest_path}")
+    elif len(manifest) > 1:
+        raise ValueError(
+            f"Multiple images found in {manifest_path}; disambiguate with"
+            " --repo-tag or --config"
+        )
 
-    with open(jsons[0], "rb") as stream:
+    with open(op.join(path, manifest[0]["Config"]), "rb") as stream:
         return hashlib.sha256(stream.read()).hexdigest()
 
 
-def load(path):
+def load(path, repo_tag, config):
     """Load the Docker image from `path`.
 
     Parameters
     ----------
     path : str
         A directory with an extracted tar archive.
+    repo_tag : str or None
+        `image:tag` of image to load
+    config : str or None
+        "Config" value or prefix of image to load
 
     Returns
     -------
     The image ID (str)
     """
     # FIXME: If we load a dataset, it may overwrite the current tag. Say that
     # (1) a dataset has a saved neurodebian:latest from a month ago, (2) a
     # newer neurodebian:latest has been pulled, and (3) the old image have been
     # deleted (e.g., with 'docker image prune --all'). Given all three of these
     # things, loading the image from the dataset will tag the old neurodebian
     # image as the latest.
-    image_id = "sha256:" + get_image(path)
+    image_id = "sha256:" + get_image(path, repo_tag, config)
     if image_id not in _list_images():
         lgr.debug("Loading %s", image_id)
         cmd = ["docker", "load"]
         p = sp.Popen(cmd, stdin=sp.PIPE, stdout=sp.PIPE, stderr=sp.PIPE)
         with tarfile.open(fileobj=p.stdin, mode="w|", dereference=True) as tar:
             tar.add(path, arcname="")
         out, err = p.communicate()
@@ -142,15 +157,15 @@
 
 
 def cli_save(namespace):
     save(namespace.image, namespace.path)
 
 
 def cli_run(namespace):
-    image_id = load(namespace.path)
+    image_id = load(namespace.path, namespace.repo_tag, namespace.config)
     prefix = ["docker", "run",
               # FIXME: The -v/-w settings are convenient for testing, but they
               # should be configurable.
               "-v", "{}:/tmp".format(os.getcwd()),
               "-w", "/tmp",
               "--rm",
               "--interactive"]
@@ -195,14 +210,22 @@
     parser_save.set_defaults(func=cli_save)
     # TODO: Add command for updating an archive directory.
 
     parser_run = subparsers.add_parser(
         "run",
         help="run a command with a directory's image")
     parser_run.add_argument(
+        "--repo-tag", metavar="IMAGE:TAG", help="Tag of image to load"
+    )
+    parser_run.add_argument(
+        "--config",
+        metavar="IDPREFIX",
+        help="Config value or prefix of image to load"
+    )
+    parser_run.add_argument(
         "path", metavar="PATH",
         help="run the image in this directory")
     parser_run.add_argument(
         "cmd", metavar="CMD", nargs=argparse.REMAINDER,
         help="command to execute")
     parser_run.set_defaults(func=cli_run)
```

### Comparing `datalad_container-1.1.9/datalad_container/adapters/tests/test_docker.py` & `datalad_container-1.2.0/datalad_container/adapters/tests/test_docker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import json
 import os.path as op
+from shutil import unpack_archive, which
 import sys
-from distutils.spawn import find_executable
 
+import pytest
 from datalad.cmd import (
     StdOutCapture,
     WitlessRunner,
 )
 from datalad.support.exceptions import CommandError
 from datalad.tests.utils_pytest import (
     SkipTest,
@@ -15,15 +17,15 @@
     ok_exists,
     with_tempfile,
     with_tree,
 )
 
 import datalad_container.adapters.docker as da
 
-if not find_executable("docker"):
+if not which("docker"):
     raise SkipTest("'docker' not found on path")
 
 
 def call(args, **kwds):
     return WitlessRunner().run(
         [sys.executable, "-m", "datalad_container.adapters.docker"] + args,
         **kwds)
@@ -108,7 +110,27 @@
         # Data can be received on stdin.
         with (ds.pathobj / "foo").open() as ifh:
             out = WitlessRunner(cwd=ds.path).run(
                 ["datalad", "containers-run", "-n", "bb", "cat"],
                 protocol=StdOutCapture,
                 stdin=ifh)
         assert_in("content", out["stdout"])
+
+
+def test_load_multi_image(tmp_path):
+    for v in ["3.15", "3.16", "3.17"]:
+        WitlessRunner().run(["docker", "pull", f"alpine:{v}"])
+    WitlessRunner().run(["docker", "save", "alpine", "-o", str(tmp_path / "alpine.tar")])
+    unpack_archive(tmp_path / "alpine.tar", tmp_path / "alpine")
+    with pytest.raises(CommandError):
+        call(["run", str(tmp_path / "alpine"), "ls"])
+    call(["run", "--repo-tag", "alpine:3.16", str(tmp_path / "alpine"), "ls"])
+
+
+def test_save_multi_image(tmp_path):
+    for v in ["3.15", "3.16", "latest"]:
+        WitlessRunner().run(["docker", "pull", f"alpine:{v}"])
+    call(["save", "alpine", str(tmp_path)])
+    with (tmp_path / "manifest.json").open() as fp:
+        manifest = json.load(fp)
+    assert len(manifest) == 1
+    assert manifest[0]["RepoTags"] == ["alpine:latest"]
```

### Comparing `datalad_container-1.1.9/datalad_container/containers_add.py` & `datalad_container-1.2.0/datalad_container/containers_add.py`

 * *Files 7% similar despite different names*

```diff
@@ -136,19 +136,37 @@
         # container datasets
         call_fmt=Parameter(
             args=("--call-fmt",),
             doc="""Command format string indicating how to execute a command in
             this container, e.g. "singularity exec {img} {cmd}". Where '{img}'
             is a placeholder for the path to the container image and '{cmd}' is
             replaced with the desired command. Additional placeholders:
-            '{img_dspath}' is relative path to the dataset containing the image.
+            '{img_dspath}' is relative path to the dataset containing the image,
+            '{img_dirpath}' is the directory containing the '{img}'.
             """,
             metavar="FORMAT",
             constraints=EnsureStr() | EnsureNone(),
         ),
+        extra_input=Parameter(
+            args=("--extra-input",),
+            doc="""Additional file the container invocation depends on (e.g.
+            overlays used in --call-fmt). Can be specified multiple times.
+            Similar to --call-fmt, the placeholders {img_dspath} and
+            {img_dirpath} are available. Will be stored in the dataset config and
+            later added alongside the container image to the `extra_inputs`
+            field in the run-record and thus automatically be fetched when
+            needed.
+            """,
+            action="append",
+            default=[],
+            metavar="FILE",
+            # Can't use EnsureListOf(str) yet as it handles strings as iterables...
+            # See this PR: https://github.com/datalad/datalad/pull/7267
+            # constraints=EnsureListOf(str) | EnsureNone(),
+        ),
         image=Parameter(
             args=("-i", "--image"),
             doc="""Relative path of the container image within the dataset. If not
                 given, a default location will be determined using the
                 `name` argument.""",
             metavar="IMAGE",
             constraints=EnsureStr() | EnsureNone(),
@@ -164,15 +182,15 @@
         )
     )
 
     @staticmethod
     @datasetmethod(name='containers_add')
     @eval_results
     def __call__(name, url=None, dataset=None, call_fmt=None, image=None,
-                 update=False):
+                 update=False, extra_input=None):
         if not name:
             raise InsufficientArgumentsError("`name` argument is required")
 
         ds = require_dataset(dataset, check_installed=True,
                              purpose='add container')
         runner = WitlessRunner()
 
@@ -317,14 +335,36 @@
             op.relpath(image, start=ds.path),
             force=True)
         if call_fmt:
             ds.config.set(
                 "{}.cmdexec".format(cfgbasevar),
                 call_fmt,
                 force=True)
+        # --extra-input sanity check
+        # TODO: might also want to do that for --call-fmt above?
+        extra_input_placeholders = dict(img_dirpath="", img_dspath="")
+        for xi in (extra_input or []):
+            try:
+                xi.format(**extra_input_placeholders)
+            except KeyError as exc:
+                yield get_status_dict(
+                    action="containers_add", ds=ds, logger=lgr,
+                    status="error",
+                    message=("--extra-input %r contains unknown placeholder %s. "
+                             "Available placeholders: %s",
+                             repr(xi), exc, ', '.join(extra_input_placeholders)))
+                return
+
+        # actually setting --extra-input config
+        cfgextravar = "{}.extra-input".format(cfgbasevar)
+        if ds.config.get(cfgextravar) is not None:
+            ds.config.unset(cfgextravar)
+        for xi in (extra_input or []):
+            ds.config.add(cfgextravar, xi)
+
         # store changes
         to_save.append(op.join(".datalad", "config"))
         for r in ds.save(
                 path=to_save,
                 message="[DATALAD] {do} containerized environment '{name}'".format(
                     do="Update" if was_updated else "Configure",
                     name=name)):
```

### Comparing `datalad_container-1.1.9/datalad_container/containers_list.py` & `datalad_container-1.2.0/datalad_container/containers_list.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/containers_remove.py` & `datalad_container-1.2.0/datalad_container/containers_remove.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/containers_run.py` & `datalad_container-1.2.0/datalad_container/containers_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from datalad.interface.base import Interface
 from datalad.interface.base import build_doc
 from datalad.support.param import Parameter
 from datalad.distribution.dataset import datasetmethod
 from datalad.distribution.dataset import require_dataset
 from datalad.interface.base import eval_results
+from datalad.utils import ensure_iter
 
 from datalad.interface.results import get_status_dict
 from datalad.core.local.run import (
     Run,
     get_command_pwds,
     normalize_command,
     run_command,
@@ -110,14 +111,15 @@
                         'cmdexe {!r} is in an old, unsupported format. '
                         'Convert it to a plain string.'.format(callspec))
             try:
                 cmd_kwargs = dict(
                     img=image_path,
                     cmd=cmd,
                     img_dspath=image_dspath,
+                    img_dirpath=op.dirname(image_path) or ".",
                 )
                 cmd = callspec.format(**cmd_kwargs)
             except KeyError as exc:
                 yield get_status_dict(
                     'run',
                     ds=ds,
                     status='error',
@@ -127,21 +129,43 @@
                         exc,
                         ", ".join(cmd_kwargs)))
                 return
         else:
             # just prepend and pray
             cmd = container['path'] + ' ' + cmd
 
+        extra_inputs = []
+        for extra_input in ensure_iter(container.get("extra-input",[]), set):
+            try:
+                xi_kwargs = dict(
+                    img_dspath=image_dspath,
+                    img_dirpath=op.dirname(image_path) or ".",
+                )
+                extra_inputs.append(extra_input.format(**xi_kwargs))
+            except KeyError as exc:
+                yield get_status_dict(
+                    'run',
+                    ds=ds,
+                    status='error',
+                    message=(
+                        'Unrecognized extra_input placeholder: %s. '
+                        'See containers-add for information on known ones: %s',
+                        exc,
+                        ", ".join(xi_kwargs)))
+                return
+
+        lgr.debug("extra_inputs = %r", extra_inputs)
+
         with patch.dict('os.environ',
                         {CONTAINER_NAME_ENVVAR: container['name']}):
             # fire!
             for r in run_command(
                     cmd=cmd,
                     dataset=dataset or (ds if ds.path == pwd else None),
                     inputs=inputs,
-                    extra_inputs=[image_path],
+                    extra_inputs=[image_path] + extra_inputs,
                     outputs=outputs,
                     message=message,
                     expand=expand,
                     explicit=explicit,
                     sidecar=sidecar):
                 yield r
```

### Comparing `datalad_container-1.1.9/datalad_container/find_container.py` & `datalad_container-1.2.0/datalad_container/find_container.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/tests/test_add.py` & `datalad_container-1.2.0/datalad_container/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/tests/test_containers.py` & `datalad_container-1.2.0/datalad_container/tests/test_containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,54 @@
     res = ds.containers_remove('first', remove_image=True)
     assert_status('ok', res)
     assert_result_count(ds.containers_list(**RAW_KWDS), 0)
     # image removed
     assert(not op.lexists(target_path))
 
 
+@with_tree(tree={
+    "container.img": "container",
+    "overlay1.img":  "overlay 1",
+    "overlay2.img":  "overlay 2",
+})
+def test_extra_inputs(ds_path=None):
+    container_file = 'container.img'
+    overlay1_file  = 'overlay1.img'
+    overlay2_file  = 'overlay2.img'
+
+    # prepare dataset:
+    ds = Dataset(ds_path).create(force=True)
+    ds.save()
+
+    ds.containers_add(
+        name="container",
+        image=container_file,
+        call_fmt="apptainer exec {img} {cmd}",
+    )
+    ds.containers_add(
+        name="container-with-overlay",
+        image=container_file,
+        call_fmt="apptainer exec --overlay {img_dirpath}/overlay1.img {img} {cmd}",
+        extra_input=[overlay1_file]
+    )
+    ds.containers_add(
+        name="container-with-two-overlays",
+        image=container_file,
+        call_fmt="apptainer exec --overlay {img_dirpath}/overlay1.img --overlay {img_dirpath}/overlay2.img:ro {img} {cmd}",
+        extra_input=[overlay1_file, overlay2_file]
+    )
+
+    res = ds.containers_list(**RAW_KWDS)
+    assert_result_count(res, 3)
+
+    assert_equal(ds.config.get("datalad.containers.container.extra-input"), None)
+    assert_equal(ds.config.get("datalad.containers.container-with-overlay.extra-input",get_all=True), "overlay1.img")
+    assert_equal(ds.config.get("datalad.containers.container-with-two-overlays.extra-input",get_all=True), ("overlay1.img", "overlay2.img"))
+
+
 @with_tempfile
 @with_tree(tree={'foo.img': "foo",
                  'bar.img': "bar"})
 @serve_path_via_http
 def test_container_update(ds_path=None, local_file=None, url=None):
     url_foo = get_local_file_url(op.join(local_file, 'foo.img'))
     url_bar = get_local_file_url(op.join(local_file, 'bar.img'))
```

### Comparing `datalad_container-1.1.9/datalad_container/tests/test_find.py` & `datalad_container-1.2.0/datalad_container/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/tests/test_run.py` & `datalad_container-1.2.0/datalad_container/tests/test_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Dataset,
     clone,
     containers_add,
     containers_list,
     containers_run,
     create,
 )
+from datalad.local.rerun import get_run_info
 from datalad.cmd import (
     StdOutCapture,
     WitlessRunner,
 )
 from datalad.support.network import get_local_file_url
 from datalad.tests.utils_pytest import (
     assert_false,
@@ -187,14 +188,55 @@
     os.mkdir(subdir)
     out = WitlessRunner(cwd=subdir).run(
         ['datalad', 'containers-run', '-n', 'sub/mycontainer', 'XXX'],
         protocol=StdOutCapture)
     assert_in('image=../sub/righthere cmd=XXX img_dspath=../sub', out['stdout'])
 
 
+@with_tree(
+    tree={
+        "overlay1.img": "overlay1",
+        "sub": {
+            "containers": {"container.img": "image file"},
+            "overlays": {"overlay2.img": "overlay2", "overlay3.img": "overlay3"},
+        },
+    }
+)
+def test_extra_inputs(path=None):
+    ds = Dataset(path).create(force=True)
+    subds = ds.create("sub", force=True)
+    subds.containers_add(
+        "mycontainer",
+        image="containers/container.img",
+        call_fmt="echo image={img} cmd={cmd} img_dspath={img_dspath} img_dirpath={img_dirpath} > out.log",
+        extra_input=[
+            "overlay1.img",
+            "{img_dirpath}/../overlays/overlay2.img",
+            "{img_dspath}/overlays/overlay3.img",
+        ],
+    )
+    ds.save(recursive=True)  # record the entire tree of files etc
+    ds.containers_run("XXX", container_name="sub/mycontainer")
+    ok_file_has_content(
+        os.path.join(ds.repo.path, "out.log"),
+        "image=sub/containers/container.img",
+        re_=True,
+    )
+    commit_msg = ds.repo.call_git(["show", "--format=%B"])
+    cmd, runinfo = get_run_info(ds, commit_msg)
+    assert set(
+        [
+            "sub/containers/container.img",
+            "overlay1.img",
+            "sub/containers/../overlays/overlay2.img",
+            "sub/overlays/overlay3.img",
+        ]
+    ) == set(runinfo.get("extra_inputs", set()))
+
+
 @skip_if_no_network
 @with_tree(tree={"subdir": {"in": "innards"}})
 def test_run_no_explicit_dataset(path=None):
     ds = Dataset(path).create(force=True)
     ds.save()
     ds.containers_add("deb", url=testimg_url,
                       call_fmt="singularity exec {img} {cmd}")
```

### Comparing `datalad_container-1.1.9/datalad_container/tests/test_schemes.py` & `datalad_container-1.2.0/datalad_container/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container/tests/utils.py` & `datalad_container-1.2.0/datalad_container/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/datalad_container.egg-info/PKG-INFO` & `datalad_container-1.2.0/datalad_container.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-container
-Version: 1.1.9
+Version: 1.2.0
 Summary: DataLad extension package for working with containerized environments
 Home-page: https://github.com/datalad/datalad-container
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `datalad_container-1.1.9/datalad_container.egg-info/SOURCES.txt` & `datalad_container-1.2.0/datalad_container.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,35 +14,42 @@
 datalad_container/conftest.py
 datalad_container/containers_add.py
 datalad_container/containers_list.py
 datalad_container/containers_remove.py
 datalad_container/containers_run.py
 datalad_container/definitions.py
 datalad_container/find_container.py
+datalad_container/utils.py
 datalad_container/version.py
 datalad_container.egg-info/PKG-INFO
 datalad_container.egg-info/SOURCES.txt
 datalad_container.egg-info/dependency_links.txt
 datalad_container.egg-info/entry_points.txt
 datalad_container.egg-info/requires.txt
 datalad_container.egg-info/top_level.txt
 datalad_container/adapters/__init__.py
 datalad_container/adapters/docker.py
 datalad_container/adapters/tests/__init__.py
 datalad_container/adapters/tests/test_docker.py
+datalad_container/extractors/__init__.py
+datalad_container/extractors/_load_singularity_versions.py
+datalad_container/extractors/metalad_container.py
 datalad_container/tests/__init__.py
 datalad_container/tests/test_add.py
 datalad_container/tests/test_containers.py
 datalad_container/tests/test_find.py
 datalad_container/tests/test_register.py
 datalad_container/tests/test_run.py
 datalad_container/tests/test_schemes.py
 datalad_container/tests/utils.py
+datalad_container/tests/fixtures/__init__.py
+datalad_container/tests/fixtures/singularity_image.py
 docs/Makefile
 docs/examples/basic_demo.sh
 docs/source/acknowledgements.rst
 docs/source/changelog.rst
 docs/source/conf.py
 docs/source/index.rst
+docs/source/metadata-extraction.rst
 docs/source/_static/datalad_logo.png
 docs/source/_templates/autosummary/module.rst
 docs/utils/pygments_ansi_color.py
```

### Comparing `datalad_container-1.1.9/docs/Makefile` & `datalad_container-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/docs/examples/basic_demo.sh` & `datalad_container-1.2.0/docs/examples/basic_demo.sh`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/docs/source/_static/datalad_logo.png` & `datalad_container-1.2.0/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/docs/source/acknowledgements.rst` & `datalad_container-1.2.0/docs/source/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/docs/source/changelog.rst` & `datalad_container-1.2.0/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/docs/source/conf.py` & `datalad_container-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/docs/source/index.rst` & `datalad_container-1.2.0/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 * `API reference`_
 
 .. toctree::
    :maxdepth: 1
 
    changelog
    acknowledgements
+   metadata-extraction
 
 
 API Reference
 =============
 
 Command manuals
 ---------------
```

### Comparing `datalad_container-1.1.9/docs/utils/pygments_ansi_color.py` & `datalad_container-1.2.0/docs/utils/pygments_ansi_color.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.1.9/setup.cfg` & `datalad_container-1.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 [options.packages.find]
 exclude = 
 	_datalad_buildsupport
 
 [options.entry_points]
 datalad.extensions = 
 	container = datalad_container:command_suite
+datalad.metadata.extractors = 
+	container_inspect = datalad_container.extractors.metalad_container:MetaladContainerInspect
 
 [versioneer]
 VCS = git
 style = pep440
 versionfile_source = datalad_container/_version.py
 versionfile_build = datalad_container/_version.py
 tag_prefix =
```

### Comparing `datalad_container-1.1.9/versioneer.py` & `datalad_container-1.2.0/versioneer.py`

 * *Files identical despite different names*

